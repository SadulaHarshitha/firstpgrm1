# firstpgrm1
pluraltosingular
public pluraltosingular(string str)
{
	if(str.endsWith("ies"))
	return str.substr(0,str.length()-3)+"y";

	if(str.endsWith("ves"))
	return str.substr(0,str.length()-3)+"fe";

	if(str.endsWith("oes") || str.endsWith("ses") || str.endsWith("xes"))
	return 	str.substr(0,str.length()-2);

	if(str.endsWith("es"))
	return  str.substr(0,str.length()-2)+"is";
	
	return str.substr(0,str.length()-1);
}
