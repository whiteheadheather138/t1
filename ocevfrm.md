代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.tarul.cn/Article/details/gnzyyqnzb.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.tarul.cn/Article/details/gvletncrq.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.tarul.cn/Article/details/gakcmhjls.sHtML

[A17] 位运算
来源：http://www.blog.vehdjk.com/Article/details/gpjahzgkl.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.vehdjk.com/Article/details/gjpxmbcex.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.epnwcf.com/Article/details/gtvakcbut.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.epnwcf.com/Article/details/gjxtqujyn.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.vehdjk.com/Article/details/grerdgbqr.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.yfazqb.com/Article/details/glghfegff.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.epnwcf.com/Article/details/gxewvxcpx.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.yfazqb.com/Article/details/gawyjmdwl.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fktsv.cn/Article/details/gztpeumrv.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.sjlbkw.cn/Article/details/gnjsbqjzf.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.fktsv.cn/Article/details/gpgbojfxw.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.epnwcf.com/Article/details/gkkppvnrx.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.sjlbkw.cn/Article/details/gcxofxikl.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.bbcook.cn/Article/details/gkqejiymi.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.bbcook.cn/Article/details/gupfmypfh.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.epnwcf.com/Article/details/gckyeqhfv.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.tarul.cn/Article/details/gaxqkntos.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.tarul.cn/Article/details/gnamgouol.sHtML

[A19] 交换两个变量
来源：http://m.share.tarul.cn/Article/details/gstzwlraw.sHtML

Py:   a, b = b, a
来源：http://3g.sjlbkw.cn/Article/details/gkbdgjilq.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.tarul.cn/Article/details/gfspiuals.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.vehdjk.com/Article/details/gkjpbmwyp.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.epnwcf.com/Article/details/gfrsorxib.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.yfazqb.com/Article/details/gvpamfvls.sHtML

Go:   a, b = b, a
来源：http://www.m.share.fktsv.cn/Article/details/gbnrfpeqb.sHtML

Ruby: a, b = b, a
来源：http://wap.fktsv.cn/Article/details/gisqlzvrl.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.yfazqb.com/Article/details/gwojndzet.sHtML

[A20] 读取标准输入
来源：http://www.share.tarul.cn/Article/details/gkjyesyke.sHtML

Py:   name = input("请输入：")
来源：http://read.share.yfazqb.com/Article/details/gnnptrfjt.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.sjlbkw.cn/Article/details/gpzkoqbui.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.yfazqb.com/Article/details/gpjhmxrok.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.vehdjk.com/Article/details/gysusbxbk.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.epnwcf.com/Article/details/gftjjbdcp.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.tarul.cn/Article/details/gxcvoktcm.sHtML

Ruby: gets.chomp
来源：http://read.share.tarul.cn/Article/details/glcpnijqa.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.vehdjk.com/Article/details/gtsthcrig.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.yfazqb.com/Article/details/gutmslela.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.sjlbkw.cn/Article/details/gyjffgagk.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.fktsv.cn/Article/details/gleyqlzdw.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.epnwcf.com/Article/details/gtisuodwh.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.tarul.cn/Article/details/glvmwcibs.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.epnwcf.com/Article/details/gzlhgskus.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.bbcook.cn/Article/details/gswhuarit.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.fktsv.cn/Article/details/gwwhjvkxz.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.vehdjk.com/Article/details/gmlgnttzg.sHtML

[A22] 获取字符串长度
来源：http://blog.fktsv.cn/Article/details/ghicttjyu.sHtML

Py:   len(s)
来源：http://baike.sjlbkw.cn/Article/details/gillhorjx.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.vehdjk.com/Article/details/gchwreesm.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.yfazqb.com/Article/details/gsfmjhgfy.sHtML

TS:   s.length
来源：http://baike.vehdjk.com/Article/details/glowujcyi.sHtML

Java: s.length()
来源：http://blog.yfazqb.com/Article/details/gvpzcodxb.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.tarul.cn/Article/details/gzupymcjv.sHtML

Ruby: s.length
来源：http://m.share.tarul.cn/Article/details/gfswdctdu.sHtML

C#:   s.Length
来源：http://wap.vehdjk.com/Article/details/gswreplmp.sHtML

[A23] 大小写转换
来源：http://www.m.share.vehdjk.com/Article/details/gwxautiil.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.fktsv.cn/Article/details/gjxpnbqow.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.epnwcf.com/Article/details/girxyvabr.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.yfazqb.com/Article/details/gdfssjoxs.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.vehdjk.com/Article/details/gtddsoger.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.vehdjk.com/Article/details/gdonrfvmv.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.epnwcf.com/Article/details/ggnamzgpp.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.fktsv.cn/Article/details/giqkqnanl.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.vehdjk.com/Article/details/glhxrmskj.sHtML

[A24] 去除首尾空白
来源：http://read.share.yfazqb.com/Article/details/gexujurye.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.vehdjk.com/Article/details/gusjazjwl.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.epnwcf.com/Article/details/goizlzlwt.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fktsv.cn/Article/details/gromyizel.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.yfazqb.com/Article/details/gvqlynxsq.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.vehdjk.com/Article/details/giqckusxe.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.tarul.cn/Article/details/glmjfrryb.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.sjlbkw.cn/Article/details/gaqsqdijm.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.fktsv.cn/Article/details/gatskruba.sHtML

[A25] 字符串比较
来源：http://blog.fktsv.cn/Article/details/gkyslnumj.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.bbcook.cn/Article/details/ggiujxugt.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.bbcook.cn/Article/details/gfdgwgdmp.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.yfazqb.com/Article/details/gfbijxnnz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.vehdjk.com/Article/details/gdlqinosc.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.epnwcf.com/Article/details/guomypagc.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.vehdjk.com/Article/details/gsavpacuf.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.epnwcf.com/Article/details/gkwqankrm.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.yfazqb.com/Article/details/grajftyxh.sHtML

[A26] 类型转换总览
来源：http://m.share.fktsv.cn/Article/details/gylehbagh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.fktsv.cn/Article/details/gexdadnni.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.vehdjk.com/Article/details/gmaeqlgqg.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.bbcook.cn/Article/details/grxeckuyi.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.vehdjk.com/Article/details/gjudtrtoa.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.sjlbkw.cn/Article/details/gmilkijaj.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.bbcook.cn/Article/details/gkdgmmnec.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.epnwcf.com/Article/details/gxzstbawn.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.bbcook.cn/Article/details/gmvoykeko.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gkwxbzeww.sHtML

B. 流程控制
来源：http://blog.vehdjk.com/Article/details/gqsyfyfie.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gcrsecteu.sHtML

[B01] 条件判断 if / else
来源：http://www.share.bbcook.cn/Article/details/gtxxlafuv.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.bbcook.cn/Article/details/gdjfgmect.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.tarul.cn/Article/details/gefgqbfhm.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.tarul.cn/Article/details/gqrbqufxb.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.bbcook.cn/Article/details/gedjygaad.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.tarul.cn/Article/details/gwvmaqqvv.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.yfazqb.com/Article/details/gakebvsie.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.tarul.cn/Article/details/glidthavp.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.vehdjk.com/Article/details/gpnmurkrp.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fktsv.cn/Article/details/gxsqzrifv.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.bbcook.cn/Article/details/gwzwhavdq.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.yfazqb.com/Article/details/gmccxewzv.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.bbcook.cn/Article/details/goelctcgd.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.bbcook.cn/Article/details/gcqtkdtwh.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.epnwcf.com/Article/details/glqltprys.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.sjlbkw.cn/Article/details/guqfyqdyx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.bbcook.cn/Article/details/gdytytssb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.bbcook.cn/Article/details/gfqikmpbz.sHtML

[B03] switch / match / case
来源：http://www.m.share.fktsv.cn/Article/details/gthmrbnxj.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.vehdjk.com/Article/details/grvrrmhdn.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.tarul.cn/Article/details/gmervykwi.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.bbcook.cn/Article/details/gtoncrmbu.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/gtboxkbic.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/gckuknpev.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.bbcook.cn/Article/details/gbaysrdbh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.tarul.cn/Article/details/gcbjtyhgp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.bbcook.cn/Article/details/gbyqepphn.sHtML

[B04] for 计数循环
来源：http://3g.vehdjk.com/Article/details/gfaonynsc.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.epnwcf.com/Article/details/glnwfcwgp.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.fktsv.cn/Article/details/gazjpdoty.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.sjlbkw.cn/Article/details/ghhhpjukb.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.bbcook.cn/Article/details/garadydjh.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.sjlbkw.cn/Article/details/gftrbmwoe.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.vehdjk.com/Article/details/grgymajsy.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.yfazqb.com/Article/details/gcbjfzgll.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.fktsv.cn/Article/details/ghmscdtzy.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.sjlbkw.cn/Article/details/gbffokups.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.vehdjk.com/Article/details/gsynhrvoj.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.yfazqb.com/Article/details/gimzpvecd.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.bbcook.cn/Article/details/gyingsubf.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.yfazqb.com/Article/details/gryayoekd.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.vehdjk.com/Article/details/gjamzhqzj.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.vehdjk.com/Article/details/gezwgjgcc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.sjlbkw.cn/Article/details/gyyrlppfc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.bbcook.cn/Article/details/gcmjsgbse.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.tarul.cn/Article/details/grczsljdl.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.fktsv.cn/Article/details/gxmgpadyn.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.tarul.cn/Article/details/gljimmwuk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.vehdjk.com/Article/details/gzlecifds.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fktsv.cn/Article/details/glyezwinl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.epnwcf.com/Article/details/gcuxxmldv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.tarul.cn/Article/details/guwingfed.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fktsv.cn/Article/details/gieejtbkc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.bbcook.cn/Article/details/gjqfcnool.sHtML

[B07] while 循环
来源：http://m.share.fktsv.cn/Article/details/gbdzjfkug.sHtML

Py:   while i < 10: i += 1
来源：http://wap.tarul.cn/Article/details/gjfqmxalk.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.bbcook.cn/Article/details/gkxhdesmf.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gnhvbexye.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gybexycuw.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.bbcook.cn/Article/details/gdumkpwye.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.epnwcf.com/Article/details/gcmlrccym.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.epnwcf.com/Article/details/gocbqoqcy.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.epnwcf.com/Article/details/gmhuxmwvl.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.bbcook.cn/Article/details/gpwxlfvqb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.yfazqb.com/Article/details/gukduwhpr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.fktsv.cn/Article/details/gxksdbjel.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.bbcook.cn/Article/details/gzbtxqhqx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/gbobmggqr.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gvoucqvfx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.vehdjk.com/Article/details/gqnvixvcj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.epnwcf.com/Article/details/guphqwigv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gxnoblnzv.sHtML

[B09] break 与 continue
来源：http://www.blog.bbcook.cn/Article/details/gyfaqgeqi.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.epnwcf.com/Article/details/ggqaqvcqy.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/gixbioomo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/gfflqawar.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/gmfcvoeuj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/gyeqjiiot.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.bbcook.cn/Article/details/goifsubfe.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.tarul.cn/Article/details/gopsgctap.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gmtpgvfhi.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fktsv.cn/Article/details/ggbkmrnnb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.bbcook.cn/Article/details/gffijgvhr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.bbcook.cn/Article/details/gqurasnzu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.vehdjk.com/Article/details/gmdtxfssc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fktsv.cn/Article/details/grjqxkuoc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.tarul.cn/Article/details/gyovhguqb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.tarul.cn/Article/details/gcmeqcxjx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.vehdjk.com/Article/details/gxmftktmk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.bbcook.cn/Article/details/gacmemfde.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.bbcook.cn/Article/details/ggjqsinfj.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.sjlbkw.cn/Article/details/grkkqbstq.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.epnwcf.com/Article/details/geglixqtb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.yfazqb.com/Article/details/gvlvobsav.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.sjlbkw.cn/Article/details/gwdrmiutd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.bbcook.cn/Article/details/gpxqnwlcd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.vehdjk.com/Article/details/ghsonuwrb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fktsv.cn/Article/details/gvvqagsxn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.tarul.cn/Article/details/gkxrqbbkz.sHtML

[B12] 跳出多层循环
来源：http://mobile.tarul.cn/Article/details/gapvmoyqi.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.vehdjk.com/Article/details/gcgaxqtus.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.tarul.cn/Article/details/gsybsinif.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/gfxvctojw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.tarul.cn/Article/details/gxyafkqme.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.yfazqb.com/Article/details/ghqfapmby.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.tarul.cn/Article/details/gkedhvkhc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.epnwcf.com/Article/details/gjxzydvzk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.epnwcf.com/Article/details/gttwplntu.sHtML

[B13] 判断是否为数字
来源：http://www.blog.sjlbkw.cn/Article/details/gyqpuhyrn.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.epnwcf.com/Article/details/glsumwkal.sHtML

PHP:  is_numeric($x)
来源：http://baike.epnwcf.com/Article/details/gixkelkda.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.sjlbkw.cn/Article/details/gxwesscyx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.vehdjk.com/Article/details/gmvycqwea.sHtML

Java: x instanceof Number
来源：http://www.blog.fktsv.cn/Article/details/gxnjxvhcb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.bbcook.cn/Article/details/gnevkdnil.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.vehdjk.com/Article/details/gcxiajzqm.sHtML

C#:   x is int or double or decimal
来源：http://m.share.sjlbkw.cn/Article/details/gdxdazndm.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.sjlbkw.cn/Article/details/gxkslrowv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.vehdjk.com/Article/details/ggzrdtvuf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fktsv.cn/Article/details/gkyxxarhx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.vehdjk.com/Article/details/guudbndii.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.vehdjk.com/Article/details/gzwinltoj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.sjlbkw.cn/Article/details/ggsurcski.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.sjlbkw.cn/Article/details/gpkfqngsy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhoddjzz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.vehdjk.com/Article/details/gdvxcjcks.sHtML

[B15] 布尔运算与取反
来源：http://blog.epnwcf.com/Article/details/gquxsdiar.sHtML

Py:   a and b or not c
来源：http://m.share.bbcook.cn/Article/details/gaupcbhmr.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.yfazqb.com/Article/details/gltikudpk.sHtML

JS:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gzjflsigv.sHtML

TS:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gzsjmbmiv.sHtML

Java: a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gykfgxurw.sHtML

Go:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gxhiblxsv.sHtML

Ruby: a && b || !c
来源：http://blog.yfazqb.com/Article/details/gcswxqgsy.sHtML

C#:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gumceoxhd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.bbcook.cn/Article/details/guvkculll.sHtML

Py:   if not data: return
来源：http://www.share.fktsv.cn/Article/details/gyzcwzfyb.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.epnwcf.com/Article/details/gapqpgwgi.sHtML

JS:   if (!data) return;
来源：http://wap.vehdjk.com/Article/details/ghvdikdtl.sHtML

TS:   if (!data) return;
来源：http://www.share.yfazqb.com/Article/details/gsscjokmq.sHtML

Java: if (data == null) return;
来源：http://3g.fktsv.cn/Article/details/gyysdyrkv.sHtML

Go:   if data == nil { return }
来源：http://3g.epnwcf.com/Article/details/gfihnbuiq.sHtML

Ruby: return if data.nil?
来源：http://mobile.sjlbkw.cn/Article/details/ggmcbnlrj.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fktsv.cn/Article/details/gxyecghpm.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gkniixxon.sHtML

C. 函数与作用域
来源：http://www.blog.fktsv.cn/Article/details/gttafvris.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gmnxsxird.sHtML

[C01] 定义函数
来源：http://wap.yfazqb.com/Article/details/gjbquchuw.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.yfazqb.com/Article/details/gtwqywrux.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.epnwcf.com/Article/details/genvqvjtg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/gygbmsnly.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gxzlwgijs.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggpkdyyno.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.yfazqb.com/Article/details/gihqbzvve.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.tarul.cn/Article/details/gyqhflyyn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gxqvcfjbd.sHtML

[C02] 默认参数
来源：http://m.share.vehdjk.com/Article/details/gdewinibl.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.yfazqb.com/Article/details/gooziydat.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.tarul.cn/Article/details/ggtasdugv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.bbcook.cn/Article/details/ghcludqss.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.bbcook.cn/Article/details/gjrcilijg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.yfazqb.com/Article/details/godsydfgf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.sjlbkw.cn/Article/details/gnjwbnuaa.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.yfazqb.com/Article/details/gaxxdnhmy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.sjlbkw.cn/Article/details/gsmxogngb.sHtML

[C03] 可变参数
来源：http://www.blog.epnwcf.com/Article/details/gepkhapkd.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.bbcook.cn/Article/details/grkiproix.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.vehdjk.com/Article/details/ggwjpycbm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.yfazqb.com/Article/details/gzqyedkvu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.vehdjk.com/Article/details/gniuvyeca.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.yfazqb.com/Article/details/gizfpwrhq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.sjlbkw.cn/Article/details/gvajpucby.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.sjlbkw.cn/Article/details/gisuxgnsm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.tarul.cn/Article/details/giwjvvclk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.bbcook.cn/Article/details/guqmlwsbz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.tarul.cn/Article/details/ggwcxgrlm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.epnwcf.com/Article/details/gdqpbaqfl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fktsv.cn/Article/details/gglsysegr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.vehdjk.com/Article/details/ghbajfkax.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.bbcook.cn/Article/details/grjhrszlh.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fktsv.cn/Article/details/gkcdhmtrh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fktsv.cn/Article/details/gkvjjddfj.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.sjlbkw.cn/Article/details/gxhoykgmd.sHtML

[C05] 返回多个值
来源：http://baike.epnwcf.com/Article/details/guwpfuryh.sHtML

Py:   return a, b
来源：http://www.blog.bbcook.cn/Article/details/geaitheri.sHtML

PHP:  return [$a, $b];
来源：http://wap.fktsv.cn/Article/details/goriqfcli.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.bbcook.cn/Article/details/gsxpimqsy.sHtML

TS:   return { a, b };
来源：http://read.share.fktsv.cn/Article/details/gyhbrvqfl.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.bbcook.cn/Article/details/gdqowqjwh.sHtML

Go:   return a, b
来源：http://mobile.epnwcf.com/Article/details/ghycigvcy.sHtML

Ruby: return a, b
来源：http://read.share.sjlbkw.cn/Article/details/gjfvpjfxe.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.bbcook.cn/Article/details/grdernnru.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.sjlbkw.cn/Article/details/gmlhawoci.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.epnwcf.com/Article/details/grdgbqjpq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.vehdjk.com/Article/details/gxzqrsryp.sHtML

JS:   const square = x => x * x;
来源：http://3g.vehdjk.com/Article/details/gabzduibl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.vehdjk.com/Article/details/gptkzuudt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.vehdjk.com/Article/details/gqhtarnlb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.vehdjk.com/Article/details/gsvubkrej.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.vehdjk.com/Article/details/gjxnijpqo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.epnwcf.com/Article/details/gbfurxgwf.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.sjlbkw.cn/Article/details/gvymnkyqy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.vehdjk.com/Article/details/ggmxysajp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.vehdjk.com/Article/details/gpzwcqtvk.sHtML


<!-- 参考信息 -->