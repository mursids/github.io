# github.io
Simple Encription with str_replace

1. create table array 
2. rename position character 
3. show this script
 
<!DOCTYPE html>
<html>
<body>
Simple Encription with str_replace<br>@mursids<br><br>
<?php

function search($type,$arr,$cari){
	foreach( $arr as $key=>$val )
    { if($type=="E") { $x=$key;$y=$val;} else { $x=$val;$y=$key;}
	if (ord($x) == ord($cari)){
		return $y;
}}return $cari;	}
function ec($in,$key){
	$out='';
	for($i=0;$i<strlen($in);$i++){
		$temp=($in[$i]);
		//$r=golek($key,$temp);
		$r=search("E",$key,$temp);
		$R=str_replace($temp, $r, $temp);
		$out=$out.$R; 
	}
	return $out;
	}
function dc($in,$key){
	$out='';
	for($i=0;$i<strlen($in);$i++){
		$temp=($in[$i]);
		$r=search("D",$key,$temp);
		$out=$out. str_replace($temp, $r, $temp);
	}
	return $out;
}		
$text ="@SamPLe TekS<>#$"; // "ProFilex";//
$text2= "@wDSseI=xIOw<>#$";
$key = array(
	'd' => 'A','j' => 'K','r' => 'U','A' => 'a','6' => 'k','4' => 'u',
	'f' => 'B','3' => 'L','5' => 'V','R' => 'b','J' => 'l','0' => 'v',
	'g' => 'C','l' => 'M','s' => 'W','B' => 'c','Z' => 'm','S' => 'w',
	'a' => 'D','p' => 'N','x' => 'X','M' => 'd','i' => 'n','T' => 'x',
	'I' => 'E','k' => 'O','z' => 'Y','L' => 'e','u' => 'o','Y' => 'y',
	'h' => 'F','o' => 'P','t' => 'Z','C' => 'f','H' => 'p','7' => 'z',
	'b' => 'G','n' => 'Q','v' => '1','K' => 'g','N' => 'q','W' => '5',
	'1' => 'H','2' => 'R','y' => '2','O' => 'h','G' => 'r','8' => '6',
	'e' => 'I','m' => 'S','U' => '3','D' => 'i','P' => 's','9' => '7',
	'c' => 'J','q' => 'T','w' => '4','Q' => 'j','F' => 't','V' => '8',	
	'E' => '9','=' => ' ','X' => '0','`' => '~','~' => '`','=' => ' ',
	' ' => '=','"' => '%','.' => '*','*' => '"','*' => '%'); //please adding your table

echo "<strong>Teks </strong>".$text;
echo "<br>";		
echo "<strong>Encript =</strong> ".ec($text,$key);
echo "<br>";
echo "<strong>Decript =</strong>".dc($text,$key);

$text3="A computer is a general purpose device that can be programmed to carry out a set of arithmetic or logical operations automatically. Since a sequence of operations can be readily changed, the computer can solve more than one kind of problem.

Conventionally, a computer consists of at least one processing element, typically a central processing unit (CPU), and some form of memory. The processing element carries out arithmetic and logic operations, and a sequencing and control unit can change the order of operations in response to stored information. Peripheral devices allow information to be retrieved from an external source, and the result of operations saved and retrieved.

Mechanical analog computers started appearing in the first century and were later used in the medieval era for astronomical calculations. In World War II, mechanical analog computers were used for specialized military applications such as calculating torpedo aiming. During this time the first electronic digital computers were developed. Originally they were the size of a large room, consuming as much power as several hundred modern personal computers (PCs).[1]

Modern computers based on integrated circuits are millions to billions of times more capable than the early machines, and occupy a fraction of the space.[2] Computers are small enough to fit into mobile devices, and mobile computers can be powered by small batteries. Personal computers in their various forms are icons of the Information Age and are generally considered as \"computers\". However, the embedded computers found in many devices from MP3 players to fighter aircraft and from electronic toys to industrial robots are the most numerous.";

$text4="JPSNoZIU=nW=D=CIQIUDM=NoUNPWI=AI1nJI=ZFDZ=JDQ=GI=NUPCUDSSIA=ZP=JDUU2=PoZ=D=WIZ=PB=DUnZFSIZnJ=PU=MPCnJDM=PNIUDZnPQW=DoZPSDZnJDMM2*=wnQJI=D=WIToIQJI=PB=PNIUDZnPQW=JDQ=GI=UIDAnM2=JFDQCIA,=ZFI=JPSNoZIU=JDQ=WPM1I=SPUI=ZFDQ=PQI=OnQA=PB=NUPGMIS* fPQ1IQZnPQDMM2,=D=JPSNoZIU=JPQWnWZW=PB=DZ=MIDWZ=PQI=NUPJIWWnQC=IMISIQZ,=Z2NnJDMM2=D=JIQZUDM=NUPJIWWnQC=oQnZ=(fs3),=DQA=WPSI=BPUS=PB=SISPU2*=xFI=NUPJIWWnQC=IMISIQZ=JDUUnIW=PoZ=DUnZFSIZnJ=DQA=MPCnJ=PNIUDZnPQW,=DQA=D=WIToIQJnQC=DQA=JPQZUPM=oQnZ=JDQ=JFDQCI=ZFI=PUAIU=PB=PNIUDZnPQW=nQ=UIWNPQWI=ZP=WZPUIA=nQBPUSDZnPQ*=sIUnNFIUDM=AI1nJIW=DMMP4=nQBPUSDZnPQ=ZP=GI=UIZUnI1IA=BUPS=DQ=IXZIUQDM=WPoUJI,=DQA=ZFI=UIWoMZ=PB=PNIUDZnPQW=WD1IA=DQA=UIZUnI1IA* dIJFDQnJDM=DQDMPC=JPSNoZIUW=WZDUZIA=DNNIDUnQC=nQ=ZFI=BnUWZ=JIQZoU2=DQA=4IUI=MDZIU=oWIA=nQ=ZFI=SIAnI1DM=IUD=BPU=DWZUPQPSnJDM=JDMJoMDZnPQW*=EQ=5PUMA=5DU=EE,=SIJFDQnJDM=DQDMPC=JPSNoZIUW=4IUI=oWIA=BPU=WNIJnDMnYIA=SnMnZDU2=DNNMnJDZnPQW=WoJF=DW=JDMJoMDZnQC=ZPUNIAP=DnSnQC*=ioUnQC=ZFnW=ZnSI=ZFI=BnUWZ=IMIJZUPQnJ=AnCnZDM=JPSNoZIUW=4IUI=AI1IMPNIA*=hUnCnQDMM2=ZFI2=4IUI=ZFI=WnYI=PB=D=MDUCI=UPPS,=JPQWoSnQC=DW=SoJF=NP4IU=DW=WI1IUDM=FoQAUIA=SPAIUQ=NIUWPQDM=JPSNoZIUW=(sfW)*[H] dPAIUQ=JPSNoZIUW=GDWIA=PQ=nQZICUDZIA=JnUJonZW=DUI=SnMMnPQW=ZP=GnMMnPQW=PB=ZnSIW=SPUI=JDNDGMI=ZFDQ=ZFI=IDUM2=SDJFnQIW,=DQA=PJJoN2=D=BUDJZnPQ=PB=ZFI=WNDJI*[R]=fPSNoZIUW=DUI=WSDMM=IQPoCF=ZP=BnZ=nQZP=SPGnMI=AI1nJIW,=DQA=SPGnMI=JPSNoZIUW=JDQ=GI=NP4IUIA=G2=WSDMM=GDZZIUnIW*=sIUWPQDM=JPSNoZIUW=nQ=ZFInU=1DUnPoW=BPUSW=DUI=nJPQW=PB=ZFI=EQBPUSDZnPQ=aCI=DQA=DUI=CIQIUDMM2=JPQWnAIUIA=DW=%JPSNoZIUW%*=pP4I1IU,=ZFI=ISGIAAIA=JPSNoZIUW=BPoQA=nQ=SDQ2=AI1nJIW=BUPS=dsL=NMD2IUW=ZP=BnCFZIU=DnUJUDBZ=DQA=BUPS=IMIJZUPQnJ=ZP2W=ZP=nQAoWZUnDM=UPGPZW=DUI=ZFI=SPWZ=QoSIUPoW*
JPSNoZIU=nW=D=CIQIUDM=NoUNPWI=AI1nJI=ZFDZ=JDQ=GI=NUPCUDSSIA=ZP=JDUU2=PoZ=D=WIZ=PB=DUnZFSIZnJ=PU=MPCnJDM=PNIUDZnPQW=DoZPSDZnJDMM2.=wnQJI=D=WIToIQJI=PB=PNIUDZnPQW=JDQ=GI=UIDAnM2=JFDQCIA,=ZFI=JPSNoZIU=JDQ=WPM1I=SPUI=ZFDQ=PQI=OnQA=PB=NUPGMIS. fPQ1IQZnPQDMM2,=D=JPSNoZIU=JPQWnWZW=PB=DZ=MIDWZ=PQI=NUPJIWWnQC=IMISIQZ,=Z2NnJDMM2=D=JIQZUDM=NUPJIWWnQC=oQnZ=(fs3),=DQA=WPSI=BPUS=PB=SISPU2.=xFI=NUPJIWWnQC=IMISIQZ=JDUUnIW=PoZ=DUnZFSIZnJ=DQA=MPCnJ=PNIUDZnPQW,=DQA=D=WIToIQJnQC=DQA=JPQZUPM=oQnZ=JDQ=JFDQCI=ZFI=PUAIU=PB=PNIUDZnPQW=nQ=UIWNPQWI=ZP=WZPUIA=nQBPUSDZnPQ.=sIUnNFIUDM=AI1nJIW=DMMP4=nQBPUSDZnPQ=ZP=GI=UIZUnI1IA=BUPS=DQ=IXZIUQDM=WPoUJI,=DQA=ZFI=UIWoMZ=PB=PNIUDZnPQW=WD1IA=DQA=UIZUnI1IA. dIJFDQnJDM=DQDMPC=JPSNoZIUW=WZDUZIA=DNNIDUnQC=nQ=ZFI=BnUWZ=JIQZoU2=DQA=4IUI=MDZIU=oWIA=nQ=ZFI=SIAnI1DM=IUD=BPU=DWZUPQPSnJDM=JDMJoMDZnPQW.=EQ=5PUMA=5DU=EE,=SIJFDQnJDM=DQDMPC=JPSNoZIUW=4IUI=oWIA=BPU=WNIJnDMnYIA=SnMnZDU2=DNNMnJDZnPQW=WoJF=DW=JDMJoMDZnQC=ZPUNIAP=DnSnQC.=ioUnQC=ZFnW=ZnSI=ZFI=BnUWZ=IMIJZUPQnJ=AnCnZDM=JPSNoZIUW=4IUI=AI1IMPNIA.=hUnCnQDMM2=ZFI2=4IUI=ZFI=WnYI=PB=D=MDUCI=UPPS,=JPQWoSnQC=DW=SoJF=NP4IU=DW=WI1IUDM=FoQAUIA=SPAIUQ=NIUWPQDM=JPSNoZIUW=(sfW).[H] dPAIUQ=JPSNoZIUW=GDWIA=PQ=nQZICUDZIA=JnUJonZW=DUI=SnMMnPQW=ZP=GnMMnPQW=PB=ZnSIW=SPUI=JDNDGMI=ZFDQ=ZFI=IDUM2=SDJFnQIW,=DQA=PJJoN2=D=BUDJZnPQ=PB=ZFI=WNDJI.[R]=fPSNoZIUW=DUI=WSDMM=IQPoCF=ZP=BnZ=nQZP=SPGnMI=AI1nJIW,=DQA=SPGnMI=JPSNoZIUW=JDQ=GI=NP4IUIA=G2=WSDMM=GDZZIUnIW.=sIUWPQDM=JPSNoZIUW=nQ=ZFInU=1DUnPoW=BPUSW=DUI=nJPQW=PB=ZFI=EQBPUSDZnPQ=aCI=DQA=DUI=CIQIUDMM2=JPQWnAIUIA=DW=JPSNoZIUW=pP4I1IU,=ZFI=ISGIAAIA=JPSNoZIUW=BPoQA=nQ=SDQ2=AI1nJIW=BUPS=dsL=NMD2IUW=ZP=BnCFZIU=DnUJUDBZ=DQA=BUPS=IMIJZUPQnJ=ZP2W=ZP=nQAoWZUnDM=UPGPZW=DUI=ZFI=SPWZ=QoSIUPoW.";
echo "<br>";		
echo "<strong>Teks = </strong>";
echo "<br>";		
echo $text3;
echo "<br>";		
echo "<strong>Encript = </strong>  ";
echo "<br>".ec($text3,$key);
echo "<br>";
echo $text4;
echo "<br>";
echo "<strong>Decript =</strong>   ";
echo "<br>".dc($text4,$key);


?>
</body>
</html>
