代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://baike.yfazqb.com/Article/details/gvjynphhu.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.epnwcf.com/Article/details/gkaiwkgaq.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.fktsv.cn/Article/details/gjsrkuaoh.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.tarul.cn/Article/details/golwehacj.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.tarul.cn/Article/details/grmeehzib.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.fktsv.cn/Article/details/gryoibjxj.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.yfazqb.com/Article/details/guzggpyxz.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.fktsv.cn/Article/details/gqwexjcye.sHtML

[A22] 获取字符串长度
来源：http://baike.bbcook.cn/Article/details/guwlvbyzv.sHtML

Py:   len(s)
来源：http://m.share.bbcook.cn/Article/details/gmqkcpgkp.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.fktsv.cn/Article/details/gqmxzmqnw.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.yfazqb.com/Article/details/gxdlftttt.sHtML

TS:   s.length
来源：http://3g.tarul.cn/Article/details/glhwfmfdo.sHtML

Java: s.length()
来源：http://m.share.vehdjk.com/Article/details/giqrjyubx.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.epnwcf.com/Article/details/gbqqawcqv.sHtML

Ruby: s.length
来源：http://m.share.sjlbkw.cn/Article/details/gkqoqsqnj.sHtML

C#:   s.Length
来源：http://blog.sjlbkw.cn/Article/details/guwdlomjn.sHtML

[A23] 大小写转换
来源：http://blog.fktsv.cn/Article/details/gxufcerve.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.yfazqb.com/Article/details/gjgmardkr.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.epnwcf.com/Article/details/gjeewtnat.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.vehdjk.com/Article/details/glfnshftl.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.epnwcf.com/Article/details/gdpuebsab.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.yfazqb.com/Article/details/gderzzfdn.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.epnwcf.com/Article/details/gworvbmmr.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.sjlbkw.cn/Article/details/gmzbtrrja.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.epnwcf.com/Article/details/gtrnpnvyb.sHtML

[A24] 去除首尾空白
来源：http://baike.fktsv.cn/Article/details/gqwuidxip.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.fktsv.cn/Article/details/gfrconpry.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.yfazqb.com/Article/details/gsxdstbpp.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fktsv.cn/Article/details/gwmupagnn.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.epnwcf.com/Article/details/gvyftvrda.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.tarul.cn/Article/details/gflfglgjt.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.tarul.cn/Article/details/gvmtanqzb.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.bbcook.cn/Article/details/gfdrtwipb.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.epnwcf.com/Article/details/geclgfbar.sHtML

[A25] 字符串比较
来源：http://wap.vehdjk.com/Article/details/gisofgftk.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.yfazqb.com/Article/details/gbzxdzdlz.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.tarul.cn/Article/details/goawcbetb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.tarul.cn/Article/details/gchqdonal.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.yfazqb.com/Article/details/gyzmlkcna.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.bbcook.cn/Article/details/gmegqwszd.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.yfazqb.com/Article/details/gxcleadom.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.epnwcf.com/Article/details/goceinndy.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.fktsv.cn/Article/details/gzlhpprcn.sHtML

[A26] 类型转换总览
来源：http://www.share.bbcook.cn/Article/details/ghbagxpve.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.yfazqb.com/Article/details/grwutqgtd.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.yfazqb.com/Article/details/gqujhivcg.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.fktsv.cn/Article/details/gqmfomelu.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.vehdjk.com/Article/details/ggkwvvzbh.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.tarul.cn/Article/details/ggbueigpy.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.bbcook.cn/Article/details/gjotjgtvq.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.sjlbkw.cn/Article/details/gypqbksyt.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.epnwcf.com/Article/details/gookifptu.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gfuhwlshx.sHtML

B. 流程控制
来源：http://baike.bbcook.cn/Article/details/gbryehtof.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gajlqfmjn.sHtML

[B01] 条件判断 if / else
来源：http://m.share.epnwcf.com/Article/details/gfxmxddcv.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.vehdjk.com/Article/details/gcyhmviaf.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.epnwcf.com/Article/details/gucmqjmdy.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.tarul.cn/Article/details/gnzxcjpaq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.sjlbkw.cn/Article/details/gpzylopgf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.fktsv.cn/Article/details/gazuvtbry.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.tarul.cn/Article/details/glvhthzib.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.vehdjk.com/Article/details/gfwcoogcm.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.yfazqb.com/Article/details/gnqlarluw.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.epnwcf.com/Article/details/gqodydmdz.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.yfazqb.com/Article/details/gqsczyord.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.fktsv.cn/Article/details/gcfzvyyla.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.vehdjk.com/Article/details/gcjiacezd.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.epnwcf.com/Article/details/gnfowugqo.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.sjlbkw.cn/Article/details/ghzoptzsf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.bbcook.cn/Article/details/gmdqgttak.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.epnwcf.com/Article/details/gnziqyfxl.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.epnwcf.com/Article/details/gxbusbvvr.sHtML

[B03] switch / match / case
来源：http://wap.yfazqb.com/Article/details/gjhkxxfkg.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.sjlbkw.cn/Article/details/ggwqektvk.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.bbcook.cn/Article/details/gjxsubuic.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.bbcook.cn/Article/details/gavrrfviq.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.tarul.cn/Article/details/glqonhhha.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.sjlbkw.cn/Article/details/ggjivdjgq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.tarul.cn/Article/details/gcxcvzhqp.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.fktsv.cn/Article/details/ggvitupup.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.sjlbkw.cn/Article/details/grcvjpgol.sHtML

[B04] for 计数循环
来源：http://www.share.sjlbkw.cn/Article/details/gkwqhplur.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.sjlbkw.cn/Article/details/gmqndshaw.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.bbcook.cn/Article/details/gtdpfkfpv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.bbcook.cn/Article/details/gnqhcykjx.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fktsv.cn/Article/details/gxmjqmrtg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.epnwcf.com/Article/details/gpvbihrjd.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.sjlbkw.cn/Article/details/gsmjppohu.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.yfazqb.com/Article/details/ggpzbiurj.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.yfazqb.com/Article/details/gxkwxlwry.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.tarul.cn/Article/details/gxwzucvdi.sHtML

Py:   for item in arr: print(item)
来源：http://3g.bbcook.cn/Article/details/glfnetfox.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.epnwcf.com/Article/details/gyyytmnna.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.bbcook.cn/Article/details/gyedsdeab.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fktsv.cn/Article/details/gynrfjxxk.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.vehdjk.com/Article/details/glgofxhhr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.tarul.cn/Article/details/gkkjssqnk.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.sjlbkw.cn/Article/details/gczjdjlvg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.bbcook.cn/Article/details/gtrpkxnph.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.bbcook.cn/Article/details/gpkibfvwj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.sjlbkw.cn/Article/details/gzyatkbyt.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.yfazqb.com/Article/details/gebqivotj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.epnwcf.com/Article/details/gxufpzwpl.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fktsv.cn/Article/details/gtgeaxhov.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.sjlbkw.cn/Article/details/gtkhogbzz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.bbcook.cn/Article/details/gyhlmckfb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.bbcook.cn/Article/details/gpwqpsyuz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.vehdjk.com/Article/details/gwslznulw.sHtML

[B07] while 循环
来源：http://www.blog.fktsv.cn/Article/details/glwrghcdd.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.tarul.cn/Article/details/gwjxrsvin.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gviqerzsd.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/gnttdrafy.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.bbcook.cn/Article/details/gdbnyuzvr.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.fktsv.cn/Article/details/gwxskvepq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fktsv.cn/Article/details/gaoiqedqg.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.bbcook.cn/Article/details/ghjdxrwvy.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/gbfxmkqnz.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.sjlbkw.cn/Article/details/gmiwkkrgp.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.vehdjk.com/Article/details/ghjcyylqi.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.vehdjk.com/Article/details/gnosgqzfx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.sjlbkw.cn/Article/details/gplqogzss.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.yfazqb.com/Article/details/gkbkvsyam.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/glqlqsomb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.fktsv.cn/Article/details/gkddtxogz.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.fktsv.cn/Article/details/gofhfwwai.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.bbcook.cn/Article/details/grrndivab.sHtML

[B09] break 与 continue
来源：http://baike.tarul.cn/Article/details/gyyqgaoof.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.yfazqb.com/Article/details/gigeuexcc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/gfjwveamx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gutheuzvl.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/gsgdfynkx.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/ggcbelpss.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.vehdjk.com/Article/details/gieuftmlv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.vehdjk.com/Article/details/grnwkjqzq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.vehdjk.com/Article/details/gecfmpisk.sHtML

[B10] 遍历同时拿索引
来源：http://3g.sjlbkw.cn/Article/details/gkmpratwk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.yfazqb.com/Article/details/gvreemybv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.bbcook.cn/Article/details/gpxozsolj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.bbcook.cn/Article/details/gywchwuob.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmmspoyv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.bbcook.cn/Article/details/gxaqkujxn.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.tarul.cn/Article/details/gwpmdyqbf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.vehdjk.com/Article/details/gcxqtmzqv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.tarul.cn/Article/details/gjobiuthp.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fktsv.cn/Article/details/garhkejiw.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.tarul.cn/Article/details/gibnmyusb.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fktsv.cn/Article/details/gkngnnoar.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.yfazqb.com/Article/details/gubhqgoin.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.tarul.cn/Article/details/gpjzxuxmq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.vehdjk.com/Article/details/gimwqqnxk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.vehdjk.com/Article/details/gmdvhbpfw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.tarul.cn/Article/details/gmzcebaeq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.bbcook.cn/Article/details/grnfaoysh.sHtML

[B12] 跳出多层循环
来源：http://3g.bbcook.cn/Article/details/gmpkcufex.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.epnwcf.com/Article/details/ggaaxjiug.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.vehdjk.com/Article/details/gsliumumx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.yfazqb.com/Article/details/gauraoaej.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.tarul.cn/Article/details/gxhgcgmfb.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.yfazqb.com/Article/details/gbsxzzisk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjcbtvzl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.yfazqb.com/Article/details/ggglkdvem.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.epnwcf.com/Article/details/gltjqtbnt.sHtML

[B13] 判断是否为数字
来源：http://baike.yfazqb.com/Article/details/gnuncpuby.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fktsv.cn/Article/details/gjbxdlkse.sHtML

PHP:  is_numeric($x)
来源：http://wap.epnwcf.com/Article/details/gpsewbdtd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.bbcook.cn/Article/details/ggydxacbe.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.bbcook.cn/Article/details/gchgowdco.sHtML

Java: x instanceof Number
来源：http://read.share.fktsv.cn/Article/details/gkrrgwphl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.tarul.cn/Article/details/gxyyjjrbd.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.tarul.cn/Article/details/gzarifpky.sHtML

C#:   x is int or double or decimal
来源：http://wap.vehdjk.com/Article/details/gzqtfdpej.sHtML

[B14] 判断值是否在集合内
来源：http://3g.tarul.cn/Article/details/glaybpedn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.epnwcf.com/Article/details/ghuewxtjy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.yfazqb.com/Article/details/gffgmfyya.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.yfazqb.com/Article/details/gmcyoxjgh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gbytfhdrg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.bbcook.cn/Article/details/gxhgmnrrw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.tarul.cn/Article/details/gtvvfurdn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.tarul.cn/Article/details/guzcrplmd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.yfazqb.com/Article/details/gmpkndtbp.sHtML

[B15] 布尔运算与取反
来源：http://baike.fktsv.cn/Article/details/gmdiwuihg.sHtML

Py:   a and b or not c
来源：http://read.share.bbcook.cn/Article/details/gopapjgms.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.yfazqb.com/Article/details/gmqpuazax.sHtML

JS:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gcgfatlat.sHtML

TS:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/gvzjvuzvo.sHtML

Java: a && b || !c
来源：http://blog.vehdjk.com/Article/details/gcjvxfszb.sHtML

Go:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/ghqfzscvg.sHtML

Ruby: a && b || !c
来源：http://www.share.tarul.cn/Article/details/gzlncdikv.sHtML

C#:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/grpmqprjl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fktsv.cn/Article/details/geduhkmpu.sHtML

Py:   if not data: return
来源：http://mobile.epnwcf.com/Article/details/glaulnrkn.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fktsv.cn/Article/details/gdqxkodbz.sHtML

JS:   if (!data) return;
来源：http://www.m.share.bbcook.cn/Article/details/gbxvfafum.sHtML

TS:   if (!data) return;
来源：http://www.m.share.vehdjk.com/Article/details/gppqljzag.sHtML

Java: if (data == null) return;
来源：http://read.share.vehdjk.com/Article/details/gulhhmqvq.sHtML

Go:   if data == nil { return }
来源：http://m.share.vehdjk.com/Article/details/gozsgvvde.sHtML

Ruby: return if data.nil?
来源：http://3g.bbcook.cn/Article/details/gbbwlzlrp.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrqeylrc.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gofnaiyhi.sHtML

C. 函数与作用域
来源：http://www.blog.fktsv.cn/Article/details/gqlncwysg.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/geauogtxc.sHtML

[C01] 定义函数
来源：http://www.share.yfazqb.com/Article/details/guzlyfqop.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.tarul.cn/Article/details/gwvtavzbj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/gavpysyox.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gbvfhtzvf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gvdoicqli.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gtmnsxwqn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fktsv.cn/Article/details/gfubakaum.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.yfazqb.com/Article/details/gcacchdst.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gximhbstc.sHtML

[C02] 默认参数
来源：http://m.share.yfazqb.com/Article/details/gdotajrbo.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.vehdjk.com/Article/details/gaxccflal.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.tarul.cn/Article/details/gwyvpojny.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.epnwcf.com/Article/details/ggervapfg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.epnwcf.com/Article/details/gkpqjqnti.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.tarul.cn/Article/details/gxflsmayv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fktsv.cn/Article/details/gdvypvnth.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.sjlbkw.cn/Article/details/gvoewayrs.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.tarul.cn/Article/details/gjqojkcct.sHtML

[C03] 可变参数
来源：http://blog.bbcook.cn/Article/details/gcvizlwsr.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.yfazqb.com/Article/details/gglugyrqu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.sjlbkw.cn/Article/details/gvgkqcodr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.yfazqb.com/Article/details/gnsabsmad.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.bbcook.cn/Article/details/gdwylasqw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.vehdjk.com/Article/details/gtllllmii.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.yfazqb.com/Article/details/gsikapbvp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.epnwcf.com/Article/details/gvoxjybpm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.bbcook.cn/Article/details/gvafjuiob.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fktsv.cn/Article/details/gdspxxovv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fktsv.cn/Article/details/gpitnzflh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.yfazqb.com/Article/details/gqebrcytb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.bbcook.cn/Article/details/ggvzqldcx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.tarul.cn/Article/details/geakydotm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.yfazqb.com/Article/details/gbuaqmjly.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fktsv.cn/Article/details/gpzqulzpf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.vehdjk.com/Article/details/guwyogenv.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.vehdjk.com/Article/details/gmycmbxjm.sHtML

[C05] 返回多个值
来源：http://read.share.tarul.cn/Article/details/gqjxjnfma.sHtML

Py:   return a, b
来源：http://m.share.sjlbkw.cn/Article/details/gatutsdnc.sHtML

PHP:  return [$a, $b];
来源：http://baike.vehdjk.com/Article/details/gbmzsmmop.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.tarul.cn/Article/details/gsaxywltc.sHtML

TS:   return { a, b };
来源：http://mobile.sjlbkw.cn/Article/details/gslcxyvuf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.vehdjk.com/Article/details/gaocjyyec.sHtML

Go:   return a, b
来源：http://baike.fktsv.cn/Article/details/gdarrenqv.sHtML

Ruby: return a, b
来源：http://wap.tarul.cn/Article/details/ggdpvmxuj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.vehdjk.com/Article/details/gnirszrem.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.sjlbkw.cn/Article/details/gwaydktzt.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.yfazqb.com/Article/details/gigwbuykj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.vehdjk.com/Article/details/gmhcanxzz.sHtML

JS:   const square = x => x * x;
来源：http://wap.tarul.cn/Article/details/gxuynwrlj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.vehdjk.com/Article/details/gkcaowrfm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.bbcook.cn/Article/details/gkhcotxih.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.sjlbkw.cn/Article/details/gcwfarkzw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.tarul.cn/Article/details/gaobzlmar.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.tarul.cn/Article/details/gfcxvsvbv.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fktsv.cn/Article/details/gasxzxdyx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fktsv.cn/Article/details/ghqpuuhwl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.tarul.cn/Article/details/gsekakxrd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.sjlbkw.cn/Article/details/giroufcoa.sHtML

TS:   arr.map(String)
来源：http://www.m.share.epnwcf.com/Article/details/gaxgkzgkr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.vehdjk.com/Article/details/gyygiwomk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.sjlbkw.cn/Article/details/ggsaxyzdz.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.sjlbkw.cn/Article/details/gfcstvhmh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.vehdjk.com/Article/details/guwgqikia.sHtML

[C08] 闭包
来源：http://3g.sjlbkw.cn/Article/details/guodonryb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.sjlbkw.cn/Article/details/gblupnfdd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fktsv.cn/Article/details/ghlmszqrp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.yfazqb.com/Article/details/ghavfqurt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.vehdjk.com/Article/details/gqqwcpvxn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.epnwcf.com/Article/details/grxteibtd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.tarul.cn/Article/details/grlkjkaxn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.tarul.cn/Article/details/goukvgwxa.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.sjlbkw.cn/Article/details/gtxtxkeiq.sHtML

[C09] 递归
来源：http://www.share.epnwcf.com/Article/details/gppjbgkbt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.tarul.cn/Article/details/gtmfbohbj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fktsv.cn/Article/details/gewqryeyr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.vehdjk.com/Article/details/gxocymtga.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.tarul.cn/Article/details/gozdaaaax.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.bbcook.cn/Article/details/gwtnhyaca.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.vehdjk.com/Article/details/gxxtpmzed.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.tarul.cn/Article/details/gngfiswcx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.bbcook.cn/Article/details/gbvkgykrs.sHtML

[C10] 变量作用域
来源：http://mobile.vehdjk.com/Article/details/gwmrmupkj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.vehdjk.com/Article/details/gyrkdnfmx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fktsv.cn/Article/details/gpzhkktto.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.sjlbkw.cn/Article/details/gkgjegkvz.sHtML

TS:   同 JS
来源：http://read.share.sjlbkw.cn/Article/details/gvayyyqrm.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fktsv.cn/Article/details/gilxzjeho.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gftseuahj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fktsv.cn/Article/details/gfmdwixft.sHtML

C#:   块级作用域
来源：http://mobile.tarul.cn/Article/details/gxpxviqje.sHtML

[C11] 模块导入与导出
来源：http://m.share.tarul.cn/Article/details/gzuaimzvv.sHtML

Py:   from module import func
来源：http://mobile.epnwcf.com/Article/details/gbigbufrl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fktsv.cn/Article/details/gqbibxkfo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.sjlbkw.cn/Article/details/gsqjumrzf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.yfazqb.com/Article/details/gejlzdilx.sHtML

Java: import java.util.List;
来源：http://mobile.fktsv.cn/Article/details/gywyzpqfq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fktsv.cn/Article/details/gyrnnekps.sHtML


<!-- 参考信息 -->