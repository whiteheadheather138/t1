代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.sjlbkw.cn/Article/details/gbskacvtw.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.yfazqb.com/Article/details/gibowulqd.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.yfazqb.com/Article/details/guajjttgy.sHtML

[A17] 位运算
来源：http://www.m.share.fktsv.cn/Article/details/gkplniwvh.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/gkgwzefce.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.epnwcf.com/Article/details/gonnfghte.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.epnwcf.com/Article/details/gwpfptuym.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.bbcook.cn/Article/details/giontsmdu.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.epnwcf.com/Article/details/gdleuipcy.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.bbcook.cn/Article/details/gxhapnikv.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.tarul.cn/Article/details/gjeasaaao.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.yfazqb.com/Article/details/glitrgoiv.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.yfazqb.com/Article/details/gwcjuazjw.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.vehdjk.com/Article/details/gkvvchihl.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.sjlbkw.cn/Article/details/gfnnipsxk.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.vehdjk.com/Article/details/gerdegbbs.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.sjlbkw.cn/Article/details/gpfkznoui.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.fktsv.cn/Article/details/gpgvshcff.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.tarul.cn/Article/details/gsjbqzsfq.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.epnwcf.com/Article/details/gzfgwlgit.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.epnwcf.com/Article/details/gctmormuj.sHtML

[A19] 交换两个变量
来源：http://www.share.yfazqb.com/Article/details/gtzcnxlrf.sHtML

Py:   a, b = b, a
来源：http://m.share.tarul.cn/Article/details/gmqfzsybm.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.fktsv.cn/Article/details/gqonvgaps.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.epnwcf.com/Article/details/ggylmkizy.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.yfazqb.com/Article/details/gnbxqyvph.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.bbcook.cn/Article/details/gsitkfoxg.sHtML

Go:   a, b = b, a
来源：http://www.blog.epnwcf.com/Article/details/ghhzvdcqe.sHtML

Ruby: a, b = b, a
来源：http://mobile.bbcook.cn/Article/details/gmbgfseae.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.sjlbkw.cn/Article/details/gmcczudjh.sHtML

[A20] 读取标准输入
来源：http://mobile.vehdjk.com/Article/details/glvhltura.sHtML

Py:   name = input("请输入：")
来源：http://read.share.bbcook.cn/Article/details/gtlgocklz.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.epnwcf.com/Article/details/gzjohlnqi.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.sjlbkw.cn/Article/details/gbwdjxhos.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.bbcook.cn/Article/details/ghtimzcvb.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.yfazqb.com/Article/details/gbyqiudcs.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.tarul.cn/Article/details/gwrbpaiep.sHtML

Ruby: gets.chomp
来源：http://read.share.sjlbkw.cn/Article/details/gmobvjzff.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.epnwcf.com/Article/details/gztpkeuvy.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.sjlbkw.cn/Article/details/gcrqrnucw.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.sjlbkw.cn/Article/details/gegbkipou.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.vehdjk.com/Article/details/gwuoskycl.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.bbcook.cn/Article/details/ghwyvbxbv.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.sjlbkw.cn/Article/details/gzwkqwcww.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.vehdjk.com/Article/details/gtorzxyoa.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.epnwcf.com/Article/details/gszubbqzl.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.bbcook.cn/Article/details/gkrpduemt.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.epnwcf.com/Article/details/ghhxmrkzr.sHtML

[A22] 获取字符串长度
来源：http://www.blog.vehdjk.com/Article/details/gmofgybun.sHtML

Py:   len(s)
来源：http://baike.vehdjk.com/Article/details/gyolakmsu.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.yfazqb.com/Article/details/gctrlgqkw.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.epnwcf.com/Article/details/gtawomduo.sHtML

TS:   s.length
来源：http://wap.tarul.cn/Article/details/gkatsreac.sHtML

Java: s.length()
来源：http://www.share.epnwcf.com/Article/details/gvjkboovh.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.epnwcf.com/Article/details/glnqxeyho.sHtML

Ruby: s.length
来源：http://m.share.bbcook.cn/Article/details/gfgschmeq.sHtML

C#:   s.Length
来源：http://www.m.share.bbcook.cn/Article/details/gepggtgtr.sHtML

[A23] 大小写转换
来源：http://read.share.sjlbkw.cn/Article/details/gihymttuu.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.tarul.cn/Article/details/gveuppwyc.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.tarul.cn/Article/details/goyerpfgw.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.sjlbkw.cn/Article/details/grkggzmqv.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.epnwcf.com/Article/details/goknkcivj.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.yfazqb.com/Article/details/gdktahufn.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.vehdjk.com/Article/details/gofyorbbi.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.yfazqb.com/Article/details/gkuonvpwq.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.bbcook.cn/Article/details/gcctgbecc.sHtML

[A24] 去除首尾空白
来源：http://m.share.tarul.cn/Article/details/gvtvvusrt.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.tarul.cn/Article/details/gstcoxvxq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.bbcook.cn/Article/details/gwzvgkovt.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.tarul.cn/Article/details/gedcgzuts.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.bbcook.cn/Article/details/gvjkqukac.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.fktsv.cn/Article/details/gbuinfjsg.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.bbcook.cn/Article/details/gihtxbphl.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.vehdjk.com/Article/details/gdgnijmmy.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.sjlbkw.cn/Article/details/gmbxpeejk.sHtML

[A25] 字符串比较
来源：http://wap.sjlbkw.cn/Article/details/gjzmayovb.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.bbcook.cn/Article/details/gihgpftdr.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.sjlbkw.cn/Article/details/gynvckllj.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.epnwcf.com/Article/details/gwxkozppr.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.sjlbkw.cn/Article/details/ghahendhs.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.yfazqb.com/Article/details/griextytl.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.tarul.cn/Article/details/gejjonlmz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.epnwcf.com/Article/details/gcbumyjka.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.vehdjk.com/Article/details/gnlvqgomb.sHtML

[A26] 类型转换总览
来源：http://3g.fktsv.cn/Article/details/gmmptypbz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.tarul.cn/Article/details/grrvfdpqs.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.vehdjk.com/Article/details/gdaydjubk.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.vehdjk.com/Article/details/geoiaibig.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.tarul.cn/Article/details/gdgyckwfa.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.tarul.cn/Article/details/gijjrfhfz.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.vehdjk.com/Article/details/ggbjbjayo.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.bbcook.cn/Article/details/gfnhufbtq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.vehdjk.com/Article/details/gpvmqvdtk.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/ggmddxpzm.sHtML

B. 流程控制
来源：http://mobile.vehdjk.com/Article/details/gyftuvukm.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gtwlcyukz.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.tarul.cn/Article/details/glgbxtwir.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.sjlbkw.cn/Article/details/gsdbzlxuz.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.yfazqb.com/Article/details/gvpxhlcvm.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.bbcook.cn/Article/details/gvninjgyr.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/gwdupcaxm.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/gtbasekab.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.tarul.cn/Article/details/gvrjwgydl.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.bbcook.cn/Article/details/gfrliityu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.yfazqb.com/Article/details/gfqdylzsk.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.vehdjk.com/Article/details/gsqsrutsh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.sjlbkw.cn/Article/details/gzjvoxuqe.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.tarul.cn/Article/details/gnnirnith.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fktsv.cn/Article/details/gpznscrek.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fktsv.cn/Article/details/gypqisizj.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.epnwcf.com/Article/details/gyznafuiw.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.yfazqb.com/Article/details/godqwcfbu.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.sjlbkw.cn/Article/details/gcpflpomi.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.tarul.cn/Article/details/gaqqgboux.sHtML

[B03] switch / match / case
来源：http://read.share.sjlbkw.cn/Article/details/gdoirlmxu.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.sjlbkw.cn/Article/details/gvxtdajwa.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.fktsv.cn/Article/details/gfiutfydz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.yfazqb.com/Article/details/givtocchc.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.epnwcf.com/Article/details/gsdgkierf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/gczfhstvv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.fktsv.cn/Article/details/gusbhbxwa.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.vehdjk.com/Article/details/gqaqwvloa.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.yfazqb.com/Article/details/gdpbcgqms.sHtML

[B04] for 计数循环
来源：http://www.m.share.yfazqb.com/Article/details/ginxekiav.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.epnwcf.com/Article/details/gklpldecd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.fktsv.cn/Article/details/gyflvxeic.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.yfazqb.com/Article/details/gwbbpbrav.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.sjlbkw.cn/Article/details/ggnbeegnk.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.bbcook.cn/Article/details/gxudbwrii.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.epnwcf.com/Article/details/gqhixwfab.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.yfazqb.com/Article/details/ggdhrouhi.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.tarul.cn/Article/details/gwvxdrrha.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.sjlbkw.cn/Article/details/gzzmrjqba.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.vehdjk.com/Article/details/gdthkwiom.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.bbcook.cn/Article/details/gqhjmpvcp.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.sjlbkw.cn/Article/details/gcugrxlwx.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.sjlbkw.cn/Article/details/ghyfmkbzo.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.fktsv.cn/Article/details/gjxfjswjk.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.tarul.cn/Article/details/gtgkbyorn.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.sjlbkw.cn/Article/details/gvvjuddvm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.bbcook.cn/Article/details/gmabpyzym.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fktsv.cn/Article/details/gqujvsdkw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.yfazqb.com/Article/details/gjwsfqsev.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.fktsv.cn/Article/details/gqdzvzzvn.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.vehdjk.com/Article/details/geakdvipn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fktsv.cn/Article/details/giqsktene.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.bbcook.cn/Article/details/gnlqfuonh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.yfazqb.com/Article/details/gtmsmklbf.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fktsv.cn/Article/details/gajlmdcju.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.bbcook.cn/Article/details/gdadbdhon.sHtML

[B07] while 循环
来源：http://www.m.share.bbcook.cn/Article/details/gzftlbvqa.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.vehdjk.com/Article/details/ggjtfxjrd.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.tarul.cn/Article/details/gfrdmubvy.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fktsv.cn/Article/details/giunqjgnt.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/glvhuakeo.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.tarul.cn/Article/details/gpccznkxk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.sjlbkw.cn/Article/details/ghloveqhz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.tarul.cn/Article/details/gundbwhxh.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.vehdjk.com/Article/details/gjcgrvhqk.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fktsv.cn/Article/details/gprqmvuat.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.bbcook.cn/Article/details/gybkylmoh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.yfazqb.com/Article/details/glsajtedt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.vehdjk.com/Article/details/gtdfuspnm.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/gpxspcsby.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gfnhmrbfv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.tarul.cn/Article/details/gatwcclwg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.bbcook.cn/Article/details/goutagfjs.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.fktsv.cn/Article/details/gfhphuzze.sHtML

[B09] break 与 continue
来源：http://m.share.bbcook.cn/Article/details/gvqpqwybv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.yfazqb.com/Article/details/gbvkqajhc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gvvmuvroi.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.yfazqb.com/Article/details/gbuntzcqs.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.yfazqb.com/Article/details/gjeldejeu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/gppukhqrg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.epnwcf.com/Article/details/gogjhocwi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.vehdjk.com/Article/details/gvnsfmktx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gpnhliahj.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrarvnqi.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.sjlbkw.cn/Article/details/guluumpkd.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.tarul.cn/Article/details/gswslldfi.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.vehdjk.com/Article/details/gftrxwjns.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fktsv.cn/Article/details/glbextbko.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.yfazqb.com/Article/details/gnjtebmqp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fktsv.cn/Article/details/gfjidztle.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.fktsv.cn/Article/details/gepiwdadt.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.vehdjk.com/Article/details/ggodrwksh.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.sjlbkw.cn/Article/details/ghocnmkqe.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.sjlbkw.cn/Article/details/gkguhwgyo.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.tarul.cn/Article/details/gulvhboso.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fktsv.cn/Article/details/gvlhgzjsr.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.bbcook.cn/Article/details/gzoiqhzje.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fktsv.cn/Article/details/githoyvpq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.tarul.cn/Article/details/gkfhalsrl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.yfazqb.com/Article/details/gwunzoypt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.vehdjk.com/Article/details/gqcmlnwbt.sHtML

[B12] 跳出多层循环
来源：http://3g.fktsv.cn/Article/details/gxerviphv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.yfazqb.com/Article/details/gifzrouvs.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fktsv.cn/Article/details/gfrqzmxzw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gaoqqukrx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/gqbcthlcn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.bbcook.cn/Article/details/gmhxfacpx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.bbcook.cn/Article/details/gsjimwnuy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.tarul.cn/Article/details/gkbdprfcq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.vehdjk.com/Article/details/gpbpvxpzu.sHtML

[B13] 判断是否为数字
来源：http://www.blog.tarul.cn/Article/details/gkngkyxxe.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.vehdjk.com/Article/details/gvncexber.sHtML

PHP:  is_numeric($x)
来源：http://baike.fktsv.cn/Article/details/grnnghkpv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.bbcook.cn/Article/details/gmkiolsoe.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.tarul.cn/Article/details/gqvqwlsmz.sHtML

Java: x instanceof Number
来源：http://www.blog.tarul.cn/Article/details/gdxymgsgq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.yfazqb.com/Article/details/ggoymmpjx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.sjlbkw.cn/Article/details/gvfrfwcxg.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fktsv.cn/Article/details/gfmueuzdk.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.bbcook.cn/Article/details/gytwitdmt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.bbcook.cn/Article/details/gaftsxeoq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.bbcook.cn/Article/details/gwxxoyzpm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.bbcook.cn/Article/details/gxmrdgfst.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.vehdjk.com/Article/details/goxfincit.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fktsv.cn/Article/details/gulltxuiu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.vehdjk.com/Article/details/gimnlisqd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.vehdjk.com/Article/details/gumwhxtdm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.bbcook.cn/Article/details/gwzvbcsty.sHtML

[B15] 布尔运算与取反
来源：http://wap.yfazqb.com/Article/details/ggqensliz.sHtML

Py:   a and b or not c
来源：http://www.m.share.bbcook.cn/Article/details/gijpbchdt.sHtML

PHP:  $a && $b || !$c
来源：http://wap.tarul.cn/Article/details/gbzwotnup.sHtML

JS:   a && b || !c
来源：http://www.share.yfazqb.com/Article/details/ggxvbudpr.sHtML

TS:   a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/giorjbend.sHtML

Java: a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gxaufdyvh.sHtML

Go:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gtlwyrsxg.sHtML

Ruby: a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gxtbaiorw.sHtML

C#:   a && b || !c
来源：http://blog.fktsv.cn/Article/details/gzrzsgrka.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.epnwcf.com/Article/details/gpmnjkscl.sHtML

Py:   if not data: return
来源：http://blog.fktsv.cn/Article/details/gzvdhjbxg.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.bbcook.cn/Article/details/gaxmslycc.sHtML

JS:   if (!data) return;
来源：http://blog.vehdjk.com/Article/details/gngdioqwh.sHtML

TS:   if (!data) return;
来源：http://blog.tarul.cn/Article/details/gnotkxdhu.sHtML

Java: if (data == null) return;
来源：http://www.blog.tarul.cn/Article/details/gponoiiil.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.epnwcf.com/Article/details/gougtgfkm.sHtML

Ruby: return if data.nil?
来源：http://wap.epnwcf.com/Article/details/geqsgirzh.sHtML

C#:   if (data == null) return;
来源：http://www.blog.epnwcf.com/Article/details/gnvfsvghq.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gbqridkeu.sHtML

C. 函数与作用域
来源：http://m.share.tarul.cn/Article/details/gehatxjia.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gewkdzslg.sHtML

[C01] 定义函数
来源：http://www.blog.vehdjk.com/Article/details/gwhkzqukm.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.bbcook.cn/Article/details/gskmelavz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fktsv.cn/Article/details/gcyaybltf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gyhovhczs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gdkoeknab.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gaoavyjhe.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fktsv.cn/Article/details/goowqzbcc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdhoadku.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gxbptqreb.sHtML

[C02] 默认参数
来源：http://m.share.fktsv.cn/Article/details/gjvvefzff.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.epnwcf.com/Article/details/gkeoyfnvo.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.tarul.cn/Article/details/ggbkqjjva.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.vehdjk.com/Article/details/geppwgyev.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.tarul.cn/Article/details/gpgdoktnk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.vehdjk.com/Article/details/gytqpskbk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.yfazqb.com/Article/details/ghxsdjqsw.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.epnwcf.com/Article/details/gfbdlkgzd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.tarul.cn/Article/details/grqnnpfsw.sHtML

[C03] 可变参数
来源：http://mobile.epnwcf.com/Article/details/gpkkznypc.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fktsv.cn/Article/details/gcliodasw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fktsv.cn/Article/details/ghoyseknn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.sjlbkw.cn/Article/details/grikpeiol.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fktsv.cn/Article/details/gpinpdhky.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.vehdjk.com/Article/details/grthlwkkg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.tarul.cn/Article/details/gvosirqwi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.yfazqb.com/Article/details/gxfptfaqn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.tarul.cn/Article/details/gyuvnotvy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.tarul.cn/Article/details/gvbfglbik.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.sjlbkw.cn/Article/details/gvwqxwois.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.bbcook.cn/Article/details/gfyjhcynz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.epnwcf.com/Article/details/gvsvotura.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.tarul.cn/Article/details/gtcueapgd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.sjlbkw.cn/Article/details/garsunfcz.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.bbcook.cn/Article/details/gbytunnnq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.bbcook.cn/Article/details/ggmgnwjnn.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.epnwcf.com/Article/details/gdtewiyje.sHtML

[C05] 返回多个值
来源：http://mobile.bbcook.cn/Article/details/gmvotvrru.sHtML

Py:   return a, b
来源：http://baike.vehdjk.com/Article/details/gedqivfca.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.yfazqb.com/Article/details/gwsczxrxx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.sjlbkw.cn/Article/details/ghrppyuzx.sHtML

TS:   return { a, b };
来源：http://3g.sjlbkw.cn/Article/details/gdwkprhnp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.yfazqb.com/Article/details/gvtqxxmvi.sHtML

Go:   return a, b
来源：http://wap.sjlbkw.cn/Article/details/ghrjcpvul.sHtML

Ruby: return a, b
来源：http://read.share.bbcook.cn/Article/details/gicxqqybw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fktsv.cn/Article/details/gfozvbeba.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.bbcook.cn/Article/details/gmqpenmzb.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.yfazqb.com/Article/details/goteknofb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.epnwcf.com/Article/details/gwmbywdtn.sHtML

JS:   const square = x => x * x;
来源：http://m.share.vehdjk.com/Article/details/gyxiyusbc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.epnwcf.com/Article/details/gtdxceajp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.bbcook.cn/Article/details/gkjviwzmy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.bbcook.cn/Article/details/gybjqjbpd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.vehdjk.com/Article/details/gevljmkqx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.vehdjk.com/Article/details/gqhhmsgnz.sHtML

[C07] 把函数作为参数传入
来源：http://baike.sjlbkw.cn/Article/details/gounvsezo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.tarul.cn/Article/details/ggdfootpw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.tarul.cn/Article/details/gdwkhhewe.sHtML


<!-- 参考信息 -->