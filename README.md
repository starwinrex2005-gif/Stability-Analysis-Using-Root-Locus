# Stability Analysis using Root Locus
## Aim:
To analyse the stability of the system having open loop transfer function, G(S)=K/(S(S+5)(S+10)) using root locus and verify it using MATLAB. 
## Apparatus Required:
Computer with MATLAB software

## Theory:

<img width="638" height="951" alt="image" src="https://github.com/user-attachments/assets/05ec1a46-d52c-4d75-80f4-fc7986d7c0f6" />
<img width="433" height="947" alt="image" src="https://github.com/user-attachments/assets/cf770ec2-368e-43ce-bc99-4c6eb9f17ed7" />
<img width="342" height="936" alt="image" src="https://github.com/user-attachments/assets/00244e5d-225d-4c8b-91ce-869eb46eb3a5" />


## Procedure:
	Open MATLAB software
	Open a new script file.
	Type the program.
	Save and Execute the program.
	Click on the crossing point of the root locus to find the value of K and poles at the crossing point.
	From the value of K, analyse the stability.

## Program: 

num=[1];

	den=[1 15 50 0];
	
	sys=tf(num,den);
	
	rlocus(sys);
	
	[k,poles]=rlocfind(sys)
	
## Output:
<img width="692" height="587" alt="image" src="https://github.com/user-attachments/assets/ba924f3c-f007-4dad-8773-419132221bc0" />
<img width="236" height="290" alt="image" src="https://github.com/user-attachments/assets/cb583f97-f057-4c9b-8498-d3ca072fea78" />

## Result:
Thus the root locus for the given transfer function was drawn and verified using MATLAB. The conditions for stability is 0<k<753.1393
