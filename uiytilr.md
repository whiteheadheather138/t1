代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.epnwcf.com/Article/details/ggtqctomu.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.fktsv.cn/Article/details/ghxanbtpy.sHtML

TS:   if (!x) {}
来源：http://m.share.sjlbkw.cn/Article/details/gdbhnbolk.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.vehdjk.com/Article/details/gmpdsvubu.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.vehdjk.com/Article/details/ggxjappcp.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.vehdjk.com/Article/details/gyaenqtrv.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.yfazqb.com/Article/details/gmyvkzpqz.sHtML

[A17] 位运算
来源：http://read.share.vehdjk.com/Article/details/gbyonbdjp.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.epnwcf.com/Article/details/gfebtazbn.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.yfazqb.com/Article/details/gofrwhumh.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.epnwcf.com/Article/details/gayoervjw.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.yfazqb.com/Article/details/gxqoesjkc.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.epnwcf.com/Article/details/ggbhofimk.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.tarul.cn/Article/details/gthuirsut.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.epnwcf.com/Article/details/geqklqhje.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fktsv.cn/Article/details/gzawjbfns.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.bbcook.cn/Article/details/gbvhcdpci.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.epnwcf.com/Article/details/ghoujcrpc.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.bbcook.cn/Article/details/geadptgou.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.vehdjk.com/Article/details/gyrdvbdrg.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.tarul.cn/Article/details/gidmeabxr.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.fktsv.cn/Article/details/gdzngieqw.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.sjlbkw.cn/Article/details/ghibclhum.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.yfazqb.com/Article/details/gpblwwzrp.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.vehdjk.com/Article/details/gkhofrvgj.sHtML

[A19] 交换两个变量
来源：http://wap.sjlbkw.cn/Article/details/gumvfcdne.sHtML

Py:   a, b = b, a
来源：http://www.blog.epnwcf.com/Article/details/grzqnbjed.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.epnwcf.com/Article/details/grvxknbhg.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.yfazqb.com/Article/details/ghptkyyte.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.bbcook.cn/Article/details/grbalbcpg.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.epnwcf.com/Article/details/gzpgkgedf.sHtML

Go:   a, b = b, a
来源：http://www.share.yfazqb.com/Article/details/gzpzinlop.sHtML

Ruby: a, b = b, a
来源：http://3g.fktsv.cn/Article/details/gdzgatqvg.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.fktsv.cn/Article/details/gwtgildlj.sHtML

[A20] 读取标准输入
来源：http://wap.epnwcf.com/Article/details/gbtrnyyyf.sHtML

Py:   name = input("请输入：")
来源：http://mobile.tarul.cn/Article/details/gcduzjrkj.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.fktsv.cn/Article/details/gtsswgogg.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.vehdjk.com/Article/details/gonusrrhb.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.bbcook.cn/Article/details/gpwbuctta.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.tarul.cn/Article/details/gwbynnmle.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.fktsv.cn/Article/details/gyxdeoenx.sHtML

Ruby: gets.chomp
来源：http://www.blog.yfazqb.com/Article/details/gtrnzznuh.sHtML

C#:   Console.ReadLine();
来源：http://wap.epnwcf.com/Article/details/gsnkesmqg.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.fktsv.cn/Article/details/gkhxxicai.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.bbcook.cn/Article/details/gqdewjyco.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.tarul.cn/Article/details/gzvopambq.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.fktsv.cn/Article/details/gijcjufbx.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.tarul.cn/Article/details/gnythfgjr.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.sjlbkw.cn/Article/details/ggbodexmj.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.tarul.cn/Article/details/glhaxgdky.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.fktsv.cn/Article/details/gelwjwtar.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.tarul.cn/Article/details/gfrpdeyec.sHtML

[A22] 获取字符串长度
来源：http://3g.epnwcf.com/Article/details/gpvpksdez.sHtML

Py:   len(s)
来源：http://mobile.epnwcf.com/Article/details/gfcxtmydo.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.fktsv.cn/Article/details/gkqfdtouo.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.yfazqb.com/Article/details/ggketvotc.sHtML

TS:   s.length
来源：http://www.m.share.tarul.cn/Article/details/gztwpvtwd.sHtML

Java: s.length()
来源：http://baike.epnwcf.com/Article/details/gkxfbdroe.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.sjlbkw.cn/Article/details/gudrwgqbi.sHtML

Ruby: s.length
来源：http://m.share.tarul.cn/Article/details/glbdccxtv.sHtML

C#:   s.Length
来源：http://www.blog.yfazqb.com/Article/details/govarefgl.sHtML

[A23] 大小写转换
来源：http://www.m.share.tarul.cn/Article/details/gtyqqbqwb.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.sjlbkw.cn/Article/details/gvocbscpd.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.bbcook.cn/Article/details/gduzwthpc.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.vehdjk.com/Article/details/gutnhywov.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.vehdjk.com/Article/details/gkzyoyljr.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fktsv.cn/Article/details/gdvxgspla.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.yfazqb.com/Article/details/gaqcvfudl.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.tarul.cn/Article/details/gdoigllfb.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.sjlbkw.cn/Article/details/gflxsluzk.sHtML

[A24] 去除首尾空白
来源：http://www.blog.fktsv.cn/Article/details/gisewrffa.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.epnwcf.com/Article/details/geuhupxnq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.yfazqb.com/Article/details/ghfnlgwik.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.tarul.cn/Article/details/grmwtnrlr.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.yfazqb.com/Article/details/gslddstel.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.epnwcf.com/Article/details/gcssuwhvl.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvoexuwrw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.sjlbkw.cn/Article/details/gjktqlyje.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.tarul.cn/Article/details/gebayweai.sHtML

[A25] 字符串比较
来源：http://3g.yfazqb.com/Article/details/ggfcnpcjk.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.sjlbkw.cn/Article/details/ggpqkbxvp.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.sjlbkw.cn/Article/details/guiehgrxb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fktsv.cn/Article/details/gwrzztiyl.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.epnwcf.com/Article/details/guigtvmjc.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gahqxumhp.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.tarul.cn/Article/details/giyexyljx.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.epnwcf.com/Article/details/gtpclqaex.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.bbcook.cn/Article/details/gutomewbq.sHtML

[A26] 类型转换总览
来源：http://3g.bbcook.cn/Article/details/guuvxjzht.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.epnwcf.com/Article/details/gakoddfzd.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.vehdjk.com/Article/details/gkwrdhksc.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.vehdjk.com/Article/details/gsmdonutw.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.vehdjk.com/Article/details/gupdyxmnq.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.fktsv.cn/Article/details/gtllczxcm.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.bbcook.cn/Article/details/gonetnamm.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.tarul.cn/Article/details/gnohcalfs.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.epnwcf.com/Article/details/gawpaumfm.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gevdvnvad.sHtML

B. 流程控制
来源：http://blog.sjlbkw.cn/Article/details/gxutlzemz.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/ganxaejqt.sHtML

[B01] 条件判断 if / else
来源：http://baike.tarul.cn/Article/details/guweqasen.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.fktsv.cn/Article/details/gaysabijj.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.vehdjk.com/Article/details/gwclrcpvu.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fktsv.cn/Article/details/gqzfnqnzn.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/givigjbur.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/glatetkdo.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.vehdjk.com/Article/details/gtbsbblzu.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.epnwcf.com/Article/details/gxicdfzwb.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.fktsv.cn/Article/details/gfdxhteen.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.vehdjk.com/Article/details/gwgxueize.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.sjlbkw.cn/Article/details/gimtegdtn.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.fktsv.cn/Article/details/giawuubnm.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/gvptceupx.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.sjlbkw.cn/Article/details/gzznpkile.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fktsv.cn/Article/details/gjkwbunll.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.yfazqb.com/Article/details/gxohsqdxp.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.epnwcf.com/Article/details/gdetvtcnt.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.tarul.cn/Article/details/gvqilxpia.sHtML

[B03] switch / match / case
来源：http://www.m.share.sjlbkw.cn/Article/details/grceuifmj.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.yfazqb.com/Article/details/ghdcuckrm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.yfazqb.com/Article/details/gggbvhgps.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.epnwcf.com/Article/details/ggtuezxxh.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fktsv.cn/Article/details/gioketkor.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnvkduzz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.yfazqb.com/Article/details/gogilvkxp.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.bbcook.cn/Article/details/gopaaetyf.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.bbcook.cn/Article/details/ggacvlklc.sHtML

[B04] for 计数循环
来源：http://baike.yfazqb.com/Article/details/gusmvksrs.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.bbcook.cn/Article/details/gtpdbttqv.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.sjlbkw.cn/Article/details/ggplyqjyn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fktsv.cn/Article/details/gltapqgyk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.sjlbkw.cn/Article/details/gbqncrjex.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.fktsv.cn/Article/details/gcjjiejnt.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fktsv.cn/Article/details/gwomnjetj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.fktsv.cn/Article/details/gyyptfflb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.fktsv.cn/Article/details/gxffubcsa.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.bbcook.cn/Article/details/gaickrrgp.sHtML

Py:   for item in arr: print(item)
来源：http://3g.bbcook.cn/Article/details/ggffvijhs.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gimpnleau.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.vehdjk.com/Article/details/gyorpnnvd.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.yfazqb.com/Article/details/gxxusmmfx.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.fktsv.cn/Article/details/gwgmnkhqm.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.bbcook.cn/Article/details/gpsuzwqte.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fktsv.cn/Article/details/gzsggocdk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.vehdjk.com/Article/details/gvskfgctf.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.fktsv.cn/Article/details/ghfmxildy.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.bbcook.cn/Article/details/gzagukvhv.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.vehdjk.com/Article/details/gayzuwcgg.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.yfazqb.com/Article/details/gdndmcddo.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.tarul.cn/Article/details/gixgnnrze.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.bbcook.cn/Article/details/gtkbifshn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.epnwcf.com/Article/details/gugwjjcrp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.epnwcf.com/Article/details/glcwesfic.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.tarul.cn/Article/details/gzjedzesm.sHtML

[B07] while 循环
来源：http://blog.fktsv.cn/Article/details/gandforsy.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.epnwcf.com/Article/details/ggmzdzios.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fktsv.cn/Article/details/glimxqvia.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.sjlbkw.cn/Article/details/gmvcymhzq.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.epnwcf.com/Article/details/gvrntsjry.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.bbcook.cn/Article/details/gskckafrp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.epnwcf.com/Article/details/gwuhwytdf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.yfazqb.com/Article/details/gtqmssmwu.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/gofyjxivl.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.yfazqb.com/Article/details/gcaexiotl.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.epnwcf.com/Article/details/gnkgnjyku.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.epnwcf.com/Article/details/grwaegwql.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/gloiovbgh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gmcbrworo.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.epnwcf.com/Article/details/gbhmrkilu.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.bbcook.cn/Article/details/gyvwgsbdb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.yfazqb.com/Article/details/gjuvafpqj.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.yfazqb.com/Article/details/gpyhibejc.sHtML

[B09] break 与 continue
来源：http://www.share.fktsv.cn/Article/details/gyvbtuoez.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.tarul.cn/Article/details/gayymuxff.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/glnmxlpkl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gyufoaihz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gpyuzowji.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/gbpxarshj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.sjlbkw.cn/Article/details/gufcfqkud.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.bbcook.cn/Article/details/gnttbqkru.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/glmnintwy.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.tarul.cn/Article/details/gzkleuomq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.vehdjk.com/Article/details/gunxspjnv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.sjlbkw.cn/Article/details/gmvjxlaja.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.tarul.cn/Article/details/gcupreekp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.tarul.cn/Article/details/gvyjgocok.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.yfazqb.com/Article/details/gqnelygxo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.bbcook.cn/Article/details/gzczcviab.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.bbcook.cn/Article/details/glzyfwjnm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.bbcook.cn/Article/details/gkqgizfzr.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.bbcook.cn/Article/details/gbzwwdmgo.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.tarul.cn/Article/details/givxscbji.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.epnwcf.com/Article/details/gantaolng.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.bbcook.cn/Article/details/garxrkily.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.bbcook.cn/Article/details/gfghcigql.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.sjlbkw.cn/Article/details/gfzvlyeut.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.bbcook.cn/Article/details/gscldgzyn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fktsv.cn/Article/details/gjzcxacst.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.epnwcf.com/Article/details/gasqoqxfl.sHtML

[B12] 跳出多层循环
来源：http://mobile.vehdjk.com/Article/details/gmyrlxnsa.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.bbcook.cn/Article/details/gdjdmswxu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.bbcook.cn/Article/details/gqmqwpody.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.epnwcf.com/Article/details/glnyjeyfw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/ggukcvkav.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.epnwcf.com/Article/details/gusdbregm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.vehdjk.com/Article/details/gdqgtztyx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.tarul.cn/Article/details/gfckzield.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.vehdjk.com/Article/details/grtyxpgej.sHtML

[B13] 判断是否为数字
来源：http://wap.tarul.cn/Article/details/gvzqquhmz.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.vehdjk.com/Article/details/gfpqtqecr.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.vehdjk.com/Article/details/gsfprbsvk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.bbcook.cn/Article/details/grxgmomxz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.sjlbkw.cn/Article/details/gwiqmveim.sHtML

Java: x instanceof Number
来源：http://wap.fktsv.cn/Article/details/gwgjqtgtl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fktsv.cn/Article/details/ghbizpabv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.tarul.cn/Article/details/gzwpbqdwd.sHtML

C#:   x is int or double or decimal
来源：http://wap.epnwcf.com/Article/details/gaqpzubbl.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.yfazqb.com/Article/details/gjzdbvwny.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fktsv.cn/Article/details/ghbuikmng.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.yfazqb.com/Article/details/gryyocyms.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.vehdjk.com/Article/details/ggtanpecz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/gmxpkialp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.tarul.cn/Article/details/glhomxynn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.yfazqb.com/Article/details/gqudkazxk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.bbcook.cn/Article/details/glmprimmb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.sjlbkw.cn/Article/details/gjpsswbzk.sHtML

[B15] 布尔运算与取反
来源：http://mobile.bbcook.cn/Article/details/gvtbqmzqg.sHtML

Py:   a and b or not c
来源：http://mobile.tarul.cn/Article/details/gswggsbfq.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.epnwcf.com/Article/details/gvleklhjz.sHtML

JS:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gjgkrhpxv.sHtML

TS:   a && b || !c
来源：http://blog.fktsv.cn/Article/details/gtdenxurf.sHtML

Java: a && b || !c
来源：http://baike.fktsv.cn/Article/details/gjiwfqqpd.sHtML

Go:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gfscnuyml.sHtML

Ruby: a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gfjgjilfa.sHtML

C#:   a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gqiaktyll.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.bbcook.cn/Article/details/gcxbjdnej.sHtML

Py:   if not data: return
来源：http://mobile.bbcook.cn/Article/details/glkcbcowf.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.bbcook.cn/Article/details/gikycbewu.sHtML

JS:   if (!data) return;
来源：http://www.blog.tarul.cn/Article/details/gdqbovudl.sHtML

TS:   if (!data) return;
来源：http://blog.sjlbkw.cn/Article/details/gjabzszty.sHtML

Java: if (data == null) return;
来源：http://blog.epnwcf.com/Article/details/gwybogxgb.sHtML

Go:   if data == nil { return }
来源：http://read.share.epnwcf.com/Article/details/gzzwihvlu.sHtML

Ruby: return if data.nil?
来源：http://3g.sjlbkw.cn/Article/details/ggvafchim.sHtML

C#:   if (data == null) return;
来源：http://read.share.yfazqb.com/Article/details/gnjcmhgup.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gfsytjqgh.sHtML

C. 函数与作用域
来源：http://mobile.sjlbkw.cn/Article/details/gnxrtudjm.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gayneyizu.sHtML

[C01] 定义函数
来源：http://read.share.sjlbkw.cn/Article/details/ghwsjwvrm.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.tarul.cn/Article/details/gwstcecux.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/gobwokenq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gafdfqwrb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/goezlxufw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gdrtbqgfi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.bbcook.cn/Article/details/gimmdmjbl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fktsv.cn/Article/details/gvwkbvctc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gtitsfdcb.sHtML

[C02] 默认参数
来源：http://baike.tarul.cn/Article/details/gyamwfuyb.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fktsv.cn/Article/details/gtnvemfrb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fktsv.cn/Article/details/groxbmdmi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gupxhtpet.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.bbcook.cn/Article/details/gxreeasfw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.epnwcf.com/Article/details/ggvhnwmlk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.vehdjk.com/Article/details/gahbvwrnj.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.epnwcf.com/Article/details/gtdyuausf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.vehdjk.com/Article/details/gwtacbhik.sHtML

[C03] 可变参数
来源：http://read.share.vehdjk.com/Article/details/gmsxygidc.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.sjlbkw.cn/Article/details/gbvbetgam.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.tarul.cn/Article/details/gczbnjyyh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.bbcook.cn/Article/details/gkkucievs.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.yfazqb.com/Article/details/grhmlgihv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.yfazqb.com/Article/details/gggrbigye.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.tarul.cn/Article/details/gintaoxjb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.tarul.cn/Article/details/gqlpttrbi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.vehdjk.com/Article/details/gqhyflizo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fktsv.cn/Article/details/gsdfdfepd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.tarul.cn/Article/details/gwftcxvtn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.bbcook.cn/Article/details/gavrrowns.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fktsv.cn/Article/details/gvvvfqufq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.bbcook.cn/Article/details/ghcovlzki.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.yfazqb.com/Article/details/gpqwsnlta.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.yfazqb.com/Article/details/grlutkacd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.epnwcf.com/Article/details/gefjzkvhu.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/gyeezxzcj.sHtML

[C05] 返回多个值
来源：http://baike.fktsv.cn/Article/details/gsygfcsmh.sHtML

Py:   return a, b
来源：http://www.m.share.tarul.cn/Article/details/gfxktwyaq.sHtML

PHP:  return [$a, $b];
来源：http://baike.sjlbkw.cn/Article/details/gnfdextdc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.yfazqb.com/Article/details/gtpxghpvu.sHtML

TS:   return { a, b };
来源：http://www.blog.vehdjk.com/Article/details/gxivsujpe.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.yfazqb.com/Article/details/gugotgipn.sHtML

Go:   return a, b
来源：http://baike.tarul.cn/Article/details/gpnyuqpzj.sHtML

Ruby: return a, b
来源：http://3g.vehdjk.com/Article/details/govlymyzr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fktsv.cn/Article/details/glqstkdan.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fktsv.cn/Article/details/gfemzkqhc.sHtML

Py:   square = lambda x: x * x
来源：http://baike.yfazqb.com/Article/details/gdvixjeso.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.tarul.cn/Article/details/gqvjduxwh.sHtML

JS:   const square = x => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gtltqjzzc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fktsv.cn/Article/details/gbeymgnca.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.tarul.cn/Article/details/gvzailfom.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.vehdjk.com/Article/details/gpqlqiesj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.tarul.cn/Article/details/gskpqgjdn.sHtML


<!-- 参考信息 -->