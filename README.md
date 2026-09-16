# enigma

```
 -- L1C5 4PR353N74 --
```

Você achou o repositório. Metade do caminho.

O arquivo [`enigma.txt`](enigma.txt) não está corrompido.
Está **codificado**.

Olhe o conteúdo: apenas `A-Z`, `a-z`, `0-9`, `+`, `/` e um `=` no fim.
Isso não é aleatório. São 64 caracteres, sempre os mesmos 64.

---

### Como decodificar

**Linux / macOS**
```bash
base64 -d enigma.txt
```

**Windows (PowerShell)**
```powershell
[Text.Encoding]::UTF8.GetString([Convert]::FromBase64String((Get-Content enigma.txt -Raw) -replace '\s',''))
```

**Python**
```python
import base64
print(base64.b64decode(open("enigma.txt").read()).decode())
```

**Sem terminal:** use o [CyberChef](https://gchq.github.io/CyberChef/).
Cole o conteúdo em *Input*, arraste a receita **From Base64** para a área de
*Recipe* e o texto aparece em *Output*. Roda inteiro no seu navegador, nada
do que você colar sai da sua máquina.

---

`N3M TUD0 QU3 3574 0CU170 P3RMAN3C3 35C0ND1D0`
