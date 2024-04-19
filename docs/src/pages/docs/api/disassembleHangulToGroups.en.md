---
title: disassembleHangulToGroups
---

# disassembleHangulToGroups

한글 문자열을 글자별로 초성/중성/종성 단위로 완전히 분리합니다.

`ㄵ`와 같은 겹자음은 `['ㄴ', 'ㅈ']`와 같이 풀고, `ㅘ`와 같은 겹모음은 `['ㅗ', 'ㅏ']`와 같이 풉니다.

자세한 예시는 아래 Example을 참고하세요.

```typescript
function disassembleHangulToGroups(
  // The Korean string to be disassembled
  str: string
): string[][];
```

## Examples

```typescript
disassembleHangulToGroups('값'); // [['ㄱ', 'ㅏ', 'ㅂ', 'ㅅ']]
disassembleHangulToGroups('ㅘ'); // [['ㅗ', 'ㅏ']]
disassembleHangulToGroups('ㄵ'); // [['ㄴ', 'ㅈ']]
```