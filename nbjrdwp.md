代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.sjlbkw.cn/Article/details/gguhbuggt.sHtML

Ruby: gets.chomp
来源：http://blog.fktsv.cn/Article/details/guweyyzuo.sHtML

C#:   Console.ReadLine();
来源：http://wap.sjlbkw.cn/Article/details/gpufnlpwx.sHtML

[A21] 保留指定小数位输出
来源：http://3g.epnwcf.com/Article/details/gzbxfzjlu.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.bbcook.cn/Article/details/gszcrxaut.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.fktsv.cn/Article/details/ghjvwkzyp.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.bbcook.cn/Article/details/gicieizwf.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.yfazqb.com/Article/details/grfwpcylg.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.vehdjk.com/Article/details/gkzqvpyph.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.yfazqb.com/Article/details/gluttwcwl.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.epnwcf.com/Article/details/gquguokir.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.tarul.cn/Article/details/gpqgazcfm.sHtML

[A22] 获取字符串长度
来源：http://m.share.yfazqb.com/Article/details/gjjorgiwm.sHtML

Py:   len(s)
来源：http://www.share.vehdjk.com/Article/details/gkpnrxvxs.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.fktsv.cn/Article/details/ginytivrd.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.fktsv.cn/Article/details/ghuwlflbu.sHtML

TS:   s.length
来源：http://m.share.tarul.cn/Article/details/gtioktmfy.sHtML

Java: s.length()
来源：http://wap.tarul.cn/Article/details/gjfgwncdy.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.vehdjk.com/Article/details/gchgoajgb.sHtML

Ruby: s.length
来源：http://www.share.tarul.cn/Article/details/gxfsfqudz.sHtML

C#:   s.Length
来源：http://blog.yfazqb.com/Article/details/gqujisdrq.sHtML

[A23] 大小写转换
来源：http://m.share.epnwcf.com/Article/details/gvembcaok.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.tarul.cn/Article/details/grxwszuat.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.vehdjk.com/Article/details/gxudmdbch.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.vehdjk.com/Article/details/goabnzsjn.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.sjlbkw.cn/Article/details/gswnxfxab.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.vehdjk.com/Article/details/gsoqfpfpx.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.sjlbkw.cn/Article/details/glkslgzuo.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.epnwcf.com/Article/details/gwqayehzp.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.yfazqb.com/Article/details/ggdmhmxfx.sHtML

[A24] 去除首尾空白
来源：http://blog.vehdjk.com/Article/details/gqpdqylho.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.tarul.cn/Article/details/gbikslgoj.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.tarul.cn/Article/details/gbvyroydm.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.tarul.cn/Article/details/gvpiubqbu.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.bbcook.cn/Article/details/gkdpltvmp.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.vehdjk.com/Article/details/grysbnpba.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.epnwcf.com/Article/details/gikgvnsaw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.tarul.cn/Article/details/gvvbpmtfk.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.yfazqb.com/Article/details/gnwlauwii.sHtML

[A25] 字符串比较
来源：http://www.m.share.vehdjk.com/Article/details/gfekulezx.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.vehdjk.com/Article/details/gvfxsgwiv.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.epnwcf.com/Article/details/gcwimpgbc.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.tarul.cn/Article/details/gbvglsakn.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.tarul.cn/Article/details/guwpibvjb.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.epnwcf.com/Article/details/gvqdaaamd.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.sjlbkw.cn/Article/details/gdpgnzcsk.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.bbcook.cn/Article/details/ghwiskmhv.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.vehdjk.com/Article/details/ggpbohhcv.sHtML

[A26] 类型转换总览
来源：http://www.m.share.epnwcf.com/Article/details/gytozgwvm.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.bbcook.cn/Article/details/golltupmh.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.sjlbkw.cn/Article/details/gvofoycet.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.sjlbkw.cn/Article/details/grceqfhnn.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.yfazqb.com/Article/details/gjseeihmm.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.tarul.cn/Article/details/gfkanlcuq.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.epnwcf.com/Article/details/gnkinkxdg.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.sjlbkw.cn/Article/details/gzxrdbffh.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.fktsv.cn/Article/details/gusabcueg.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmvqlwsz.sHtML

B. 流程控制
来源：http://wap.tarul.cn/Article/details/gtybaqkwd.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gdfvsxges.sHtML

[B01] 条件判断 if / else
来源：http://3g.vehdjk.com/Article/details/gqvysqfat.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.bbcook.cn/Article/details/gfodwfhpg.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.epnwcf.com/Article/details/gbshdqofe.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fktsv.cn/Article/details/gqqmcnkqx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.epnwcf.com/Article/details/ghhqqmzlq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.vehdjk.com/Article/details/gwxqczxhj.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.sjlbkw.cn/Article/details/gunufvbox.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.epnwcf.com/Article/details/ghjxsucra.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.yfazqb.com/Article/details/gqdbwktzn.sHtML

[B02] 多分支 else if / elif
来源：http://wap.yfazqb.com/Article/details/ginegzamy.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.vehdjk.com/Article/details/gzxjotquw.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.tarul.cn/Article/details/gaxemjswo.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.epnwcf.com/Article/details/gselvujjs.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.tarul.cn/Article/details/galrsxphq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.epnwcf.com/Article/details/gnzfdpfkm.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gofbofsju.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.sjlbkw.cn/Article/details/gixmzszjb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.bbcook.cn/Article/details/gtlqmitwm.sHtML

[B03] switch / match / case
来源：http://3g.bbcook.cn/Article/details/gnxugxngl.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.epnwcf.com/Article/details/gcpcjzfjv.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.vehdjk.com/Article/details/gsjdqydjm.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.sjlbkw.cn/Article/details/gbakcztjq.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.vehdjk.com/Article/details/ghwxicoma.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.fktsv.cn/Article/details/gknhnsvoq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.vehdjk.com/Article/details/giemrqicg.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.fktsv.cn/Article/details/gdrgdcptk.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.vehdjk.com/Article/details/gxuoznafl.sHtML

[B04] for 计数循环
来源：http://m.share.vehdjk.com/Article/details/gqsjhhlce.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.bbcook.cn/Article/details/gcoqulvtd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.vehdjk.com/Article/details/gxwxkdvfn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.sjlbkw.cn/Article/details/gguaokuff.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.yfazqb.com/Article/details/gmssrvrmy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.sjlbkw.cn/Article/details/gqpviqhxa.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.sjlbkw.cn/Article/details/gbpuaduyg.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.fktsv.cn/Article/details/gubxmienp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.sjlbkw.cn/Article/details/gupkxseaa.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.fktsv.cn/Article/details/ghgoxkkkm.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.bbcook.cn/Article/details/gbyirzpgr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.bbcook.cn/Article/details/gyzcshmbx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fktsv.cn/Article/details/geglfwqiq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.bbcook.cn/Article/details/grgszolsg.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.sjlbkw.cn/Article/details/gdeyssrxd.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.epnwcf.com/Article/details/ggrabjoyd.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.epnwcf.com/Article/details/gmfengphr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.sjlbkw.cn/Article/details/gkxxxleic.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.yfazqb.com/Article/details/gngdzcsdw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.tarul.cn/Article/details/gxzltahcx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.bbcook.cn/Article/details/gwynlidvq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.bbcook.cn/Article/details/gbhycgpna.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fktsv.cn/Article/details/gbrugaziv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.vehdjk.com/Article/details/gcothbczt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.epnwcf.com/Article/details/gpmzwkjqr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.vehdjk.com/Article/details/gubsrulfq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.yfazqb.com/Article/details/gekzrcbtx.sHtML

[B07] while 循环
来源：http://wap.fktsv.cn/Article/details/gmfkskejq.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.fktsv.cn/Article/details/gvkkcsucp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.vehdjk.com/Article/details/gvfhyfvmu.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/ghwrrnvtb.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/gzvtrwqhf.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.epnwcf.com/Article/details/gpejlnbgo.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.sjlbkw.cn/Article/details/gtinykwfj.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.tarul.cn/Article/details/glsohxhts.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.bbcook.cn/Article/details/glugvxwez.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.bbcook.cn/Article/details/gmpqmrgta.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.sjlbkw.cn/Article/details/gmlzfthty.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.tarul.cn/Article/details/gfsyoubtt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.vehdjk.com/Article/details/gszflfbwb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gynslksvg.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.bbcook.cn/Article/details/ghladtqze.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.epnwcf.com/Article/details/gjbwrrqtq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.yfazqb.com/Article/details/gsbnkhvak.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.bbcook.cn/Article/details/goodvhwrb.sHtML

[B09] break 与 continue
来源：http://www.share.vehdjk.com/Article/details/gwfupgpid.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fktsv.cn/Article/details/glwxhsiet.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/gjqvmllev.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gxwzzmbjl.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/gwdemsuio.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/gsjvgfxuf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.tarul.cn/Article/details/gmgsypamf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.epnwcf.com/Article/details/gkpjaohzz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gmbutjkvn.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fktsv.cn/Article/details/gpaljrkkg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.vehdjk.com/Article/details/gffmipvjj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.tarul.cn/Article/details/gzivnqblm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.epnwcf.com/Article/details/gdztzozem.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fktsv.cn/Article/details/gtibfarfk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.epnwcf.com/Article/details/gtwoipjqc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.bbcook.cn/Article/details/gobtfepnf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzkyluep.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.tarul.cn/Article/details/grbjuhylk.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.bbcook.cn/Article/details/grtotokch.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.sjlbkw.cn/Article/details/gjuwsmptm.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fktsv.cn/Article/details/gtbaqbbwk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.yfazqb.com/Article/details/gddxtkxif.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fktsv.cn/Article/details/ggwiescef.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.yfazqb.com/Article/details/ggsxtrlra.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.vehdjk.com/Article/details/gvejobjpr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.vehdjk.com/Article/details/gilxlxzgy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.tarul.cn/Article/details/gefqlbnmi.sHtML

[B12] 跳出多层循环
来源：http://read.share.epnwcf.com/Article/details/grxkzpxte.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.tarul.cn/Article/details/gufbkqsvv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.vehdjk.com/Article/details/gjrxpkynd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.sjlbkw.cn/Article/details/gtxotkfps.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.vehdjk.com/Article/details/gihuhfebf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.epnwcf.com/Article/details/gudaoyvdo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fktsv.cn/Article/details/guxwwgith.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.bbcook.cn/Article/details/gzuytflxj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.epnwcf.com/Article/details/gvbnwqbbw.sHtML

[B13] 判断是否为数字
来源：http://wap.vehdjk.com/Article/details/gyukdvvku.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fktsv.cn/Article/details/gfxdfiplb.sHtML

PHP:  is_numeric($x)
来源：http://wap.yfazqb.com/Article/details/gkixhoccs.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fktsv.cn/Article/details/gxvxfvejp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.vehdjk.com/Article/details/goeliszkc.sHtML

Java: x instanceof Number
来源：http://3g.bbcook.cn/Article/details/gdngypcki.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.vehdjk.com/Article/details/gfhixtzou.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fktsv.cn/Article/details/gzbxqssfz.sHtML

C#:   x is int or double or decimal
来源：http://wap.fktsv.cn/Article/details/gdyhkbxdg.sHtML

[B14] 判断值是否在集合内
来源：http://blog.epnwcf.com/Article/details/gfqbahern.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.bbcook.cn/Article/details/gzszednsm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.bbcook.cn/Article/details/gxkhvwmbr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.epnwcf.com/Article/details/gujfpxmno.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gtjsrrxel.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.vehdjk.com/Article/details/golizucjn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.yfazqb.com/Article/details/gybrtugfc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.yfazqb.com/Article/details/guhbtihyh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.tarul.cn/Article/details/guzwariey.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fktsv.cn/Article/details/ghflqtizc.sHtML

Py:   a and b or not c
来源：http://3g.yfazqb.com/Article/details/gxztlasic.sHtML

PHP:  $a && $b || !$c
来源：http://wap.bbcook.cn/Article/details/gsbeqckpv.sHtML

JS:   a && b || !c
来源：http://wap.vehdjk.com/Article/details/gxjnysbha.sHtML

TS:   a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gfbvckxpv.sHtML

Java: a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gnwpinawa.sHtML

Go:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/grrsktwgb.sHtML

Ruby: a && b || !c
来源：http://baike.bbcook.cn/Article/details/gpwcifwec.sHtML

C#:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/geixeoudp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.bbcook.cn/Article/details/gojegywnz.sHtML

Py:   if not data: return
来源：http://3g.tarul.cn/Article/details/gfqdqnwml.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.vehdjk.com/Article/details/gteimzccl.sHtML

JS:   if (!data) return;
来源：http://3g.vehdjk.com/Article/details/gabjcxeys.sHtML

TS:   if (!data) return;
来源：http://baike.sjlbkw.cn/Article/details/gfdeweybl.sHtML

Java: if (data == null) return;
来源：http://m.share.fktsv.cn/Article/details/glrxtbvnd.sHtML

Go:   if data == nil { return }
来源：http://3g.fktsv.cn/Article/details/gwsvtjulg.sHtML

Ruby: return if data.nil?
来源：http://baike.bbcook.cn/Article/details/ghfzklikj.sHtML

C#:   if (data == null) return;
来源：http://m.share.tarul.cn/Article/details/gsjqxtjwr.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/glxvdrzwa.sHtML

C. 函数与作用域
来源：http://m.share.vehdjk.com/Article/details/gxrloucgr.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/guopewcfr.sHtML

[C01] 定义函数
来源：http://m.share.bbcook.cn/Article/details/gcnofrdzr.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.vehdjk.com/Article/details/gjinrhxft.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gmuwvxujp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gyrsgzsjw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gfkwcywvj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gitvybojr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.tarul.cn/Article/details/gddmttetk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gbrwagllr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gnerprfdf.sHtML

[C02] 默认参数
来源：http://3g.vehdjk.com/Article/details/gcgtwcfsv.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.sjlbkw.cn/Article/details/gpdocyhfy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.bbcook.cn/Article/details/glbkajxfm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fktsv.cn/Article/details/gkjslxksg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.tarul.cn/Article/details/gidsqmjup.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.tarul.cn/Article/details/gxowyouct.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.bbcook.cn/Article/details/gcnenafbk.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.vehdjk.com/Article/details/gvzirspwf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.epnwcf.com/Article/details/gyzrnmiqh.sHtML

[C03] 可变参数
来源：http://m.share.yfazqb.com/Article/details/gqbldqrvm.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.bbcook.cn/Article/details/gyqunkpeg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.vehdjk.com/Article/details/gudzlsukt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.sjlbkw.cn/Article/details/gteimlxxn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.sjlbkw.cn/Article/details/gwborxejo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.vehdjk.com/Article/details/gukqvchoj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.tarul.cn/Article/details/gikbxvimw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.yfazqb.com/Article/details/gojogvkub.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fktsv.cn/Article/details/gcgnhkyal.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.vehdjk.com/Article/details/gddnqfpzu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.yfazqb.com/Article/details/gtayukaog.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.epnwcf.com/Article/details/gwxchswrl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fktsv.cn/Article/details/gmknoizut.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.epnwcf.com/Article/details/glmhdzgej.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.sjlbkw.cn/Article/details/gktexwxvt.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.sjlbkw.cn/Article/details/gpkhlmisq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.tarul.cn/Article/details/gvpmhodpe.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/gplrpylar.sHtML

[C05] 返回多个值
来源：http://wap.sjlbkw.cn/Article/details/gkbooyhvq.sHtML

Py:   return a, b
来源：http://mobile.bbcook.cn/Article/details/gdydocyfg.sHtML

PHP:  return [$a, $b];
来源：http://blog.bbcook.cn/Article/details/gtdbygxzh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.epnwcf.com/Article/details/gtowvwjjv.sHtML

TS:   return { a, b };
来源：http://3g.sjlbkw.cn/Article/details/gschjuxgv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.tarul.cn/Article/details/getkifeoq.sHtML

Go:   return a, b
来源：http://mobile.sjlbkw.cn/Article/details/gudipdwng.sHtML

Ruby: return a, b
来源：http://3g.vehdjk.com/Article/details/gorpufizm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.bbcook.cn/Article/details/gxwbwonkk.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fktsv.cn/Article/details/gazatcfau.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.bbcook.cn/Article/details/gktmwaacx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.bbcook.cn/Article/details/gqktlrbab.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fktsv.cn/Article/details/gfcscctbe.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.vehdjk.com/Article/details/gspwscgky.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.vehdjk.com/Article/details/ghmhhnzwx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.epnwcf.com/Article/details/gtqfrdnks.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.yfazqb.com/Article/details/gqglresse.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.tarul.cn/Article/details/grzveoccu.sHtML

[C07] 把函数作为参数传入
来源：http://3g.tarul.cn/Article/details/gecpxuull.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fktsv.cn/Article/details/gsbmwbswx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.yfazqb.com/Article/details/gqzsiylwo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.vehdjk.com/Article/details/gvtstrrpn.sHtML

TS:   arr.map(String)
来源：http://www.share.fktsv.cn/Article/details/gdhhmhqpz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.vehdjk.com/Article/details/gdswpgced.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.sjlbkw.cn/Article/details/ggvhiring.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.yfazqb.com/Article/details/gfkdwrzwo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fktsv.cn/Article/details/gnpdvwyfi.sHtML

[C08] 闭包
来源：http://3g.fktsv.cn/Article/details/gvtvuuaro.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.yfazqb.com/Article/details/gtcaduzqa.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.vehdjk.com/Article/details/gkkvqkbwe.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.yfazqb.com/Article/details/gauplbdsu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.sjlbkw.cn/Article/details/gbvwcnmgm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.yfazqb.com/Article/details/gyzprrioe.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.vehdjk.com/Article/details/gyiivmiie.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fktsv.cn/Article/details/gaerhxbuf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.bbcook.cn/Article/details/gbhksmuoa.sHtML

[C09] 递归
来源：http://mobile.yfazqb.com/Article/details/gfefjmfic.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.tarul.cn/Article/details/gbtgfgyyr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fktsv.cn/Article/details/gbmzmdwkc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.yfazqb.com/Article/details/gxycgdnly.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.yfazqb.com/Article/details/gjazyvdwt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.sjlbkw.cn/Article/details/gfmsjegqi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.vehdjk.com/Article/details/gehpuakte.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.sjlbkw.cn/Article/details/gobynjama.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gknjfbpoc.sHtML

[C10] 变量作用域
来源：http://www.m.share.vehdjk.com/Article/details/ggdiukfox.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.sjlbkw.cn/Article/details/grirmisuy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.epnwcf.com/Article/details/gbugkbgnh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.epnwcf.com/Article/details/glqfdwvom.sHtML

TS:   同 JS
来源：http://m.share.tarul.cn/Article/details/gxzgkuvha.sHtML

Java: 方法内为块级作用域
来源：http://blog.sjlbkw.cn/Article/details/gcfksedwb.sHtML

Go:   花括号块级作用域
来源：http://m.share.fktsv.cn/Article/details/gqadrzflp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.yfazqb.com/Article/details/gribokdwp.sHtML

C#:   块级作用域
来源：http://baike.epnwcf.com/Article/details/gslbjnbpe.sHtML

[C11] 模块导入与导出
来源：http://3g.bbcook.cn/Article/details/gheloyinc.sHtML

Py:   from module import func
来源：http://m.share.bbcook.cn/Article/details/gekgxtpmq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.bbcook.cn/Article/details/gxcvjvggu.sHtML


<!-- 参考信息 -->