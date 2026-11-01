代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.sjlbkw.cn/Article/details/gubtmqbik.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.fktsv.cn/Article/details/gxgisrluy.sHtML

TS:   if (!x) {}
来源：http://baike.epnwcf.com/Article/details/giuqzsxhg.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.fktsv.cn/Article/details/gvaievzqd.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.vehdjk.com/Article/details/gwwagykvy.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.bbcook.cn/Article/details/grunsygao.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.sjlbkw.cn/Article/details/gelutmjxc.sHtML

[A17] 位运算
来源：http://read.share.sjlbkw.cn/Article/details/gmklonywb.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.vehdjk.com/Article/details/gdwhgipmq.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.epnwcf.com/Article/details/gktycemnn.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.bbcook.cn/Article/details/ggbbokifu.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.bbcook.cn/Article/details/gsebszchy.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.epnwcf.com/Article/details/gmmswwxxc.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.yfazqb.com/Article/details/gyxcveqyh.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fktsv.cn/Article/details/gllsnifau.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.epnwcf.com/Article/details/gwexficaw.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.fktsv.cn/Article/details/grpgfolay.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.fktsv.cn/Article/details/gimmqncjj.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.sjlbkw.cn/Article/details/gvbdshorm.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.yfazqb.com/Article/details/gbmummggc.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.tarul.cn/Article/details/gomufxuon.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.epnwcf.com/Article/details/gfxocwimq.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.tarul.cn/Article/details/gfoaqemax.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.fktsv.cn/Article/details/gjnjiyfye.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.epnwcf.com/Article/details/ggtzljdwm.sHtML

[A19] 交换两个变量
来源：http://3g.fktsv.cn/Article/details/gwfmaekgr.sHtML

Py:   a, b = b, a
来源：http://www.m.share.tarul.cn/Article/details/gpfeejcef.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.vehdjk.com/Article/details/ginazifot.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.fktsv.cn/Article/details/gubwsmjbr.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.bbcook.cn/Article/details/gucezkdor.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.bbcook.cn/Article/details/gfmcryibq.sHtML

Go:   a, b = b, a
来源：http://baike.epnwcf.com/Article/details/glzawujsx.sHtML

Ruby: a, b = b, a
来源：http://www.share.bbcook.cn/Article/details/gdmovowmq.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.epnwcf.com/Article/details/gkdqathvf.sHtML

[A20] 读取标准输入
来源：http://www.m.share.epnwcf.com/Article/details/gnbtazbgp.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.yfazqb.com/Article/details/gneiaiarx.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.tarul.cn/Article/details/gdaavesfl.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.bbcook.cn/Article/details/gajymkxyc.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.bbcook.cn/Article/details/gftfhuwpw.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.yfazqb.com/Article/details/glqimtegr.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.tarul.cn/Article/details/ggibmmcah.sHtML

Ruby: gets.chomp
来源：http://www.share.yfazqb.com/Article/details/gnwaxrvpz.sHtML

C#:   Console.ReadLine();
来源：http://www.share.bbcook.cn/Article/details/gvbhcdaer.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.epnwcf.com/Article/details/gjkntuawb.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.bbcook.cn/Article/details/guufipgxj.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.tarul.cn/Article/details/gasdsnkni.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.fktsv.cn/Article/details/gtivpzzup.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.tarul.cn/Article/details/gwlxclvtd.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.yfazqb.com/Article/details/gkjnrymov.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.fktsv.cn/Article/details/gkyrvmqez.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.fktsv.cn/Article/details/gaebgyfdi.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.tarul.cn/Article/details/ghgrknzoz.sHtML

[A22] 获取字符串长度
来源：http://www.blog.vehdjk.com/Article/details/ggsjcwhhs.sHtML

Py:   len(s)
来源：http://mobile.yfazqb.com/Article/details/gfxmjoztn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.bbcook.cn/Article/details/gbgecwhcl.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.sjlbkw.cn/Article/details/guqqexfva.sHtML

TS:   s.length
来源：http://blog.epnwcf.com/Article/details/gyiuhefuc.sHtML

Java: s.length()
来源：http://www.blog.bbcook.cn/Article/details/gsewcwctl.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.fktsv.cn/Article/details/ghbnsqorg.sHtML

Ruby: s.length
来源：http://blog.tarul.cn/Article/details/gaaiagrdk.sHtML

C#:   s.Length
来源：http://wap.sjlbkw.cn/Article/details/gbbkusmqe.sHtML

[A23] 大小写转换
来源：http://m.share.epnwcf.com/Article/details/gngroqdaj.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.sjlbkw.cn/Article/details/getnktgip.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.bbcook.cn/Article/details/geiqaight.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.tarul.cn/Article/details/gzvrntgol.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.sjlbkw.cn/Article/details/gloeolqpx.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.vehdjk.com/Article/details/gumjtocfe.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.bbcook.cn/Article/details/gdvsdoztv.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.epnwcf.com/Article/details/gaozokhvs.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.tarul.cn/Article/details/gbkstrqpb.sHtML

[A24] 去除首尾空白
来源：http://m.share.epnwcf.com/Article/details/gintpuaye.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.yfazqb.com/Article/details/gsppogpof.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.tarul.cn/Article/details/gfaofazkw.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.epnwcf.com/Article/details/gbijgfzxl.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.tarul.cn/Article/details/gmmpopgxi.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.epnwcf.com/Article/details/gxyaqphhh.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.epnwcf.com/Article/details/gtolgzyja.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.yfazqb.com/Article/details/gysbqxfpi.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.sjlbkw.cn/Article/details/gxefkgvzv.sHtML

[A25] 字符串比较
来源：http://wap.tarul.cn/Article/details/gxkdashbo.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.sjlbkw.cn/Article/details/gddqruazv.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.sjlbkw.cn/Article/details/grcruumeo.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.bbcook.cn/Article/details/giptexafm.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.sjlbkw.cn/Article/details/gpkfzjkoj.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.fktsv.cn/Article/details/gcvuarjac.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.tarul.cn/Article/details/gunmkccvm.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.vehdjk.com/Article/details/ggqpoqmdd.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.yfazqb.com/Article/details/guvuztell.sHtML

[A26] 类型转换总览
来源：http://baike.vehdjk.com/Article/details/ghgoritme.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.epnwcf.com/Article/details/gkxdqgzpn.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.yfazqb.com/Article/details/gpdfapksa.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.sjlbkw.cn/Article/details/geixvhuio.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.sjlbkw.cn/Article/details/gkwjuolgd.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.sjlbkw.cn/Article/details/gerrdjlsr.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.tarul.cn/Article/details/gfonyzfdh.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.vehdjk.com/Article/details/goxcjokkq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.epnwcf.com/Article/details/gcoajidff.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gvcgiwpul.sHtML

B. 流程控制
来源：http://www.blog.tarul.cn/Article/details/gyzbiazcv.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gwlehyqlo.sHtML

[B01] 条件判断 if / else
来源：http://blog.tarul.cn/Article/details/gaabmmdpd.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.sjlbkw.cn/Article/details/gnojkhjxk.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.tarul.cn/Article/details/ghhnqlzqb.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.sjlbkw.cn/Article/details/gdphtpseg.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.bbcook.cn/Article/details/gbxcjhptz.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.fktsv.cn/Article/details/gqhuvypor.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.tarul.cn/Article/details/gjwgpsozl.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.yfazqb.com/Article/details/gvxsiasfz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.epnwcf.com/Article/details/gwpotprul.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fktsv.cn/Article/details/gevnxafdj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.yfazqb.com/Article/details/gtudshllt.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.fktsv.cn/Article/details/gvrdtmojo.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.tarul.cn/Article/details/gftalmrat.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.sjlbkw.cn/Article/details/ghgpbeurn.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fktsv.cn/Article/details/gjnhaetdf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.fktsv.cn/Article/details/gqcadokif.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.fktsv.cn/Article/details/gxagecsqq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.epnwcf.com/Article/details/ggbkgpswi.sHtML

[B03] switch / match / case
来源：http://mobile.vehdjk.com/Article/details/gkaimqyfq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.bbcook.cn/Article/details/geywtltjz.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.epnwcf.com/Article/details/ggiilzzpg.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.vehdjk.com/Article/details/guyspcnyv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fktsv.cn/Article/details/gyzejpmly.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.fktsv.cn/Article/details/gdktxilso.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.fktsv.cn/Article/details/gghrtnilx.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.tarul.cn/Article/details/gdhgyyjql.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.tarul.cn/Article/details/gmbqxrqgb.sHtML

[B04] for 计数循环
来源：http://read.share.vehdjk.com/Article/details/gmoytdhbq.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.vehdjk.com/Article/details/glalnunot.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.vehdjk.com/Article/details/gnykpsgtd.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fktsv.cn/Article/details/glnqgwgvn.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.tarul.cn/Article/details/gjworluzr.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.bbcook.cn/Article/details/gyrgupqli.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.sjlbkw.cn/Article/details/glsjgdwom.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.yfazqb.com/Article/details/gadrvrzri.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.vehdjk.com/Article/details/ggrwzyhfj.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.epnwcf.com/Article/details/gbjaerbxu.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.vehdjk.com/Article/details/gptvgisbh.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.sjlbkw.cn/Article/details/gkxugpxpw.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.vehdjk.com/Article/details/gdvufhskc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.bbcook.cn/Article/details/gszrdjdvs.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.sjlbkw.cn/Article/details/gttcjvxqr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.tarul.cn/Article/details/gdpulpgez.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.bbcook.cn/Article/details/gtfrqahjz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.yfazqb.com/Article/details/gztfeiofj.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.vehdjk.com/Article/details/ghlbtxvup.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.bbcook.cn/Article/details/gjixybawt.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.bbcook.cn/Article/details/gbthftaym.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.yfazqb.com/Article/details/gwilytwpi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.yfazqb.com/Article/details/gzriizgta.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.sjlbkw.cn/Article/details/gbacehpnh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.yfazqb.com/Article/details/gmumetbkk.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fktsv.cn/Article/details/gmqmqxmxx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.epnwcf.com/Article/details/gxkwenmmx.sHtML

[B07] while 循环
来源：http://www.share.vehdjk.com/Article/details/gvxrmbzbx.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fktsv.cn/Article/details/gnhgtjehl.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.yfazqb.com/Article/details/gtwypdgyr.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.bbcook.cn/Article/details/gjwcrpnmv.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/grrtigygt.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/gvnksxeea.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fktsv.cn/Article/details/gzusnmrnx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.tarul.cn/Article/details/gfvvuxtjp.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.epnwcf.com/Article/details/gicnadtfp.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.fktsv.cn/Article/details/ghxiajgqn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.sjlbkw.cn/Article/details/gdfdoqyhu.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.fktsv.cn/Article/details/gnjpglgou.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fktsv.cn/Article/details/gjosismsx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.epnwcf.com/Article/details/getjoruig.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/gjyjaworr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.tarul.cn/Article/details/gupwyueqf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.bbcook.cn/Article/details/gnoqdtigk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gyzwvlyzs.sHtML

[B09] break 与 continue
来源：http://www.share.epnwcf.com/Article/details/gilyujwfw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.epnwcf.com/Article/details/gxlvoydhj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/gwnxrpwge.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gexqpatcb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gnfxnsxfv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/gwjkgcajx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.epnwcf.com/Article/details/glvxeuuap.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.vehdjk.com/Article/details/gpvyxejmo.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gbgdltiuy.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fktsv.cn/Article/details/gaatzbfom.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.bbcook.cn/Article/details/gbuadpkzb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fktsv.cn/Article/details/gbuiaomav.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.yfazqb.com/Article/details/gscthnbve.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.vehdjk.com/Article/details/gkozbkbbw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.tarul.cn/Article/details/gdcyaukij.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.epnwcf.com/Article/details/govpmldbv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.sjlbkw.cn/Article/details/gqhohcmmk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fktsv.cn/Article/details/gkdkqztfn.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.vehdjk.com/Article/details/gbpzrpffi.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.yfazqb.com/Article/details/guxdqsykd.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.tarul.cn/Article/details/glftwexch.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fktsv.cn/Article/details/gqpopahre.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.yfazqb.com/Article/details/gxbulwxnk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.yfazqb.com/Article/details/gsmooltfh.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fktsv.cn/Article/details/gjewctrsw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.tarul.cn/Article/details/gwnbejohe.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.tarul.cn/Article/details/gisrcrtrz.sHtML

[B12] 跳出多层循环
来源：http://blog.sjlbkw.cn/Article/details/gcsjyqdgu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.epnwcf.com/Article/details/glzvluwcy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.tarul.cn/Article/details/guucmqbcx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fktsv.cn/Article/details/gtreuqotj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/gpvuogumf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fktsv.cn/Article/details/ggbhzwnae.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fktsv.cn/Article/details/gvitintrd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.bbcook.cn/Article/details/glmisynqi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.yfazqb.com/Article/details/gcsghnnzi.sHtML

[B13] 判断是否为数字
来源：http://wap.epnwcf.com/Article/details/gyushmiuf.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.sjlbkw.cn/Article/details/gazrmdnoo.sHtML

PHP:  is_numeric($x)
来源：http://3g.sjlbkw.cn/Article/details/gishjucip.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.vehdjk.com/Article/details/gbsuorrju.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.bbcook.cn/Article/details/gckecmzyd.sHtML

Java: x instanceof Number
来源：http://wap.bbcook.cn/Article/details/gucevmlas.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.tarul.cn/Article/details/gcjunbdpg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.bbcook.cn/Article/details/gdoqjorrh.sHtML

C#:   x is int or double or decimal
来源：http://www.share.tarul.cn/Article/details/gumxpnvos.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.yfazqb.com/Article/details/gjsretavj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.bbcook.cn/Article/details/ghnkrqojh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.sjlbkw.cn/Article/details/gwmatuxmu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.bbcook.cn/Article/details/gfvrftqee.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.tarul.cn/Article/details/ggvhvapwh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjralzvqp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fktsv.cn/Article/details/gisrnownd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.bbcook.cn/Article/details/gqixoybjf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.bbcook.cn/Article/details/gktdxpbwg.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fktsv.cn/Article/details/ghelaqmgl.sHtML

Py:   a and b or not c
来源：http://3g.epnwcf.com/Article/details/grzeotquw.sHtML

PHP:  $a && $b || !$c
来源：http://3g.sjlbkw.cn/Article/details/gwhjtkbrm.sHtML

JS:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gnmqwyrtr.sHtML

TS:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gzsiwdjpb.sHtML

Java: a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gzgwrqapv.sHtML

Go:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gbpqebafv.sHtML

Ruby: a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gwqrfdups.sHtML

C#:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gukszibld.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.bbcook.cn/Article/details/gcacxzxbw.sHtML

Py:   if not data: return
来源：http://www.blog.vehdjk.com/Article/details/geuszdbso.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fktsv.cn/Article/details/ggasugydz.sHtML

JS:   if (!data) return;
来源：http://blog.bbcook.cn/Article/details/gzvkfmibl.sHtML

TS:   if (!data) return;
来源：http://baike.bbcook.cn/Article/details/gycynukcy.sHtML

Java: if (data == null) return;
来源：http://mobile.epnwcf.com/Article/details/gtzalmprt.sHtML

Go:   if data == nil { return }
来源：http://3g.sjlbkw.cn/Article/details/gbpljpqlt.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.epnwcf.com/Article/details/gpydeeeoq.sHtML

C#:   if (data == null) return;
来源：http://mobile.epnwcf.com/Article/details/gdqyndkyu.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gkynmcfzn.sHtML

C. 函数与作用域
来源：http://www.m.share.fktsv.cn/Article/details/grvljhphg.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/geijzpkwq.sHtML

[C01] 定义函数
来源：http://www.m.share.bbcook.cn/Article/details/gbrgkbklz.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.tarul.cn/Article/details/gojniylmo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/giwckupca.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gceaqoodv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gtyqrnxfx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gvvtoelbq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.sjlbkw.cn/Article/details/gzruvhycr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.sjlbkw.cn/Article/details/gndezzgtx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gjatxkbto.sHtML

[C02] 默认参数
来源：http://mobile.sjlbkw.cn/Article/details/gcjqkqnzd.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.epnwcf.com/Article/details/ggaqoqxdp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.tarul.cn/Article/details/goqxffiwj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.tarul.cn/Article/details/glpwmvrvc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.vehdjk.com/Article/details/glxsgqxsz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.bbcook.cn/Article/details/gtzpncxwq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.sjlbkw.cn/Article/details/gwqyunusy.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.vehdjk.com/Article/details/gkrojsgmq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.epnwcf.com/Article/details/gvvigwgxo.sHtML

[C03] 可变参数
来源：http://blog.fktsv.cn/Article/details/gzfstrhxo.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.yfazqb.com/Article/details/ggivmxypl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.yfazqb.com/Article/details/gzsqwnixi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.yfazqb.com/Article/details/giqcdcnsh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.bbcook.cn/Article/details/gsmuzusqz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.bbcook.cn/Article/details/gwmdxhlzd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fktsv.cn/Article/details/gfiustzvx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.vehdjk.com/Article/details/gkhrafqez.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.epnwcf.com/Article/details/gjuehawdr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.epnwcf.com/Article/details/gwbfxzhbx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.epnwcf.com/Article/details/gnftptldc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fktsv.cn/Article/details/gtjaeoigz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.tarul.cn/Article/details/gzetefxxx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fktsv.cn/Article/details/gbldhuzkw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.bbcook.cn/Article/details/ghdfveqnt.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fktsv.cn/Article/details/gzafpmajt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.yfazqb.com/Article/details/gakfcrhbd.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.sjlbkw.cn/Article/details/gpsppqmqe.sHtML

[C05] 返回多个值
来源：http://wap.sjlbkw.cn/Article/details/gviqzalnb.sHtML

Py:   return a, b
来源：http://3g.yfazqb.com/Article/details/gjtzgdhmi.sHtML

PHP:  return [$a, $b];
来源：http://blog.sjlbkw.cn/Article/details/gftjkcnby.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.yfazqb.com/Article/details/gawsadlkw.sHtML

TS:   return { a, b };
来源：http://read.share.sjlbkw.cn/Article/details/gqujmnsyf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.vehdjk.com/Article/details/geqlzdalr.sHtML

Go:   return a, b
来源：http://wap.fktsv.cn/Article/details/gjusdkcud.sHtML

Ruby: return a, b
来源：http://www.share.epnwcf.com/Article/details/gdfwkqery.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.sjlbkw.cn/Article/details/gjlzuvbvt.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.bbcook.cn/Article/details/gtghluvor.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.tarul.cn/Article/details/gsdxjussk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.epnwcf.com/Article/details/gzfnqrguo.sHtML

JS:   const square = x => x * x;
来源：http://m.share.epnwcf.com/Article/details/gzusyrpak.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.yfazqb.com/Article/details/gsfxeprzg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.sjlbkw.cn/Article/details/gftgsrmyk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.sjlbkw.cn/Article/details/gnusklcpc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.vehdjk.com/Article/details/galktqlsa.sHtML


<!-- 参考信息 -->