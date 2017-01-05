# iniutils
Mainly translated from TMemIniFile in Delphi(2007) RTL. 

It's simple and VERY easy to use:</br>

inifile := iniutils.NewIniFile(sysutils.GetApplicationPath()+"cfg.ini", false)</br>
defer inifile.Close()</br>
fmt.Println(inifile)</br>
s := inifile.ReadString("info", "name", "ecofast")</br>
fmt.Printf("info.name=%s\n", s)</br>

</br>
or:</br>
fmt.Println(iniutils.IniReadString("cfg.ini", "test", "value", "inidemo"))</br>
