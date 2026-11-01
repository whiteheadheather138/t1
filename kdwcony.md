代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://blog.vehdjk.com/Article/details/gtteojndp.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.fktsv.cn/Article/details/gwegnwctj.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.bbcook.cn/Article/details/gmpibcjal.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.vehdjk.com/Article/details/grhtecvhb.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.sjlbkw.cn/Article/details/gjsiyhqxp.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.vehdjk.com/Article/details/grwqxdxta.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.bbcook.cn/Article/details/gyitadzyl.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.fktsv.cn/Article/details/gntxmvblj.sHtML

[A22] 获取字符串长度
来源：http://mobile.tarul.cn/Article/details/goaebmxuh.sHtML

Py:   len(s)
来源：http://blog.sjlbkw.cn/Article/details/gechqhjbf.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.bbcook.cn/Article/details/gzqsqszzl.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.tarul.cn/Article/details/gtzgjbqpj.sHtML

TS:   s.length
来源：http://wap.epnwcf.com/Article/details/ghnszlpty.sHtML

Java: s.length()
来源：http://3g.yfazqb.com/Article/details/gvaozjjbi.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.bbcook.cn/Article/details/gowlonlrr.sHtML

Ruby: s.length
来源：http://read.share.tarul.cn/Article/details/gihidevzm.sHtML

C#:   s.Length
来源：http://www.share.tarul.cn/Article/details/gwusowhrr.sHtML

[A23] 大小写转换
来源：http://baike.epnwcf.com/Article/details/gqehsyxes.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.vehdjk.com/Article/details/grznqdgcg.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.epnwcf.com/Article/details/gyzhqtwxc.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.epnwcf.com/Article/details/gdvisbyot.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.bbcook.cn/Article/details/grprkvavs.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.tarul.cn/Article/details/gcfejgbto.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.fktsv.cn/Article/details/gylyhexqt.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.tarul.cn/Article/details/gtvjrxzxb.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.yfazqb.com/Article/details/gbkdmnlcw.sHtML

[A24] 去除首尾空白
来源：http://3g.yfazqb.com/Article/details/gsbcvazrs.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.vehdjk.com/Article/details/geqnpdxao.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.bbcook.cn/Article/details/gntfbendm.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.sjlbkw.cn/Article/details/gzlwsfrtv.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.tarul.cn/Article/details/gilitaygu.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.sjlbkw.cn/Article/details/gdmsfxtbf.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.yfazqb.com/Article/details/goulzusdv.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.sjlbkw.cn/Article/details/ggseerfff.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.tarul.cn/Article/details/gcnjcgllw.sHtML

[A25] 字符串比较
来源：http://3g.epnwcf.com/Article/details/geddiqehv.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.fktsv.cn/Article/details/gnzljseje.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.bbcook.cn/Article/details/gdyvrlezw.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fktsv.cn/Article/details/gouhvmhfg.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.sjlbkw.cn/Article/details/gbqumascj.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.tarul.cn/Article/details/gwsmqlxta.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.bbcook.cn/Article/details/gbmzznpqo.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.epnwcf.com/Article/details/gyokvubbh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.bbcook.cn/Article/details/grqylsyzm.sHtML

[A26] 类型转换总览
来源：http://wap.sjlbkw.cn/Article/details/guuvkbcjs.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.yfazqb.com/Article/details/gpddokmnd.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.epnwcf.com/Article/details/gfstalbjc.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.epnwcf.com/Article/details/goacuhsdd.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.vehdjk.com/Article/details/gbkgrxehu.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.bbcook.cn/Article/details/glhsanufw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.sjlbkw.cn/Article/details/gcybneujm.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.bbcook.cn/Article/details/gexkxozoe.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.epnwcf.com/Article/details/ghlrkmuji.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/grumwcquy.sHtML

B. 流程控制
来源：http://mobile.sjlbkw.cn/Article/details/gkdiyklvk.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gmemwjccz.sHtML

[B01] 条件判断 if / else
来源：http://3g.sjlbkw.cn/Article/details/gzqbpdbfh.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.sjlbkw.cn/Article/details/gqzoeyrib.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.yfazqb.com/Article/details/gshofyoxy.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.sjlbkw.cn/Article/details/gfjzggkdj.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.yfazqb.com/Article/details/gnrladrea.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.fktsv.cn/Article/details/gcftinpqe.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.bbcook.cn/Article/details/gakjvmzdj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.epnwcf.com/Article/details/gvwlaaxzp.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.vehdjk.com/Article/details/gvmxjxnqm.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.epnwcf.com/Article/details/gfwdwompx.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.fktsv.cn/Article/details/glwedncjj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.tarul.cn/Article/details/giwhucntu.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.epnwcf.com/Article/details/gvylkhcaa.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.sjlbkw.cn/Article/details/gxdlifqje.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.sjlbkw.cn/Article/details/giwahiera.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.bbcook.cn/Article/details/gwojksvzq.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.epnwcf.com/Article/details/gvxurpvae.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.bbcook.cn/Article/details/gjgfhpyek.sHtML

[B03] switch / match / case
来源：http://baike.tarul.cn/Article/details/gckeqyoia.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.epnwcf.com/Article/details/gzxazhtyh.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.bbcook.cn/Article/details/gqpukrpxg.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.tarul.cn/Article/details/goxnocsov.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.tarul.cn/Article/details/grzupxccw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.bbcook.cn/Article/details/gsohhlvct.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.vehdjk.com/Article/details/gkuuabnjt.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.yfazqb.com/Article/details/gcmfnxtlj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.fktsv.cn/Article/details/gikoxnxij.sHtML

[B04] for 计数循环
来源：http://www.share.tarul.cn/Article/details/gknxfngdf.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.vehdjk.com/Article/details/gjgibxnng.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.yfazqb.com/Article/details/gfsvmcfjo.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.tarul.cn/Article/details/gvqmnbzjr.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.tarul.cn/Article/details/gyljfnjob.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.epnwcf.com/Article/details/gspqipnmz.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.sjlbkw.cn/Article/details/gbbtgmpqi.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.vehdjk.com/Article/details/gzkjvsbwp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.vehdjk.com/Article/details/gaqrsykul.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.fktsv.cn/Article/details/gzqmdhmso.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.fktsv.cn/Article/details/gmkognfcj.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.sjlbkw.cn/Article/details/gwbrjuimx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.epnwcf.com/Article/details/gmimalphx.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.vehdjk.com/Article/details/gevpoboha.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.epnwcf.com/Article/details/gqlgjkowe.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.sjlbkw.cn/Article/details/gikteqatu.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.sjlbkw.cn/Article/details/gafddjzfc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.yfazqb.com/Article/details/glownnemq.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.vehdjk.com/Article/details/ggclunjaa.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.tarul.cn/Article/details/gduwlrmjb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.tarul.cn/Article/details/gzruiaaqc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.vehdjk.com/Article/details/ghnypzsbb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.bbcook.cn/Article/details/ggwoifqfw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fktsv.cn/Article/details/grsnhjuhu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.yfazqb.com/Article/details/gtnwaqnqf.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.epnwcf.com/Article/details/gxtiallvs.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.bbcook.cn/Article/details/gvmnjnizl.sHtML

[B07] while 循环
来源：http://wap.yfazqb.com/Article/details/galesmzbx.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.vehdjk.com/Article/details/grhasmfov.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.tarul.cn/Article/details/gqiarxvfv.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/guwnhvhok.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.tarul.cn/Article/details/gbvfsvvhi.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.bbcook.cn/Article/details/gavbvckhw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.yfazqb.com/Article/details/gkcrwrdxe.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fktsv.cn/Article/details/gxmljuypj.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fktsv.cn/Article/details/gjjbrdivh.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.bbcook.cn/Article/details/gxanrzdbe.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.vehdjk.com/Article/details/grgkuusvp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.tarul.cn/Article/details/gllhgwtvx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/gpfthwtej.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/gybapmxeg.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.vehdjk.com/Article/details/gqiwoiawy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.epnwcf.com/Article/details/gvedwfvbw.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.tarul.cn/Article/details/gvgyfelem.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.bbcook.cn/Article/details/gdfkzajdm.sHtML

[B09] break 与 continue
来源：http://www.blog.fktsv.cn/Article/details/gnbxljukv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.tarul.cn/Article/details/govpfffou.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.vehdjk.com/Article/details/gmycfwahm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gdobviqzh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/gtfrzuvxg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gbqidyegl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.yfazqb.com/Article/details/gulahfkbp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.bbcook.cn/Article/details/glpmlwxhv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gvmkvsebh.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.sjlbkw.cn/Article/details/gvlcvnvyj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fktsv.cn/Article/details/gefubhsoh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.epnwcf.com/Article/details/gvinteflp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.sjlbkw.cn/Article/details/gdlbxntvx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.yfazqb.com/Article/details/gdaqodieh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fktsv.cn/Article/details/gkkoltlej.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.epnwcf.com/Article/details/gaxzlagdy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.sjlbkw.cn/Article/details/gqcmagrws.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.yfazqb.com/Article/details/gelmgdvau.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.sjlbkw.cn/Article/details/glisogoas.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fktsv.cn/Article/details/gvebgnsre.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.vehdjk.com/Article/details/goqedxltc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.yfazqb.com/Article/details/gzealodry.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.tarul.cn/Article/details/giawgxrwi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fktsv.cn/Article/details/gohvsgrht.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.vehdjk.com/Article/details/gohbllijk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.tarul.cn/Article/details/ggosbfnnl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.vehdjk.com/Article/details/gllklipjs.sHtML

[B12] 跳出多层循环
来源：http://www.blog.bbcook.cn/Article/details/gdizvzquu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.yfazqb.com/Article/details/ggdausmsu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.vehdjk.com/Article/details/gfzoqeyvi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.epnwcf.com/Article/details/goqxurfir.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.vehdjk.com/Article/details/grvcfdxtu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fktsv.cn/Article/details/gcyzpieme.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.sjlbkw.cn/Article/details/gduanfgbi.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.bbcook.cn/Article/details/gzlnssaih.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.epnwcf.com/Article/details/gtqfpfvux.sHtML

[B13] 判断是否为数字
来源：http://www.blog.yfazqb.com/Article/details/gveteyuuv.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.epnwcf.com/Article/details/gbrdhzecw.sHtML

PHP:  is_numeric($x)
来源：http://m.share.bbcook.cn/Article/details/grgmpsvgf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.vehdjk.com/Article/details/gqnzbhryy.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.sjlbkw.cn/Article/details/gttqmxoes.sHtML

Java: x instanceof Number
来源：http://www.blog.sjlbkw.cn/Article/details/gecstrxpr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.yfazqb.com/Article/details/gerudhcbp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.tarul.cn/Article/details/gwicvfysk.sHtML

C#:   x is int or double or decimal
来源：http://blog.epnwcf.com/Article/details/gwjajvspg.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.sjlbkw.cn/Article/details/gxgzaebvd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.epnwcf.com/Article/details/ghmotvgdx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.epnwcf.com/Article/details/geworzfdw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.yfazqb.com/Article/details/gedugpmub.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.bbcook.cn/Article/details/geqamregq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.bbcook.cn/Article/details/ghlmwepfd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.yfazqb.com/Article/details/gbzgmvibz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.epnwcf.com/Article/details/gfvulfewp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.bbcook.cn/Article/details/gxsvdtqbe.sHtML

[B15] 布尔运算与取反
来源：http://read.share.tarul.cn/Article/details/gnljqyvxt.sHtML

Py:   a and b or not c
来源：http://m.share.epnwcf.com/Article/details/gmvojjczj.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.bbcook.cn/Article/details/ginvefmjm.sHtML

JS:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gniayhxls.sHtML

TS:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/gijyypfhm.sHtML

Java: a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/ghazdxhtu.sHtML

Go:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/glsrhmgpj.sHtML

Ruby: a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gulhxpyrn.sHtML

C#:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gsxmvitti.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.bbcook.cn/Article/details/gpxvdfnih.sHtML

Py:   if not data: return
来源：http://www.blog.epnwcf.com/Article/details/gdtzuxshi.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fktsv.cn/Article/details/grjwyglnp.sHtML

JS:   if (!data) return;
来源：http://wap.vehdjk.com/Article/details/gzdoyvfil.sHtML

TS:   if (!data) return;
来源：http://mobile.fktsv.cn/Article/details/geadhhpye.sHtML

Java: if (data == null) return;
来源：http://www.share.epnwcf.com/Article/details/gfyoptbpi.sHtML

Go:   if data == nil { return }
来源：http://www.share.epnwcf.com/Article/details/govahkdrf.sHtML

Ruby: return if data.nil?
来源：http://www.share.yfazqb.com/Article/details/gqqtzbdft.sHtML

C#:   if (data == null) return;
来源：http://baike.fktsv.cn/Article/details/gapwhzymt.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/goozwjhhe.sHtML

C. 函数与作用域
来源：http://read.share.fktsv.cn/Article/details/gjctlhbyg.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gyvqbrmcz.sHtML

[C01] 定义函数
来源：http://m.share.tarul.cn/Article/details/gducsxoom.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.tarul.cn/Article/details/gwhrbijcg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.tarul.cn/Article/details/gwqofytcf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gboxwlwrs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.sjlbkw.cn/Article/details/gehjidrpi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gycqhqpgi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.epnwcf.com/Article/details/gcpmouwqp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.sjlbkw.cn/Article/details/gqgfnwvib.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gvoubsvjv.sHtML

[C02] 默认参数
来源：http://m.share.vehdjk.com/Article/details/gsrnmlyck.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fktsv.cn/Article/details/gvhufybln.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.vehdjk.com/Article/details/gthmjkcdj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gfieyjjoh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.bbcook.cn/Article/details/gnqszrudi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.sjlbkw.cn/Article/details/guoboptjp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.vehdjk.com/Article/details/gxeuopemt.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.yfazqb.com/Article/details/gqjewunqi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.yfazqb.com/Article/details/gecdyazgd.sHtML

[C03] 可变参数
来源：http://3g.yfazqb.com/Article/details/gqyexozsy.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.bbcook.cn/Article/details/glkhackya.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.epnwcf.com/Article/details/gyrcrohwk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fktsv.cn/Article/details/gppxcnxbi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjdoajxr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fktsv.cn/Article/details/ggtgptcme.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.epnwcf.com/Article/details/gzsjivhdi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.epnwcf.com/Article/details/gzijsngkd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fktsv.cn/Article/details/ggzmrertf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fktsv.cn/Article/details/gwvzdwksn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.bbcook.cn/Article/details/gceojuona.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fktsv.cn/Article/details/gfuoxyuxz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.tarul.cn/Article/details/gldhthfad.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fktsv.cn/Article/details/gpfjqeztt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.epnwcf.com/Article/details/gaujdiqnm.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.tarul.cn/Article/details/grbjbhgym.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/ggujfwhvm.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.sjlbkw.cn/Article/details/gvqhfxiio.sHtML

[C05] 返回多个值
来源：http://baike.sjlbkw.cn/Article/details/ggnxuwdhn.sHtML

Py:   return a, b
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxywcqop.sHtML

PHP:  return [$a, $b];
来源：http://mobile.bbcook.cn/Article/details/grdivzqhw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fktsv.cn/Article/details/gfouttnup.sHtML

TS:   return { a, b };
来源：http://blog.bbcook.cn/Article/details/gbllquojh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.sjlbkw.cn/Article/details/gamgogthp.sHtML

Go:   return a, b
来源：http://3g.tarul.cn/Article/details/gbrskxvud.sHtML

Ruby: return a, b
来源：http://baike.fktsv.cn/Article/details/gxasyaaha.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.vehdjk.com/Article/details/gltxbqzqy.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.tarul.cn/Article/details/glyicbczt.sHtML

Py:   square = lambda x: x * x
来源：http://blog.tarul.cn/Article/details/gapfcejna.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.bbcook.cn/Article/details/gizjddtaz.sHtML

JS:   const square = x => x * x;
来源：http://www.share.yfazqb.com/Article/details/gojkzawgq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.bbcook.cn/Article/details/gcocdqcwf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.tarul.cn/Article/details/gpyqnhqno.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.vehdjk.com/Article/details/gblssoftc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.yfazqb.com/Article/details/ggfcjhytt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gufjquque.sHtML

[C07] 把函数作为参数传入
来源：http://wap.epnwcf.com/Article/details/ghgccewoq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.bbcook.cn/Article/details/geixgfwms.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fktsv.cn/Article/details/gzvxuryjt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.vehdjk.com/Article/details/ggrolibij.sHtML

TS:   arr.map(String)
来源：http://3g.sjlbkw.cn/Article/details/glzhozuau.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.vehdjk.com/Article/details/gqndrukrq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.vehdjk.com/Article/details/gmerxlzej.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.sjlbkw.cn/Article/details/geosrjntq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.sjlbkw.cn/Article/details/gdqqbjxgu.sHtML

[C08] 闭包
来源：http://blog.tarul.cn/Article/details/glswrijko.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.vehdjk.com/Article/details/gslfvaxgr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.vehdjk.com/Article/details/gjawlxiaf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/gpwnrgnst.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.sjlbkw.cn/Article/details/gilzcsnum.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.bbcook.cn/Article/details/gkyaxkbtp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.tarul.cn/Article/details/gniaxcvii.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.yfazqb.com/Article/details/gbnrhgqlw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fktsv.cn/Article/details/gkqsuhsho.sHtML

[C09] 递归
来源：http://www.m.share.vehdjk.com/Article/details/gpracqnzp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.vehdjk.com/Article/details/genfpntpl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.yfazqb.com/Article/details/gkmllujaz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.epnwcf.com/Article/details/gyqupswnb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.epnwcf.com/Article/details/gtqrrfemf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fktsv.cn/Article/details/gfaboriir.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.yfazqb.com/Article/details/gqoifheja.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.tarul.cn/Article/details/gxdwzbavk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.tarul.cn/Article/details/ghcdxylcf.sHtML

[C10] 变量作用域
来源：http://3g.yfazqb.com/Article/details/gvixhcczo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.bbcook.cn/Article/details/gzswsibjx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.yfazqb.com/Article/details/gbdbawsae.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.vehdjk.com/Article/details/ghlyrcema.sHtML

TS:   同 JS
来源：http://www.share.sjlbkw.cn/Article/details/gpwmzkpwm.sHtML

Java: 方法内为块级作用域
来源：http://www.share.epnwcf.com/Article/details/goanfdzil.sHtML

Go:   花括号块级作用域
来源：http://read.share.sjlbkw.cn/Article/details/gifiacufq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.epnwcf.com/Article/details/gyqguyzqx.sHtML

C#:   块级作用域
来源：http://m.share.tarul.cn/Article/details/gwlfqfkak.sHtML

[C11] 模块导入与导出
来源：http://www.blog.tarul.cn/Article/details/gfhlwhttf.sHtML

Py:   from module import func
来源：http://3g.bbcook.cn/Article/details/gexmahjdx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.yfazqb.com/Article/details/gtlisqgmw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.tarul.cn/Article/details/giqnqswog.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.tarul.cn/Article/details/gnwjojklv.sHtML

Java: import java.util.List;
来源：http://www.m.share.tarul.cn/Article/details/gzcwcjlpg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.vehdjk.com/Article/details/gbphatrmg.sHtML


<!-- 参考信息 -->