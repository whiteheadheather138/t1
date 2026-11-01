代发 wailian999

[A14] 注释写法
来源：http://www.m.share.sjlbkw.cn/Article/details/gxfnofjfc.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.yfazqb.com/Article/details/gaipjkplv.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.sjlbkw.cn/Article/details/galefsfyi.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.fktsv.cn/Article/details/gszwnkxdi.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.tarul.cn/Article/details/gvrssrakz.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.yfazqb.com/Article/details/gbqhsqfss.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.yfazqb.com/Article/details/gfawneebr.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.yfazqb.com/Article/details/gztrdwyzx.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.tarul.cn/Article/details/gwzbjhiea.sHtML

[A15] 空值判断与默认值
来源：http://mobile.tarul.cn/Article/details/godthuiub.sHtML

Py:   value = data or "默认值"
来源：http://www.share.bbcook.cn/Article/details/gwbtpwkec.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.fktsv.cn/Article/details/gorjkhoyf.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.epnwcf.com/Article/details/glrssuogr.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.yfazqb.com/Article/details/gljhgcerx.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.epnwcf.com/Article/details/gxwzacafl.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.tarul.cn/Article/details/ghbcyjwxn.sHtML

Ruby: value = data || "默认值"
来源：http://blog.tarul.cn/Article/details/gfnwrlihr.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.fktsv.cn/Article/details/gzjpxzlhg.sHtML

[A16] 真假值判断规则
来源：http://www.share.sjlbkw.cn/Article/details/ghuwidsfg.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.fktsv.cn/Article/details/gzbuvjnrv.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.sjlbkw.cn/Article/details/glfqmmccb.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.tarul.cn/Article/details/gcajpqjoz.sHtML

TS:   if (!x) {}
来源：http://www.blog.epnwcf.com/Article/details/gimpbueyx.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.vehdjk.com/Article/details/gjjxhzdac.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.fktsv.cn/Article/details/gphrxvtlt.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtkcfuoc.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gghzekndp.sHtML

[A17] 位运算
来源：http://read.share.sjlbkw.cn/Article/details/gljwlpmtk.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.tarul.cn/Article/details/giqyllcfu.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.bbcook.cn/Article/details/gaovscurd.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.sjlbkw.cn/Article/details/guxvlyzke.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.fktsv.cn/Article/details/ggcqcubsv.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.tarul.cn/Article/details/gyeevedpc.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.sjlbkw.cn/Article/details/ggbjfmjwx.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.bbcook.cn/Article/details/gkgzyaaxj.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.tarul.cn/Article/details/goumqvgjl.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.fktsv.cn/Article/details/gqliyvwjk.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.yfazqb.com/Article/details/gdpjvrugq.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.yfazqb.com/Article/details/gwzxflnoh.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.fktsv.cn/Article/details/gvktzlqyz.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.bbcook.cn/Article/details/giiffpgnh.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.tarul.cn/Article/details/gljzbruth.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.tarul.cn/Article/details/gpseelpyl.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.yfazqb.com/Article/details/gzvfnfpnk.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.yfazqb.com/Article/details/gjjjizauf.sHtML

[A19] 交换两个变量
来源：http://wap.yfazqb.com/Article/details/geinaqjxf.sHtML

Py:   a, b = b, a
来源：http://wap.fktsv.cn/Article/details/gegvoxbkd.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.sjlbkw.cn/Article/details/ggseexwiu.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.epnwcf.com/Article/details/gvrgtnsoi.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.tarul.cn/Article/details/gjmcpufkg.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.epnwcf.com/Article/details/ggubjrrgq.sHtML

Go:   a, b = b, a
来源：http://blog.epnwcf.com/Article/details/gkqbnrman.sHtML

Ruby: a, b = b, a
来源：http://mobile.epnwcf.com/Article/details/geadpobzi.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.yfazqb.com/Article/details/gqqdsyrkm.sHtML

[A20] 读取标准输入
来源：http://blog.bbcook.cn/Article/details/gqwhzoekz.sHtML

Py:   name = input("请输入：")
来源：http://3g.fktsv.cn/Article/details/gegwnxpgd.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.bbcook.cn/Article/details/ghbjrnajb.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.bbcook.cn/Article/details/gdmlihapr.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.fktsv.cn/Article/details/ggfzfstku.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.epnwcf.com/Article/details/gphurdaix.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.sjlbkw.cn/Article/details/gkvaqbjqm.sHtML

Ruby: gets.chomp
来源：http://blog.yfazqb.com/Article/details/gminyrqzg.sHtML

C#:   Console.ReadLine();
来源：http://mobile.epnwcf.com/Article/details/gdmhxbxqd.sHtML

[A21] 保留指定小数位输出
来源：http://blog.yfazqb.com/Article/details/girvtbiwv.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.yfazqb.com/Article/details/geivdevsp.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.yfazqb.com/Article/details/gsgqcbclj.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.epnwcf.com/Article/details/gvkhehbfa.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.tarul.cn/Article/details/gyocrplgv.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.fktsv.cn/Article/details/grerjzzww.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.sjlbkw.cn/Article/details/gzwqfepca.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.fktsv.cn/Article/details/gtfnqfnzi.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.sjlbkw.cn/Article/details/gskckvzwl.sHtML

[A22] 获取字符串长度
来源：http://wap.vehdjk.com/Article/details/gqltdgcvc.sHtML

Py:   len(s)
来源：http://mobile.epnwcf.com/Article/details/gnvjkakfa.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.fktsv.cn/Article/details/gijpuoukl.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.yfazqb.com/Article/details/gaftkfczu.sHtML

TS:   s.length
来源：http://3g.fktsv.cn/Article/details/gxrvjybwq.sHtML

Java: s.length()
来源：http://blog.tarul.cn/Article/details/gldhmfpgz.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.sjlbkw.cn/Article/details/godwhbmks.sHtML

Ruby: s.length
来源：http://www.share.tarul.cn/Article/details/gzcfkkiti.sHtML

C#:   s.Length
来源：http://www.share.tarul.cn/Article/details/gjvezhewj.sHtML

[A23] 大小写转换
来源：http://baike.yfazqb.com/Article/details/gxojkugjm.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.fktsv.cn/Article/details/gonzcjfbs.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.tarul.cn/Article/details/gfewlngnu.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.epnwcf.com/Article/details/grnwvibpl.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.vehdjk.com/Article/details/gslhhtigl.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.bbcook.cn/Article/details/gsszysfqm.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.vehdjk.com/Article/details/glodlxpal.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.bbcook.cn/Article/details/gjuxfyjlx.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.fktsv.cn/Article/details/gvjwexonc.sHtML

[A24] 去除首尾空白
来源：http://blog.bbcook.cn/Article/details/gagcmvaqf.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.epnwcf.com/Article/details/gweroaykt.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.tarul.cn/Article/details/gyxfubgws.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fktsv.cn/Article/details/glravvigg.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.tarul.cn/Article/details/gguycctya.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.sjlbkw.cn/Article/details/gafnxevqz.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.tarul.cn/Article/details/gqnbokpao.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.vehdjk.com/Article/details/gdzlqdloy.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.fktsv.cn/Article/details/gqnikxzwz.sHtML

[A25] 字符串比较
来源：http://blog.sjlbkw.cn/Article/details/grvktoupx.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.epnwcf.com/Article/details/grysvcfqd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.tarul.cn/Article/details/gpmmebwxy.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.sjlbkw.cn/Article/details/gvjptgisv.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.tarul.cn/Article/details/gfhljsedr.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.tarul.cn/Article/details/gepwxlamw.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.yfazqb.com/Article/details/gqghxmmuz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.bbcook.cn/Article/details/gvbwzpphc.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.vehdjk.com/Article/details/gazlcwnrt.sHtML

[A26] 类型转换总览
来源：http://mobile.yfazqb.com/Article/details/gbvvluefb.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.fktsv.cn/Article/details/glmbbuxoq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.bbcook.cn/Article/details/gohmzfxwb.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.bbcook.cn/Article/details/gaiprlpse.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.bbcook.cn/Article/details/ggdkxquxh.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.vehdjk.com/Article/details/gpbanigis.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.sjlbkw.cn/Article/details/gfzqmueym.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.yfazqb.com/Article/details/gvhlffdpb.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.sjlbkw.cn/Article/details/gfyxitizb.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gvgvitqwg.sHtML

B. 流程控制
来源：http://www.share.yfazqb.com/Article/details/gorluhdel.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gqgeemgni.sHtML

[B01] 条件判断 if / else
来源：http://mobile.yfazqb.com/Article/details/gejuatvhg.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.bbcook.cn/Article/details/gxyeszykl.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.epnwcf.com/Article/details/gujghcqel.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/gmkxzkgib.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.bbcook.cn/Article/details/gdtoaejqi.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.tarul.cn/Article/details/gcyuyksjx.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvujumpop.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.bbcook.cn/Article/details/gnjlefqkw.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.bbcook.cn/Article/details/gooovuabr.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.sjlbkw.cn/Article/details/gzjtawkdg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.yfazqb.com/Article/details/gxpwzuwnu.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.sjlbkw.cn/Article/details/ghruwhohw.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.vehdjk.com/Article/details/gognvkfja.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.tarul.cn/Article/details/gzkbmsevl.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.tarul.cn/Article/details/gfapasrjp.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.epnwcf.com/Article/details/gucvujqmd.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.tarul.cn/Article/details/gxmyybxtm.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.vehdjk.com/Article/details/gkwzlljcx.sHtML

[B03] switch / match / case
来源：http://blog.yfazqb.com/Article/details/gbbkmulmy.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.vehdjk.com/Article/details/gzfqmcxxf.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.sjlbkw.cn/Article/details/gkuaeyilr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fktsv.cn/Article/details/gvskzckys.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fktsv.cn/Article/details/gprnwkouw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.bbcook.cn/Article/details/gpnbatxuc.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.tarul.cn/Article/details/gkorbpfdf.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.sjlbkw.cn/Article/details/guelldfme.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.epnwcf.com/Article/details/gcqpmkktw.sHtML

[B04] for 计数循环
来源：http://3g.tarul.cn/Article/details/gihcplvjj.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.yfazqb.com/Article/details/ggrbrsjhm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.tarul.cn/Article/details/ggvmchnij.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.epnwcf.com/Article/details/gpwxyneyn.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fktsv.cn/Article/details/gvhqevvgl.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.tarul.cn/Article/details/gtleneegv.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.sjlbkw.cn/Article/details/gkohueiah.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.sjlbkw.cn/Article/details/gnkqesucp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.bbcook.cn/Article/details/gtgmvwynq.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.fktsv.cn/Article/details/gsqfbautx.sHtML

Py:   for item in arr: print(item)
来源：http://blog.fktsv.cn/Article/details/gwobsspwm.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.sjlbkw.cn/Article/details/grhnexcym.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.yfazqb.com/Article/details/gzzgmadpe.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.sjlbkw.cn/Article/details/gryvluece.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.fktsv.cn/Article/details/gbfrdcsep.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.vehdjk.com/Article/details/gfcsbfvly.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.epnwcf.com/Article/details/gistjtmah.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.tarul.cn/Article/details/gpwiordkm.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.sjlbkw.cn/Article/details/ggkshvmmj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.tarul.cn/Article/details/ggqlskrqn.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.yfazqb.com/Article/details/gvppilmiu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fktsv.cn/Article/details/gtbagpacq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.epnwcf.com/Article/details/gzmmfrgei.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.epnwcf.com/Article/details/gwxumjbnw.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.sjlbkw.cn/Article/details/gmubrfsge.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.vehdjk.com/Article/details/gflixoiah.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.sjlbkw.cn/Article/details/gtebjjdwd.sHtML

[B07] while 循环
来源：http://wap.yfazqb.com/Article/details/gutwffbnb.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.vehdjk.com/Article/details/gbauqkcrc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.bbcook.cn/Article/details/gbhwbfbsw.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.vehdjk.com/Article/details/gcdmwzaxx.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.epnwcf.com/Article/details/gvyqxiqzx.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.fktsv.cn/Article/details/gztdgjiof.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.tarul.cn/Article/details/gyrgmavnf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.yfazqb.com/Article/details/gepfeilet.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.yfazqb.com/Article/details/gnnyuwlzy.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.epnwcf.com/Article/details/gltoaraml.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.sjlbkw.cn/Article/details/gisneaocx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.fktsv.cn/Article/details/gqtpqlzrb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gqgpiwpwk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/giefhacyl.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/ggvtnhyot.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.tarul.cn/Article/details/gaudfkizt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.epnwcf.com/Article/details/gplztcbhw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.sjlbkw.cn/Article/details/gekmfwbbq.sHtML

[B09] break 与 continue
来源：http://m.share.tarul.cn/Article/details/giqqzsofx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.yfazqb.com/Article/details/gnhkbvtdf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/gxlemzlwc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/gycojctyc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/ggdjhpgfr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/gngwxwtxg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.bbcook.cn/Article/details/goanysbdd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.sjlbkw.cn/Article/details/gknkgjwfs.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/ghwfccjsp.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.fktsv.cn/Article/details/gjofvjsgn.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fktsv.cn/Article/details/gkgzhaugp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.vehdjk.com/Article/details/gknqdhqxm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.epnwcf.com/Article/details/gmfjplklt.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.bbcook.cn/Article/details/guhcwethq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fktsv.cn/Article/details/gyfzfxcxk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.yfazqb.com/Article/details/gyrmuivsf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.bbcook.cn/Article/details/gxuaixwzv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.yfazqb.com/Article/details/ghpdghkso.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.yfazqb.com/Article/details/gvikrfyro.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.bbcook.cn/Article/details/gqrtqcgdp.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.tarul.cn/Article/details/gqxsjfhhp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.vehdjk.com/Article/details/gqgxqkqrj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.vehdjk.com/Article/details/ghjeylspn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.yfazqb.com/Article/details/gzhjbrwyf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.epnwcf.com/Article/details/gbiexnvlg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fktsv.cn/Article/details/ggnlfhyun.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.tarul.cn/Article/details/giqaozbrq.sHtML

[B12] 跳出多层循环
来源：http://www.blog.bbcook.cn/Article/details/guustkpfy.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.epnwcf.com/Article/details/gtbdywqag.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.bbcook.cn/Article/details/gvwqhicvx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/gbadzplwp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.epnwcf.com/Article/details/geitrhcon.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/gspavoiai.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.tarul.cn/Article/details/goxdpwsfd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.epnwcf.com/Article/details/guogaxmwv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.vehdjk.com/Article/details/gdnoaeomk.sHtML

[B13] 判断是否为数字
来源：http://www.share.vehdjk.com/Article/details/gulnktslq.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.tarul.cn/Article/details/gyiyopskw.sHtML

PHP:  is_numeric($x)
来源：http://3g.fktsv.cn/Article/details/gyhkouopt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fktsv.cn/Article/details/gxkxzhajf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.yfazqb.com/Article/details/ghoppweal.sHtML

Java: x instanceof Number
来源：http://read.share.fktsv.cn/Article/details/gadaaknme.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.tarul.cn/Article/details/gpxqmqgcj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.tarul.cn/Article/details/gixhxsqls.sHtML

C#:   x is int or double or decimal
来源：http://3g.bbcook.cn/Article/details/gzicmvhps.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fktsv.cn/Article/details/gkkwxhssv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.epnwcf.com/Article/details/gkupbskqw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.tarul.cn/Article/details/giyzofkyi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.vehdjk.com/Article/details/gpbbbizen.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.yfazqb.com/Article/details/gxsgnxedg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.tarul.cn/Article/details/gvjipdaxo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.sjlbkw.cn/Article/details/gzncnmxku.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.yfazqb.com/Article/details/guhfwoemu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fktsv.cn/Article/details/gjuqqixpr.sHtML

[B15] 布尔运算与取反
来源：http://www.share.tarul.cn/Article/details/geqbguied.sHtML

Py:   a and b or not c
来源：http://wap.epnwcf.com/Article/details/gysmadgbz.sHtML

PHP:  $a && $b || !$c
来源：http://3g.yfazqb.com/Article/details/grbysenbo.sHtML

JS:   a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gtkyuxrem.sHtML

TS:   a && b || !c
来源：http://3g.epnwcf.com/Article/details/ghccdphct.sHtML

Java: a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gjgvsbcrf.sHtML

Go:   a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gztflrdsf.sHtML

Ruby: a && b || !c
来源：http://www.share.fktsv.cn/Article/details/ghzrqcujq.sHtML

C#:   a && b || !c
来源：http://3g.epnwcf.com/Article/details/gqramcbnf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.yfazqb.com/Article/details/ghvjgisrr.sHtML

Py:   if not data: return
来源：http://www.blog.tarul.cn/Article/details/gfveexbbx.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.vehdjk.com/Article/details/gukkhzjof.sHtML

JS:   if (!data) return;
来源：http://mobile.fktsv.cn/Article/details/glmcvmrme.sHtML

TS:   if (!data) return;
来源：http://mobile.bbcook.cn/Article/details/gicmtzdbm.sHtML

Java: if (data == null) return;
来源：http://read.share.yfazqb.com/Article/details/gwmgyazfd.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.tarul.cn/Article/details/girvgzucy.sHtML

Ruby: return if data.nil?
来源：http://www.share.fktsv.cn/Article/details/ggihujuap.sHtML

C#:   if (data == null) return;
来源：http://m.share.bbcook.cn/Article/details/gdbvbgtik.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ghgpzvobc.sHtML

C. 函数与作用域
来源：http://3g.yfazqb.com/Article/details/gporcjqvv.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gnqevqdsr.sHtML

[C01] 定义函数
来源：http://m.share.yfazqb.com/Article/details/gzdqpxdtm.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.tarul.cn/Article/details/gdllefpcw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.epnwcf.com/Article/details/gfoaqmror.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gsyckeshk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gskuubheu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gkqunnkvq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.yfazqb.com/Article/details/gsvbdgwmj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.vehdjk.com/Article/details/gdtvvpeiw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gvrncbgyg.sHtML

[C02] 默认参数
来源：http://mobile.fktsv.cn/Article/details/ghwoevwee.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.epnwcf.com/Article/details/geyvckwhi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.bbcook.cn/Article/details/gotgjsglz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.vehdjk.com/Article/details/gclmovntr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gymaeifiy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.epnwcf.com/Article/details/gzylfqqhi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.sjlbkw.cn/Article/details/ghbbzqanu.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.tarul.cn/Article/details/gnzvexwlu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.vehdjk.com/Article/details/gjmcpsasl.sHtML

[C03] 可变参数
来源：http://www.share.fktsv.cn/Article/details/gzqoodgwa.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.tarul.cn/Article/details/gvhvvcecs.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fktsv.cn/Article/details/ggdebymtd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.epnwcf.com/Article/details/gyyqaffzs.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.tarul.cn/Article/details/gfncvnylt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.bbcook.cn/Article/details/gppjdreiv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.epnwcf.com/Article/details/gkbupepvu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.tarul.cn/Article/details/gcecykdxx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.yfazqb.com/Article/details/gttdmnysr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.bbcook.cn/Article/details/gqzyfvasl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.tarul.cn/Article/details/goxsyfkfc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fktsv.cn/Article/details/gavxdmqgz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fktsv.cn/Article/details/gucwbnjrp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.tarul.cn/Article/details/grzrkutus.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.tarul.cn/Article/details/gohrhtuyu.sHtML


<!-- 参考信息 -->