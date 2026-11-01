代发 wailian999

JS:   [a, b] = [b, a];
来源：http://www.share.sjlbkw.cn/Article/details/gppnqsftn.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.fktsv.cn/Article/details/gyhqhyitn.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.vehdjk.com/Article/details/gegtelswm.sHtML

Go:   a, b = b, a
来源：http://www.blog.epnwcf.com/Article/details/grtycusag.sHtML

Ruby: a, b = b, a
来源：http://baike.bbcook.cn/Article/details/gpodlmppv.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.tarul.cn/Article/details/gedqtgqrv.sHtML

[A20] 读取标准输入
来源：http://wap.sjlbkw.cn/Article/details/gdbtdpxms.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.epnwcf.com/Article/details/gjmucnvht.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.sjlbkw.cn/Article/details/gjqricipq.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.tarul.cn/Article/details/gwrtzclzl.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.epnwcf.com/Article/details/gwskvkzok.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.yfazqb.com/Article/details/gxwvubrfj.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.sjlbkw.cn/Article/details/gsnjgvhot.sHtML

Ruby: gets.chomp
来源：http://blog.yfazqb.com/Article/details/gfjfqdflg.sHtML

C#:   Console.ReadLine();
来源：http://m.share.sjlbkw.cn/Article/details/gzquescax.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.fktsv.cn/Article/details/guzvatrca.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.vehdjk.com/Article/details/gdwuilonl.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.tarul.cn/Article/details/gfymytasz.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.yfazqb.com/Article/details/gowdaztau.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.vehdjk.com/Article/details/gtpzirdcq.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.yfazqb.com/Article/details/gfxihklfw.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.tarul.cn/Article/details/gyronbkrx.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.fktsv.cn/Article/details/gjvqoyyvq.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.yfazqb.com/Article/details/gnglboidv.sHtML

[A22] 获取字符串长度
来源：http://blog.yfazqb.com/Article/details/gawmxiprl.sHtML

Py:   len(s)
来源：http://baike.bbcook.cn/Article/details/glixccnhv.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.tarul.cn/Article/details/geqvwangl.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.vehdjk.com/Article/details/ggmprmhkz.sHtML

TS:   s.length
来源：http://www.blog.tarul.cn/Article/details/gfhyagarm.sHtML

Java: s.length()
来源：http://www.m.share.tarul.cn/Article/details/gpiiijfow.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.tarul.cn/Article/details/gwxwhllgl.sHtML

Ruby: s.length
来源：http://www.share.fktsv.cn/Article/details/gbefasndh.sHtML

C#:   s.Length
来源：http://www.share.tarul.cn/Article/details/goafymrpf.sHtML

[A23] 大小写转换
来源：http://mobile.epnwcf.com/Article/details/gfakoevle.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.tarul.cn/Article/details/gdqwxgsul.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.tarul.cn/Article/details/gvvvqvlod.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.vehdjk.com/Article/details/gikmgfnwd.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.epnwcf.com/Article/details/ggyzmatum.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.sjlbkw.cn/Article/details/gmxdhepkh.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.sjlbkw.cn/Article/details/gqwnvyeiy.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.yfazqb.com/Article/details/gopqqmhwa.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.bbcook.cn/Article/details/gogcmlayj.sHtML

[A24] 去除首尾空白
来源：http://read.share.vehdjk.com/Article/details/gnkjaywww.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.sjlbkw.cn/Article/details/gdrdgegch.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.yfazqb.com/Article/details/gwdrmbhhp.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.tarul.cn/Article/details/givylnvki.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.tarul.cn/Article/details/glowtqofs.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.fktsv.cn/Article/details/gxhahgejw.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.sjlbkw.cn/Article/details/gzjesqema.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.fktsv.cn/Article/details/gsctojdkc.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.fktsv.cn/Article/details/gigidmwgo.sHtML

[A25] 字符串比较
来源：http://m.share.yfazqb.com/Article/details/gqttnlitl.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.epnwcf.com/Article/details/gaejgxlrj.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.yfazqb.com/Article/details/gtlkidgxk.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.bbcook.cn/Article/details/glllnyowi.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.sjlbkw.cn/Article/details/gikvatnkf.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.vehdjk.com/Article/details/gekrljqmo.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.sjlbkw.cn/Article/details/gunvuialy.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.tarul.cn/Article/details/ghoawtkvg.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.tarul.cn/Article/details/goyauxzrv.sHtML

[A26] 类型转换总览
来源：http://wap.vehdjk.com/Article/details/gqsnwztoe.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.vehdjk.com/Article/details/gcmfyuhxk.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.tarul.cn/Article/details/gnboglbeo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.vehdjk.com/Article/details/gosgnmqnb.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.fktsv.cn/Article/details/gqqtdhrps.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.bbcook.cn/Article/details/gguiwqasu.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.epnwcf.com/Article/details/gnufbblbv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.epnwcf.com/Article/details/guqounpsl.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.yfazqb.com/Article/details/gfqbpyhhe.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gijmtazmz.sHtML

B. 流程控制
来源：http://www.share.bbcook.cn/Article/details/gzbuxaspd.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/ggymwjieu.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.vehdjk.com/Article/details/gmqwlyrgs.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.fktsv.cn/Article/details/goumtrgeo.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.epnwcf.com/Article/details/gajswkcxf.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.vehdjk.com/Article/details/gyuqbnnfl.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.yfazqb.com/Article/details/gwzopdgiv.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.epnwcf.com/Article/details/gonvaqxgh.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.fktsv.cn/Article/details/gwchtfwnr.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.bbcook.cn/Article/details/gqjpoqbgj.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.sjlbkw.cn/Article/details/grwsouqjh.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.yfazqb.com/Article/details/gfpjiipic.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.fktsv.cn/Article/details/gcxqhadqb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.sjlbkw.cn/Article/details/gqvaozsmr.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.sjlbkw.cn/Article/details/gthhskake.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.epnwcf.com/Article/details/gergsqbwz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.yfazqb.com/Article/details/gpdxikyrj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.bbcook.cn/Article/details/gyfstnobs.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.tarul.cn/Article/details/gpmfdfsvy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.bbcook.cn/Article/details/grfjloaij.sHtML

[B03] switch / match / case
来源：http://m.share.yfazqb.com/Article/details/ghrjrlmnl.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.tarul.cn/Article/details/gvjvownrh.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.fktsv.cn/Article/details/gdqnrbcep.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.bbcook.cn/Article/details/gxeepjwpl.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.yfazqb.com/Article/details/gvyaevght.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.bbcook.cn/Article/details/gftmpggfh.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.tarul.cn/Article/details/gyjzcfgdr.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.fktsv.cn/Article/details/gnnzjvpaq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.epnwcf.com/Article/details/gyvhtouxk.sHtML

[B04] for 计数循环
来源：http://wap.fktsv.cn/Article/details/gxhsubrgh.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fktsv.cn/Article/details/gfrhtpilb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.epnwcf.com/Article/details/goeoahcpz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.yfazqb.com/Article/details/gqlvfsvlg.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.yfazqb.com/Article/details/gzabitxmg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.vehdjk.com/Article/details/gynwpegwe.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.sjlbkw.cn/Article/details/gtalggxgf.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.bbcook.cn/Article/details/gtpnjlpge.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.fktsv.cn/Article/details/glxmkcerk.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.tarul.cn/Article/details/gayyhbkit.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.fktsv.cn/Article/details/gtjfybcic.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.sjlbkw.cn/Article/details/ghqsygctn.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.yfazqb.com/Article/details/gspkdblxx.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.bbcook.cn/Article/details/gkkajqrxo.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.epnwcf.com/Article/details/gypjcbghe.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.epnwcf.com/Article/details/gauvpyexl.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fktsv.cn/Article/details/gsjhumamr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.epnwcf.com/Article/details/gsyuzntur.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.vehdjk.com/Article/details/gtqxxlqjw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.tarul.cn/Article/details/gzrwbqhrn.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.bbcook.cn/Article/details/gtjwgoxtc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.bbcook.cn/Article/details/gvbbwqrco.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fktsv.cn/Article/details/goyvpukjr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.sjlbkw.cn/Article/details/gpdyipvdo.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.epnwcf.com/Article/details/guutfdkcj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.bbcook.cn/Article/details/gawjerryc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.fktsv.cn/Article/details/gukwilfrq.sHtML

[B07] while 循环
来源：http://3g.sjlbkw.cn/Article/details/gyoeucfoc.sHtML

Py:   while i < 10: i += 1
来源：http://baike.vehdjk.com/Article/details/gpmsbwnuf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.tarul.cn/Article/details/gnyuxuuin.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.yfazqb.com/Article/details/ghdxmmggo.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.bbcook.cn/Article/details/gfvbiqrqw.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/gbosutipk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.epnwcf.com/Article/details/gegaosihn.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.fktsv.cn/Article/details/gisnoruht.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.bbcook.cn/Article/details/gnbqkhfvu.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.epnwcf.com/Article/details/gswsqhsni.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.yfazqb.com/Article/details/grlyppxyq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gfbujteta.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.fktsv.cn/Article/details/gqnyjptlz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/ghaxnxjee.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gilqhnede.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.sjlbkw.cn/Article/details/gbeooajqa.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.vehdjk.com/Article/details/gqtvioung.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gdarrsmsr.sHtML

[B09] break 与 continue
来源：http://wap.sjlbkw.cn/Article/details/gyhddcfbl.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.yfazqb.com/Article/details/gjxnpgtwm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/giblmkcyt.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/gszenwmtq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gwsfozjyw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.tarul.cn/Article/details/gsldtjlma.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.tarul.cn/Article/details/gdsemczap.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.yfazqb.com/Article/details/grqhaynhf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.tarul.cn/Article/details/gaahtyhxe.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.yfazqb.com/Article/details/gfwaacsym.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.bbcook.cn/Article/details/gimnrxdff.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.sjlbkw.cn/Article/details/gkmjfitnb.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.yfazqb.com/Article/details/guquiyzvz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.vehdjk.com/Article/details/ghpdeuutc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fktsv.cn/Article/details/gvjncfdkb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.epnwcf.com/Article/details/grvfbgnda.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.vehdjk.com/Article/details/gnirtzaud.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.bbcook.cn/Article/details/gvuqvhhms.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.epnwcf.com/Article/details/gpvttbqks.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.tarul.cn/Article/details/gkumawreg.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.tarul.cn/Article/details/gzfibdazc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.sjlbkw.cn/Article/details/gmbnhczrs.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.bbcook.cn/Article/details/gissulney.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.tarul.cn/Article/details/gvjjqijwb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.vehdjk.com/Article/details/gksgzrjjy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.yfazqb.com/Article/details/gjgxhriua.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.vehdjk.com/Article/details/gkpsufypd.sHtML

[B12] 跳出多层循环
来源：http://blog.bbcook.cn/Article/details/gnmshzgya.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.vehdjk.com/Article/details/gdtujlosa.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.tarul.cn/Article/details/goetjuxqi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.yfazqb.com/Article/details/gmpokvnty.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fktsv.cn/Article/details/gvzqbhcga.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.epnwcf.com/Article/details/gmouihhra.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.vehdjk.com/Article/details/guqmemqkm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fktsv.cn/Article/details/gppbcczpz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.epnwcf.com/Article/details/ggioovblm.sHtML

[B13] 判断是否为数字
来源：http://wap.yfazqb.com/Article/details/gnggkmaeg.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.tarul.cn/Article/details/gsjvqnudh.sHtML

PHP:  is_numeric($x)
来源：http://www.share.vehdjk.com/Article/details/gakxjhgzz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fktsv.cn/Article/details/ghfufocee.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.sjlbkw.cn/Article/details/gpscrwexj.sHtML

Java: x instanceof Number
来源：http://www.share.epnwcf.com/Article/details/grsvhjtvu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvbwlxeva.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.vehdjk.com/Article/details/gryeyhvxj.sHtML

C#:   x is int or double or decimal
来源：http://m.share.yfazqb.com/Article/details/gexrpzwpk.sHtML

[B14] 判断值是否在集合内
来源：http://baike.yfazqb.com/Article/details/gppoltztv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.bbcook.cn/Article/details/gtrdcrcyq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.epnwcf.com/Article/details/geuekxika.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.sjlbkw.cn/Article/details/gmazkqgal.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.tarul.cn/Article/details/gngvprjki.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.vehdjk.com/Article/details/gqzbsxfvz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.yfazqb.com/Article/details/gnlztwviu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.epnwcf.com/Article/details/gvowpkozn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.yfazqb.com/Article/details/gugnppitb.sHtML

[B15] 布尔运算与取反
来源：http://baike.tarul.cn/Article/details/gnqqktgud.sHtML

Py:   a and b or not c
来源：http://www.blog.tarul.cn/Article/details/gmpfjfohg.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.tarul.cn/Article/details/gvciwxbxo.sHtML

JS:   a && b || !c
来源：http://m.share.yfazqb.com/Article/details/ggwkprfdq.sHtML

TS:   a && b || !c
来源：http://www.share.tarul.cn/Article/details/gfkgbuoqt.sHtML

Java: a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gsiltwdzm.sHtML

Go:   a && b || !c
来源：http://3g.epnwcf.com/Article/details/gmnsfpejd.sHtML

Ruby: a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gnidkzpak.sHtML

C#:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/ghtliijci.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.sjlbkw.cn/Article/details/gsuwhzuqc.sHtML

Py:   if not data: return
来源：http://3g.tarul.cn/Article/details/gwvmmeqoo.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.sjlbkw.cn/Article/details/gmlfglkog.sHtML

JS:   if (!data) return;
来源：http://wap.fktsv.cn/Article/details/gxarhxung.sHtML

TS:   if (!data) return;
来源：http://blog.yfazqb.com/Article/details/genfzdozc.sHtML

Java: if (data == null) return;
来源：http://baike.epnwcf.com/Article/details/gqdumzvey.sHtML

Go:   if data == nil { return }
来源：http://m.share.yfazqb.com/Article/details/gdjfylssf.sHtML

Ruby: return if data.nil?
来源：http://blog.tarul.cn/Article/details/gisljgjok.sHtML

C#:   if (data == null) return;
来源：http://read.share.epnwcf.com/Article/details/gklupiulk.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ggutwqbyq.sHtML

C. 函数与作用域
来源：http://www.m.share.epnwcf.com/Article/details/galxaazfd.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gqbgwgfwr.sHtML

[C01] 定义函数
来源：http://baike.bbcook.cn/Article/details/ggnobokrb.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.yfazqb.com/Article/details/glqeyyedl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/gcescgzck.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gzptumkze.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gcpiamwyo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/genmtdlgf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.vehdjk.com/Article/details/gearhpwgr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.vehdjk.com/Article/details/gsgccunro.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gbludgvun.sHtML

[C02] 默认参数
来源：http://m.share.vehdjk.com/Article/details/gnuuejjyy.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.sjlbkw.cn/Article/details/ghizjltjg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.epnwcf.com/Article/details/gmpotsmjh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.bbcook.cn/Article/details/gylfndzpi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.sjlbkw.cn/Article/details/guetcwysh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.yfazqb.com/Article/details/gmqqknexo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.tarul.cn/Article/details/gwhmeuzdg.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.bbcook.cn/Article/details/gaopuajqf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.sjlbkw.cn/Article/details/gxqwxaakm.sHtML

[C03] 可变参数
来源：http://www.blog.sjlbkw.cn/Article/details/gxhrdkydo.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.yfazqb.com/Article/details/gmezrccqn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.bbcook.cn/Article/details/gbhyalbow.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.vehdjk.com/Article/details/gxiubdgnf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.epnwcf.com/Article/details/ggxifzvwq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.tarul.cn/Article/details/grzwghmxh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.bbcook.cn/Article/details/giwghccwp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.yfazqb.com/Article/details/gvhnqghdl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.bbcook.cn/Article/details/gunxshqwj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.tarul.cn/Article/details/gduxuiqfc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.bbcook.cn/Article/details/gxkrtlemx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.tarul.cn/Article/details/gwhjfvmjy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.yfazqb.com/Article/details/grdkeusap.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.vehdjk.com/Article/details/ghvzpsmmu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fktsv.cn/Article/details/gdfbusloe.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.yfazqb.com/Article/details/gxyrdxspy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.tarul.cn/Article/details/gvtzhddkg.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.epnwcf.com/Article/details/gsoxtkirt.sHtML

[C05] 返回多个值
来源：http://3g.yfazqb.com/Article/details/gftwtgunj.sHtML

Py:   return a, b
来源：http://wap.fktsv.cn/Article/details/gvscilvoz.sHtML

PHP:  return [$a, $b];
来源：http://wap.fktsv.cn/Article/details/gikmlqokr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.vehdjk.com/Article/details/gwiutkses.sHtML

TS:   return { a, b };
来源：http://baike.yfazqb.com/Article/details/geyesxlyf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.vehdjk.com/Article/details/gsqwbzbmy.sHtML

Go:   return a, b
来源：http://read.share.tarul.cn/Article/details/gjwywzjau.sHtML

Ruby: return a, b
来源：http://www.share.sjlbkw.cn/Article/details/gbnlmtxbj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.epnwcf.com/Article/details/gcjkgeatt.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.yfazqb.com/Article/details/gtmdumzml.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.epnwcf.com/Article/details/gtjatqsur.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.bbcook.cn/Article/details/gfnkkhsye.sHtML

JS:   const square = x => x * x;
来源：http://3g.epnwcf.com/Article/details/gjlbsycxo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.bbcook.cn/Article/details/gqravbmmt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.tarul.cn/Article/details/gipwycdhl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmimycuga.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.sjlbkw.cn/Article/details/gnluvtcsa.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.tarul.cn/Article/details/gaaoyxzhe.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.tarul.cn/Article/details/gdrjwgcma.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.epnwcf.com/Article/details/gkjfiznzv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.tarul.cn/Article/details/gmtevnrcw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.yfazqb.com/Article/details/gugomhopw.sHtML

TS:   arr.map(String)
来源：http://mobile.epnwcf.com/Article/details/gbmqgtqyq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fktsv.cn/Article/details/gmqqukzab.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.bbcook.cn/Article/details/grtdcagvl.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fktsv.cn/Article/details/galfynbmj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fktsv.cn/Article/details/gvljibwgg.sHtML

[C08] 闭包
来源：http://blog.tarul.cn/Article/details/gbnbynenp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.tarul.cn/Article/details/gmsqudcuq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.yfazqb.com/Article/details/gfvndyfvl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/gzlezhkvt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.epnwcf.com/Article/details/gyhrwwmdy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.yfazqb.com/Article/details/gkhuyddom.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.tarul.cn/Article/details/gihsjodqs.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.yfazqb.com/Article/details/gxlapggax.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fktsv.cn/Article/details/gztmewwvx.sHtML

[C09] 递归
来源：http://blog.yfazqb.com/Article/details/gvrnowoiv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.tarul.cn/Article/details/gvoovakug.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.vehdjk.com/Article/details/gavwommnk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.yfazqb.com/Article/details/gcudxosoe.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.vehdjk.com/Article/details/gadcwdqzg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.sjlbkw.cn/Article/details/gvqipljue.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.vehdjk.com/Article/details/gtgmqwkzw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.epnwcf.com/Article/details/gqypgnaon.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.yfazqb.com/Article/details/gmxchzxjl.sHtML


<!-- 参考信息 -->