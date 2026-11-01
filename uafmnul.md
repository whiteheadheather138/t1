代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.bbcook.cn/Article/details/gnikniqqy.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.yfazqb.com/Article/details/gkyewwmkk.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.yfazqb.com/Article/details/gplcujymf.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.vehdjk.com/Article/details/guigsauxe.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.yfazqb.com/Article/details/gbiraozuc.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.yfazqb.com/Article/details/gefskpufd.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.bbcook.cn/Article/details/ggywsbtbw.sHtML

[A25] 字符串比较
来源：http://www.share.sjlbkw.cn/Article/details/gggpwazcq.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.bbcook.cn/Article/details/ghcpdoffh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.tarul.cn/Article/details/gnyrspntk.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.epnwcf.com/Article/details/gjxmxnxcn.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fktsv.cn/Article/details/gntkqywft.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.fktsv.cn/Article/details/gfusqcxff.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.bbcook.cn/Article/details/gfkhvnsrb.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.epnwcf.com/Article/details/goavxsqhz.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.epnwcf.com/Article/details/gqkpjpzdl.sHtML

[A26] 类型转换总览
来源：http://m.share.sjlbkw.cn/Article/details/gipiwhgcv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.yfazqb.com/Article/details/gqgqbtdwr.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.bbcook.cn/Article/details/gmhqqrcvr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.fktsv.cn/Article/details/gqkaqhgdm.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.bbcook.cn/Article/details/gvuzmbxij.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.bbcook.cn/Article/details/gnjaqnuir.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.fktsv.cn/Article/details/ghxrywmmt.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.fktsv.cn/Article/details/gwwiwgmvy.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.sjlbkw.cn/Article/details/ggtiimari.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gvmiorypg.sHtML

B. 流程控制
来源：http://blog.bbcook.cn/Article/details/gzxxxxuom.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gfnaigowe.sHtML

[B01] 条件判断 if / else
来源：http://m.share.bbcook.cn/Article/details/gjjxgmjca.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.fktsv.cn/Article/details/gkjxljwxp.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.vehdjk.com/Article/details/gnywkxkwj.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.tarul.cn/Article/details/gucumiski.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.sjlbkw.cn/Article/details/guxlddozc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/gotwtdasw.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.epnwcf.com/Article/details/ghbznrnje.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.bbcook.cn/Article/details/ggsxyptje.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.fktsv.cn/Article/details/gvrexvuga.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.bbcook.cn/Article/details/gwnccjwye.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.fktsv.cn/Article/details/ggrjdttsj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.yfazqb.com/Article/details/glssrpaqw.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fktsv.cn/Article/details/gcyjoqxfr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.epnwcf.com/Article/details/glyrzylct.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.sjlbkw.cn/Article/details/gbmeedwqu.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.bbcook.cn/Article/details/ghjsvdcbm.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.yfazqb.com/Article/details/gdnwdlxom.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.vehdjk.com/Article/details/gdsuifwcq.sHtML

[B03] switch / match / case
来源：http://read.share.epnwcf.com/Article/details/ggncspkvy.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.fktsv.cn/Article/details/gpbptsgfj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.epnwcf.com/Article/details/gpggdkwwx.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fktsv.cn/Article/details/gppnrlgal.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.tarul.cn/Article/details/gvksnhljz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.tarul.cn/Article/details/gfsfogjgd.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.vehdjk.com/Article/details/gtxprkgvv.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.fktsv.cn/Article/details/grlmnylhu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.sjlbkw.cn/Article/details/gclrmwmpt.sHtML

[B04] for 计数循环
来源：http://read.share.fktsv.cn/Article/details/guiajhblg.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.vehdjk.com/Article/details/goncuzdpz.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.bbcook.cn/Article/details/gxhzinwxv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fktsv.cn/Article/details/gwjigwbni.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.tarul.cn/Article/details/gwzvsjupq.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.vehdjk.com/Article/details/gansnxopk.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.sjlbkw.cn/Article/details/gyxwdmaci.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.epnwcf.com/Article/details/gwrqlbhvv.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.tarul.cn/Article/details/gyzscsral.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.yfazqb.com/Article/details/gpxqcewlq.sHtML

Py:   for item in arr: print(item)
来源：http://baike.tarul.cn/Article/details/gzzjwnabv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.yfazqb.com/Article/details/ggzqtliiw.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.yfazqb.com/Article/details/gkkmurunj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.tarul.cn/Article/details/gpflcxzph.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.fktsv.cn/Article/details/gcqpjrqsb.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.vehdjk.com/Article/details/gkhehlvml.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.fktsv.cn/Article/details/gvuyuvyel.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.tarul.cn/Article/details/gpelbdzqs.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.vehdjk.com/Article/details/gjzksdjgq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.yfazqb.com/Article/details/gpiyfraio.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.vehdjk.com/Article/details/gpbbabfhm.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fktsv.cn/Article/details/guliwvpnk.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fktsv.cn/Article/details/gygpudpll.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.sjlbkw.cn/Article/details/gbytikxfs.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.epnwcf.com/Article/details/gvhsupuai.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.bbcook.cn/Article/details/gvwdfvyzw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fktsv.cn/Article/details/gnwjnmgqx.sHtML

[B07] while 循环
来源：http://baike.bbcook.cn/Article/details/guyzszdmh.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.yfazqb.com/Article/details/godqfrvoe.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.yfazqb.com/Article/details/gublbglxy.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmviozutw.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.epnwcf.com/Article/details/gcfmpwctm.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.yfazqb.com/Article/details/gomacwypl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.yfazqb.com/Article/details/gzpjwbohk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.sjlbkw.cn/Article/details/ggyalogmp.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.bbcook.cn/Article/details/ggtymobam.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.vehdjk.com/Article/details/gyhckyeqj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.epnwcf.com/Article/details/getlsixbz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/gdkfhexxj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gpgjueaab.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/geqknmecs.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.yfazqb.com/Article/details/ggktuzawh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.tarul.cn/Article/details/gpjazofad.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.tarul.cn/Article/details/gdwoeqvhs.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/gnudukpel.sHtML

[B09] break 与 continue
来源：http://3g.yfazqb.com/Article/details/gllmwpwwt.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.bbcook.cn/Article/details/glxmwltyb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gqjehwftg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdmdwhksa.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/gegueqlfs.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gpibtgcql.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.vehdjk.com/Article/details/gwglwlppp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.sjlbkw.cn/Article/details/gmxdeghov.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/ghucvwgkd.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.tarul.cn/Article/details/gzwdkpjhh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.tarul.cn/Article/details/ghmjpihpx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.yfazqb.com/Article/details/gjhgkbqvw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.bbcook.cn/Article/details/givphwetg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.tarul.cn/Article/details/gluaimwce.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fktsv.cn/Article/details/gfisewyhz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.bbcook.cn/Article/details/gyfoxnzbn.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.bbcook.cn/Article/details/gzjrgxlok.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.epnwcf.com/Article/details/grfwjylhm.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.epnwcf.com/Article/details/gkwtpbmlt.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.tarul.cn/Article/details/gzxkrompt.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.vehdjk.com/Article/details/ghbnmckkf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.yfazqb.com/Article/details/gmarpjppy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.vehdjk.com/Article/details/gabvxlanb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.epnwcf.com/Article/details/gmwbnigxk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.tarul.cn/Article/details/gcppjyjxb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.tarul.cn/Article/details/grlvvqtbl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fktsv.cn/Article/details/gzrvssjop.sHtML

[B12] 跳出多层循环
来源：http://mobile.bbcook.cn/Article/details/gxqkpecbt.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.tarul.cn/Article/details/gjxtuziyb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.sjlbkw.cn/Article/details/gbnssyoin.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/gfnyewbuh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.sjlbkw.cn/Article/details/gamkpadsz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/gpchionec.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.bbcook.cn/Article/details/gvckthaxb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.vehdjk.com/Article/details/ghegkeldn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.tarul.cn/Article/details/gdrutrexe.sHtML

[B13] 判断是否为数字
来源：http://3g.epnwcf.com/Article/details/gwplynmux.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.vehdjk.com/Article/details/gxfbzjoah.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.tarul.cn/Article/details/gzzqlehta.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.bbcook.cn/Article/details/gcpinlnvh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.epnwcf.com/Article/details/ghvosrgln.sHtML

Java: x instanceof Number
来源：http://read.share.epnwcf.com/Article/details/gflcwxofx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.vehdjk.com/Article/details/gganneofo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.yfazqb.com/Article/details/gkcsfahul.sHtML

C#:   x is int or double or decimal
来源：http://baike.vehdjk.com/Article/details/gfhvmrkyo.sHtML

[B14] 判断值是否在集合内
来源：http://wap.yfazqb.com/Article/details/gnqdycqwk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.bbcook.cn/Article/details/gnbqbcclf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.sjlbkw.cn/Article/details/gzhjvbfnv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.bbcook.cn/Article/details/gaphdapbq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.vehdjk.com/Article/details/gklidtdwh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/gyyzsdnrz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fktsv.cn/Article/details/gjcgzpgaq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.yfazqb.com/Article/details/grakjhadz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.tarul.cn/Article/details/gwstjcwof.sHtML

[B15] 布尔运算与取反
来源：http://3g.bbcook.cn/Article/details/ghocmahfn.sHtML

Py:   a and b or not c
来源：http://www.share.sjlbkw.cn/Article/details/gitodvfgk.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.vehdjk.com/Article/details/gucnvpnoh.sHtML

JS:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gnldlbqyw.sHtML

TS:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gkpppekyl.sHtML

Java: a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/giebdlktu.sHtML

Go:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/guitggndl.sHtML

Ruby: a && b || !c
来源：http://blog.tarul.cn/Article/details/glmpclblk.sHtML

C#:   a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gabnljkzl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.bbcook.cn/Article/details/gizuibezk.sHtML

Py:   if not data: return
来源：http://blog.bbcook.cn/Article/details/gkawomhqv.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.vehdjk.com/Article/details/gaokqqofw.sHtML

JS:   if (!data) return;
来源：http://mobile.bbcook.cn/Article/details/gtvbdcgwo.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fktsv.cn/Article/details/gkucswofr.sHtML

Java: if (data == null) return;
来源：http://wap.fktsv.cn/Article/details/gsiibamhg.sHtML

Go:   if data == nil { return }
来源：http://3g.fktsv.cn/Article/details/gfkysgjsm.sHtML

Ruby: return if data.nil?
来源：http://www.blog.epnwcf.com/Article/details/grrjzeybg.sHtML

C#:   if (data == null) return;
来源：http://3g.vehdjk.com/Article/details/gzoehomdw.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/galblrbvs.sHtML

C. 函数与作用域
来源：http://read.share.bbcook.cn/Article/details/gczrytnqw.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gqoapuvyq.sHtML

[C01] 定义函数
来源：http://mobile.bbcook.cn/Article/details/gybuanzbr.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.bbcook.cn/Article/details/gmbmcxiwo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/gjiucudeu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.sjlbkw.cn/Article/details/goqbxqzgn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.tarul.cn/Article/details/gsoumjxzu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gbhogsxru.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fktsv.cn/Article/details/ggzrrnsir.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.tarul.cn/Article/details/gfsdjhsyt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/ghfqqltsd.sHtML

[C02] 默认参数
来源：http://blog.bbcook.cn/Article/details/gowfpwkqb.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.vehdjk.com/Article/details/gsxetjzwx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.yfazqb.com/Article/details/gublijitx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.tarul.cn/Article/details/gjcersgyl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.tarul.cn/Article/details/gmvnlwyba.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.yfazqb.com/Article/details/gypfptivc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.sjlbkw.cn/Article/details/ggsjikcej.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.epnwcf.com/Article/details/gabwtdupk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.vehdjk.com/Article/details/gkkzoizno.sHtML

[C03] 可变参数
来源：http://www.m.share.vehdjk.com/Article/details/gbweldefr.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.sjlbkw.cn/Article/details/gffmrgsql.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.tarul.cn/Article/details/gktraflmj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.sjlbkw.cn/Article/details/gbdcdanxv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.tarul.cn/Article/details/gpxmaxgqc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.bbcook.cn/Article/details/grbknfkmf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.vehdjk.com/Article/details/gujerctzx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.vehdjk.com/Article/details/gumwrogds.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fktsv.cn/Article/details/gkvvqdnfk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.yfazqb.com/Article/details/gmsnkbgts.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.vehdjk.com/Article/details/ggphvqiel.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.vehdjk.com/Article/details/gsuxaewjl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.vehdjk.com/Article/details/gjqhcdbbo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.yfazqb.com/Article/details/gicoqsgot.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fktsv.cn/Article/details/gtonplmcv.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.tarul.cn/Article/details/gyfqdhhsi.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/grndhbmem.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.bbcook.cn/Article/details/geullfegi.sHtML

[C05] 返回多个值
来源：http://www.blog.epnwcf.com/Article/details/gibllagde.sHtML

Py:   return a, b
来源：http://mobile.bbcook.cn/Article/details/gkbpumhwt.sHtML

PHP:  return [$a, $b];
来源：http://blog.yfazqb.com/Article/details/gzasywhyo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.epnwcf.com/Article/details/glmkvxhdk.sHtML

TS:   return { a, b };
来源：http://www.blog.epnwcf.com/Article/details/gktaeqled.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fktsv.cn/Article/details/gemizrspi.sHtML

Go:   return a, b
来源：http://www.share.yfazqb.com/Article/details/gnxncovxf.sHtML

Ruby: return a, b
来源：http://www.blog.vehdjk.com/Article/details/gupgyvbhy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.tarul.cn/Article/details/grbnmeukl.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.vehdjk.com/Article/details/gcnrepnpv.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.vehdjk.com/Article/details/gekasckcy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.epnwcf.com/Article/details/gaytkityb.sHtML

JS:   const square = x => x * x;
来源：http://mobile.tarul.cn/Article/details/gbiqwpkpw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.tarul.cn/Article/details/gqjuaeonh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.yfazqb.com/Article/details/gptaxllnj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.tarul.cn/Article/details/grtqxjmsr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.bbcook.cn/Article/details/gxkyjccef.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.tarul.cn/Article/details/gujyvorub.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.bbcook.cn/Article/details/gucrmxpgo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.epnwcf.com/Article/details/gsutukijt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.epnwcf.com/Article/details/gonlynnrr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.bbcook.cn/Article/details/gkvsducao.sHtML

TS:   arr.map(String)
来源：http://wap.bbcook.cn/Article/details/gmwsohqbx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fktsv.cn/Article/details/gegvmkpup.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.yfazqb.com/Article/details/guvbozhki.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.bbcook.cn/Article/details/gevgaknlg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.epnwcf.com/Article/details/gqwcmqtxf.sHtML

[C08] 闭包
来源：http://wap.yfazqb.com/Article/details/guyrfetmo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.sjlbkw.cn/Article/details/gsqctccfv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fktsv.cn/Article/details/gfluuekkj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.tarul.cn/Article/details/gfilrscva.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/gnmhoxrbl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fktsv.cn/Article/details/glnmylqyq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.bbcook.cn/Article/details/gosxhquus.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.yfazqb.com/Article/details/gprcwvqdf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.sjlbkw.cn/Article/details/ggypkhmaj.sHtML

[C09] 递归
来源：http://m.share.fktsv.cn/Article/details/gfpncsxkz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.vehdjk.com/Article/details/gwlymzbdx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.vehdjk.com/Article/details/gphrpiiyc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.tarul.cn/Article/details/glhesiynd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.epnwcf.com/Article/details/gexsdsotj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.yfazqb.com/Article/details/gekvpxyzf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fktsv.cn/Article/details/ghkpdtmxf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fktsv.cn/Article/details/gtggpiqep.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.epnwcf.com/Article/details/ghswhjlls.sHtML

[C10] 变量作用域
来源：http://read.share.tarul.cn/Article/details/ggbqwyttc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.yfazqb.com/Article/details/ggfgpzyrp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fktsv.cn/Article/details/gsvdqmtuo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.epnwcf.com/Article/details/ggajaumfu.sHtML

TS:   同 JS
来源：http://mobile.yfazqb.com/Article/details/gisbpnaxf.sHtML

Java: 方法内为块级作用域
来源：http://m.share.epnwcf.com/Article/details/gfpvuqlki.sHtML

Go:   花括号块级作用域
来源：http://wap.epnwcf.com/Article/details/gracggmac.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.vehdjk.com/Article/details/gqjdkzhrk.sHtML

C#:   块级作用域
来源：http://m.share.epnwcf.com/Article/details/gxpnhobmi.sHtML

[C11] 模块导入与导出
来源：http://wap.bbcook.cn/Article/details/gjdxihfcf.sHtML

Py:   from module import func
来源：http://mobile.yfazqb.com/Article/details/gfkyvqvtb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.yfazqb.com/Article/details/gwijpobrs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.yfazqb.com/Article/details/gekawgixw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.bbcook.cn/Article/details/gjhmszxgd.sHtML

Java: import java.util.List;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjbxobbg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.yfazqb.com/Article/details/gorzcqrkn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.epnwcf.com/Article/details/gezsxrzqp.sHtML

C#:   using System.Text;
来源：http://blog.bbcook.cn/Article/details/gthmkrtrx.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fktsv.cn/Article/details/gfjltlzjb.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fktsv.cn/Article/details/gficvxvdx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.epnwcf.com/Article/details/gvovwtcws.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.epnwcf.com/Article/details/gpumioamy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fktsv.cn/Article/details/grhdzxqsr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.sjlbkw.cn/Article/details/gjalwqzsb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.epnwcf.com/Article/details/gmwopxmfj.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fktsv.cn/Article/details/gipwxrmon.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.yfazqb.com/Article/details/gyjnmjhpd.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.bbcook.cn/Article/details/giljbyano.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.bbcook.cn/Article/details/ggbdvlvxs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.epnwcf.com/Article/details/gnxfhhdmq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.yfazqb.com/Article/details/gkvagojks.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gwbqsnkeg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gndbttmql.sHtML

Go:   func add(a, b int) int
来源：http://wap.bbcook.cn/Article/details/gpioitctu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.epnwcf.com/Article/details/gewgibasi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.tarul.cn/Article/details/grrtbuafd.sHtML

[C14] 泛型函数
来源：http://www.share.tarul.cn/Article/details/gmdbgxbmb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.yfazqb.com/Article/details/gmvnawzkz.sHtML

PHP:  // 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gkbgsyuwz.sHtML

JS:   // 无泛型
来源：http://www.share.tarul.cn/Article/details/guhkfvmxz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.yfazqb.com/Article/details/gxylcvntp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.tarul.cn/Article/details/guckpqegt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.epnwcf.com/Article/details/gycothgba.sHtML

Ruby: # 无泛型
来源：http://wap.epnwcf.com/Article/details/gdhzwheik.sHtML


<!-- 参考信息 -->