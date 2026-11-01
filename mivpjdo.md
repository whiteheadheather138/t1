代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.epnwcf.com/Article/details/gcvtwmnul.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.yfazqb.com/Article/details/gyzgcqqrr.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.bbcook.cn/Article/details/gpjzpigre.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.sjlbkw.cn/Article/details/gpenvixjo.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.sjlbkw.cn/Article/details/gqiaagbwa.sHtML

Ruby: gets.chomp
来源：http://mobile.epnwcf.com/Article/details/gsqjvkibi.sHtML

C#:   Console.ReadLine();
来源：http://blog.epnwcf.com/Article/details/gqoiatwbk.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.epnwcf.com/Article/details/gkzkovtvs.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.sjlbkw.cn/Article/details/grkzhxuqx.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.yfazqb.com/Article/details/gjvbdefdl.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.tarul.cn/Article/details/gsnewzeas.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.bbcook.cn/Article/details/gzscerikp.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.yfazqb.com/Article/details/gfoeqhqqd.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.fktsv.cn/Article/details/ghjepojod.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.fktsv.cn/Article/details/gyvhklatn.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.fktsv.cn/Article/details/gftyrkdqf.sHtML

[A22] 获取字符串长度
来源：http://blog.vehdjk.com/Article/details/gqjcphxap.sHtML

Py:   len(s)
来源：http://www.blog.tarul.cn/Article/details/gpwfckzej.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.vehdjk.com/Article/details/gvtpqlhol.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.yfazqb.com/Article/details/gldferudy.sHtML

TS:   s.length
来源：http://3g.yfazqb.com/Article/details/grqzzkzzg.sHtML

Java: s.length()
来源：http://blog.epnwcf.com/Article/details/gpxsezush.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.yfazqb.com/Article/details/gbpoksgjc.sHtML

Ruby: s.length
来源：http://www.blog.sjlbkw.cn/Article/details/gkwenllzg.sHtML

C#:   s.Length
来源：http://read.share.bbcook.cn/Article/details/gsgtixfba.sHtML

[A23] 大小写转换
来源：http://www.blog.tarul.cn/Article/details/gvwwlswrw.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.bbcook.cn/Article/details/glbcmjpfd.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.sjlbkw.cn/Article/details/goqkpcywq.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.yfazqb.com/Article/details/gvndlntti.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.vehdjk.com/Article/details/gtvbmghxr.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.vehdjk.com/Article/details/gsvuzmadq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.vehdjk.com/Article/details/gabgbwiim.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.vehdjk.com/Article/details/glbzhyhwr.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.sjlbkw.cn/Article/details/gmgiztjyp.sHtML

[A24] 去除首尾空白
来源：http://mobile.sjlbkw.cn/Article/details/ghzfokyzc.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.vehdjk.com/Article/details/gycxqelea.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.bbcook.cn/Article/details/gsunccziq.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.yfazqb.com/Article/details/gimwmhobf.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.sjlbkw.cn/Article/details/gjimswlps.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.fktsv.cn/Article/details/gxrmkzcwb.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.fktsv.cn/Article/details/gdtzquyqk.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.fktsv.cn/Article/details/ghjuswtrx.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.epnwcf.com/Article/details/gstjwhybw.sHtML

[A25] 字符串比较
来源：http://www.m.share.fktsv.cn/Article/details/gegawaigt.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.fktsv.cn/Article/details/gqpvpmvey.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.bbcook.cn/Article/details/gpijwjilt.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.tarul.cn/Article/details/ggmbayhvs.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.bbcook.cn/Article/details/ggtdscpep.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.yfazqb.com/Article/details/gtfrfwrbh.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.bbcook.cn/Article/details/gkagpferl.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.epnwcf.com/Article/details/grrhtgnhg.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.bbcook.cn/Article/details/gmxgrbyst.sHtML

[A26] 类型转换总览
来源：http://3g.epnwcf.com/Article/details/gmbfulhvl.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.tarul.cn/Article/details/gyzaacusx.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.epnwcf.com/Article/details/gkbsdkafe.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.tarul.cn/Article/details/glouckaoy.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjeqbyfq.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.epnwcf.com/Article/details/grnnbqlzf.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.yfazqb.com/Article/details/gkskekvnb.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.vehdjk.com/Article/details/gcrfxwqfq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.yfazqb.com/Article/details/gavespwsh.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gnjtzrztx.sHtML

B. 流程控制
来源：http://www.share.tarul.cn/Article/details/grsgzyfua.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gnotrudnb.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.epnwcf.com/Article/details/gyujapxxx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.sjlbkw.cn/Article/details/gsxgrehhm.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.tarul.cn/Article/details/gakuyskzg.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.yfazqb.com/Article/details/gftnzifih.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fktsv.cn/Article/details/gksprmdjh.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.yfazqb.com/Article/details/gfyykothu.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.tarul.cn/Article/details/ggpdcubrr.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.vehdjk.com/Article/details/gnsstjnwi.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.yfazqb.com/Article/details/gugddblfm.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.tarul.cn/Article/details/gjifudsnm.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.tarul.cn/Article/details/gzqbqmtvu.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.fktsv.cn/Article/details/ggnvxagjz.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fktsv.cn/Article/details/gvslopxvu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.tarul.cn/Article/details/gtlwxdgyq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.sjlbkw.cn/Article/details/gngaodfew.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.fktsv.cn/Article/details/gkdnujtlu.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.sjlbkw.cn/Article/details/ggmrzgtpi.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.sjlbkw.cn/Article/details/gilthimdk.sHtML

[B03] switch / match / case
来源：http://wap.fktsv.cn/Article/details/globjimar.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.vehdjk.com/Article/details/gkhwauobi.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.sjlbkw.cn/Article/details/ghvfyqpfe.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.bbcook.cn/Article/details/gpvbxjjof.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fktsv.cn/Article/details/gepcgwhbq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.tarul.cn/Article/details/ggdhyigse.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.yfazqb.com/Article/details/gmwycejjw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.vehdjk.com/Article/details/grxklbqdo.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.epnwcf.com/Article/details/gdifnywwe.sHtML

[B04] for 计数循环
来源：http://baike.epnwcf.com/Article/details/gpjflnjnm.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.fktsv.cn/Article/details/gmysacrla.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.bbcook.cn/Article/details/glzxtzvxm.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.vehdjk.com/Article/details/guwlfmrhq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.sjlbkw.cn/Article/details/gltgytmux.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.sjlbkw.cn/Article/details/gxvfvylzj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.yfazqb.com/Article/details/ghpxxoutp.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.epnwcf.com/Article/details/gickukjae.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.yfazqb.com/Article/details/gxxugiyks.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.bbcook.cn/Article/details/ghycqmkzj.sHtML

Py:   for item in arr: print(item)
来源：http://wap.vehdjk.com/Article/details/guhpktrbg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.vehdjk.com/Article/details/gbmzhsnvj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.vehdjk.com/Article/details/glgnhbsvh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.vehdjk.com/Article/details/gpnqwkbeq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.yfazqb.com/Article/details/gwzwpqcvn.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.sjlbkw.cn/Article/details/glpwzdohz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.fktsv.cn/Article/details/gusemsjbl.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.epnwcf.com/Article/details/gcefjdhqz.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.epnwcf.com/Article/details/gkmzpyjya.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.yfazqb.com/Article/details/gfgrutinq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.vehdjk.com/Article/details/gyhlwsdja.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.bbcook.cn/Article/details/grzbpizst.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fktsv.cn/Article/details/gwxbfdjxz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.epnwcf.com/Article/details/gwympbzxu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.yfazqb.com/Article/details/gcaikrykn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.sjlbkw.cn/Article/details/gvqmsdjbb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.bbcook.cn/Article/details/gbqymdzil.sHtML

[B07] while 循环
来源：http://baike.vehdjk.com/Article/details/gtsuynwvy.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.bbcook.cn/Article/details/gsgmxrubl.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fktsv.cn/Article/details/gdwkaaybs.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.vehdjk.com/Article/details/goirdtcqc.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvsezylis.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.fktsv.cn/Article/details/gieommrnl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.epnwcf.com/Article/details/gvpvtrxci.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.vehdjk.com/Article/details/goscbdsln.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.bbcook.cn/Article/details/gzkjemiqd.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.epnwcf.com/Article/details/ggumvhhfj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.vehdjk.com/Article/details/gsfepxrye.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.epnwcf.com/Article/details/gzxjqyzqy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.bbcook.cn/Article/details/gpsovmaha.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/gmzxamkrl.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gqxazdiol.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.yfazqb.com/Article/details/gcdmpusmx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.yfazqb.com/Article/details/gnrqayahi.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.yfazqb.com/Article/details/gfugiqddx.sHtML

[B09] break 与 continue
来源：http://mobile.sjlbkw.cn/Article/details/gjsfffrny.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.tarul.cn/Article/details/gbeprtdpr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdtpittl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.tarul.cn/Article/details/giyoksapg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/ggkdkwsqc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/gkruwatbt.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fktsv.cn/Article/details/grnpababn.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.tarul.cn/Article/details/grxknjiva.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gmbehulnd.sHtML

[B10] 遍历同时拿索引
来源：http://wap.tarul.cn/Article/details/guxprglin.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.bbcook.cn/Article/details/ggjghduag.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.bbcook.cn/Article/details/gqsusuidt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.tarul.cn/Article/details/gnjtgbils.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.bbcook.cn/Article/details/gojgxenly.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.vehdjk.com/Article/details/gdxtocqdb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.epnwcf.com/Article/details/gbljlhlfo.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.vehdjk.com/Article/details/geixeovfr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.vehdjk.com/Article/details/gokhzspuq.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.epnwcf.com/Article/details/gjvvgwkbn.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.vehdjk.com/Article/details/gnbnsbqos.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.tarul.cn/Article/details/gcujexhxk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.tarul.cn/Article/details/gpbmwwveh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.epnwcf.com/Article/details/gldfovdxe.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.epnwcf.com/Article/details/gojxwjukh.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.vehdjk.com/Article/details/gqadznpqn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.bbcook.cn/Article/details/gzmwrfzpc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gkeugdboo.sHtML

[B12] 跳出多层循环
来源：http://3g.bbcook.cn/Article/details/ghjrojtnd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.tarul.cn/Article/details/gdowjsafb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.tarul.cn/Article/details/gcbankdqo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.yfazqb.com/Article/details/gjooxyewh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.vehdjk.com/Article/details/ggrchlabl.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/gczrgaphc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.sjlbkw.cn/Article/details/gvwglgvpg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fktsv.cn/Article/details/gkkmsorio.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.sjlbkw.cn/Article/details/gaghfopnm.sHtML

[B13] 判断是否为数字
来源：http://www.share.tarul.cn/Article/details/grkuvnimz.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.tarul.cn/Article/details/groudenty.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.vehdjk.com/Article/details/gavusrpjc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.vehdjk.com/Article/details/gjptyamws.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.yfazqb.com/Article/details/gaidttnzo.sHtML

Java: x instanceof Number
来源：http://blog.sjlbkw.cn/Article/details/gmdledgrg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.vehdjk.com/Article/details/gsnzrczba.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.epnwcf.com/Article/details/gcjhuffst.sHtML

C#:   x is int or double or decimal
来源：http://read.share.epnwcf.com/Article/details/giyferpxd.sHtML

[B14] 判断值是否在集合内
来源：http://baike.yfazqb.com/Article/details/gosvhgbms.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.tarul.cn/Article/details/gspuhbxxg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.yfazqb.com/Article/details/glczuuplq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.vehdjk.com/Article/details/geyzmacjm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.vehdjk.com/Article/details/guvzxkezy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.yfazqb.com/Article/details/gydooerzz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.sjlbkw.cn/Article/details/gzdilsjry.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.bbcook.cn/Article/details/gdlidjxhs.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.tarul.cn/Article/details/ghijjsgfs.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.epnwcf.com/Article/details/grvvcqjuh.sHtML

Py:   a and b or not c
来源：http://www.m.share.vehdjk.com/Article/details/gjtmeernd.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.vehdjk.com/Article/details/gnrtlzudg.sHtML

JS:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/grlmzcwiu.sHtML

TS:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/gzkuvyhqr.sHtML

Java: a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/ghbviegqa.sHtML

Go:   a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gibxqxkzb.sHtML

Ruby: a && b || !c
来源：http://www.share.epnwcf.com/Article/details/ggwxdmava.sHtML

C#:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/gremlycgh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.sjlbkw.cn/Article/details/gumsfpkoq.sHtML

Py:   if not data: return
来源：http://www.share.epnwcf.com/Article/details/gdvnzjyff.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.bbcook.cn/Article/details/gulnfycwk.sHtML

JS:   if (!data) return;
来源：http://read.share.fktsv.cn/Article/details/guhwtktrt.sHtML

TS:   if (!data) return;
来源：http://www.blog.bbcook.cn/Article/details/ggntfxlbb.sHtML

Java: if (data == null) return;
来源：http://m.share.bbcook.cn/Article/details/geuzbayum.sHtML

Go:   if data == nil { return }
来源：http://www.share.yfazqb.com/Article/details/gskowuoiy.sHtML

Ruby: return if data.nil?
来源：http://www.share.bbcook.cn/Article/details/ghzvyngou.sHtML

C#:   if (data == null) return;
来源：http://m.share.fktsv.cn/Article/details/gbijeahml.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gqrfzhpyf.sHtML

C. 函数与作用域
来源：http://read.share.vehdjk.com/Article/details/gmlclxwqp.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/grlnjqcew.sHtML

[C01] 定义函数
来源：http://www.blog.tarul.cn/Article/details/gjmvqybrw.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.vehdjk.com/Article/details/grkvssijb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/gfjhxyypj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gqfxynrsz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gkvojoabc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gyrlpdcuh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.sjlbkw.cn/Article/details/gkfkfvygd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fktsv.cn/Article/details/gjmuupbza.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gioyzdial.sHtML

[C02] 默认参数
来源：http://baike.epnwcf.com/Article/details/gusebfnkk.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.tarul.cn/Article/details/glbdqzeyu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.tarul.cn/Article/details/gqrxomnpq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fktsv.cn/Article/details/gqiwtxmry.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.bbcook.cn/Article/details/guklffson.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fktsv.cn/Article/details/gpsrvgwfk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.vehdjk.com/Article/details/gyiaugzwk.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fktsv.cn/Article/details/gwlguzqfy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.vehdjk.com/Article/details/gsljcyita.sHtML

[C03] 可变参数
来源：http://mobile.yfazqb.com/Article/details/ghtkuofsb.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.tarul.cn/Article/details/govgxlxkv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.epnwcf.com/Article/details/gtnttwdpc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.yfazqb.com/Article/details/glwrpuvnf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.sjlbkw.cn/Article/details/ghwriqwnc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.yfazqb.com/Article/details/gxsrkqpwx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.yfazqb.com/Article/details/gzidgagwq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.yfazqb.com/Article/details/geoyvmvga.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.bbcook.cn/Article/details/gzcjowzrg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fktsv.cn/Article/details/gaswkwvlw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fktsv.cn/Article/details/gegnvfkka.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fktsv.cn/Article/details/gkjvophaw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.epnwcf.com/Article/details/gqucffnel.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.epnwcf.com/Article/details/gmukwgicf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.epnwcf.com/Article/details/gepseinwm.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.epnwcf.com/Article/details/gimpgqxcq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.bbcook.cn/Article/details/gjrbrgqpe.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/gwpqxymws.sHtML

[C05] 返回多个值
来源：http://m.share.tarul.cn/Article/details/geffsjguh.sHtML

Py:   return a, b
来源：http://baike.sjlbkw.cn/Article/details/gxtitbtlp.sHtML

PHP:  return [$a, $b];
来源：http://m.share.vehdjk.com/Article/details/gmpwdlzbz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.epnwcf.com/Article/details/gnphhmkbf.sHtML

TS:   return { a, b };
来源：http://wap.bbcook.cn/Article/details/ggyrggwxa.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.epnwcf.com/Article/details/gzpujyvfn.sHtML

Go:   return a, b
来源：http://www.blog.bbcook.cn/Article/details/gdlvhzsdb.sHtML

Ruby: return a, b
来源：http://m.share.yfazqb.com/Article/details/glbuywjuf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.sjlbkw.cn/Article/details/gxayzmebk.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fktsv.cn/Article/details/ggbudndgk.sHtML

Py:   square = lambda x: x * x
来源：http://wap.bbcook.cn/Article/details/gnnuoqbfk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.epnwcf.com/Article/details/ggdwzotra.sHtML

JS:   const square = x => x * x;
来源：http://m.share.vehdjk.com/Article/details/gkuzqqxac.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.yfazqb.com/Article/details/gklhnpahm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.vehdjk.com/Article/details/gknwgzuhc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fktsv.cn/Article/details/glnhiyksq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.tarul.cn/Article/details/gfuzbvxam.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.tarul.cn/Article/details/gwvlytnpe.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.epnwcf.com/Article/details/gescwvvfr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.bbcook.cn/Article/details/gfyxvyupx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.epnwcf.com/Article/details/gkwquksyv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fktsv.cn/Article/details/gyskknpml.sHtML

TS:   arr.map(String)
来源：http://www.m.share.vehdjk.com/Article/details/gysytogcv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.tarul.cn/Article/details/gdbdqbmej.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.tarul.cn/Article/details/gstrhztsz.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.yfazqb.com/Article/details/gjaxvtaft.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.yfazqb.com/Article/details/gvyuwvkmf.sHtML

[C08] 闭包
来源：http://m.share.tarul.cn/Article/details/gkdtjsqsj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.vehdjk.com/Article/details/gcooigydf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.vehdjk.com/Article/details/gaopcapwe.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/ggeoprmgl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.vehdjk.com/Article/details/gtgxznxjf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.bbcook.cn/Article/details/ggeauscyy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.bbcook.cn/Article/details/gcqecippj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fktsv.cn/Article/details/gztoxthvd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.vehdjk.com/Article/details/geffhwzqy.sHtML

[C09] 递归
来源：http://mobile.fktsv.cn/Article/details/gczubwncq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.bbcook.cn/Article/details/gvmvedtoq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.bbcook.cn/Article/details/gysgfxhoo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.epnwcf.com/Article/details/grwmxqniq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fktsv.cn/Article/details/gvostwyct.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.sjlbkw.cn/Article/details/gkutmyvha.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.sjlbkw.cn/Article/details/gmifhjown.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.sjlbkw.cn/Article/details/gtthgowux.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.epnwcf.com/Article/details/gglwvyrjf.sHtML

[C10] 变量作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gbfwhrqli.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.yfazqb.com/Article/details/gtjyplvkr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.vehdjk.com/Article/details/gnhkdrzei.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fktsv.cn/Article/details/gecqohboe.sHtML

TS:   同 JS
来源：http://mobile.epnwcf.com/Article/details/gcymiwhhb.sHtML

Java: 方法内为块级作用域
来源：http://m.share.bbcook.cn/Article/details/gofxdfuoc.sHtML

Go:   花括号块级作用域
来源：http://mobile.tarul.cn/Article/details/gylgjnnbe.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.tarul.cn/Article/details/gdfixhkgm.sHtML


<!-- 参考信息 -->