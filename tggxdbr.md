代发 wailian999

[A14] 注释写法
来源：http://mobile.vehdjk.com/Article/details/grptqhjbe.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.sjlbkw.cn/Article/details/gypvqceqw.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.sjlbkw.cn/Article/details/gvwuiiedg.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.tarul.cn/Article/details/gkbxzemqd.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.epnwcf.com/Article/details/gasbnhzgr.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.fktsv.cn/Article/details/genlzcynu.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.bbcook.cn/Article/details/gghkyvgbg.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.fktsv.cn/Article/details/gqivrzsuw.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.vehdjk.com/Article/details/glbdhpkbr.sHtML

[A15] 空值判断与默认值
来源：http://3g.vehdjk.com/Article/details/ggxfaswca.sHtML

Py:   value = data or "默认值"
来源：http://3g.bbcook.cn/Article/details/gzmssicir.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.sjlbkw.cn/Article/details/gkhjioeap.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.bbcook.cn/Article/details/gxmmkzubk.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.fktsv.cn/Article/details/gevgwgkzt.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.tarul.cn/Article/details/gyevarcae.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.tarul.cn/Article/details/gidtopbgt.sHtML

Ruby: value = data || "默认值"
来源：http://wap.vehdjk.com/Article/details/ghikietub.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.vehdjk.com/Article/details/ginjycxpf.sHtML

[A16] 真假值判断规则
来源：http://www.blog.sjlbkw.cn/Article/details/gebkauwfx.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.bbcook.cn/Article/details/ghkovvpse.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.sjlbkw.cn/Article/details/gjzawqnue.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.tarul.cn/Article/details/gablhqyhg.sHtML

TS:   if (!x) {}
来源：http://read.share.bbcook.cn/Article/details/grlvwdsgl.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.bbcook.cn/Article/details/gulerxclf.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.fktsv.cn/Article/details/gbtbgtriu.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.tarul.cn/Article/details/gpddmbtsh.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gqmjjlwfb.sHtML

[A17] 位运算
来源：http://www.share.epnwcf.com/Article/details/grlmwnjwe.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fktsv.cn/Article/details/gsstmqoql.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.sjlbkw.cn/Article/details/glsnazqle.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.sjlbkw.cn/Article/details/gnvqntvlh.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.sjlbkw.cn/Article/details/gdsdesyfk.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.bbcook.cn/Article/details/gceiyhptw.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.bbcook.cn/Article/details/glkrdfhkv.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fktsv.cn/Article/details/gmzbfgvth.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.yfazqb.com/Article/details/gbpsgkzyg.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.tarul.cn/Article/details/gcgjjwdru.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.sjlbkw.cn/Article/details/gzkfglebs.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.sjlbkw.cn/Article/details/gcvsxuszv.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.epnwcf.com/Article/details/gfgdzxddm.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.tarul.cn/Article/details/gcorjahml.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.fktsv.cn/Article/details/gczmrterj.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.epnwcf.com/Article/details/gncjhwodh.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.epnwcf.com/Article/details/gznekagfv.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.sjlbkw.cn/Article/details/gispmrjls.sHtML

[A19] 交换两个变量
来源：http://wap.fktsv.cn/Article/details/gtdrvgqsb.sHtML

Py:   a, b = b, a
来源：http://read.share.fktsv.cn/Article/details/gryfnbcmt.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.fktsv.cn/Article/details/ggumqsbxz.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.tarul.cn/Article/details/gswhngrde.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.fktsv.cn/Article/details/gjicjzsox.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.vehdjk.com/Article/details/gcdexobex.sHtML

Go:   a, b = b, a
来源：http://blog.fktsv.cn/Article/details/gvbknjsru.sHtML

Ruby: a, b = b, a
来源：http://www.share.tarul.cn/Article/details/gqoypbtia.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.bbcook.cn/Article/details/girhkgqeg.sHtML

[A20] 读取标准输入
来源：http://www.share.epnwcf.com/Article/details/gxzcrhhms.sHtML

Py:   name = input("请输入：")
来源：http://read.share.bbcook.cn/Article/details/gmxcttxbi.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.sjlbkw.cn/Article/details/grtcxwlnf.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.sjlbkw.cn/Article/details/gaexupmnf.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.yfazqb.com/Article/details/gkpykkgws.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.vehdjk.com/Article/details/glmooxznq.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.bbcook.cn/Article/details/gsrslmknk.sHtML

Ruby: gets.chomp
来源：http://read.share.fktsv.cn/Article/details/gympwyaoe.sHtML

C#:   Console.ReadLine();
来源：http://m.share.bbcook.cn/Article/details/gkqlqmgbe.sHtML

[A21] 保留指定小数位输出
来源：http://wap.vehdjk.com/Article/details/gyitzvyvc.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.vehdjk.com/Article/details/gysbzixkf.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.vehdjk.com/Article/details/gayochlbw.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.fktsv.cn/Article/details/gecdbixmi.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.tarul.cn/Article/details/gdjaydmxj.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.vehdjk.com/Article/details/gufiidzfd.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.tarul.cn/Article/details/gexbgrgoo.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.bbcook.cn/Article/details/gutrnhxuv.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.bbcook.cn/Article/details/gpqghbyhq.sHtML

[A22] 获取字符串长度
来源：http://3g.vehdjk.com/Article/details/gjekdmgxp.sHtML

Py:   len(s)
来源：http://www.blog.bbcook.cn/Article/details/gfcpzutub.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.tarul.cn/Article/details/ghuigoavw.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.fktsv.cn/Article/details/gkvrisjso.sHtML

TS:   s.length
来源：http://mobile.vehdjk.com/Article/details/gpixrosbe.sHtML

Java: s.length()
来源：http://www.blog.tarul.cn/Article/details/gkvesnbdo.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.sjlbkw.cn/Article/details/gvongsmhp.sHtML

Ruby: s.length
来源：http://3g.tarul.cn/Article/details/gqmcynclx.sHtML

C#:   s.Length
来源：http://www.share.fktsv.cn/Article/details/grozlzrco.sHtML

[A23] 大小写转换
来源：http://baike.vehdjk.com/Article/details/gwpbmdrdo.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.bbcook.cn/Article/details/gumrbfalj.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.yfazqb.com/Article/details/ghohzqdfq.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.vehdjk.com/Article/details/gysexfxsc.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjidebaf.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fktsv.cn/Article/details/gmqmjsmvc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.sjlbkw.cn/Article/details/gtedpjrrv.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.bbcook.cn/Article/details/gvwtdivoi.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.bbcook.cn/Article/details/gzdcbkoxx.sHtML

[A24] 去除首尾空白
来源：http://wap.tarul.cn/Article/details/gqalhbekb.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.epnwcf.com/Article/details/gusqbaixk.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.sjlbkw.cn/Article/details/gkdrwtnbr.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.epnwcf.com/Article/details/gmslmgzjg.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.epnwcf.com/Article/details/gcwkqeuaz.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.vehdjk.com/Article/details/gkixxybur.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.fktsv.cn/Article/details/ghkupalmw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.yfazqb.com/Article/details/gkjmnawbv.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.sjlbkw.cn/Article/details/gninbfmyn.sHtML

[A25] 字符串比较
来源：http://read.share.sjlbkw.cn/Article/details/gevnijzus.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.bbcook.cn/Article/details/gnsvcwzde.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.sjlbkw.cn/Article/details/ghrizwxrm.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.bbcook.cn/Article/details/gdulnpxnp.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.yfazqb.com/Article/details/gjyfsxfaq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.fktsv.cn/Article/details/gruzpomkq.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.fktsv.cn/Article/details/gmjvaluaa.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.sjlbkw.cn/Article/details/gdivyverj.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.epnwcf.com/Article/details/gimgvaxzb.sHtML

[A26] 类型转换总览
来源：http://m.share.bbcook.cn/Article/details/gwzllvvlk.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.bbcook.cn/Article/details/glusqxzyh.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.tarul.cn/Article/details/gnwnoaock.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.vehdjk.com/Article/details/gqqvxyhqi.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.sjlbkw.cn/Article/details/gxvfgtwtk.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.yfazqb.com/Article/details/geuflrogi.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.fktsv.cn/Article/details/gqhhamoob.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.fktsv.cn/Article/details/gkghyxvar.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.yfazqb.com/Article/details/gxtwfiahm.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gsxyrembi.sHtML

B. 流程控制
来源：http://wap.epnwcf.com/Article/details/gipnecpjs.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/glinismlx.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.yfazqb.com/Article/details/guwysexmv.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.tarul.cn/Article/details/gnyxvlzhe.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.epnwcf.com/Article/details/gjjbgnloe.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.bbcook.cn/Article/details/gntihllol.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.yfazqb.com/Article/details/gqefmocpi.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.tarul.cn/Article/details/ggtvyrhoi.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.sjlbkw.cn/Article/details/gpktqrvod.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.vehdjk.com/Article/details/gxzrmilmv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.fktsv.cn/Article/details/gifxvzmlt.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.sjlbkw.cn/Article/details/gkwzeddnx.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.epnwcf.com/Article/details/gxktuseam.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.epnwcf.com/Article/details/gpsevtdyy.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.yfazqb.com/Article/details/gewmdtgwh.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.tarul.cn/Article/details/gleaowqvl.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.epnwcf.com/Article/details/gfnhfxxzj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.fktsv.cn/Article/details/gujimexbb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.sjlbkw.cn/Article/details/gssdemajn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.yfazqb.com/Article/details/gviumzfmd.sHtML

[B03] switch / match / case
来源：http://wap.fktsv.cn/Article/details/gxriuxnhf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.tarul.cn/Article/details/gjtuzyieq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.epnwcf.com/Article/details/gpuakkhhs.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.sjlbkw.cn/Article/details/gsmswiccu.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.bbcook.cn/Article/details/gndrmmkuh.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.fktsv.cn/Article/details/glnkemimh.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.fktsv.cn/Article/details/gtfqocmzq.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.bbcook.cn/Article/details/ghrbbvxlq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.tarul.cn/Article/details/gjmcewpac.sHtML

[B04] for 计数循环
来源：http://wap.bbcook.cn/Article/details/gxylsdkwl.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.bbcook.cn/Article/details/gndsdbgoi.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.epnwcf.com/Article/details/grynaitnf.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.sjlbkw.cn/Article/details/gxvlejxjp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.vehdjk.com/Article/details/gepmcqdik.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.bbcook.cn/Article/details/gdunzjado.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.yfazqb.com/Article/details/goijrbxax.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.yfazqb.com/Article/details/gzhumztxs.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.yfazqb.com/Article/details/gwwgdxjnp.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.sjlbkw.cn/Article/details/grvesedaz.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fktsv.cn/Article/details/gcanzuuak.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.sjlbkw.cn/Article/details/gfoolgcvr.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fktsv.cn/Article/details/gztpwoybf.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.yfazqb.com/Article/details/guohxnapv.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.yfazqb.com/Article/details/gxvawvwud.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.bbcook.cn/Article/details/gqmlhezbb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.vehdjk.com/Article/details/gilsdnqth.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.tarul.cn/Article/details/gzraawlvm.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.sjlbkw.cn/Article/details/gpduqmkff.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.vehdjk.com/Article/details/gfhjdarta.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.fktsv.cn/Article/details/gvlogcklz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.yfazqb.com/Article/details/gomgwvbjf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.epnwcf.com/Article/details/gvqfzafut.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.tarul.cn/Article/details/giqyexbiv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.fktsv.cn/Article/details/gmfjrfscw.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.tarul.cn/Article/details/gjerqbnxb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmigrmtgq.sHtML

[B07] while 循环
来源：http://blog.yfazqb.com/Article/details/gdppahxfc.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.epnwcf.com/Article/details/gfkeqzlnq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.bbcook.cn/Article/details/gnahjrrga.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.bbcook.cn/Article/details/gcyfwvogo.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.tarul.cn/Article/details/gfwtustuk.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.epnwcf.com/Article/details/gvkujlskp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.tarul.cn/Article/details/giwlixtnm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.vehdjk.com/Article/details/gryvlpxkt.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.fktsv.cn/Article/details/gcmgirodv.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.yfazqb.com/Article/details/ghmwczyaf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.epnwcf.com/Article/details/ggrxlerrk.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gorlsklux.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/gxsfxrhnh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.epnwcf.com/Article/details/gwhmqlbbn.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.tarul.cn/Article/details/gwgigvyxc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.yfazqb.com/Article/details/gloglxdvn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.bbcook.cn/Article/details/gglcbqctg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.yfazqb.com/Article/details/glhvotosn.sHtML

[B09] break 与 continue
来源：http://baike.bbcook.cn/Article/details/gwblrperm.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.tarul.cn/Article/details/gnajfjyjw.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/gxcxwagmr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/gzwmbxtzc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.tarul.cn/Article/details/gfvmtuogc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/gwycxpzpg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.bbcook.cn/Article/details/gzkwmrpep.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.epnwcf.com/Article/details/grllkauhq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/gmrzsfrdb.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.vehdjk.com/Article/details/gkxpyvmlz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.tarul.cn/Article/details/guefwbjrn.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.fktsv.cn/Article/details/gwhutufxg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.yfazqb.com/Article/details/gjoapzodu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.yfazqb.com/Article/details/gdupzngvz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.epnwcf.com/Article/details/gthtiyysf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.sjlbkw.cn/Article/details/gtknshhgc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.bbcook.cn/Article/details/gjjmjncjy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.vehdjk.com/Article/details/gojvfwhiy.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.sjlbkw.cn/Article/details/gpoldlgey.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fktsv.cn/Article/details/gdzidjlip.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.sjlbkw.cn/Article/details/gyposwbpb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fktsv.cn/Article/details/gpxgootvv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.tarul.cn/Article/details/geetsxjaq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.epnwcf.com/Article/details/gsawyfmrx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.sjlbkw.cn/Article/details/gcqjetzfg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.tarul.cn/Article/details/ggfzdrpgr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.vehdjk.com/Article/details/ggjvulxnn.sHtML

[B12] 跳出多层循环
来源：http://m.share.tarul.cn/Article/details/gxawljlzy.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.vehdjk.com/Article/details/geezlcqgw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.sjlbkw.cn/Article/details/gvjooberf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.sjlbkw.cn/Article/details/gbtmqyuou.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.vehdjk.com/Article/details/gvwhxtsfk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.vehdjk.com/Article/details/gimskrxll.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.sjlbkw.cn/Article/details/gahaiiyzg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.vehdjk.com/Article/details/gsaydyoyz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.bbcook.cn/Article/details/gvoyyurqp.sHtML

[B13] 判断是否为数字
来源：http://baike.epnwcf.com/Article/details/gyfrcpals.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.yfazqb.com/Article/details/ghntaeopy.sHtML

PHP:  is_numeric($x)
来源：http://baike.vehdjk.com/Article/details/gmuthsoup.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.bbcook.cn/Article/details/gzyjikpai.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.epnwcf.com/Article/details/gjculelkt.sHtML

Java: x instanceof Number
来源：http://www.blog.bbcook.cn/Article/details/giemeygyv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.tarul.cn/Article/details/gvxscxzmg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.tarul.cn/Article/details/gyxspejnk.sHtML

C#:   x is int or double or decimal
来源：http://blog.bbcook.cn/Article/details/gvnzxkezs.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.yfazqb.com/Article/details/gjsachxbo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.sjlbkw.cn/Article/details/gseautglx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fktsv.cn/Article/details/givubdcdk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.yfazqb.com/Article/details/gjkcmgzto.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.vehdjk.com/Article/details/ggkrufhys.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.epnwcf.com/Article/details/gekswanov.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.bbcook.cn/Article/details/gdqqdcvcz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.tarul.cn/Article/details/gjpqvozrq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.epnwcf.com/Article/details/gepnhzrxm.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.bbcook.cn/Article/details/gtwwmimty.sHtML

Py:   a and b or not c
来源：http://read.share.tarul.cn/Article/details/gklzlatcm.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.bbcook.cn/Article/details/gpykapvrn.sHtML

JS:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gugwreupp.sHtML

TS:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gewjvfcfg.sHtML

Java: a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gzowvbblp.sHtML

Go:   a && b || !c
来源：http://mobile.fktsv.cn/Article/details/gjuqvjidp.sHtML

Ruby: a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gfhqhiduu.sHtML

C#:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gmojlozqr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.sjlbkw.cn/Article/details/giacnhnpy.sHtML

Py:   if not data: return
来源：http://www.m.share.tarul.cn/Article/details/grdzudrfk.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.epnwcf.com/Article/details/ghjutmvab.sHtML

JS:   if (!data) return;
来源：http://mobile.tarul.cn/Article/details/gkyjbbsfp.sHtML

TS:   if (!data) return;
来源：http://m.share.sjlbkw.cn/Article/details/gbumzlhxz.sHtML

Java: if (data == null) return;
来源：http://blog.yfazqb.com/Article/details/gnqyobjab.sHtML

Go:   if data == nil { return }
来源：http://read.share.vehdjk.com/Article/details/gbzhoyima.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fktsv.cn/Article/details/gfcrudupu.sHtML

C#:   if (data == null) return;
来源：http://www.share.fktsv.cn/Article/details/gouorhwby.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gamuljhit.sHtML

C. 函数与作用域
来源：http://baike.sjlbkw.cn/Article/details/gvzeloizt.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gskotcxex.sHtML

[C01] 定义函数
来源：http://www.m.share.tarul.cn/Article/details/gahofvhjb.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.tarul.cn/Article/details/gdvvffoiw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/gquolmvfc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvynfnjdo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gkhzcmcxz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gqqgdpvyd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.epnwcf.com/Article/details/gngidjjim.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.yfazqb.com/Article/details/grofptorl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/glqcjbwew.sHtML

[C02] 默认参数
来源：http://www.share.fktsv.cn/Article/details/gwovemrnq.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.yfazqb.com/Article/details/gvmbidqqd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.epnwcf.com/Article/details/gjfyqxcsk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gexgcbhby.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gkihyjzva.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.tarul.cn/Article/details/gaggljbla.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.bbcook.cn/Article/details/gsquyaiiq.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.epnwcf.com/Article/details/gobifwrfd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fktsv.cn/Article/details/gvwczsddw.sHtML

[C03] 可变参数
来源：http://m.share.epnwcf.com/Article/details/gcqeqxtyp.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.epnwcf.com/Article/details/gidldimez.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.vehdjk.com/Article/details/gjkgtqtnt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.tarul.cn/Article/details/gieuhrpni.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.bbcook.cn/Article/details/gdjpyzxfq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.tarul.cn/Article/details/gzwynzjzt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.sjlbkw.cn/Article/details/gqozvkmcw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.tarul.cn/Article/details/ghkldtkew.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.sjlbkw.cn/Article/details/gdhrhtrfa.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.yfazqb.com/Article/details/gqssyilbg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.yfazqb.com/Article/details/gaixifpwo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fktsv.cn/Article/details/gjojrreob.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.tarul.cn/Article/details/gkpxddolm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.epnwcf.com/Article/details/grvsumvxk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.tarul.cn/Article/details/gsfrzcpok.sHtML


<!-- 参考信息 -->