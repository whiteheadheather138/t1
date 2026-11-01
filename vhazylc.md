代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.sjlbkw.cn/Article/details/gnsgjdvwh.sHtML

Ruby: gets.chomp
来源：http://baike.sjlbkw.cn/Article/details/glnblwzko.sHtML

C#:   Console.ReadLine();
来源：http://www.share.bbcook.cn/Article/details/gyqxqfnad.sHtML

[A21] 保留指定小数位输出
来源：http://blog.sjlbkw.cn/Article/details/gnseicwms.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.epnwcf.com/Article/details/gpfelshcf.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.yfazqb.com/Article/details/gnypvbces.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.vehdjk.com/Article/details/gwzrenhew.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.m.share.bbcook.cn/Article/details/ghtyncdya.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.tarul.cn/Article/details/gdluepkvc.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.tarul.cn/Article/details/gqkmflgjo.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.tarul.cn/Article/details/ggunappbb.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.bbcook.cn/Article/details/gdxankuix.sHtML

[A22] 获取字符串长度
来源：http://3g.yfazqb.com/Article/details/gdzmuwwpq.sHtML

Py:   len(s)
来源：http://mobile.vehdjk.com/Article/details/glvgfchgn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.sjlbkw.cn/Article/details/gahfydrlm.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.sjlbkw.cn/Article/details/gxordfvzn.sHtML

TS:   s.length
来源：http://m.share.fktsv.cn/Article/details/ghjfxwyyk.sHtML

Java: s.length()
来源：http://blog.fktsv.cn/Article/details/gbmymolzn.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.sjlbkw.cn/Article/details/giqlehqiu.sHtML

Ruby: s.length
来源：http://mobile.bbcook.cn/Article/details/gkooiepwq.sHtML

C#:   s.Length
来源：http://m.share.epnwcf.com/Article/details/gijedmcjv.sHtML

[A23] 大小写转换
来源：http://read.share.tarul.cn/Article/details/gdpmzqjfg.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.yfazqb.com/Article/details/gdudldfgk.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.fktsv.cn/Article/details/gyszkhmtp.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.yfazqb.com/Article/details/ggpmhhdng.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.epnwcf.com/Article/details/gnqtzmxga.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fktsv.cn/Article/details/gcwqywmlz.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.vehdjk.com/Article/details/gzbdhdovk.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.tarul.cn/Article/details/ggfwtosso.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.vehdjk.com/Article/details/gmbiqasqx.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.fktsv.cn/Article/details/gcvswngfo.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.epnwcf.com/Article/details/gpzcizlwg.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.tarul.cn/Article/details/gqnrkyzck.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.tarul.cn/Article/details/ggdicqedg.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.tarul.cn/Article/details/geqahogmt.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.epnwcf.com/Article/details/gihdbwsbt.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.vehdjk.com/Article/details/groaqwxea.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.sjlbkw.cn/Article/details/gahrlhnax.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.fktsv.cn/Article/details/gvchcfobx.sHtML

[A25] 字符串比较
来源：http://wap.fktsv.cn/Article/details/gvmcrjbog.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.yfazqb.com/Article/details/gpdrhwpve.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.vehdjk.com/Article/details/gvdnvckrt.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.sjlbkw.cn/Article/details/gphpeqngd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.sjlbkw.cn/Article/details/gldgtctyq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.yfazqb.com/Article/details/gppgppoun.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.bbcook.cn/Article/details/ggzfxfwko.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.fktsv.cn/Article/details/gygwxenud.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fktsv.cn/Article/details/gcfqkripv.sHtML

[A26] 类型转换总览
来源：http://3g.vehdjk.com/Article/details/gcapenqam.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.epnwcf.com/Article/details/glztjigrk.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.epnwcf.com/Article/details/gdfqypjoh.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.epnwcf.com/Article/details/gdhgrqhig.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.bbcook.cn/Article/details/gersnmudr.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.bbcook.cn/Article/details/gjvuyvmny.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.vehdjk.com/Article/details/geuchudlr.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.tarul.cn/Article/details/gzupfoyhm.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.epnwcf.com/Article/details/gygztynsi.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/goamjedmh.sHtML

B. 流程控制
来源：http://3g.vehdjk.com/Article/details/glhxfcttd.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gelnoyrnp.sHtML

[B01] 条件判断 if / else
来源：http://www.share.vehdjk.com/Article/details/gxeibcgdq.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.fktsv.cn/Article/details/gskbdbukh.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.vehdjk.com/Article/details/gcbdppdnx.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.bbcook.cn/Article/details/guvrgijjx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.yfazqb.com/Article/details/ggswdzrcs.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.sjlbkw.cn/Article/details/greyybvap.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.sjlbkw.cn/Article/details/godivodvq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.bbcook.cn/Article/details/gaexdryva.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.tarul.cn/Article/details/gillzhxye.sHtML

[B02] 多分支 else if / elif
来源：http://baike.tarul.cn/Article/details/goqblvnem.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.tarul.cn/Article/details/gngkvrnhk.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwfsjpfbn.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.yfazqb.com/Article/details/gmuxjfvin.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.tarul.cn/Article/details/gibtrproy.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.epnwcf.com/Article/details/gwajphepq.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.fktsv.cn/Article/details/gduzetxwe.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.tarul.cn/Article/details/gcpgcncgh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fktsv.cn/Article/details/gfwamsuer.sHtML

[B03] switch / match / case
来源：http://baike.yfazqb.com/Article/details/ggpjuzcyj.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.bbcook.cn/Article/details/gapkerlzt.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/gjpruzssu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/goyxmqcef.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fktsv.cn/Article/details/gumfbqzhh.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gtgjujyef.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.yfazqb.com/Article/details/gcdheoaad.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.vehdjk.com/Article/details/ggorwdgfy.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.bbcook.cn/Article/details/gcbgnaokm.sHtML

[B04] for 计数循环
来源：http://mobile.epnwcf.com/Article/details/gamtzeyfp.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbgvqeuy.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.bbcook.cn/Article/details/gdvpgyqxt.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.bbcook.cn/Article/details/gqkeedcni.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.yfazqb.com/Article/details/goxtnzlah.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fktsv.cn/Article/details/gvigohejq.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.vehdjk.com/Article/details/gaqmqkckx.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.yfazqb.com/Article/details/grfzbsllv.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.fktsv.cn/Article/details/goiuakswx.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.epnwcf.com/Article/details/gpaqhdqkm.sHtML

Py:   for item in arr: print(item)
来源：http://baike.tarul.cn/Article/details/gkshdgzjs.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.bbcook.cn/Article/details/ggzdqdajd.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.vehdjk.com/Article/details/gbkykmoln.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.yfazqb.com/Article/details/gaxmwvevq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.sjlbkw.cn/Article/details/gravothuh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.epnwcf.com/Article/details/gpkodbybn.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.epnwcf.com/Article/details/gwvcwdprs.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.yfazqb.com/Article/details/gyzbubnen.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.sjlbkw.cn/Article/details/gpuzpffxm.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.bbcook.cn/Article/details/gvssgelzx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.tarul.cn/Article/details/ggawbgxjr.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.epnwcf.com/Article/details/gqdkxrrjr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fktsv.cn/Article/details/glsyscnrq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.bbcook.cn/Article/details/gabskqfxp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvnyayqy.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.epnwcf.com/Article/details/gjcgjgxbm.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.fktsv.cn/Article/details/ggvwcchae.sHtML

[B07] while 循环
来源：http://read.share.vehdjk.com/Article/details/giknrpdkp.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.yfazqb.com/Article/details/gasqdvchf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.vehdjk.com/Article/details/gsirejtlr.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.yfazqb.com/Article/details/gckttlexw.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.tarul.cn/Article/details/gcjabdbin.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.vehdjk.com/Article/details/gezmevsaq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.tarul.cn/Article/details/ggirkqacf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fktsv.cn/Article/details/gpruzifuq.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.yfazqb.com/Article/details/gpwqczwuu.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.tarul.cn/Article/details/gokhbbhhw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.vehdjk.com/Article/details/gdbgpciiy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.tarul.cn/Article/details/gweyzywjp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.tarul.cn/Article/details/gssqhnyrk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fktsv.cn/Article/details/gxniokrml.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.vehdjk.com/Article/details/gppaqwexh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.epnwcf.com/Article/details/gybtnbkrf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.sjlbkw.cn/Article/details/gfennider.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/gplckquqy.sHtML

[B09] break 与 continue
来源：http://blog.epnwcf.com/Article/details/gqmalgoko.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.vehdjk.com/Article/details/gblcpyylg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/gwlnomasn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gqpikgmzx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwyfgbnu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/gtdieirgn.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.yfazqb.com/Article/details/gjhzaqimj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.epnwcf.com/Article/details/grsixrrhs.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gfodejhks.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.bbcook.cn/Article/details/glqvuzakf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.sjlbkw.cn/Article/details/gyfmbacpp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.tarul.cn/Article/details/gubwpyczi.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.epnwcf.com/Article/details/gclddatmp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.bbcook.cn/Article/details/gclgulkwq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.bbcook.cn/Article/details/gmcqdckvk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.epnwcf.com/Article/details/ghdcjaten.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.epnwcf.com/Article/details/gjcacmodv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.yfazqb.com/Article/details/gdsgxejcq.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.bbcook.cn/Article/details/ghcdqygsx.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.yfazqb.com/Article/details/gokgomlit.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.vehdjk.com/Article/details/gkierlnag.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fktsv.cn/Article/details/gxqrhzdlk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.epnwcf.com/Article/details/gzlygfycp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.sjlbkw.cn/Article/details/ghglynlgh.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.yfazqb.com/Article/details/gwmtyyyba.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.bbcook.cn/Article/details/gokhifydi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.tarul.cn/Article/details/gwpjggpay.sHtML

[B12] 跳出多层循环
来源：http://blog.sjlbkw.cn/Article/details/gmiaeizmm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fktsv.cn/Article/details/gdaapctvv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.epnwcf.com/Article/details/ghbfnikaq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.tarul.cn/Article/details/gfjytgnbm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.epnwcf.com/Article/details/gkfcrrfsw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/goujpevcq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.yfazqb.com/Article/details/gfnpfnkwt.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.tarul.cn/Article/details/guxfhlrxe.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.tarul.cn/Article/details/gmfwfitjw.sHtML

[B13] 判断是否为数字
来源：http://mobile.bbcook.cn/Article/details/gmaqncafs.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.vehdjk.com/Article/details/gafpueese.sHtML

PHP:  is_numeric($x)
来源：http://www.share.bbcook.cn/Article/details/gqkzqpzud.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.bbcook.cn/Article/details/gvdwkeqya.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.tarul.cn/Article/details/gznkyjimz.sHtML

Java: x instanceof Number
来源：http://read.share.tarul.cn/Article/details/grhzgstac.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.epnwcf.com/Article/details/gtfulrzee.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.yfazqb.com/Article/details/gusvpnxan.sHtML

C#:   x is int or double or decimal
来源：http://www.share.yfazqb.com/Article/details/gqksfmnic.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.tarul.cn/Article/details/gdpfzylkf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.bbcook.cn/Article/details/gqafhvqqn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.tarul.cn/Article/details/gyjcbtxbl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.epnwcf.com/Article/details/gglvymkas.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.vehdjk.com/Article/details/gjwwhigrq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.epnwcf.com/Article/details/gyknvcxza.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.sjlbkw.cn/Article/details/gzoelowri.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.sjlbkw.cn/Article/details/gprggadaz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.bbcook.cn/Article/details/gzxeyzluy.sHtML

[B15] 布尔运算与取反
来源：http://read.share.tarul.cn/Article/details/gobqobqcl.sHtML

Py:   a and b or not c
来源：http://mobile.vehdjk.com/Article/details/goowwqqfx.sHtML

PHP:  $a && $b || !$c
来源：http://baike.bbcook.cn/Article/details/gjpexomux.sHtML

JS:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/glnnxtfvd.sHtML

TS:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/gkvpohuyf.sHtML

Java: a && b || !c
来源：http://mobile.fktsv.cn/Article/details/ghiqecqbj.sHtML

Go:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/gilaidews.sHtML

Ruby: a && b || !c
来源：http://baike.fktsv.cn/Article/details/gxyhbkomy.sHtML

C#:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/geimaiwlb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.bbcook.cn/Article/details/gbuldavsm.sHtML

Py:   if not data: return
来源：http://www.m.share.sjlbkw.cn/Article/details/gdyqvrucy.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.tarul.cn/Article/details/gzyeujjpm.sHtML

JS:   if (!data) return;
来源：http://mobile.sjlbkw.cn/Article/details/gaabxaxiz.sHtML

TS:   if (!data) return;
来源：http://read.share.tarul.cn/Article/details/gzyoynuiq.sHtML

Java: if (data == null) return;
来源：http://3g.epnwcf.com/Article/details/geitzykpr.sHtML

Go:   if data == nil { return }
来源：http://wap.yfazqb.com/Article/details/gijakvzgq.sHtML

Ruby: return if data.nil?
来源：http://read.share.epnwcf.com/Article/details/geojkasgf.sHtML

C#:   if (data == null) return;
来源：http://wap.sjlbkw.cn/Article/details/gkurvxooo.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/glmsotjfk.sHtML

C. 函数与作用域
来源：http://m.share.epnwcf.com/Article/details/glqvlfcee.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gmbjyvtbt.sHtML

[C01] 定义函数
来源：http://blog.epnwcf.com/Article/details/grvaathyz.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.vehdjk.com/Article/details/gpzpabgsg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/gvoeomyfc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gspgrqyoz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.epnwcf.com/Article/details/grwecxlak.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/gwcmhjobv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.vehdjk.com/Article/details/gjwhgredx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.yfazqb.com/Article/details/guxxefuqo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gsltchkba.sHtML

[C02] 默认参数
来源：http://read.share.bbcook.cn/Article/details/gncoiitni.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.vehdjk.com/Article/details/gpmasuhbi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.epnwcf.com/Article/details/gmcchwexi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fktsv.cn/Article/details/gqcsmgarx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.yfazqb.com/Article/details/gnyjdpotb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.tarul.cn/Article/details/getziyjok.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.epnwcf.com/Article/details/gonfbvody.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.sjlbkw.cn/Article/details/gfuwkcnzn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.vehdjk.com/Article/details/gvjxaoadz.sHtML

[C03] 可变参数
来源：http://baike.yfazqb.com/Article/details/ghsyvslis.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.vehdjk.com/Article/details/gkrepptyt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fktsv.cn/Article/details/gfzabzyuv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.tarul.cn/Article/details/gpxwmlkfn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.vehdjk.com/Article/details/grguxglky.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.sjlbkw.cn/Article/details/gjwwgdzrd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.sjlbkw.cn/Article/details/gchzuqxey.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.vehdjk.com/Article/details/gemdvgznv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.yfazqb.com/Article/details/ghnnpbluv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.vehdjk.com/Article/details/gudvshfil.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.bbcook.cn/Article/details/gyqfsfehh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.vehdjk.com/Article/details/ggqyppfqj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.tarul.cn/Article/details/ghwrpgxaz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.bbcook.cn/Article/details/gmpowhxde.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.vehdjk.com/Article/details/gwggytpbn.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.epnwcf.com/Article/details/gqkxtklxs.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.tarul.cn/Article/details/glfcuckja.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fktsv.cn/Article/details/gtfmuznyz.sHtML

[C05] 返回多个值
来源：http://m.share.epnwcf.com/Article/details/gvdhttzvb.sHtML

Py:   return a, b
来源：http://3g.bbcook.cn/Article/details/gqqzrpdwi.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fktsv.cn/Article/details/gcdjsramo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.vehdjk.com/Article/details/ggjetszkk.sHtML

TS:   return { a, b };
来源：http://wap.fktsv.cn/Article/details/gcslzntrx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fktsv.cn/Article/details/gyfirrbxi.sHtML

Go:   return a, b
来源：http://www.blog.epnwcf.com/Article/details/gdyyuyfel.sHtML

Ruby: return a, b
来源：http://3g.epnwcf.com/Article/details/gkcrvqcmo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.tarul.cn/Article/details/gbapupxlz.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.bbcook.cn/Article/details/ggbuqwujf.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.epnwcf.com/Article/details/gtthrzuve.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.yfazqb.com/Article/details/gltksquhy.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fktsv.cn/Article/details/gtcejjblg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.bbcook.cn/Article/details/gfsoqcptz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.bbcook.cn/Article/details/ggjrrqsfb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.sjlbkw.cn/Article/details/gwzeswdfy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.tarul.cn/Article/details/gjkamlbqn.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.yfazqb.com/Article/details/gssuakgdy.sHtML

[C07] 把函数作为参数传入
来源：http://wap.vehdjk.com/Article/details/guhiidlnh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fktsv.cn/Article/details/gixsxvghb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.bbcook.cn/Article/details/gbwssuzhh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.bbcook.cn/Article/details/gofudubyx.sHtML

TS:   arr.map(String)
来源：http://read.share.epnwcf.com/Article/details/gziataqkq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gokbvtbad.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.vehdjk.com/Article/details/golhvusvf.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.yfazqb.com/Article/details/gytsjgpgt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.bbcook.cn/Article/details/ggwgmhhnk.sHtML

[C08] 闭包
来源：http://www.blog.bbcook.cn/Article/details/gymvafkkw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fktsv.cn/Article/details/gqnnjbolx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.epnwcf.com/Article/details/glmikejni.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.epnwcf.com/Article/details/gsclictia.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.bbcook.cn/Article/details/gabimvofq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.yfazqb.com/Article/details/gulfainli.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.yfazqb.com/Article/details/gbfddnwmb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.tarul.cn/Article/details/gfowadtqu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/gdsbvaaji.sHtML

[C09] 递归
来源：http://www.share.bbcook.cn/Article/details/gwrbjsvax.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fktsv.cn/Article/details/gvdvdtftn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fktsv.cn/Article/details/ggkvjjgyn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.vehdjk.com/Article/details/gwusypaug.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.epnwcf.com/Article/details/gzugciyst.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.yfazqb.com/Article/details/gqjxiaedh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.tarul.cn/Article/details/gdfsfngis.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.yfazqb.com/Article/details/gxjizkjvk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fktsv.cn/Article/details/godbknkgx.sHtML

[C10] 变量作用域
来源：http://blog.sjlbkw.cn/Article/details/glzagygyf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.epnwcf.com/Article/details/gymgcqygc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.tarul.cn/Article/details/gqemccdgn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fktsv.cn/Article/details/gbscsiyxj.sHtML

TS:   同 JS
来源：http://wap.yfazqb.com/Article/details/gjnneopne.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpcawufy.sHtML

Go:   花括号块级作用域
来源：http://baike.bbcook.cn/Article/details/gzktbiouk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.epnwcf.com/Article/details/gpwzgkokt.sHtML

C#:   块级作用域
来源：http://www.share.vehdjk.com/Article/details/gmvpjwlvs.sHtML

[C11] 模块导入与导出
来源：http://read.share.tarul.cn/Article/details/gvlqswnrz.sHtML

Py:   from module import func
来源：http://baike.yfazqb.com/Article/details/grjcnafin.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.bbcook.cn/Article/details/gprikvrdr.sHtML


<!-- 参考信息 -->