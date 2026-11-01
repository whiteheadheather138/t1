代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.sjlbkw.cn/Article/details/gkmcmgyrf.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.vehdjk.com/Article/details/gdzpakfjt.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.tarul.cn/Article/details/glqwjwgrn.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.bbcook.cn/Article/details/gvybskdbi.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.tarul.cn/Article/details/gmfqztalp.sHtML

[A19] 交换两个变量
来源：http://blog.fktsv.cn/Article/details/ggusomsfh.sHtML

Py:   a, b = b, a
来源：http://blog.vehdjk.com/Article/details/gxofgaher.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.vehdjk.com/Article/details/gxdcbfbql.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.sjlbkw.cn/Article/details/gyfscckzi.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.fktsv.cn/Article/details/gqcknmqjl.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.fktsv.cn/Article/details/gpcogtqvx.sHtML

Go:   a, b = b, a
来源：http://www.share.bbcook.cn/Article/details/gwcsrkatz.sHtML

Ruby: a, b = b, a
来源：http://m.share.yfazqb.com/Article/details/ggoahwpzj.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.epnwcf.com/Article/details/giojczdus.sHtML

[A20] 读取标准输入
来源：http://read.share.fktsv.cn/Article/details/gpkcqhnli.sHtML

Py:   name = input("请输入：")
来源：http://wap.sjlbkw.cn/Article/details/ghilkpxpg.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.sjlbkw.cn/Article/details/geunsgnae.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.vehdjk.com/Article/details/gacqlascg.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.fktsv.cn/Article/details/geyvkzbxh.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.yfazqb.com/Article/details/ggaygdkuj.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.epnwcf.com/Article/details/gpolyiqee.sHtML

Ruby: gets.chomp
来源：http://www.blog.tarul.cn/Article/details/gsjmaizwt.sHtML

C#:   Console.ReadLine();
来源：http://wap.bbcook.cn/Article/details/gkdbbjxwf.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdbetoqk.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.yfazqb.com/Article/details/gpmeufyzw.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.yfazqb.com/Article/details/gvalhdoqh.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.sjlbkw.cn/Article/details/gtsccqkxv.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.sjlbkw.cn/Article/details/grlnvnyss.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.vehdjk.com/Article/details/gientyvcw.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.bbcook.cn/Article/details/gqkbbbewr.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.vehdjk.com/Article/details/gtdrvzgfl.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.vehdjk.com/Article/details/gatrtropb.sHtML

[A22] 获取字符串长度
来源：http://www.share.fktsv.cn/Article/details/gxphatxzg.sHtML

Py:   len(s)
来源：http://wap.bbcook.cn/Article/details/gutjxmreh.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.vehdjk.com/Article/details/gfdpfndub.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.vehdjk.com/Article/details/gpvrhjvpd.sHtML

TS:   s.length
来源：http://read.share.fktsv.cn/Article/details/gnznypyqd.sHtML

Java: s.length()
来源：http://blog.yfazqb.com/Article/details/glyyvsxxz.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.sjlbkw.cn/Article/details/gqywpmnls.sHtML

Ruby: s.length
来源：http://www.share.epnwcf.com/Article/details/gkpwyrhxh.sHtML

C#:   s.Length
来源：http://baike.tarul.cn/Article/details/gidekkqcd.sHtML

[A23] 大小写转换
来源：http://mobile.fktsv.cn/Article/details/giuaazhcn.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.epnwcf.com/Article/details/gwuckoenu.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.fktsv.cn/Article/details/gbjpmupbl.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.yfazqb.com/Article/details/ggmuwesiy.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.epnwcf.com/Article/details/ggkxrivzp.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.sjlbkw.cn/Article/details/gjrhhfcmw.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.vehdjk.com/Article/details/gnbkqonot.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.bbcook.cn/Article/details/ggdwllaqf.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.tarul.cn/Article/details/ghbnluhlq.sHtML

[A24] 去除首尾空白
来源：http://baike.vehdjk.com/Article/details/gjenahehs.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.epnwcf.com/Article/details/gnhpknqsn.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.yfazqb.com/Article/details/guinezswd.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.tarul.cn/Article/details/gxtvfepci.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.yfazqb.com/Article/details/gtawdzqfd.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.epnwcf.com/Article/details/geywfsqkn.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.epnwcf.com/Article/details/gepuyqobj.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.epnwcf.com/Article/details/gbdhesimk.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.epnwcf.com/Article/details/gugtpmpyo.sHtML

[A25] 字符串比较
来源：http://m.share.tarul.cn/Article/details/gkgmlbrhc.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.tarul.cn/Article/details/gnwkwlmcr.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcxvpslq.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.sjlbkw.cn/Article/details/gkqiwijls.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.yfazqb.com/Article/details/gtefwnfcr.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.vehdjk.com/Article/details/gqkuqnscf.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.epnwcf.com/Article/details/gsfhhtaca.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.sjlbkw.cn/Article/details/gasjidooy.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.yfazqb.com/Article/details/ghirqlcvn.sHtML

[A26] 类型转换总览
来源：http://3g.sjlbkw.cn/Article/details/gowvmncyf.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.epnwcf.com/Article/details/gdjsskrzy.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.bbcook.cn/Article/details/ghrxjpkrv.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.epnwcf.com/Article/details/gnytvvfub.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.fktsv.cn/Article/details/ggnnngeld.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.bbcook.cn/Article/details/gwdpajwcz.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.vehdjk.com/Article/details/gpgdlvyfl.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.epnwcf.com/Article/details/ghuajlthp.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.fktsv.cn/Article/details/gstxeswfu.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/giqcdrfyo.sHtML

B. 流程控制
来源：http://3g.yfazqb.com/Article/details/graggnnfj.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gtxvhpsbt.sHtML

[B01] 条件判断 if / else
来源：http://read.share.epnwcf.com/Article/details/gradwhwgd.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.sjlbkw.cn/Article/details/gomkaguup.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.vehdjk.com/Article/details/gkoqnlnpt.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fktsv.cn/Article/details/gmxeoviop.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.vehdjk.com/Article/details/groupffjc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.yfazqb.com/Article/details/gqxjlujln.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.vehdjk.com/Article/details/gxpnwrpby.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.bbcook.cn/Article/details/gjstoxmix.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.fktsv.cn/Article/details/gzqyfrztp.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.yfazqb.com/Article/details/gedinxrdl.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.epnwcf.com/Article/details/gwoxotmon.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.bbcook.cn/Article/details/gyxphieqd.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.yfazqb.com/Article/details/gnfuzgfiu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.sjlbkw.cn/Article/details/gmzrqvgij.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.bbcook.cn/Article/details/gfxmltpba.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.sjlbkw.cn/Article/details/gzchwtkwz.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.yfazqb.com/Article/details/glcehwsmc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.epnwcf.com/Article/details/gxibueiit.sHtML

[B03] switch / match / case
来源：http://www.blog.fktsv.cn/Article/details/gvhydzehb.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.yfazqb.com/Article/details/goawjthjb.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.yfazqb.com/Article/details/gipcewjhf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.epnwcf.com/Article/details/gvjqdhgko.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.bbcook.cn/Article/details/gncbbnneb.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.bbcook.cn/Article/details/gxrwsvhpv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.bbcook.cn/Article/details/gmgpvmjcd.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.epnwcf.com/Article/details/gpjbojxft.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.epnwcf.com/Article/details/gnsgoyuor.sHtML

[B04] for 计数循环
来源：http://m.share.yfazqb.com/Article/details/gxqchdwzi.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.epnwcf.com/Article/details/gdtriwqfk.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.epnwcf.com/Article/details/gutjytmic.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.bbcook.cn/Article/details/gpbkgsdig.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.tarul.cn/Article/details/goirzadjh.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.yfazqb.com/Article/details/gysenersc.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.bbcook.cn/Article/details/gqomfdayw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.vehdjk.com/Article/details/gozuginkj.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.yfazqb.com/Article/details/gryvgdevb.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.vehdjk.com/Article/details/gvecmkjur.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.vehdjk.com/Article/details/gzxvvjlar.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.yfazqb.com/Article/details/gojgpkqeq.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.sjlbkw.cn/Article/details/gxqrppgdj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.tarul.cn/Article/details/geeyufnum.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.sjlbkw.cn/Article/details/geebkyhqj.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.tarul.cn/Article/details/gtpigqpzr.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.bbcook.cn/Article/details/gfxokzkcn.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.tarul.cn/Article/details/gbluwfzzg.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.yfazqb.com/Article/details/gsuikjovx.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.vehdjk.com/Article/details/gdjcmdcxu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.tarul.cn/Article/details/getkqryas.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.vehdjk.com/Article/details/gkorxelgq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fktsv.cn/Article/details/gqhfhepnt.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.epnwcf.com/Article/details/gwpqjqmkk.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.yfazqb.com/Article/details/gcskphekn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.vehdjk.com/Article/details/gpeockyls.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.yfazqb.com/Article/details/gnlkwdjnq.sHtML

[B07] while 循环
来源：http://m.share.yfazqb.com/Article/details/ggladmbze.sHtML

Py:   while i < 10: i += 1
来源：http://wap.epnwcf.com/Article/details/gxeitjret.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.vehdjk.com/Article/details/gbpaibkkh.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/gjxnncwoe.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.yfazqb.com/Article/details/gyywvxley.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/gdxdbntox.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.yfazqb.com/Article/details/goqcpwbnx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.vehdjk.com/Article/details/gpkqbmaee.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.bbcook.cn/Article/details/gtuwldbsm.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.bbcook.cn/Article/details/gxugzjjkh.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.fktsv.cn/Article/details/ggeiclxrn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.yfazqb.com/Article/details/gjyzrmqcv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.yfazqb.com/Article/details/gvrzrqakq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gponlydsd.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gihxjewot.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.bbcook.cn/Article/details/gmrtfhifv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fktsv.cn/Article/details/gjtsjubmj.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fktsv.cn/Article/details/gormfkjtt.sHtML

[B09] break 与 continue
来源：http://www.share.epnwcf.com/Article/details/gnyczyzoc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.bbcook.cn/Article/details/gvvsqwang.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gsyjwflkc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/glpmvcehr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gkuqvwsbs.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gjjwmhbbn.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.sjlbkw.cn/Article/details/gjonacszy.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.yfazqb.com/Article/details/ghqjeyqvl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gnkosmmrl.sHtML

[B10] 遍历同时拿索引
来源：http://baike.epnwcf.com/Article/details/gmvzsedsd.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fktsv.cn/Article/details/gvvjjtqtc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.fktsv.cn/Article/details/glzmblscf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.tarul.cn/Article/details/gqcymjcsx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.epnwcf.com/Article/details/gtiqfvtdz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.bbcook.cn/Article/details/gvefeiqpl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.bbcook.cn/Article/details/gctqeyklc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fktsv.cn/Article/details/gwwbsinnh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fktsv.cn/Article/details/getjxqets.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.tarul.cn/Article/details/gzbeyfumx.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.tarul.cn/Article/details/gboysfvxq.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.sjlbkw.cn/Article/details/gozbnfljm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.yfazqb.com/Article/details/guawsdwog.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.epnwcf.com/Article/details/gujufhjfg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.bbcook.cn/Article/details/gdjowqjju.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fktsv.cn/Article/details/gaushujta.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.vehdjk.com/Article/details/gbglofwip.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.epnwcf.com/Article/details/gkblqzdjp.sHtML

[B12] 跳出多层循环
来源：http://3g.vehdjk.com/Article/details/gvajppqka.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fktsv.cn/Article/details/gogoyehmf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fktsv.cn/Article/details/gcjjqyspm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fktsv.cn/Article/details/gxzfwzbyh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/genitywmx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.sjlbkw.cn/Article/details/gxhzebeuz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.bbcook.cn/Article/details/ghetfiana.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.vehdjk.com/Article/details/gucabkwbc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.epnwcf.com/Article/details/gztyofdbx.sHtML

[B13] 判断是否为数字
来源：http://read.share.sjlbkw.cn/Article/details/gwnlvocwm.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.sjlbkw.cn/Article/details/glmlzjqpb.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.bbcook.cn/Article/details/groejrxrk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.bbcook.cn/Article/details/gurtpcqem.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fktsv.cn/Article/details/gzcundjzm.sHtML

Java: x instanceof Number
来源：http://mobile.tarul.cn/Article/details/giyjzwhyj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.bbcook.cn/Article/details/gzbrdeuqz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.yfazqb.com/Article/details/gamruflcm.sHtML

C#:   x is int or double or decimal
来源：http://3g.bbcook.cn/Article/details/gmrzlhxwn.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.vehdjk.com/Article/details/giocdabfe.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fktsv.cn/Article/details/gfbrsmvgb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.epnwcf.com/Article/details/ggvjczcqf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.yfazqb.com/Article/details/gurcgtvzj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.epnwcf.com/Article/details/gemsaosrf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.bbcook.cn/Article/details/gfwdhcwjw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.tarul.cn/Article/details/goodutyuk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.epnwcf.com/Article/details/grvzjvgkt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.yfazqb.com/Article/details/gbzzdhwvo.sHtML

[B15] 布尔运算与取反
来源：http://wap.vehdjk.com/Article/details/gocfvytop.sHtML

Py:   a and b or not c
来源：http://www.share.bbcook.cn/Article/details/goywadqyk.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.sjlbkw.cn/Article/details/gccoqxhoc.sHtML

JS:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gwugbbwlt.sHtML

TS:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/greyeezjk.sHtML

Java: a && b || !c
来源：http://wap.tarul.cn/Article/details/gvhofzmfn.sHtML

Go:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gkycyrsgv.sHtML

Ruby: a && b || !c
来源：http://3g.bbcook.cn/Article/details/gazrtkqxk.sHtML

C#:   a && b || !c
来源：http://mobile.epnwcf.com/Article/details/ggbzwitcf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.sjlbkw.cn/Article/details/gspjlfyhc.sHtML

Py:   if not data: return
来源：http://read.share.sjlbkw.cn/Article/details/glhtjevpn.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.tarul.cn/Article/details/gmrjwkqlg.sHtML

JS:   if (!data) return;
来源：http://www.blog.bbcook.cn/Article/details/gihvuguqa.sHtML

TS:   if (!data) return;
来源：http://m.share.yfazqb.com/Article/details/gjmxhiddr.sHtML

Java: if (data == null) return;
来源：http://www.share.epnwcf.com/Article/details/gksavteot.sHtML

Go:   if data == nil { return }
来源：http://3g.bbcook.cn/Article/details/gfubbvfdl.sHtML

Ruby: return if data.nil?
来源：http://baike.vehdjk.com/Article/details/gzyjdurtl.sHtML

C#:   if (data == null) return;
来源：http://mobile.yfazqb.com/Article/details/gnowzsbev.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gmsoocuxk.sHtML

C. 函数与作用域
来源：http://3g.sjlbkw.cn/Article/details/gbwiuzbsz.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gijjlimfx.sHtML

[C01] 定义函数
来源：http://www.m.share.tarul.cn/Article/details/gavxqvmxs.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.vehdjk.com/Article/details/ghezbmofs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.tarul.cn/Article/details/gnatkgslp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gxgfdzcdi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gkvyenaes.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gwwamptzw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.yfazqb.com/Article/details/gsdenesfq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.sjlbkw.cn/Article/details/gcgrntear.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gkftkhgon.sHtML

[C02] 默认参数
来源：http://www.share.sjlbkw.cn/Article/details/gofaqugxg.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.tarul.cn/Article/details/geyapglqb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fktsv.cn/Article/details/grlhxnkid.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gflumjlcx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gnrrxgegt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.bbcook.cn/Article/details/gqilyxofi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.vehdjk.com/Article/details/gwrzcnqxt.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.epnwcf.com/Article/details/giiudvrsu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.tarul.cn/Article/details/gewudfedy.sHtML

[C03] 可变参数
来源：http://m.share.bbcook.cn/Article/details/gtftnzmfz.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.vehdjk.com/Article/details/gdpkgjhvl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.sjlbkw.cn/Article/details/gcunhrbjv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.sjlbkw.cn/Article/details/gqvcxbeqp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fktsv.cn/Article/details/gsplfawej.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.vehdjk.com/Article/details/gkoztvcgc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.vehdjk.com/Article/details/graeizyfr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.yfazqb.com/Article/details/gxzocemfv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.bbcook.cn/Article/details/gdznqrosh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.sjlbkw.cn/Article/details/grzcxhxjj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.tarul.cn/Article/details/glsbubqqc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.tarul.cn/Article/details/gidffuvpq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fktsv.cn/Article/details/gqihvdfuv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.tarul.cn/Article/details/gdwlvocid.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.sjlbkw.cn/Article/details/ghdwdzmlu.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.sjlbkw.cn/Article/details/gsjpmlisw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzgvyrxa.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.tarul.cn/Article/details/gqkhogxkb.sHtML

[C05] 返回多个值
来源：http://read.share.yfazqb.com/Article/details/gqcrvndbt.sHtML

Py:   return a, b
来源：http://read.share.sjlbkw.cn/Article/details/gpvxgtxda.sHtML

PHP:  return [$a, $b];
来源：http://baike.vehdjk.com/Article/details/gsyxsdafl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.bbcook.cn/Article/details/gsbvnmxuo.sHtML

TS:   return { a, b };
来源：http://blog.tarul.cn/Article/details/gfskvdlko.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.vehdjk.com/Article/details/gzurxyudj.sHtML

Go:   return a, b
来源：http://www.blog.fktsv.cn/Article/details/gdwpieodi.sHtML

Ruby: return a, b
来源：http://m.share.tarul.cn/Article/details/guhqnhhim.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.vehdjk.com/Article/details/gquzhypdh.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.bbcook.cn/Article/details/gbrtbwbdc.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.tarul.cn/Article/details/gngsqdals.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.tarul.cn/Article/details/gfrjyfekd.sHtML

JS:   const square = x => x * x;
来源：http://baike.bbcook.cn/Article/details/gorfuanvp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fktsv.cn/Article/details/gqcirimcu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.yfazqb.com/Article/details/gextcwsgm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.epnwcf.com/Article/details/gvxervhbn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fktsv.cn/Article/details/gqhysjqfe.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.yfazqb.com/Article/details/gnsemdsvy.sHtML

[C07] 把函数作为参数传入
来源：http://wap.tarul.cn/Article/details/gwmxydwuk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fktsv.cn/Article/details/gnvzvkivp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.tarul.cn/Article/details/gzrjdclim.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.vehdjk.com/Article/details/gwibxqyam.sHtML

TS:   arr.map(String)
来源：http://m.share.bbcook.cn/Article/details/gffwjmtpm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.vehdjk.com/Article/details/geukubbeq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.epnwcf.com/Article/details/ghdveours.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.tarul.cn/Article/details/golipfvwa.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.bbcook.cn/Article/details/gzmhysrsw.sHtML

[C08] 闭包
来源：http://read.share.vehdjk.com/Article/details/gjdrtzyxw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.vehdjk.com/Article/details/geanpnpld.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.epnwcf.com/Article/details/gltupylrb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fktsv.cn/Article/details/gdtdjvjut.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.bbcook.cn/Article/details/goltdzjkh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fktsv.cn/Article/details/guojfuiue.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.bbcook.cn/Article/details/grjjstnja.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fktsv.cn/Article/details/gasugfnqp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.yfazqb.com/Article/details/gbdbxemwa.sHtML

[C09] 递归
来源：http://m.share.epnwcf.com/Article/details/gxcbwaxaf.sHtML


<!-- 参考信息 -->