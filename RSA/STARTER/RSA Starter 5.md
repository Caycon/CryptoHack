**RSA Starter 5**
![image](https://hackmd.io/_uploads/Hyy8PgBYT.png)
- Challenge nay yêu cầu ta tìm thông tin bị encrypt dựa vào các yếu tố đã cung cấp.
- Ta biết $c \equiv m^e mod(n)$ và $m \equiv c^d mod(n)$
- Sử dụng factordb để phân tích n.
```Python
n= 882564595536224140639625987659416029426239230804614613279163
p = 857504083339712752489993810777
q = 1029224947942998075080348647219
e= 65537
c= 77578995801157823671636298847186723593814843845525223303932
phi= (p- 1)*(q- 1)
d= pow(e, -1, phi)
print(pow(c, d, n))
```
![image](https://hackmd.io/_uploads/HylY_eSK6.png)
