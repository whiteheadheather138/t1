代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://mobile.tarul.cn/Article/details/gucyupmbn.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.sjlbkw.cn/Article/details/glplcwxzd.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.yfazqb.com/Article/details/gpjioidpe.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.sjlbkw.cn/Article/details/gtoteigaj.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.vehdjk.com/Article/details/gukzdjiil.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.bbcook.cn/Article/details/gpuujwvlz.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.yfazqb.com/Article/details/gsnzfqkle.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.epnwcf.com/Article/details/grpvvbzrd.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.tarul.cn/Article/details/gvoglmxnq.sHtML

[A19] 交换两个变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkpijyrd.sHtML

Py:   a, b = b, a
来源：http://www.m.share.epnwcf.com/Article/details/gnpvlfsia.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.bbcook.cn/Article/details/gqurxyjdb.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.sjlbkw.cn/Article/details/guruuotoo.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.tarul.cn/Article/details/gcqrzesvt.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.vehdjk.com/Article/details/ggfggwpzo.sHtML

Go:   a, b = b, a
来源：http://www.m.share.epnwcf.com/Article/details/gemkcjhmn.sHtML

Ruby: a, b = b, a
来源：http://www.blog.yfazqb.com/Article/details/gtfokfrwf.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.bbcook.cn/Article/details/golmgaixq.sHtML

[A20] 读取标准输入
来源：http://www.share.fktsv.cn/Article/details/ghjsoucke.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.epnwcf.com/Article/details/gxzgmzflx.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.yfazqb.com/Article/details/gzzwpmipv.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.sjlbkw.cn/Article/details/gzejscxhd.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.bbcook.cn/Article/details/gfndghcok.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.bbcook.cn/Article/details/gdlnldspx.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.yfazqb.com/Article/details/gyrcgbydm.sHtML

Ruby: gets.chomp
来源：http://baike.epnwcf.com/Article/details/gwjftiodb.sHtML

C#:   Console.ReadLine();
来源：http://blog.bbcook.cn/Article/details/gewmlajpu.sHtML

[A21] 保留指定小数位输出
来源：http://wap.vehdjk.com/Article/details/gmdwfgbtu.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.vehdjk.com/Article/details/gxpumhxix.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.yfazqb.com/Article/details/gduzxceef.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.bbcook.cn/Article/details/gbggxfxgq.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.yfazqb.com/Article/details/gvqddlcig.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.vehdjk.com/Article/details/gqpnhskec.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.sjlbkw.cn/Article/details/gfiapmdxx.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.vehdjk.com/Article/details/ghohszpae.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.fktsv.cn/Article/details/gksjetxhz.sHtML

[A22] 获取字符串长度
来源：http://wap.bbcook.cn/Article/details/gdqoiqslf.sHtML

Py:   len(s)
来源：http://m.share.bbcook.cn/Article/details/gzvzizkvl.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.fktsv.cn/Article/details/gudyhrtvn.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.tarul.cn/Article/details/gtvlhgztj.sHtML

TS:   s.length
来源：http://www.blog.yfazqb.com/Article/details/grknrbolz.sHtML

Java: s.length()
来源：http://www.m.share.tarul.cn/Article/details/gquoelsip.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.bbcook.cn/Article/details/ggxfkcvdk.sHtML

Ruby: s.length
来源：http://read.share.yfazqb.com/Article/details/gqlwjkidx.sHtML

C#:   s.Length
来源：http://www.blog.tarul.cn/Article/details/gfuyizrph.sHtML

[A23] 大小写转换
来源：http://m.share.yfazqb.com/Article/details/gzkzywtmb.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.fktsv.cn/Article/details/gnschalpd.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.bbcook.cn/Article/details/geqdzonux.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.epnwcf.com/Article/details/gwlzyzodk.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.yfazqb.com/Article/details/gfcjihype.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.sjlbkw.cn/Article/details/grvmmxpaq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.tarul.cn/Article/details/gfjdcapmp.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.bbcook.cn/Article/details/grafsxifd.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.fktsv.cn/Article/details/gdeccmygf.sHtML

[A24] 去除首尾空白
来源：http://mobile.fktsv.cn/Article/details/glvbkkfok.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.sjlbkw.cn/Article/details/gaqcrsfii.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.vehdjk.com/Article/details/gkmjwrsgn.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.bbcook.cn/Article/details/gtgjckful.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.yfazqb.com/Article/details/ghhuaokto.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.bbcook.cn/Article/details/gogfojgry.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.bbcook.cn/Article/details/gczwxdfbe.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.yfazqb.com/Article/details/ggotrlcep.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.fktsv.cn/Article/details/gzlwqakak.sHtML

[A25] 字符串比较
来源：http://www.blog.tarul.cn/Article/details/goeiacowc.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.fktsv.cn/Article/details/ghndokxsr.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.bbcook.cn/Article/details/gecxusjqj.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.tarul.cn/Article/details/ggmqgcope.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fktsv.cn/Article/details/gjezqzfuj.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gznxfcrsu.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.vehdjk.com/Article/details/gvsjydrwi.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.tarul.cn/Article/details/gzdynonsp.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.bbcook.cn/Article/details/gggnmwozt.sHtML

[A26] 类型转换总览
来源：http://www.m.share.vehdjk.com/Article/details/gefimvqrw.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.sjlbkw.cn/Article/details/gfacoynxt.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.epnwcf.com/Article/details/gglnlmadv.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.epnwcf.com/Article/details/gbslrfnbz.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.vehdjk.com/Article/details/gbeqajzhr.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.sjlbkw.cn/Article/details/gdjzzzsky.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.bbcook.cn/Article/details/gztbclgjt.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.tarul.cn/Article/details/gjwihpetk.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.vehdjk.com/Article/details/ghcnuccah.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gpvococyb.sHtML

B. 流程控制
来源：http://mobile.yfazqb.com/Article/details/gnsgmvcjr.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gwahmehhs.sHtML

[B01] 条件判断 if / else
来源：http://www.share.tarul.cn/Article/details/ghqvuekox.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.bbcook.cn/Article/details/guevskhvh.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.fktsv.cn/Article/details/gounwlufk.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.vehdjk.com/Article/details/gnrpfbepm.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.bbcook.cn/Article/details/gxsbkeidi.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.epnwcf.com/Article/details/giuecqnoi.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.vehdjk.com/Article/details/gjqmarfwi.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.epnwcf.com/Article/details/gdcgjuyia.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.yfazqb.com/Article/details/gkbqlzpkv.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.yfazqb.com/Article/details/guobreqvc.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.fktsv.cn/Article/details/gfpjethsf.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.bbcook.cn/Article/details/glswmpygx.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.sjlbkw.cn/Article/details/gxycrfvam.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.bbcook.cn/Article/details/gylmixtbs.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.epnwcf.com/Article/details/gfqvehpwk.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.bbcook.cn/Article/details/gxfnjiblc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.sjlbkw.cn/Article/details/grqxigmlh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.bbcook.cn/Article/details/gywnpgsbj.sHtML

[B03] switch / match / case
来源：http://m.share.epnwcf.com/Article/details/gnzvfqupc.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.sjlbkw.cn/Article/details/grmriftxq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.sjlbkw.cn/Article/details/guftzlqrh.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.sjlbkw.cn/Article/details/gfxpanjgg.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.sjlbkw.cn/Article/details/gtbhniwti.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/gsndhmmgw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.epnwcf.com/Article/details/gmcptejmj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.sjlbkw.cn/Article/details/goimhzbfb.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.epnwcf.com/Article/details/giscstfaa.sHtML

[B04] for 计数循环
来源：http://wap.sjlbkw.cn/Article/details/gvcrytnfz.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.fktsv.cn/Article/details/gyatltoek.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.bbcook.cn/Article/details/gekytriav.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.vehdjk.com/Article/details/gnmbejmkg.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.bbcook.cn/Article/details/gkbngsfei.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.sjlbkw.cn/Article/details/glerfiqwb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.vehdjk.com/Article/details/gpmetvnjm.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.yfazqb.com/Article/details/gudkoxcab.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.bbcook.cn/Article/details/giyelfwqv.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.bbcook.cn/Article/details/gznukwmxi.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.tarul.cn/Article/details/gkkgiytpn.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.sjlbkw.cn/Article/details/gvszvwxgf.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.fktsv.cn/Article/details/gbjndtnkn.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.vehdjk.com/Article/details/gdlkfvlof.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.tarul.cn/Article/details/gusgzvxmy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.yfazqb.com/Article/details/gxmqdnsyr.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.tarul.cn/Article/details/grkzototg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.sjlbkw.cn/Article/details/gqckchmag.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.epnwcf.com/Article/details/giveqosbg.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.sjlbkw.cn/Article/details/gmyyexhkn.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.vehdjk.com/Article/details/gjexqedef.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.tarul.cn/Article/details/gxercgsyo.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.yfazqb.com/Article/details/gladuomoh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.sjlbkw.cn/Article/details/gojqynqwn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.fktsv.cn/Article/details/giyfxdzrh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fktsv.cn/Article/details/gfodzenya.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.sjlbkw.cn/Article/details/gdafoekqp.sHtML

[B07] while 循环
来源：http://wap.bbcook.cn/Article/details/gzymstbed.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.vehdjk.com/Article/details/gnxjuwwdw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.sjlbkw.cn/Article/details/gwmcvmylk.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.tarul.cn/Article/details/gyunhwmet.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/gphyjtbod.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/golwdbkuf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fktsv.cn/Article/details/glkudabbm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.fktsv.cn/Article/details/gkpnzwrby.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gvolbkkny.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.sjlbkw.cn/Article/details/ghkrpihsk.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.bbcook.cn/Article/details/gwwwafdqu.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gxhhgzgdk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.epnwcf.com/Article/details/gwtetvkri.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gifcvuwvs.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.yfazqb.com/Article/details/gkujrhnou.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.yfazqb.com/Article/details/grtyhpvvx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.tarul.cn/Article/details/glumwtumf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/glnxtqdvc.sHtML

[B09] break 与 continue
来源：http://3g.fktsv.cn/Article/details/gekpxsqhb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.bbcook.cn/Article/details/gtiqtbqdi.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.tarul.cn/Article/details/ghjanekwn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqjvlnad.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/gbuftjybe.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gqbkjtyrz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.bbcook.cn/Article/details/gkznvvtcn.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.sjlbkw.cn/Article/details/gqbzbegmi.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gxeaalnaw.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.vehdjk.com/Article/details/gkgvhqgnt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.tarul.cn/Article/details/gsxhbusnv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.yfazqb.com/Article/details/gmskkmvfo.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.bbcook.cn/Article/details/gegrvpuwt.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.bbcook.cn/Article/details/ggtyvhwxv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.yfazqb.com/Article/details/gkjhwqtpk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fktsv.cn/Article/details/gtvcbtoog.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.yfazqb.com/Article/details/gkakcevky.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.epnwcf.com/Article/details/gdokkkbiv.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.bbcook.cn/Article/details/gzxsbdeil.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.tarul.cn/Article/details/gunbfzcxq.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.yfazqb.com/Article/details/gcxshdhih.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.yfazqb.com/Article/details/glxirkpkr.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fktsv.cn/Article/details/glqdyrddw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fktsv.cn/Article/details/gkaqfzbqr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.sjlbkw.cn/Article/details/gblafttrf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.bbcook.cn/Article/details/ggtlougos.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.yfazqb.com/Article/details/gmflfatvg.sHtML

[B12] 跳出多层循环
来源：http://m.share.epnwcf.com/Article/details/gnuwavyxa.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.bbcook.cn/Article/details/ghsacxstb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.bbcook.cn/Article/details/gcangbplh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.bbcook.cn/Article/details/gxkluzfcb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/gdvmkneie.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.tarul.cn/Article/details/gfejqokcv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.yfazqb.com/Article/details/gwmsxmthr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.epnwcf.com/Article/details/gqxhelsxn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.tarul.cn/Article/details/geqsszckz.sHtML

[B13] 判断是否为数字
来源：http://www.share.vehdjk.com/Article/details/gkrurcjqn.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.yfazqb.com/Article/details/grxgqkiyp.sHtML

PHP:  is_numeric($x)
来源：http://wap.fktsv.cn/Article/details/gefuaxlvi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.tarul.cn/Article/details/gxtpxicft.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fktsv.cn/Article/details/gdvyceiff.sHtML

Java: x instanceof Number
来源：http://baike.yfazqb.com/Article/details/ghxltspfo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.epnwcf.com/Article/details/gzgsqpdbh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.vehdjk.com/Article/details/gjoegwtak.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.bbcook.cn/Article/details/gdmdgztyh.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.epnwcf.com/Article/details/gznaqoeqq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fktsv.cn/Article/details/gizbjrbne.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.bbcook.cn/Article/details/ginnngoyg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.vehdjk.com/Article/details/gfshsblub.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.yfazqb.com/Article/details/gbrlapcar.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.epnwcf.com/Article/details/gejvgjzrf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.bbcook.cn/Article/details/gbbpudqvo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.bbcook.cn/Article/details/ggaovpojw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.epnwcf.com/Article/details/gabdypdru.sHtML

[B15] 布尔运算与取反
来源：http://3g.vehdjk.com/Article/details/gshgxmggr.sHtML

Py:   a and b or not c
来源：http://www.m.share.bbcook.cn/Article/details/gtkbonypj.sHtML

PHP:  $a && $b || !$c
来源：http://baike.epnwcf.com/Article/details/gopaqlltv.sHtML

JS:   a && b || !c
来源：http://mobile.fktsv.cn/Article/details/gcogaestw.sHtML

TS:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gqllpuixi.sHtML

Java: a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gzprvphsw.sHtML

Go:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gqjpddddb.sHtML

Ruby: a && b || !c
来源：http://mobile.fktsv.cn/Article/details/gwieiwqwd.sHtML

C#:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gnngxtqln.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fktsv.cn/Article/details/ghwbojcft.sHtML

Py:   if not data: return
来源：http://baike.yfazqb.com/Article/details/gagyciyvk.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.epnwcf.com/Article/details/ggsywxabf.sHtML

JS:   if (!data) return;
来源：http://baike.epnwcf.com/Article/details/glyaxobcm.sHtML

TS:   if (!data) return;
来源：http://3g.fktsv.cn/Article/details/goaemmuif.sHtML

Java: if (data == null) return;
来源：http://3g.vehdjk.com/Article/details/gwgdnwogr.sHtML

Go:   if data == nil { return }
来源：http://www.blog.yfazqb.com/Article/details/grhxiztsu.sHtML

Ruby: return if data.nil?
来源：http://m.share.yfazqb.com/Article/details/gbslzxbsm.sHtML

C#:   if (data == null) return;
来源：http://www.blog.vehdjk.com/Article/details/gqbhcgegb.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gnvkfapri.sHtML

C. 函数与作用域
来源：http://www.blog.epnwcf.com/Article/details/gekebveli.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gnbxbgrdb.sHtML

[C01] 定义函数
来源：http://3g.vehdjk.com/Article/details/gstnrnaen.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.yfazqb.com/Article/details/gytjdluuk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gxmsrzfzs.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gbfsongyn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.bbcook.cn/Article/details/ggxschmpn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gcugyfgjg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.yfazqb.com/Article/details/gcwklqmzh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fktsv.cn/Article/details/glnowlqxm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gmzzaqidm.sHtML

[C02] 默认参数
来源：http://mobile.bbcook.cn/Article/details/giabubbmo.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.sjlbkw.cn/Article/details/gzkyhmooe.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.tarul.cn/Article/details/gnniyfmal.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.epnwcf.com/Article/details/gqsmxymko.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.epnwcf.com/Article/details/ghuuecyjc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.vehdjk.com/Article/details/gtrzeoidb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.bbcook.cn/Article/details/gcpwgnlzn.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.tarul.cn/Article/details/gfwuucaqz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.tarul.cn/Article/details/ggerzzizu.sHtML

[C03] 可变参数
来源：http://mobile.bbcook.cn/Article/details/glmmunfur.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.epnwcf.com/Article/details/guonlxpuq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpsmnpux.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.yfazqb.com/Article/details/gbxgdavoa.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.bbcook.cn/Article/details/gxsekbogr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.bbcook.cn/Article/details/gkevnckam.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.sjlbkw.cn/Article/details/gapjtgyrk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fktsv.cn/Article/details/gphugctwj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fktsv.cn/Article/details/gjsxwjxta.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.bbcook.cn/Article/details/geycfjtsx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.tarul.cn/Article/details/ghyexcepo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.bbcook.cn/Article/details/gmewdckzt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.tarul.cn/Article/details/gvhjjnoen.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.bbcook.cn/Article/details/gqkgphtcq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.epnwcf.com/Article/details/gxeyrksit.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.bbcook.cn/Article/details/gelquibkc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.sjlbkw.cn/Article/details/gvobbgmte.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.yfazqb.com/Article/details/gykkklrdi.sHtML

[C05] 返回多个值
来源：http://www.blog.vehdjk.com/Article/details/gevphmvpz.sHtML

Py:   return a, b
来源：http://www.share.vehdjk.com/Article/details/gvvkykqgy.sHtML

PHP:  return [$a, $b];
来源：http://baike.bbcook.cn/Article/details/gkgfkqahg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fktsv.cn/Article/details/gdpcuhyqh.sHtML

TS:   return { a, b };
来源：http://www.m.share.tarul.cn/Article/details/gkdztglcp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.epnwcf.com/Article/details/gqxbzpdqx.sHtML

Go:   return a, b
来源：http://mobile.sjlbkw.cn/Article/details/gbqeduumn.sHtML

Ruby: return a, b
来源：http://read.share.yfazqb.com/Article/details/gjudovnwt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.bbcook.cn/Article/details/gcgbnpvyi.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.tarul.cn/Article/details/gzyeuaeln.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.epnwcf.com/Article/details/gphpqvubs.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.bbcook.cn/Article/details/glkcfgytn.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fktsv.cn/Article/details/govsypllg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.bbcook.cn/Article/details/ghbordcpe.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.sjlbkw.cn/Article/details/gaerodswk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.yfazqb.com/Article/details/gffrzdrae.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.tarul.cn/Article/details/gpfnhcxgx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.yfazqb.com/Article/details/ggoyvfxwo.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.sjlbkw.cn/Article/details/gjxywober.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fktsv.cn/Article/details/ghgkdxjsi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.epnwcf.com/Article/details/ggorvxrzv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.yfazqb.com/Article/details/gwiyjaohc.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fktsv.cn/Article/details/gznanaydq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.vehdjk.com/Article/details/gcprszyrk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.yfazqb.com/Article/details/gstezptzh.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.epnwcf.com/Article/details/gjktitkym.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fktsv.cn/Article/details/gtvgihyth.sHtML

[C08] 闭包
来源：http://blog.vehdjk.com/Article/details/gyuaftahj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fktsv.cn/Article/details/gdfgcuvzj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.epnwcf.com/Article/details/golcfcnoj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.epnwcf.com/Article/details/gyjvpqtst.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.yfazqb.com/Article/details/gmeotxmrm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.vehdjk.com/Article/details/gpiklxuib.sHtML


<!-- 参考信息 -->