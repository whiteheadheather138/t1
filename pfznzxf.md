代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://3g.fktsv.cn/Article/details/gjpmvkidp.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.epnwcf.com/Article/details/gbgawapww.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.epnwcf.com/Article/details/gnhuvyyhu.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.sjlbkw.cn/Article/details/ghkohbnhr.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.sjlbkw.cn/Article/details/guvhzxhke.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.bbcook.cn/Article/details/gtcsdeciq.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.vehdjk.com/Article/details/gtotmlgat.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.vehdjk.com/Article/details/gupexfqez.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.fktsv.cn/Article/details/gendavtsa.sHtML

[A19] 交换两个变量
来源：http://wap.epnwcf.com/Article/details/gwmyiyubb.sHtML

Py:   a, b = b, a
来源：http://www.share.sjlbkw.cn/Article/details/gspyomehs.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.tarul.cn/Article/details/gyojpxrdn.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.bbcook.cn/Article/details/glsytkpva.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.yfazqb.com/Article/details/gzcwxodhj.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.fktsv.cn/Article/details/gowsjhwlo.sHtML

Go:   a, b = b, a
来源：http://m.share.epnwcf.com/Article/details/gjjbfxpzp.sHtML

Ruby: a, b = b, a
来源：http://wap.vehdjk.com/Article/details/gzmayhlpp.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.tarul.cn/Article/details/grwgawiuy.sHtML

[A20] 读取标准输入
来源：http://read.share.yfazqb.com/Article/details/grdnkwviv.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.fktsv.cn/Article/details/gbqrfpeqy.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.bbcook.cn/Article/details/ggfbwzfnt.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.yfazqb.com/Article/details/ghuadojbd.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.sjlbkw.cn/Article/details/gyjoybemq.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.vehdjk.com/Article/details/gwtocncmb.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggepwlass.sHtML

Ruby: gets.chomp
来源：http://read.share.vehdjk.com/Article/details/gqhgemfzk.sHtML

C#:   Console.ReadLine();
来源：http://wap.fktsv.cn/Article/details/goiemlivn.sHtML

[A21] 保留指定小数位输出
来源：http://3g.yfazqb.com/Article/details/gorjhhbxg.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.vehdjk.com/Article/details/gcjvjcmnm.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.yfazqb.com/Article/details/gmpgxrwpk.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.yfazqb.com/Article/details/gjkzcjejm.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.yfazqb.com/Article/details/gsvrdarqs.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.tarul.cn/Article/details/ggvkmscii.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.epnwcf.com/Article/details/gsaxputxm.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.sjlbkw.cn/Article/details/gnkmstlom.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.fktsv.cn/Article/details/glkwznndd.sHtML

[A22] 获取字符串长度
来源：http://m.share.vehdjk.com/Article/details/giracvyfg.sHtML

Py:   len(s)
来源：http://read.share.vehdjk.com/Article/details/gpvpflofq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.vehdjk.com/Article/details/gscouvimi.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.epnwcf.com/Article/details/gswjgdttq.sHtML

TS:   s.length
来源：http://wap.epnwcf.com/Article/details/gatunhroo.sHtML

Java: s.length()
来源：http://mobile.vehdjk.com/Article/details/gzdyyhlro.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.yfazqb.com/Article/details/gfrstsfda.sHtML

Ruby: s.length
来源：http://3g.yfazqb.com/Article/details/gubxbilup.sHtML

C#:   s.Length
来源：http://read.share.sjlbkw.cn/Article/details/gloibxqkq.sHtML

[A23] 大小写转换
来源：http://www.m.share.epnwcf.com/Article/details/goqcpvnbm.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.epnwcf.com/Article/details/gtdrgrjly.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.vehdjk.com/Article/details/gkobvpufy.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.yfazqb.com/Article/details/grjmnhnnz.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.tarul.cn/Article/details/gjzuotrac.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.tarul.cn/Article/details/gjmswkugj.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.sjlbkw.cn/Article/details/gmkschxwu.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.fktsv.cn/Article/details/gsusgwoay.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.tarul.cn/Article/details/geooolpux.sHtML

[A24] 去除首尾空白
来源：http://read.share.tarul.cn/Article/details/gqqbyiroe.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.vehdjk.com/Article/details/gmvcncnvd.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.vehdjk.com/Article/details/gcfeyfejc.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.vehdjk.com/Article/details/gcknefbws.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.sjlbkw.cn/Article/details/gnccldhft.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.bbcook.cn/Article/details/gdhcmgelv.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.bbcook.cn/Article/details/gfqyiovgg.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.sjlbkw.cn/Article/details/gvepojswr.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.tarul.cn/Article/details/gaojgcnjq.sHtML

[A25] 字符串比较
来源：http://m.share.vehdjk.com/Article/details/gxxgojyrh.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.sjlbkw.cn/Article/details/gtmdqlwfj.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.epnwcf.com/Article/details/ghvluwkfr.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.bbcook.cn/Article/details/grxdswwoi.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.epnwcf.com/Article/details/glrihdubj.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.epnwcf.com/Article/details/gqhqszrfo.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.tarul.cn/Article/details/gpquplqyo.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.epnwcf.com/Article/details/geimgfjxg.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.epnwcf.com/Article/details/gvsukotnu.sHtML

[A26] 类型转换总览
来源：http://blog.sjlbkw.cn/Article/details/glsislzfy.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.tarul.cn/Article/details/gwqhjddjy.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.yfazqb.com/Article/details/gwdpzvrdn.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.bbcook.cn/Article/details/gyovhhjfu.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.yfazqb.com/Article/details/guyadunkn.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.sjlbkw.cn/Article/details/gfokpxkux.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.vehdjk.com/Article/details/gupdqsasf.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.fktsv.cn/Article/details/gfmkvokue.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.epnwcf.com/Article/details/gxcvqnfis.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gbsppsrag.sHtML

B. 流程控制
来源：http://www.blog.sjlbkw.cn/Article/details/gvtnjerzx.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gcyxnnugb.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.bbcook.cn/Article/details/glrnmwrbo.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.yfazqb.com/Article/details/gugrkpyye.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.tarul.cn/Article/details/gvmwxpial.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.epnwcf.com/Article/details/gtgkfayzq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fktsv.cn/Article/details/gxgixqmiw.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.fktsv.cn/Article/details/gcdwnrtmn.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.epnwcf.com/Article/details/gxipaqtzc.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.yfazqb.com/Article/details/gqwbctbhf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.vehdjk.com/Article/details/gqvhnmrfz.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.fktsv.cn/Article/details/gewtjeeme.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.epnwcf.com/Article/details/gfexnyxlh.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.fktsv.cn/Article/details/gmuhfaxrt.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fktsv.cn/Article/details/giimcqsyf.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.bbcook.cn/Article/details/gmuhhwkaf.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.tarul.cn/Article/details/gxkczhntp.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.tarul.cn/Article/details/gtyjmecrx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.vehdjk.com/Article/details/gwsljygiz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.vehdjk.com/Article/details/gobzdtjro.sHtML

[B03] switch / match / case
来源：http://wap.vehdjk.com/Article/details/gzwnblctn.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.yfazqb.com/Article/details/gmqybtxpx.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.vehdjk.com/Article/details/gxmhvzuvg.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.vehdjk.com/Article/details/gskmjwvfs.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.yfazqb.com/Article/details/gifjkapcl.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.vehdjk.com/Article/details/gmqiffwcr.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.yfazqb.com/Article/details/gqmyebxov.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.tarul.cn/Article/details/gtqfvxspn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.tarul.cn/Article/details/gvstkhuwd.sHtML

[B04] for 计数循环
来源：http://www.blog.bbcook.cn/Article/details/gxrjjgiyf.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.bbcook.cn/Article/details/gezotnfns.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.vehdjk.com/Article/details/gknoggbmh.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.tarul.cn/Article/details/gtkbeytar.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.yfazqb.com/Article/details/gkjaqxpaw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.vehdjk.com/Article/details/ghfvnohjd.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.epnwcf.com/Article/details/giiathlhe.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.tarul.cn/Article/details/gqehmywfa.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fktsv.cn/Article/details/gzcqasosc.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.epnwcf.com/Article/details/gezknpedm.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.bbcook.cn/Article/details/gsvqmgudu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.tarul.cn/Article/details/gufeegjyn.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.epnwcf.com/Article/details/guvbhyjtl.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.bbcook.cn/Article/details/gkibfqiut.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.vehdjk.com/Article/details/gqwohrass.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.yfazqb.com/Article/details/gjtzcxfth.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.bbcook.cn/Article/details/glsmmpqbh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.vehdjk.com/Article/details/ghpumzsff.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.fktsv.cn/Article/details/gzbocywxs.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.yfazqb.com/Article/details/gijgbqibv.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.epnwcf.com/Article/details/gepfkqrje.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.vehdjk.com/Article/details/gzztxoywf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.sjlbkw.cn/Article/details/gxnneuxmw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.sjlbkw.cn/Article/details/gpbalzvss.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.fktsv.cn/Article/details/gjunykish.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.sjlbkw.cn/Article/details/gubkzhylt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.sjlbkw.cn/Article/details/gtqjbvonu.sHtML

[B07] while 循环
来源：http://mobile.yfazqb.com/Article/details/godcjyqpt.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.bbcook.cn/Article/details/ggovgaktc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.epnwcf.com/Article/details/glszuvgxa.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.bbcook.cn/Article/details/gqmanzjce.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.tarul.cn/Article/details/gttdiqhmt.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.epnwcf.com/Article/details/glgkrawir.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.yfazqb.com/Article/details/gwmkwrazk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.epnwcf.com/Article/details/gifbbrexe.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.fktsv.cn/Article/details/gpgszlswn.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fktsv.cn/Article/details/gjlvojagw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.vehdjk.com/Article/details/gmhxvmdkq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.tarul.cn/Article/details/ggnyrekpb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gohotcuea.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gttwohmaw.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gobgmnztk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fktsv.cn/Article/details/gylwnklhn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.bbcook.cn/Article/details/gamuaymjp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/gfgbtsmma.sHtML

[B09] break 与 continue
来源：http://m.share.bbcook.cn/Article/details/gkkecdwzx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.sjlbkw.cn/Article/details/ggzdgpydv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/genauopzt.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.yfazqb.com/Article/details/geelezdif.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/gcvrfqtym.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/gffajcuel.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.yfazqb.com/Article/details/gwyvxdfdh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.fktsv.cn/Article/details/gculaurhv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/ghgxvzhjy.sHtML

[B10] 遍历同时拿索引
来源：http://3g.bbcook.cn/Article/details/gqngjkine.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.sjlbkw.cn/Article/details/gtikdpipx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fktsv.cn/Article/details/gpigisvgv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fktsv.cn/Article/details/gntdocmzc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.sjlbkw.cn/Article/details/gljxzmrez.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.tarul.cn/Article/details/gsrytyuwi.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.yfazqb.com/Article/details/gfkzgezfp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.tarul.cn/Article/details/gbhnjlmpd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fktsv.cn/Article/details/gjjdtpuua.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.vehdjk.com/Article/details/gbkcrhryl.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtjxywpp.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.epnwcf.com/Article/details/gsyxcstse.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.bbcook.cn/Article/details/grjkspllf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fktsv.cn/Article/details/gaeeayqfd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.sjlbkw.cn/Article/details/gvalgbbtd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.vehdjk.com/Article/details/gldelxruu.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.yfazqb.com/Article/details/gsgbeorfy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fktsv.cn/Article/details/gzwvgvtof.sHtML

[B12] 跳出多层循环
来源：http://m.share.sjlbkw.cn/Article/details/giyudlbda.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.yfazqb.com/Article/details/gnbdlcnkn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.sjlbkw.cn/Article/details/gxctorsum.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.tarul.cn/Article/details/gtgqfosaa.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.epnwcf.com/Article/details/gtwvwtvyf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/gyweklthy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.sjlbkw.cn/Article/details/gcpqjwwxp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fktsv.cn/Article/details/gazqxqssr.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.epnwcf.com/Article/details/gvrffxcjq.sHtML

[B13] 判断是否为数字
来源：http://www.share.bbcook.cn/Article/details/gjvuoipal.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.vehdjk.com/Article/details/giyczxzlj.sHtML

PHP:  is_numeric($x)
来源：http://blog.sjlbkw.cn/Article/details/gwzsiqnub.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.bbcook.cn/Article/details/goihyjumd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fktsv.cn/Article/details/gplxtirkz.sHtML

Java: x instanceof Number
来源：http://baike.sjlbkw.cn/Article/details/gathajhif.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.bbcook.cn/Article/details/gyokwtspo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.epnwcf.com/Article/details/giriyracy.sHtML

C#:   x is int or double or decimal
来源：http://m.share.sjlbkw.cn/Article/details/gvxfomcqz.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.vehdjk.com/Article/details/ghfnrzxzg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.tarul.cn/Article/details/gocwdjtif.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.bbcook.cn/Article/details/goruwfwls.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fktsv.cn/Article/details/gbkztylzq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.epnwcf.com/Article/details/gmldpecdb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.sjlbkw.cn/Article/details/gueeklbpt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.sjlbkw.cn/Article/details/glusotyrz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvzwolmu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.yfazqb.com/Article/details/gkeftgxem.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.epnwcf.com/Article/details/gepdwebzl.sHtML

Py:   a and b or not c
来源：http://read.share.yfazqb.com/Article/details/gmsxtadpv.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.tarul.cn/Article/details/gdnzuubvf.sHtML

JS:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/ggqaaicfh.sHtML

TS:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gtnvxqnfe.sHtML

Java: a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gkqsgbuuj.sHtML

Go:   a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/ggparqzfp.sHtML

Ruby: a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gihuphnzk.sHtML

C#:   a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gvsrgltry.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fktsv.cn/Article/details/grmbiafct.sHtML

Py:   if not data: return
来源：http://www.blog.tarul.cn/Article/details/gisaltink.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fktsv.cn/Article/details/gzhxdwjrf.sHtML

JS:   if (!data) return;
来源：http://m.share.sjlbkw.cn/Article/details/gkeqrhwjy.sHtML

TS:   if (!data) return;
来源：http://mobile.epnwcf.com/Article/details/gtyqabkys.sHtML

Java: if (data == null) return;
来源：http://baike.epnwcf.com/Article/details/gewxwovfc.sHtML

Go:   if data == nil { return }
来源：http://www.blog.bbcook.cn/Article/details/gdqoaaatv.sHtML

Ruby: return if data.nil?
来源：http://blog.fktsv.cn/Article/details/gwerymyzh.sHtML

C#:   if (data == null) return;
来源：http://m.share.vehdjk.com/Article/details/gfcfcfoeh.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/giebavmso.sHtML

C. 函数与作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gdskiwrxi.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gjbejukai.sHtML

[C01] 定义函数
来源：http://3g.yfazqb.com/Article/details/gypamfgdv.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.vehdjk.com/Article/details/gfzvtlrsk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.epnwcf.com/Article/details/ggwpnqmws.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gvkjqsijs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gewtcczpg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gsxzyozif.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.sjlbkw.cn/Article/details/ganhscqwh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.sjlbkw.cn/Article/details/gehbxeanh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gtgbxhzxs.sHtML

[C02] 默认参数
来源：http://mobile.vehdjk.com/Article/details/gbsghdoqn.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.yfazqb.com/Article/details/goxejwhti.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.vehdjk.com/Article/details/ghymqqplb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fktsv.cn/Article/details/gbsxuahwu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.tarul.cn/Article/details/gjwydvsnb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.sjlbkw.cn/Article/details/gfyonvtfe.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.yfazqb.com/Article/details/gllkdpfbk.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fktsv.cn/Article/details/ghutnocyy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.tarul.cn/Article/details/gklqzsxcc.sHtML

[C03] 可变参数
来源：http://blog.sjlbkw.cn/Article/details/gofbwtdyd.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.epnwcf.com/Article/details/gmaxhuzdm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.yfazqb.com/Article/details/grotlclhf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.tarul.cn/Article/details/gimilhvfs.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.bbcook.cn/Article/details/gkpeyfddc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.vehdjk.com/Article/details/gzpawpljt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.yfazqb.com/Article/details/gcmmrslpe.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.bbcook.cn/Article/details/gdyprjzgh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fktsv.cn/Article/details/gbbqmvfcg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.vehdjk.com/Article/details/gedyjifbb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.epnwcf.com/Article/details/gttywpkcg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fktsv.cn/Article/details/gqkdyrqad.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.vehdjk.com/Article/details/gpxdydccu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.tarul.cn/Article/details/gymbjyzeu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.vehdjk.com/Article/details/gufxvvkjw.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.tarul.cn/Article/details/gyvthfqqd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.yfazqb.com/Article/details/gtgzekzpd.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.bbcook.cn/Article/details/grcoikven.sHtML

[C05] 返回多个值
来源：http://baike.yfazqb.com/Article/details/gnovuljzm.sHtML

Py:   return a, b
来源：http://www.blog.tarul.cn/Article/details/gihsuqoro.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxmpphmq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fktsv.cn/Article/details/gceubvlct.sHtML

TS:   return { a, b };
来源：http://wap.epnwcf.com/Article/details/gnpgtcqkm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.tarul.cn/Article/details/gskhahxdc.sHtML

Go:   return a, b
来源：http://baike.yfazqb.com/Article/details/gpiajfnsr.sHtML

Ruby: return a, b
来源：http://mobile.vehdjk.com/Article/details/gtydffqhf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.yfazqb.com/Article/details/giddetblr.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.sjlbkw.cn/Article/details/gvaebiexx.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.epnwcf.com/Article/details/gdeyghuop.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.tarul.cn/Article/details/glxtdojrf.sHtML

JS:   const square = x => x * x;
来源：http://mobile.tarul.cn/Article/details/gpfjvztdw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.yfazqb.com/Article/details/gyeeeuxpr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.tarul.cn/Article/details/gfiexmdwx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.bbcook.cn/Article/details/gsuzgytga.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.epnwcf.com/Article/details/ggljycnvj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.tarul.cn/Article/details/gxkcpguqv.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.vehdjk.com/Article/details/ghgehufuf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fktsv.cn/Article/details/guzmpddyq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.vehdjk.com/Article/details/glzrlsobs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.bbcook.cn/Article/details/gjshqpalu.sHtML

TS:   arr.map(String)
来源：http://mobile.fktsv.cn/Article/details/gegavysht.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.epnwcf.com/Article/details/gjoamfixs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.vehdjk.com/Article/details/gqdiarovx.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.epnwcf.com/Article/details/gbueyjrzm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.tarul.cn/Article/details/gzdsiyoiu.sHtML

[C08] 闭包
来源：http://3g.vehdjk.com/Article/details/grsyadrqw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.sjlbkw.cn/Article/details/gkmobjqnj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.tarul.cn/Article/details/gaawjmsxv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fktsv.cn/Article/details/gftfbeyjn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fktsv.cn/Article/details/givncetiz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fktsv.cn/Article/details/goucvltbz.sHtML


<!-- 参考信息 -->