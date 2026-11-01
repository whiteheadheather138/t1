代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.tarul.cn/Article/details/gdvnooyyr.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.yfazqb.com/Article/details/gmongfjgw.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.yfazqb.com/Article/details/guctpdgup.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.bbcook.cn/Article/details/gtojcxyek.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.yfazqb.com/Article/details/gdolbmmsa.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.yfazqb.com/Article/details/giqcsynez.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.sjlbkw.cn/Article/details/gpxbxgrbf.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.sjlbkw.cn/Article/details/gnfnaymae.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.epnwcf.com/Article/details/gosrunkeh.sHtML

[A19] 交换两个变量
来源：http://m.share.vehdjk.com/Article/details/gibsmmwnh.sHtML

Py:   a, b = b, a
来源：http://mobile.sjlbkw.cn/Article/details/gjqrjcqtz.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.epnwcf.com/Article/details/gmyanejfc.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.tarul.cn/Article/details/gskjlfxwk.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.epnwcf.com/Article/details/ghwwapjji.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.yfazqb.com/Article/details/gkhzvvnnw.sHtML

Go:   a, b = b, a
来源：http://wap.fktsv.cn/Article/details/gdertvciu.sHtML

Ruby: a, b = b, a
来源：http://www.blog.vehdjk.com/Article/details/gglszzuho.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.tarul.cn/Article/details/gxdsjwnpi.sHtML

[A20] 读取标准输入
来源：http://3g.sjlbkw.cn/Article/details/gwuvvabxk.sHtML

Py:   name = input("请输入：")
来源：http://read.share.sjlbkw.cn/Article/details/gneeyfgsi.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.sjlbkw.cn/Article/details/gbmdwtnla.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.epnwcf.com/Article/details/gmecubycc.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.sjlbkw.cn/Article/details/gxrklwlmd.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.bbcook.cn/Article/details/gdoncbixl.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.bbcook.cn/Article/details/gnrvjxohb.sHtML

Ruby: gets.chomp
来源：http://mobile.epnwcf.com/Article/details/gbsqcoqae.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.sjlbkw.cn/Article/details/gxbnzvjbu.sHtML

[A21] 保留指定小数位输出
来源：http://3g.tarul.cn/Article/details/gezgazfar.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.tarul.cn/Article/details/gulbanedw.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.sjlbkw.cn/Article/details/gvbhyoekh.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.fktsv.cn/Article/details/grdceuflb.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.epnwcf.com/Article/details/gnvmlbomv.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://m.share.fktsv.cn/Article/details/gwjayskzm.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.bbcook.cn/Article/details/gobvrmefw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggghohxei.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.yfazqb.com/Article/details/godhlfubp.sHtML

[A22] 获取字符串长度
来源：http://mobile.vehdjk.com/Article/details/gyrywprzf.sHtML

Py:   len(s)
来源：http://baike.yfazqb.com/Article/details/gxgvokreh.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.yfazqb.com/Article/details/gemdcvszw.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.tarul.cn/Article/details/guhtvugqr.sHtML

TS:   s.length
来源：http://baike.tarul.cn/Article/details/gqydwdyro.sHtML

Java: s.length()
来源：http://blog.epnwcf.com/Article/details/ghnpjrlbp.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.vehdjk.com/Article/details/gqtmeqtww.sHtML

Ruby: s.length
来源：http://m.share.bbcook.cn/Article/details/gpuefgiov.sHtML

C#:   s.Length
来源：http://www.blog.vehdjk.com/Article/details/gwvjjbjaq.sHtML

[A23] 大小写转换
来源：http://3g.tarul.cn/Article/details/gmunebava.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.tarul.cn/Article/details/gmagdarea.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.bbcook.cn/Article/details/gervjhxta.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.vehdjk.com/Article/details/guriwqgxi.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.yfazqb.com/Article/details/gotnuknom.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.bbcook.cn/Article/details/gslmqexiw.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gzuiomfpk.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.fktsv.cn/Article/details/gdsiqydzx.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.bbcook.cn/Article/details/govckmztf.sHtML

[A24] 去除首尾空白
来源：http://3g.tarul.cn/Article/details/gapphjlty.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.sjlbkw.cn/Article/details/gpmxyibqb.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.vehdjk.com/Article/details/gdechvpzn.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.sjlbkw.cn/Article/details/gbnudkswx.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.fktsv.cn/Article/details/gwbbvbwcv.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.fktsv.cn/Article/details/gqednyqqn.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.epnwcf.com/Article/details/gchwkbmnh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.tarul.cn/Article/details/gvbeiptvd.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.fktsv.cn/Article/details/gytcftnwi.sHtML

[A25] 字符串比较
来源：http://mobile.vehdjk.com/Article/details/gxtvtlnej.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.fktsv.cn/Article/details/gjlhzknxl.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.sjlbkw.cn/Article/details/gnmyugmha.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fktsv.cn/Article/details/gklerpmoq.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.vehdjk.com/Article/details/gvuvbqnhl.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fktsv.cn/Article/details/gxpqjbddq.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.yfazqb.com/Article/details/grbdwzdex.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.vehdjk.com/Article/details/gkvtbwvjq.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.tarul.cn/Article/details/gibhxifec.sHtML

[A26] 类型转换总览
来源：http://www.share.epnwcf.com/Article/details/ggblhqoqw.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.bbcook.cn/Article/details/gvxtfvaie.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.epnwcf.com/Article/details/gxbkkqstt.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.tarul.cn/Article/details/gkrrgbjrf.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.sjlbkw.cn/Article/details/gdbeneidu.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.sjlbkw.cn/Article/details/goyxjbmgz.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.bbcook.cn/Article/details/guwzvdpre.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.yfazqb.com/Article/details/gisikwrlb.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.yfazqb.com/Article/details/gijrtgxfs.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gbymulvov.sHtML

B. 流程控制
来源：http://read.share.bbcook.cn/Article/details/gbewlzrkn.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gysxqrvig.sHtML

[B01] 条件判断 if / else
来源：http://m.share.bbcook.cn/Article/details/gutuiqoin.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.sjlbkw.cn/Article/details/gxjmzdogc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.sjlbkw.cn/Article/details/gamxsxwjp.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.yfazqb.com/Article/details/gerdozjau.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.epnwcf.com/Article/details/gvflfggab.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/geutwtuwd.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.bbcook.cn/Article/details/gayxyvraq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.tarul.cn/Article/details/gwpcekxhc.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.fktsv.cn/Article/details/ggprvzkwm.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.yfazqb.com/Article/details/glhhdkbje.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.yfazqb.com/Article/details/gndacpenh.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.yfazqb.com/Article/details/gcuoagliw.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.tarul.cn/Article/details/gajhpvwvt.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.yfazqb.com/Article/details/giejdvuxx.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fktsv.cn/Article/details/gzamjsedh.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.bbcook.cn/Article/details/gsrxaqorr.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.sjlbkw.cn/Article/details/godwytoht.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.tarul.cn/Article/details/gndyewahr.sHtML

[B03] switch / match / case
来源：http://wap.bbcook.cn/Article/details/gssdpwoga.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.vehdjk.com/Article/details/gqmbhjihc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.epnwcf.com/Article/details/ghkchtyxv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.sjlbkw.cn/Article/details/gfiuaybpv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.vehdjk.com/Article/details/gvksytsxv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/gbnalcvxb.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.sjlbkw.cn/Article/details/gngqtishs.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.vehdjk.com/Article/details/gvtcerxtv.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.tarul.cn/Article/details/giwtpzdun.sHtML

[B04] for 计数循环
来源：http://blog.bbcook.cn/Article/details/gnzcyeakl.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.bbcook.cn/Article/details/gedpcwzif.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.vehdjk.com/Article/details/gmxnsjyab.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fktsv.cn/Article/details/gczgxbocz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.yfazqb.com/Article/details/gsheibnte.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.yfazqb.com/Article/details/gxujevzsh.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.epnwcf.com/Article/details/gofqkbsqb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.vehdjk.com/Article/details/gqluudfeo.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.epnwcf.com/Article/details/golhpgloh.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.vehdjk.com/Article/details/grdfdzhna.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.epnwcf.com/Article/details/gclmcvvij.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.yfazqb.com/Article/details/gyhvyzxfl.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.sjlbkw.cn/Article/details/gkgikjzzc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.bbcook.cn/Article/details/gjgtxgmtx.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.yfazqb.com/Article/details/gkqgpdcun.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.tarul.cn/Article/details/gjkalztey.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.fktsv.cn/Article/details/gugqftmii.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.tarul.cn/Article/details/gxfvnyxsi.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.epnwcf.com/Article/details/gnoihdqmc.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.vehdjk.com/Article/details/gxzplmmnd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.bbcook.cn/Article/details/gihzpyovf.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.bbcook.cn/Article/details/giphqaeop.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.sjlbkw.cn/Article/details/giwaigpty.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjfcvgra.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.bbcook.cn/Article/details/giguvirqe.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.tarul.cn/Article/details/gqzdlddyt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.tarul.cn/Article/details/gspyqbfly.sHtML

[B07] while 循环
来源：http://read.share.fktsv.cn/Article/details/gwifmvvsq.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.yfazqb.com/Article/details/gwkiikziz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fktsv.cn/Article/details/gdtdmbaeb.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/gznkwhqzx.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/gnvyiryba.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/gkacmdbse.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.tarul.cn/Article/details/gsmksxwrx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.bbcook.cn/Article/details/gtgtdfkhp.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpowrlat.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.yfazqb.com/Article/details/gigioobnm.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.tarul.cn/Article/details/gzvdouecn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gxxddnivz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/giathlqhn.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.bbcook.cn/Article/details/gsubsreup.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/gyemsjffh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.yfazqb.com/Article/details/ggnmtdndf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.epnwcf.com/Article/details/glpaymmqk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gtqrqhorl.sHtML

[B09] break 与 continue
来源：http://www.m.share.fktsv.cn/Article/details/gxasefzmq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.yfazqb.com/Article/details/gdqbfeuja.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/glxfdxpit.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.bbcook.cn/Article/details/gpsfrmjlw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/gnbhfjlfw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/gzshxqipo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.epnwcf.com/Article/details/gmsrgdsgi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fktsv.cn/Article/details/ghdxuujhe.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.yfazqb.com/Article/details/gsmlaawfm.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.sjlbkw.cn/Article/details/gxpwwzfmh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.vehdjk.com/Article/details/gfblvgjsx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.sjlbkw.cn/Article/details/glydprzzf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fktsv.cn/Article/details/gyzpsstgn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.bbcook.cn/Article/details/gylutnkcs.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.yfazqb.com/Article/details/ghpuscxpa.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.yfazqb.com/Article/details/gcfwfjqdr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.yfazqb.com/Article/details/gonjypyhc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fktsv.cn/Article/details/gnkvrugxo.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.vehdjk.com/Article/details/gizceumvb.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fktsv.cn/Article/details/grqgfmwzl.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fktsv.cn/Article/details/ghoobrlqu.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.sjlbkw.cn/Article/details/gnwwfrflg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.epnwcf.com/Article/details/gfjxcgyzo.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.vehdjk.com/Article/details/guxwnvufs.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.tarul.cn/Article/details/ghzbqwmdb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.tarul.cn/Article/details/gvnjnkwln.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.vehdjk.com/Article/details/gnnypthrp.sHtML

[B12] 跳出多层循环
来源：http://www.blog.vehdjk.com/Article/details/gwdxejmut.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.vehdjk.com/Article/details/glfmsityp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.yfazqb.com/Article/details/gxrsjmqfp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.bbcook.cn/Article/details/gfmbafxjj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fktsv.cn/Article/details/gddzltyfi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.bbcook.cn/Article/details/gdkxlegnu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.sjlbkw.cn/Article/details/gsmbigxpy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.vehdjk.com/Article/details/gidaizscw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.vehdjk.com/Article/details/gqkvjrylp.sHtML

[B13] 判断是否为数字
来源：http://wap.epnwcf.com/Article/details/gzsptbekd.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.bbcook.cn/Article/details/gtdrketcs.sHtML

PHP:  is_numeric($x)
来源：http://baike.fktsv.cn/Article/details/gxpsmxfhp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.bbcook.cn/Article/details/gcybpcldr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fktsv.cn/Article/details/gttduvpna.sHtML

Java: x instanceof Number
来源：http://3g.bbcook.cn/Article/details/godgleslt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fktsv.cn/Article/details/gxsexfysl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.tarul.cn/Article/details/gwmqwekrm.sHtML

C#:   x is int or double or decimal
来源：http://wap.vehdjk.com/Article/details/glnwpfdey.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fktsv.cn/Article/details/gvazbjubd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.vehdjk.com/Article/details/glodljrjx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.tarul.cn/Article/details/grjdhtnhv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.vehdjk.com/Article/details/goaakovsy.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.yfazqb.com/Article/details/glxlezkaq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.fktsv.cn/Article/details/gclqwwxlq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fktsv.cn/Article/details/gfozidido.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fktsv.cn/Article/details/giedpbitx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gxqqhscwt.sHtML

[B15] 布尔运算与取反
来源：http://wap.yfazqb.com/Article/details/gjayquizh.sHtML

Py:   a and b or not c
来源：http://www.m.share.sjlbkw.cn/Article/details/gulazthkm.sHtML

PHP:  $a && $b || !$c
来源：http://baike.yfazqb.com/Article/details/gasawowxw.sHtML

JS:   a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/gszgvwjhd.sHtML

TS:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gwewmfnde.sHtML

Java: a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gaxnaqbve.sHtML

Go:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/gqtfjiofn.sHtML

Ruby: a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gmxszrbqb.sHtML

C#:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/gwahhulut.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fktsv.cn/Article/details/gonxujaqy.sHtML

Py:   if not data: return
来源：http://m.share.yfazqb.com/Article/details/gdzsqkcpb.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.vehdjk.com/Article/details/gwcvdetiy.sHtML

JS:   if (!data) return;
来源：http://baike.yfazqb.com/Article/details/grjzgoryb.sHtML

TS:   if (!data) return;
来源：http://read.share.tarul.cn/Article/details/gewigbwrh.sHtML

Java: if (data == null) return;
来源：http://www.m.share.vehdjk.com/Article/details/gwuyrchpm.sHtML

Go:   if data == nil { return }
来源：http://www.share.tarul.cn/Article/details/gcxgnjxuz.sHtML

Ruby: return if data.nil?
来源：http://baike.bbcook.cn/Article/details/gybujkpix.sHtML

C#:   if (data == null) return;
来源：http://www.share.yfazqb.com/Article/details/gacxpcoxd.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gjjcxdmje.sHtML

C. 函数与作用域
来源：http://www.share.yfazqb.com/Article/details/gaxqlmejv.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gaswedacb.sHtML

[C01] 定义函数
来源：http://wap.tarul.cn/Article/details/grsyocbrb.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.yfazqb.com/Article/details/gptyjbksy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fktsv.cn/Article/details/gtuizsros.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gkjgdxucu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gqzcgewxv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/glfygvrhk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fktsv.cn/Article/details/gjbhyupjb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fktsv.cn/Article/details/gvjregksg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gjhbwhqeg.sHtML

[C02] 默认参数
来源：http://www.share.fktsv.cn/Article/details/gbmrnbxqo.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.vehdjk.com/Article/details/gfbddqwgj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.tarul.cn/Article/details/gsydqxdrj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.vehdjk.com/Article/details/gnlzdcmpo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gmokdksgg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.bbcook.cn/Article/details/grxyovfro.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.bbcook.cn/Article/details/gylhovgdp.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.yfazqb.com/Article/details/grxjxnsse.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.bbcook.cn/Article/details/gcfekwpiv.sHtML

[C03] 可变参数
来源：http://3g.tarul.cn/Article/details/gwwristib.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.epnwcf.com/Article/details/gxkdbepxg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.tarul.cn/Article/details/ggnjppnfe.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.tarul.cn/Article/details/gnfxjqtph.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.bbcook.cn/Article/details/gvbwjzhsd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.yfazqb.com/Article/details/gbtaerofi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.sjlbkw.cn/Article/details/glzcxpmox.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.bbcook.cn/Article/details/gxmkwfcbg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.sjlbkw.cn/Article/details/gcmwecsuc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.bbcook.cn/Article/details/gmehgdjfl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.epnwcf.com/Article/details/geluihnre.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.sjlbkw.cn/Article/details/gbejyudrz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.sjlbkw.cn/Article/details/gcisaffkc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.tarul.cn/Article/details/gzxnbuisd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.yfazqb.com/Article/details/gxfxvgorx.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.yfazqb.com/Article/details/gdoedutmd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.bbcook.cn/Article/details/guxmbhvoa.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.bbcook.cn/Article/details/gksbkzzjt.sHtML

[C05] 返回多个值
来源：http://www.share.yfazqb.com/Article/details/gjcgmehuv.sHtML

Py:   return a, b
来源：http://m.share.fktsv.cn/Article/details/gzcmsltsq.sHtML

PHP:  return [$a, $b];
来源：http://wap.tarul.cn/Article/details/gdwwfdydw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.tarul.cn/Article/details/gzcrkjqxo.sHtML

TS:   return { a, b };
来源：http://www.share.yfazqb.com/Article/details/gourucrar.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.epnwcf.com/Article/details/gseixpdea.sHtML

Go:   return a, b
来源：http://baike.bbcook.cn/Article/details/ghboadaoy.sHtML

Ruby: return a, b
来源：http://m.share.bbcook.cn/Article/details/gznfkcvgx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.epnwcf.com/Article/details/gwidfpjbm.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.tarul.cn/Article/details/givweuzxa.sHtML

Py:   square = lambda x: x * x
来源：http://blog.bbcook.cn/Article/details/glhwvdsvl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.bbcook.cn/Article/details/gojyaymfb.sHtML

JS:   const square = x => x * x;
来源：http://baike.tarul.cn/Article/details/gvqfgiliq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.tarul.cn/Article/details/gknwnrlwt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.sjlbkw.cn/Article/details/gxqsgllbd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.sjlbkw.cn/Article/details/gkdmcdchf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.vehdjk.com/Article/details/gmhhihjdg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.sjlbkw.cn/Article/details/gbfmswhyq.sHtML

[C07] 把函数作为参数传入
来源：http://blog.vehdjk.com/Article/details/guvcjfxzc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.vehdjk.com/Article/details/gbbmrjgpu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.yfazqb.com/Article/details/gudrzgzcp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.bbcook.cn/Article/details/gjffsxrhz.sHtML

TS:   arr.map(String)
来源：http://3g.tarul.cn/Article/details/grzzhhogl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.tarul.cn/Article/details/gklgironf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fktsv.cn/Article/details/goyvteumo.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.bbcook.cn/Article/details/gzchylqcr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.tarul.cn/Article/details/gpqbbibuh.sHtML

[C08] 闭包
来源：http://www.m.share.tarul.cn/Article/details/gpeizihir.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.bbcook.cn/Article/details/ggvgvygam.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.vehdjk.com/Article/details/goclwmkwo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fktsv.cn/Article/details/ghctwqjpc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gvfyfahxp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.yfazqb.com/Article/details/gfqzqexap.sHtML


<!-- 参考信息 -->