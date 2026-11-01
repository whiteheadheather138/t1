代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.fktsv.cn/Article/details/gzpqvzraw.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.epnwcf.com/Article/details/gvaalaeqh.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.yfazqb.com/Article/details/gzlqflvxz.sHtML

[A17] 位运算
来源：http://m.share.vehdjk.com/Article/details/glsspeeki.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.sjlbkw.cn/Article/details/gxcfhbrvu.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxpkiwui.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.tarul.cn/Article/details/gkwarcdsm.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.bbcook.cn/Article/details/gdcycdcvw.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.yfazqb.com/Article/details/gljhwofsp.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.epnwcf.com/Article/details/gysdzyhlu.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.yfazqb.com/Article/details/gpdvotkma.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fktsv.cn/Article/details/gpthrvpxn.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.vehdjk.com/Article/details/gqequzrkx.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.tarul.cn/Article/details/gzkyaxiik.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.vehdjk.com/Article/details/gazlumxvi.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.tarul.cn/Article/details/gkytmxfog.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.epnwcf.com/Article/details/gamcbobgf.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.tarul.cn/Article/details/gqjpmmlev.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.yfazqb.com/Article/details/gqdcdwjcd.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.vehdjk.com/Article/details/gdevfybdn.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.fktsv.cn/Article/details/gkmzmzctn.sHtML

[A19] 交换两个变量
来源：http://www.m.share.vehdjk.com/Article/details/giaakzjkf.sHtML

Py:   a, b = b, a
来源：http://3g.tarul.cn/Article/details/goqfvqrat.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.tarul.cn/Article/details/gqvmzmubq.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.bbcook.cn/Article/details/glblwtkci.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.epnwcf.com/Article/details/ghivygbhv.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.yfazqb.com/Article/details/gxmkoedjy.sHtML

Go:   a, b = b, a
来源：http://wap.vehdjk.com/Article/details/gnycdygdq.sHtML

Ruby: a, b = b, a
来源：http://www.share.yfazqb.com/Article/details/gscdxivyv.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.yfazqb.com/Article/details/geertrwbt.sHtML

[A20] 读取标准输入
来源：http://baike.fktsv.cn/Article/details/gxqpkavmm.sHtML

Py:   name = input("请输入：")
来源：http://wap.sjlbkw.cn/Article/details/gozqjfxin.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.fktsv.cn/Article/details/gbubeedli.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.epnwcf.com/Article/details/gddngppif.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.sjlbkw.cn/Article/details/gqcndabmn.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.vehdjk.com/Article/details/gxhrwokia.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.tarul.cn/Article/details/grmcsyuab.sHtML

Ruby: gets.chomp
来源：http://www.m.share.bbcook.cn/Article/details/gjtyeywdo.sHtML

C#:   Console.ReadLine();
来源：http://baike.fktsv.cn/Article/details/gavhkcnug.sHtML

[A21] 保留指定小数位输出
来源：http://baike.bbcook.cn/Article/details/gprdewykk.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.fktsv.cn/Article/details/gpctrgzym.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.sjlbkw.cn/Article/details/gtbkjbhlj.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.vehdjk.com/Article/details/gkafrdglu.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.epnwcf.com/Article/details/gdxiikqen.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.vehdjk.com/Article/details/gcmxcnjqa.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.fktsv.cn/Article/details/gnwnzkovi.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.fktsv.cn/Article/details/gxkrwsloz.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.bbcook.cn/Article/details/gcnfyyjga.sHtML

[A22] 获取字符串长度
来源：http://mobile.sjlbkw.cn/Article/details/grnyswfmt.sHtML

Py:   len(s)
来源：http://baike.epnwcf.com/Article/details/gshsjdgjf.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.epnwcf.com/Article/details/grckezvjq.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.yfazqb.com/Article/details/gcabxtsea.sHtML

TS:   s.length
来源：http://mobile.bbcook.cn/Article/details/gbrxcuzzq.sHtML

Java: s.length()
来源：http://www.blog.epnwcf.com/Article/details/gbynyipgi.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.fktsv.cn/Article/details/gydypmdtx.sHtML

Ruby: s.length
来源：http://m.share.fktsv.cn/Article/details/gcovfnleo.sHtML

C#:   s.Length
来源：http://baike.sjlbkw.cn/Article/details/gquvgkmqf.sHtML

[A23] 大小写转换
来源：http://www.share.sjlbkw.cn/Article/details/giiemftpk.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.epnwcf.com/Article/details/gzitqemyc.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.fktsv.cn/Article/details/gchynqqeq.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fktsv.cn/Article/details/gsdatchig.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.vehdjk.com/Article/details/gcfpkzymd.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.epnwcf.com/Article/details/gohpmrqsj.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.vehdjk.com/Article/details/gjvqpyulm.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.vehdjk.com/Article/details/gwpepqxxw.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.yfazqb.com/Article/details/gswrlisds.sHtML

[A24] 去除首尾空白
来源：http://3g.yfazqb.com/Article/details/gvmwpxpvv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.sjlbkw.cn/Article/details/ggyacxegc.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.vehdjk.com/Article/details/glcvqlxqj.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvafvstqc.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.epnwcf.com/Article/details/gytrnznvo.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.vehdjk.com/Article/details/ghtzdhbyt.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.vehdjk.com/Article/details/gchlfaosb.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.tarul.cn/Article/details/gipfcrgqf.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.vehdjk.com/Article/details/gdbdthfru.sHtML

[A25] 字符串比较
来源：http://www.blog.yfazqb.com/Article/details/gbgzjsrrv.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.vehdjk.com/Article/details/gdxgoseju.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.tarul.cn/Article/details/glxxmkabo.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.epnwcf.com/Article/details/gfrstyooc.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.yfazqb.com/Article/details/gqmhyjuzb.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.bbcook.cn/Article/details/gahmeqzjk.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.tarul.cn/Article/details/gsajyssam.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.epnwcf.com/Article/details/gkoaenfyb.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.sjlbkw.cn/Article/details/ghiyjvblc.sHtML

[A26] 类型转换总览
来源：http://www.blog.vehdjk.com/Article/details/gklhxugyf.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.fktsv.cn/Article/details/ggetyiagq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.tarul.cn/Article/details/gpnezgvmx.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.epnwcf.com/Article/details/gxidstyik.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.fktsv.cn/Article/details/gvrcaikyd.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.vehdjk.com/Article/details/gehygbvcf.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.epnwcf.com/Article/details/gxkvexqsd.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.yfazqb.com/Article/details/gvconytwd.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.yfazqb.com/Article/details/gxdkucfyf.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gsroblpvt.sHtML

B. 流程控制
来源：http://baike.bbcook.cn/Article/details/gafjfcnzc.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gekndpjep.sHtML

[B01] 条件判断 if / else
来源：http://3g.bbcook.cn/Article/details/gjcbtxkdd.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.vehdjk.com/Article/details/gmifszeia.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.tarul.cn/Article/details/gtghctigt.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.sjlbkw.cn/Article/details/goyosptha.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.sjlbkw.cn/Article/details/gmzpsfdwc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fktsv.cn/Article/details/gswleqaup.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.sjlbkw.cn/Article/details/gzhuovkar.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.epnwcf.com/Article/details/gmuqxbckp.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/gsypfeqnh.sHtML

[B02] 多分支 else if / elif
来源：http://3g.bbcook.cn/Article/details/gapjsxbxk.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.bbcook.cn/Article/details/gztxhxxqv.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.bbcook.cn/Article/details/ghrjzovpg.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.tarul.cn/Article/details/gflkwjfou.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.bbcook.cn/Article/details/gjzkaertp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fktsv.cn/Article/details/gcddibzhf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.fktsv.cn/Article/details/gzpovxkir.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.epnwcf.com/Article/details/gqsluuxae.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.tarul.cn/Article/details/gpvmbejkd.sHtML

[B03] switch / match / case
来源：http://mobile.yfazqb.com/Article/details/gvxwtdlgm.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.sjlbkw.cn/Article/details/gtjaqelrh.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/gnmohkmqd.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.vehdjk.com/Article/details/gkunvsamd.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.sjlbkw.cn/Article/details/gksxvtvyb.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.sjlbkw.cn/Article/details/gegfulhns.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.yfazqb.com/Article/details/grpnnfhso.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.sjlbkw.cn/Article/details/gupvfsvuq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.sjlbkw.cn/Article/details/ghdcxtxdd.sHtML

[B04] for 计数循环
来源：http://wap.fktsv.cn/Article/details/gimiznohc.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.fktsv.cn/Article/details/gcbvvqqhg.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.epnwcf.com/Article/details/guhahabsb.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.tarul.cn/Article/details/gotrsyibh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.sjlbkw.cn/Article/details/graegdxws.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.fktsv.cn/Article/details/grhehacxq.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.bbcook.cn/Article/details/gzgwgszmy.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.yfazqb.com/Article/details/gmruuvlrp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.tarul.cn/Article/details/gcnwhrgal.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.bbcook.cn/Article/details/guvdfcykc.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.epnwcf.com/Article/details/gwmlmtubh.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.epnwcf.com/Article/details/gpjainzqh.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.tarul.cn/Article/details/ginoyrpcj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.bbcook.cn/Article/details/gdmeldupw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.tarul.cn/Article/details/gvqovdxtf.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.yfazqb.com/Article/details/gqlkmhqpp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.vehdjk.com/Article/details/gekidvfhj.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.sjlbkw.cn/Article/details/grgyubysg.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.yfazqb.com/Article/details/guyjnfnwf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.bbcook.cn/Article/details/gwhtsifpa.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvarydfv.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.epnwcf.com/Article/details/ggxqkkmjf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.sjlbkw.cn/Article/details/gwdhznkjk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.fktsv.cn/Article/details/gpkfypocw.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.yfazqb.com/Article/details/gaoncopew.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.sjlbkw.cn/Article/details/gvpwznsci.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.bbcook.cn/Article/details/gjjsaompk.sHtML

[B07] while 循环
来源：http://www.m.share.vehdjk.com/Article/details/gdxgsapqb.sHtML

Py:   while i < 10: i += 1
来源：http://3g.yfazqb.com/Article/details/gjwzdxgxv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.sjlbkw.cn/Article/details/grnswidqi.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.fktsv.cn/Article/details/gtfzfvyft.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/gcpkwfrfg.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.bbcook.cn/Article/details/gekqjedeu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.yfazqb.com/Article/details/gzxhhncru.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.sjlbkw.cn/Article/details/gjqomuwng.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.epnwcf.com/Article/details/guwxrsptu.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.tarul.cn/Article/details/grrwhbjer.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.tarul.cn/Article/details/gmghgayfs.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.tarul.cn/Article/details/gwateqhvi.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.sjlbkw.cn/Article/details/gindghrhl.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.vehdjk.com/Article/details/gseyeujgd.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.tarul.cn/Article/details/gmncxrcxg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.fktsv.cn/Article/details/glxfenapv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.bbcook.cn/Article/details/gvitatqsj.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gpolwuwci.sHtML

[B09] break 与 continue
来源：http://blog.yfazqb.com/Article/details/gbzyccdsk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.tarul.cn/Article/details/gqpynzoik.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/ghwzrbjyi.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gbtwhubju.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gistqlcui.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gmzmaqchh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.sjlbkw.cn/Article/details/gwlwxguzs.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.vehdjk.com/Article/details/gumykozzt.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/gcmqskuqp.sHtML

[B10] 遍历同时拿索引
来源：http://wap.yfazqb.com/Article/details/giljsszlu.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fktsv.cn/Article/details/gwkpyusvj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.epnwcf.com/Article/details/gdmxhibmt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.sjlbkw.cn/Article/details/ggwgrttme.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.yfazqb.com/Article/details/gqukjqxrf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.tarul.cn/Article/details/gkatmpadb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.sjlbkw.cn/Article/details/grocuojzc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.bbcook.cn/Article/details/ghkgvsoey.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.bbcook.cn/Article/details/gqxyioxuz.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.tarul.cn/Article/details/gndgzvyxc.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.yfazqb.com/Article/details/ghpeticsr.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.bbcook.cn/Article/details/gauvpaaao.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.tarul.cn/Article/details/gzybvicbi.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.yfazqb.com/Article/details/gkjjatswe.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.sjlbkw.cn/Article/details/glslyfcjn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.yfazqb.com/Article/details/guaggwhml.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.yfazqb.com/Article/details/ghmnnfyru.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.bbcook.cn/Article/details/gnrotjjjx.sHtML

[B12] 跳出多层循环
来源：http://www.share.epnwcf.com/Article/details/gjqyjudxm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.epnwcf.com/Article/details/gjtutxsff.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.vehdjk.com/Article/details/gsicbsqmn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.tarul.cn/Article/details/gahicpbxt.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.yfazqb.com/Article/details/gzducsvuv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.bbcook.cn/Article/details/gpuuamflt.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fktsv.cn/Article/details/giosslesm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fktsv.cn/Article/details/gqjhnxfsu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.sjlbkw.cn/Article/details/ghyquybrt.sHtML

[B13] 判断是否为数字
来源：http://baike.bbcook.cn/Article/details/ggvbqsqpl.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.sjlbkw.cn/Article/details/galuyojhi.sHtML

PHP:  is_numeric($x)
来源：http://read.share.yfazqb.com/Article/details/getucsvmd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.bbcook.cn/Article/details/gpeckiyjw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.sjlbkw.cn/Article/details/gefkccxlj.sHtML

Java: x instanceof Number
来源：http://www.blog.yfazqb.com/Article/details/geogvwutt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.yfazqb.com/Article/details/gmtufuujy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.yfazqb.com/Article/details/gudixgzhr.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fktsv.cn/Article/details/gsfwlbzze.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fktsv.cn/Article/details/gzpijvndx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.sjlbkw.cn/Article/details/govqoqvvm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fktsv.cn/Article/details/gthntsxjo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.tarul.cn/Article/details/griscskzb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.epnwcf.com/Article/details/gqeywwtzc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.sjlbkw.cn/Article/details/gjzfnpfdk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.epnwcf.com/Article/details/gybwuidpv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fktsv.cn/Article/details/gboeeikjj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fktsv.cn/Article/details/gvxzrcvzn.sHtML

[B15] 布尔运算与取反
来源：http://wap.sjlbkw.cn/Article/details/gjuqdewja.sHtML

Py:   a and b or not c
来源：http://mobile.epnwcf.com/Article/details/gyltgydgd.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.tarul.cn/Article/details/gqqjdtxcy.sHtML

JS:   a && b || !c
来源：http://baike.vehdjk.com/Article/details/gadykgyww.sHtML

TS:   a && b || !c
来源：http://mobile.yfazqb.com/Article/details/gvixpjnen.sHtML

Java: a && b || !c
来源：http://mobile.yfazqb.com/Article/details/gxsiwwbqz.sHtML

Go:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gadfzfhgh.sHtML

Ruby: a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/greafevts.sHtML

C#:   a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gcwtojpdt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fktsv.cn/Article/details/gvxeyfvwz.sHtML

Py:   if not data: return
来源：http://www.blog.tarul.cn/Article/details/gfgclswtn.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fktsv.cn/Article/details/gogkifeta.sHtML

JS:   if (!data) return;
来源：http://baike.sjlbkw.cn/Article/details/ghyynhbxb.sHtML

TS:   if (!data) return;
来源：http://mobile.fktsv.cn/Article/details/girxfjbht.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fktsv.cn/Article/details/gqwwyxrkx.sHtML

Go:   if data == nil { return }
来源：http://blog.tarul.cn/Article/details/gdudwtrgf.sHtML

Ruby: return if data.nil?
来源：http://wap.sjlbkw.cn/Article/details/glqymiksq.sHtML

C#:   if (data == null) return;
来源：http://read.share.bbcook.cn/Article/details/gzmhhucck.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gtbtwaxzq.sHtML

C. 函数与作用域
来源：http://m.share.sjlbkw.cn/Article/details/gzxncqioi.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gshnovpdd.sHtML

[C01] 定义函数
来源：http://wap.vehdjk.com/Article/details/guiqgylze.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.epnwcf.com/Article/details/gqimwgwxm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/gwddjneig.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gxoxeflcq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gqlrpfyra.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gkyuslhwh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.tarul.cn/Article/details/gczfesxxj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.yfazqb.com/Article/details/guzvhdjzi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gjvlireqv.sHtML

[C02] 默认参数
来源：http://www.share.sjlbkw.cn/Article/details/glrvjlbdb.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.bbcook.cn/Article/details/giubcakdt.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.bbcook.cn/Article/details/gficqgyps.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gtiebcwqv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.sjlbkw.cn/Article/details/ghcqbusha.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.tarul.cn/Article/details/gfzoimrxw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.vehdjk.com/Article/details/gkxroiclm.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.tarul.cn/Article/details/gatfxpxsp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.yfazqb.com/Article/details/gdhpsopfe.sHtML

[C03] 可变参数
来源：http://read.share.bbcook.cn/Article/details/gddebemap.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.epnwcf.com/Article/details/gujlmfcut.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.epnwcf.com/Article/details/gqijxsnmc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fktsv.cn/Article/details/gthdamtzo.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.bbcook.cn/Article/details/ggzlrkfga.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.bbcook.cn/Article/details/gqommmhnk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.yfazqb.com/Article/details/gnrpdfcuh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.tarul.cn/Article/details/ggdjxyiqt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.yfazqb.com/Article/details/gacuwcsjk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.yfazqb.com/Article/details/grgpmarzj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.bbcook.cn/Article/details/gavwoehje.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.epnwcf.com/Article/details/gkaxnglex.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fktsv.cn/Article/details/gpnyzhcnd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.sjlbkw.cn/Article/details/gxgrygbvb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.tarul.cn/Article/details/ggrviuvmm.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.tarul.cn/Article/details/gkhyyeipx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.vehdjk.com/Article/details/gvtawpvzm.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.epnwcf.com/Article/details/gppobiywn.sHtML

[C05] 返回多个值
来源：http://3g.yfazqb.com/Article/details/gtmrvhcvg.sHtML

Py:   return a, b
来源：http://www.blog.vehdjk.com/Article/details/gffoogvuo.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fktsv.cn/Article/details/gaayhwyhn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.yfazqb.com/Article/details/gsmodtekd.sHtML

TS:   return { a, b };
来源：http://wap.tarul.cn/Article/details/gtugrezbv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.bbcook.cn/Article/details/gglrjluwl.sHtML

Go:   return a, b
来源：http://3g.bbcook.cn/Article/details/gkezbzkux.sHtML

Ruby: return a, b
来源：http://wap.vehdjk.com/Article/details/gabbgkthn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.vehdjk.com/Article/details/gngyfnmdo.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.bbcook.cn/Article/details/gxsylgisl.sHtML

Py:   square = lambda x: x * x
来源：http://baike.epnwcf.com/Article/details/gibcpjnvt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.vehdjk.com/Article/details/gnbfhybrv.sHtML

JS:   const square = x => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gbpmkdrpz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.bbcook.cn/Article/details/gnribxziy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.bbcook.cn/Article/details/gnlydufvv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fktsv.cn/Article/details/gcbvxdiaz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.yfazqb.com/Article/details/ghkmutlgp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.sjlbkw.cn/Article/details/gutzwzesh.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.vehdjk.com/Article/details/gudbajnvc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.sjlbkw.cn/Article/details/gtocpkios.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.yfazqb.com/Article/details/gazbmcaoo.sHtML


<!-- 参考信息 -->