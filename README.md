# CStask-2

**Phishing Email Analysis – What We Learned**

## Objective  
Understand phishing attacks through real email analysis.

## Key Learnings  
- **Phishing** is fake emails that trick you into giving passwords or money.  
- **Spoofing**: Fake sender name (e.g., Bradesco) but wrong email domain.  
- **Header Analysis**: Emails have hidden logs — check IP, SPF, DKIM to find fakes.  
- **Social Engineering**: Uses fear ("points expire today") to rush you.  
- **Threat Detection**: Spot red flags fast:  
  - Wrong sender  
  - Urgent words  
  - Fake links  
  - Typos  

## Analysis Summary  
| Red Flag | Found in Sample |
|--------|-----------------|
| Wrong sender domain | `atendimento.com.br` ≠ `bradesco.com.br` |
| SPF/DKIM fail | Forged email |
| Sent from USA | Not Brazil |
| Fake link | `blog1seguimentmydomain2bra.me` |
| Urgency | "Expiring today" |
| Typos | "LIVELO" spacing |

**Verdict**: 100% Phishing Scam

## Tools Used  
- MX Toolbox → Header check  
- Notepad++ → View raw email  
- Chrome → See HTML safely  

## Sample Source  
[phishing_pot GitHub](https://github.com/rf-peixoto/phishing_pot)

---
**Learned: Never trust emails. Always verify.**
