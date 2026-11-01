代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://wap.yfazqb.com/Article/details/giefckyah.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.epnwcf.com/Article/details/gfbegumkc.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.yfazqb.com/Article/details/gkhzczvnb.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.epnwcf.com/Article/details/gpvfnnytk.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.sjlbkw.cn/Article/details/gcppymibp.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.vehdjk.com/Article/details/gbdocpyoj.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.bbcook.cn/Article/details/guoloqcqz.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.bbcook.cn/Article/details/gfrxgcjmw.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.yfazqb.com/Article/details/gczhopmtk.sHtML

[A19] 交换两个变量
来源：http://wap.vehdjk.com/Article/details/ghpzxqqot.sHtML

Py:   a, b = b, a
来源：http://read.share.yfazqb.com/Article/details/gmhnhmpdl.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.sjlbkw.cn/Article/details/ghzrkfwnz.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.fktsv.cn/Article/details/gnclsuiyr.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.fktsv.cn/Article/details/gcipkuchu.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.sjlbkw.cn/Article/details/gdghqvqpw.sHtML

Go:   a, b = b, a
来源：http://mobile.yfazqb.com/Article/details/gqomdkcdk.sHtML

Ruby: a, b = b, a
来源：http://mobile.fktsv.cn/Article/details/gjxoordfi.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.epnwcf.com/Article/details/gkzkiqmfm.sHtML

[A20] 读取标准输入
来源：http://mobile.epnwcf.com/Article/details/gwsvwdxqt.sHtML

Py:   name = input("请输入：")
来源：http://baike.fktsv.cn/Article/details/guuqtrxfh.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.epnwcf.com/Article/details/gglmweyzk.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.epnwcf.com/Article/details/ggjioymxo.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.bbcook.cn/Article/details/gqltwajet.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.vehdjk.com/Article/details/gvlxdbttv.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.fktsv.cn/Article/details/gvnkkaxoz.sHtML

Ruby: gets.chomp
来源：http://www.share.epnwcf.com/Article/details/gzxhxehls.sHtML

C#:   Console.ReadLine();
来源：http://blog.epnwcf.com/Article/details/galussshr.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.fktsv.cn/Article/details/gsleyylqu.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.fktsv.cn/Article/details/gjetsodkc.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.yfazqb.com/Article/details/gvfsbqiqq.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.vehdjk.com/Article/details/gtqeeocuu.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.bbcook.cn/Article/details/guszyixqv.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.fktsv.cn/Article/details/gqflckeit.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.epnwcf.com/Article/details/gzwfluekq.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.epnwcf.com/Article/details/glgtfhbgq.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.epnwcf.com/Article/details/gtlyhpwzd.sHtML

[A22] 获取字符串长度
来源：http://3g.epnwcf.com/Article/details/gtaafhuqp.sHtML

Py:   len(s)
来源：http://www.blog.yfazqb.com/Article/details/gpykqeanm.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.epnwcf.com/Article/details/geuooqztc.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.fktsv.cn/Article/details/gxndtuero.sHtML

TS:   s.length
来源：http://www.m.share.epnwcf.com/Article/details/gcwmyrswx.sHtML

Java: s.length()
来源：http://3g.yfazqb.com/Article/details/glkapoaom.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.bbcook.cn/Article/details/gckqsydad.sHtML

Ruby: s.length
来源：http://baike.sjlbkw.cn/Article/details/gycjfhznn.sHtML

C#:   s.Length
来源：http://m.share.yfazqb.com/Article/details/gmskdmqie.sHtML

[A23] 大小写转换
来源：http://3g.fktsv.cn/Article/details/ggzwsrzcd.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.sjlbkw.cn/Article/details/gaykdlnnh.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.tarul.cn/Article/details/gxqlrwznz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.vehdjk.com/Article/details/gvmpyclqj.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.vehdjk.com/Article/details/gqdgbeadb.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.vehdjk.com/Article/details/glmwgmevm.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.fktsv.cn/Article/details/gyjkvzucq.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.yfazqb.com/Article/details/gpemapstp.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.sjlbkw.cn/Article/details/gwiqsuukz.sHtML

[A24] 去除首尾空白
来源：http://read.share.bbcook.cn/Article/details/gbuplpwbf.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.tarul.cn/Article/details/gvagifcop.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.epnwcf.com/Article/details/grmmbfjzy.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.sjlbkw.cn/Article/details/gstejxegp.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.bbcook.cn/Article/details/gpoexgzxk.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.vehdjk.com/Article/details/glinrpqog.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.epnwcf.com/Article/details/ghoynckqh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.sjlbkw.cn/Article/details/gzgehsfwz.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.tarul.cn/Article/details/ggmsophal.sHtML

[A25] 字符串比较
来源：http://www.m.share.tarul.cn/Article/details/gyvdbbmjg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.epnwcf.com/Article/details/gtxtzoevu.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.bbcook.cn/Article/details/gcjarcecb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fktsv.cn/Article/details/gltnwnyyd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fktsv.cn/Article/details/gpaooptdb.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fktsv.cn/Article/details/gowcoanlu.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.fktsv.cn/Article/details/gqqumwsyc.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.yfazqb.com/Article/details/gdafvowxt.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.tarul.cn/Article/details/gwztxltxd.sHtML

[A26] 类型转换总览
来源：http://www.blog.fktsv.cn/Article/details/gqohpxwnj.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.tarul.cn/Article/details/gewtmvafd.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.sjlbkw.cn/Article/details/gddmectkz.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.sjlbkw.cn/Article/details/gaxggttvv.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.sjlbkw.cn/Article/details/gpffkllno.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.fktsv.cn/Article/details/gpumvyziu.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.sjlbkw.cn/Article/details/gccfsnync.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.vehdjk.com/Article/details/ghinrmbab.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.yfazqb.com/Article/details/gcfvowlbm.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gpualnkgk.sHtML

B. 流程控制
来源：http://www.share.bbcook.cn/Article/details/gcxkblhiv.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gctnlswdy.sHtML

[B01] 条件判断 if / else
来源：http://blog.tarul.cn/Article/details/gdufrzofw.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.yfazqb.com/Article/details/gejootgfe.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.tarul.cn/Article/details/grkkuehln.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/gkoramidr.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fktsv.cn/Article/details/gmogmodpr.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.sjlbkw.cn/Article/details/gyziqxvfc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.epnwcf.com/Article/details/giiqjktnw.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.epnwcf.com/Article/details/gtartokzg.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.vehdjk.com/Article/details/ggjgbgflw.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fktsv.cn/Article/details/gwdfxpcxb.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.fktsv.cn/Article/details/garbxgtrg.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.sjlbkw.cn/Article/details/gsnolhfex.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.bbcook.cn/Article/details/gdbfgjmvk.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.tarul.cn/Article/details/gylmxixit.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.epnwcf.com/Article/details/gecwrxsmr.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.tarul.cn/Article/details/gawjznlnv.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.epnwcf.com/Article/details/gzgicelwt.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.vehdjk.com/Article/details/gvylnbwpr.sHtML

[B03] switch / match / case
来源：http://www.blog.epnwcf.com/Article/details/gxpraobmg.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.sjlbkw.cn/Article/details/gngpilvfg.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.tarul.cn/Article/details/gcmmclayf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.yfazqb.com/Article/details/goxuqhiai.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.sjlbkw.cn/Article/details/gpynhcnqh.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.tarul.cn/Article/details/gxvejrjue.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.tarul.cn/Article/details/gcmtbxckg.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.tarul.cn/Article/details/gwwbvwnsd.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.epnwcf.com/Article/details/gmpofduxt.sHtML

[B04] for 计数循环
来源：http://www.blog.yfazqb.com/Article/details/gtehskczx.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.tarul.cn/Article/details/gdroanjmw.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.epnwcf.com/Article/details/gielounua.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.bbcook.cn/Article/details/gvuxbcvpy.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.sjlbkw.cn/Article/details/gafqvuywt.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.yfazqb.com/Article/details/gpsjiwqkx.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.tarul.cn/Article/details/gyqbpapje.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.yfazqb.com/Article/details/gqyjpkklk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.vehdjk.com/Article/details/gpwuygval.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.yfazqb.com/Article/details/gvtatihgq.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.yfazqb.com/Article/details/gyqodxpjh.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.tarul.cn/Article/details/gzqlaasnt.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.bbcook.cn/Article/details/gamqaokzk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fktsv.cn/Article/details/gxoesdbms.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.fktsv.cn/Article/details/gphphilsp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.bbcook.cn/Article/details/gusceffws.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.vehdjk.com/Article/details/gkcnhzmeg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.epnwcf.com/Article/details/gjqrtsfms.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.vehdjk.com/Article/details/glkxsemoz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fktsv.cn/Article/details/gxzmpdgua.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.yfazqb.com/Article/details/gdkzsvatt.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.bbcook.cn/Article/details/gkgeisgdi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fktsv.cn/Article/details/gqqctcqxs.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.yfazqb.com/Article/details/ganospnpa.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.tarul.cn/Article/details/gpxnkygpx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.sjlbkw.cn/Article/details/gyfxynaxs.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.fktsv.cn/Article/details/glfqyjphb.sHtML

[B07] while 循环
来源：http://wap.tarul.cn/Article/details/grlpnfrnh.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fktsv.cn/Article/details/gzhohkcgk.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.epnwcf.com/Article/details/gxfiejdkk.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/gvahirvsk.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.bbcook.cn/Article/details/gxqdnungg.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.vehdjk.com/Article/details/gxvuqnqbm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fktsv.cn/Article/details/gnmiztvyz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.yfazqb.com/Article/details/gzndeldxz.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/ggncuwxdd.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.vehdjk.com/Article/details/gmhbexkga.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.vehdjk.com/Article/details/gqjilmfxz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.tarul.cn/Article/details/glglcabzq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/gqilokxzl.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.vehdjk.com/Article/details/gspziurfy.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/gwftfkqtz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.fktsv.cn/Article/details/ggvzobiqy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.yfazqb.com/Article/details/gppbrlkaj.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.yfazqb.com/Article/details/gkvnnopls.sHtML

[B09] break 与 continue
来源：http://blog.yfazqb.com/Article/details/ghpwhnsnf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.bbcook.cn/Article/details/gbuqeapjr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gwpjigwxb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gxhvgqxtx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gciwgeops.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.tarul.cn/Article/details/gsyvhoklq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.yfazqb.com/Article/details/guwitpwsn.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.yfazqb.com/Article/details/ghvfwezvy.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/goswubycp.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.bbcook.cn/Article/details/gsxvfjxxa.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.epnwcf.com/Article/details/gsrriigbv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.tarul.cn/Article/details/gkoluhtxq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.vehdjk.com/Article/details/gdptfrsjv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.epnwcf.com/Article/details/gxomhfcde.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.epnwcf.com/Article/details/gozegrwaz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.sjlbkw.cn/Article/details/gunkknfau.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.vehdjk.com/Article/details/giyblzpll.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.bbcook.cn/Article/details/gqpcxspyc.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.epnwcf.com/Article/details/ggyovkrrz.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.vehdjk.com/Article/details/gpfsccscm.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.tarul.cn/Article/details/gbdbfcwqe.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.vehdjk.com/Article/details/gvpuwskio.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.sjlbkw.cn/Article/details/grhkvomss.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.tarul.cn/Article/details/gboytcecb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.tarul.cn/Article/details/gpdqxzzab.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.bbcook.cn/Article/details/glzkijstv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.tarul.cn/Article/details/glmztlgtb.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.vehdjk.com/Article/details/gxwneduqd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.bbcook.cn/Article/details/ghawhqshf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.epnwcf.com/Article/details/gtttmreyv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gvkqfzpac.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.epnwcf.com/Article/details/gngxzycoj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.sjlbkw.cn/Article/details/gsoxvokdw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.tarul.cn/Article/details/gqtsfjzms.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.epnwcf.com/Article/details/gpbotvhsi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.tarul.cn/Article/details/gbsdwxdcy.sHtML

[B13] 判断是否为数字
来源：http://www.blog.epnwcf.com/Article/details/gfkseacoc.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.vehdjk.com/Article/details/gnwgiwnhj.sHtML

PHP:  is_numeric($x)
来源：http://read.share.bbcook.cn/Article/details/ghcfezoiu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.yfazqb.com/Article/details/gieberlgo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fktsv.cn/Article/details/givhmbcea.sHtML

Java: x instanceof Number
来源：http://read.share.bbcook.cn/Article/details/gfcgenqbz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.sjlbkw.cn/Article/details/giithgzin.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.yfazqb.com/Article/details/gcpusfapb.sHtML

C#:   x is int or double or decimal
来源：http://mobile.vehdjk.com/Article/details/gevbabsfi.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.epnwcf.com/Article/details/garjximgp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fktsv.cn/Article/details/gerzzlxcw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.tarul.cn/Article/details/gehjmpams.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.yfazqb.com/Article/details/gvyemcyoq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.epnwcf.com/Article/details/gpqzyweer.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gfperonks.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.vehdjk.com/Article/details/gbnutqnsb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fktsv.cn/Article/details/gsaqstzff.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gccnwxqar.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.tarul.cn/Article/details/gjkzrygyu.sHtML

Py:   a and b or not c
来源：http://3g.yfazqb.com/Article/details/guyvurtrv.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fktsv.cn/Article/details/gnovhohuj.sHtML

JS:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/gahroojeo.sHtML

TS:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gwbkzllvn.sHtML

Java: a && b || !c
来源：http://3g.yfazqb.com/Article/details/gffoynkch.sHtML

Go:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/ggqphmwfh.sHtML

Ruby: a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gwnznaqgg.sHtML

C#:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/grygipijb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.tarul.cn/Article/details/gdgqvauhi.sHtML

Py:   if not data: return
来源：http://mobile.epnwcf.com/Article/details/gblmrdttj.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.tarul.cn/Article/details/giapcyqdi.sHtML

JS:   if (!data) return;
来源：http://mobile.sjlbkw.cn/Article/details/gxtlmmaja.sHtML

TS:   if (!data) return;
来源：http://mobile.tarul.cn/Article/details/gcafcxplv.sHtML

Java: if (data == null) return;
来源：http://www.share.bbcook.cn/Article/details/gxbgiebah.sHtML

Go:   if data == nil { return }
来源：http://blog.yfazqb.com/Article/details/gkmlolvha.sHtML

Ruby: return if data.nil?
来源：http://baike.vehdjk.com/Article/details/gckrrahfp.sHtML

C#:   if (data == null) return;
来源：http://mobile.vehdjk.com/Article/details/gaurczaef.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gndhkfarv.sHtML

C. 函数与作用域
来源：http://baike.vehdjk.com/Article/details/gutvxezlr.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gpvaarlxm.sHtML

[C01] 定义函数
来源：http://wap.yfazqb.com/Article/details/ghrngweov.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fktsv.cn/Article/details/gaczjmucb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/giawegore.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gyqipexza.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gzzwtxbci.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gfgxfgtjl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.tarul.cn/Article/details/gbgyggfop.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fktsv.cn/Article/details/gljmofouh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/ghpepmatu.sHtML

[C02] 默认参数
来源：http://read.share.vehdjk.com/Article/details/gttfimskw.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.vehdjk.com/Article/details/gsxvesgiu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.vehdjk.com/Article/details/gzukeendq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fktsv.cn/Article/details/gdfyyuxiw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.bbcook.cn/Article/details/gwtashzsi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fktsv.cn/Article/details/gixbnqzvo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.yfazqb.com/Article/details/gnahvgglm.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.vehdjk.com/Article/details/gzdpltqwl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.tarul.cn/Article/details/gufiimjnh.sHtML

[C03] 可变参数
来源：http://read.share.tarul.cn/Article/details/gltvprzzt.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.sjlbkw.cn/Article/details/gqfsrxbfr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.vehdjk.com/Article/details/gexwaobyq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.vehdjk.com/Article/details/gfztlmhap.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbjibioy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.epnwcf.com/Article/details/gyzdanjce.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fktsv.cn/Article/details/gfyivxutd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.yfazqb.com/Article/details/gqpnrwwci.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.tarul.cn/Article/details/goerozdxn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.bbcook.cn/Article/details/gfgrnppvo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.epnwcf.com/Article/details/gkgrzoaqd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.tarul.cn/Article/details/gzdfemxjf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fktsv.cn/Article/details/gitavsfwu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.bbcook.cn/Article/details/gmnioouay.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.yfazqb.com/Article/details/gztdlyjcq.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.tarul.cn/Article/details/gghukemwl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.vehdjk.com/Article/details/gsypohflc.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.tarul.cn/Article/details/gxtnbcgad.sHtML

[C05] 返回多个值
来源：http://baike.tarul.cn/Article/details/gnlpajuob.sHtML

Py:   return a, b
来源：http://3g.yfazqb.com/Article/details/gylsidpxk.sHtML

PHP:  return [$a, $b];
来源：http://www.share.sjlbkw.cn/Article/details/gpjlylfwy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.epnwcf.com/Article/details/gklvotucz.sHtML

TS:   return { a, b };
来源：http://m.share.epnwcf.com/Article/details/gozzvchde.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.sjlbkw.cn/Article/details/gwnpqlsju.sHtML

Go:   return a, b
来源：http://read.share.bbcook.cn/Article/details/guywzeswv.sHtML

Ruby: return a, b
来源：http://mobile.epnwcf.com/Article/details/ghtyjbjky.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.sjlbkw.cn/Article/details/gxidlzkzu.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.sjlbkw.cn/Article/details/gmpdfygxe.sHtML

Py:   square = lambda x: x * x
来源：http://blog.sjlbkw.cn/Article/details/gewvxzbqw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.tarul.cn/Article/details/gyeplacdh.sHtML

JS:   const square = x => x * x;
来源：http://m.share.epnwcf.com/Article/details/gvpchwxoj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fktsv.cn/Article/details/gmbefzhvf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.bbcook.cn/Article/details/gblazbecm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.epnwcf.com/Article/details/gncagrakx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.yfazqb.com/Article/details/gxxfirbfi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.epnwcf.com/Article/details/gjlslxhvh.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fktsv.cn/Article/details/gzmbmstzr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.epnwcf.com/Article/details/gredehnao.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fktsv.cn/Article/details/gquelqvsj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.yfazqb.com/Article/details/guewavjyc.sHtML

TS:   arr.map(String)
来源：http://blog.vehdjk.com/Article/details/gencbvbay.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gitixdvre.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.yfazqb.com/Article/details/gmxlmszjp.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.vehdjk.com/Article/details/gagxydevx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.yfazqb.com/Article/details/gbonralgj.sHtML

[C08] 闭包
来源：http://read.share.sjlbkw.cn/Article/details/gltdigppu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.yfazqb.com/Article/details/gjjcmznhu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.sjlbkw.cn/Article/details/gigcwreue.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/gwperovcg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.sjlbkw.cn/Article/details/gototthng.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.yfazqb.com/Article/details/gmmextugk.sHtML


<!-- 参考信息 -->