代发 wailian999

[B01] 条件判断 if / else
来源：http://www.m.share.bbcook.cn/Article/details/gbxafjdgt.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.sjlbkw.cn/Article/details/gpywwhqqj.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.yfazqb.com/Article/details/grrhiihqo.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.yfazqb.com/Article/details/gwkcozhmw.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fktsv.cn/Article/details/gtozpeenb.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.yfazqb.com/Article/details/gjpisqlxy.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.epnwcf.com/Article/details/gcmzvypkx.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.sjlbkw.cn/Article/details/gqkdkhtug.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.vehdjk.com/Article/details/gpllkqgoi.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fktsv.cn/Article/details/goynydyvd.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.bbcook.cn/Article/details/gzkhvklzk.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.yfazqb.com/Article/details/gzhjhmwvl.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fktsv.cn/Article/details/grufclknv.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.yfazqb.com/Article/details/gjtqtpwka.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.bbcook.cn/Article/details/gfplqsimn.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.epnwcf.com/Article/details/gxtulwimn.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.bbcook.cn/Article/details/gpqkgpduh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/gtjmumznv.sHtML

[B03] switch / match / case
来源：http://mobile.fktsv.cn/Article/details/gjputcwjw.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.epnwcf.com/Article/details/glcdpmiuk.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.bbcook.cn/Article/details/gijvwbyoi.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.sjlbkw.cn/Article/details/gkgqsnlps.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fktsv.cn/Article/details/glzxaxzly.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.sjlbkw.cn/Article/details/ggdqymlwa.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.vehdjk.com/Article/details/gfqynjnmm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.epnwcf.com/Article/details/giwgmuzgg.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.vehdjk.com/Article/details/gvkejamjx.sHtML

[B04] for 计数循环
来源：http://baike.sjlbkw.cn/Article/details/gwntdwfua.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.vehdjk.com/Article/details/gmmtrmupm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.yfazqb.com/Article/details/gfvjenlxa.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.bbcook.cn/Article/details/gfyhsswlx.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.yfazqb.com/Article/details/gyozjulal.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.yfazqb.com/Article/details/gcahbfdxq.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.yfazqb.com/Article/details/gpqprbgtc.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.yfazqb.com/Article/details/gsdqefdhk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.bbcook.cn/Article/details/gvtomgoff.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.epnwcf.com/Article/details/gaiswnrcg.sHtML

Py:   for item in arr: print(item)
来源：http://blog.yfazqb.com/Article/details/gvpfxzsjk.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.epnwcf.com/Article/details/gxdthqwye.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.vehdjk.com/Article/details/gwrhwisqq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.tarul.cn/Article/details/gkqxkauex.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.fktsv.cn/Article/details/gdhadzuep.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.vehdjk.com/Article/details/gzvdbtizt.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.vehdjk.com/Article/details/gdyjryhdy.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.epnwcf.com/Article/details/gayjbewid.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fktsv.cn/Article/details/gacsaglcu.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.tarul.cn/Article/details/gwqvvjyse.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.fktsv.cn/Article/details/gjyiaxzzh.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fktsv.cn/Article/details/gzykdxsgn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.tarul.cn/Article/details/gapykyrql.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.bbcook.cn/Article/details/gxgnngvwq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.tarul.cn/Article/details/gpbdilthx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.epnwcf.com/Article/details/gkjcrnqps.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.tarul.cn/Article/details/gdzpbwjeb.sHtML

[B07] while 循环
来源：http://www.share.tarul.cn/Article/details/gvlcuyxfs.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.bbcook.cn/Article/details/gtgvyyxun.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fktsv.cn/Article/details/gdmcpymuw.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.epnwcf.com/Article/details/gnggjniqc.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.yfazqb.com/Article/details/gowwyjczd.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.tarul.cn/Article/details/gwucqljvu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.epnwcf.com/Article/details/gzzcuyein.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.yfazqb.com/Article/details/gwasgtqce.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.sjlbkw.cn/Article/details/gllctnomb.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.bbcook.cn/Article/details/gbayffjbl.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.bbcook.cn/Article/details/gymzmjwvi.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.yfazqb.com/Article/details/gaiectikx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.bbcook.cn/Article/details/gihcbfuxt.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/gjzkwwxrg.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/ggshyhtjf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.tarul.cn/Article/details/gpmhbohxn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.bbcook.cn/Article/details/gbhdqfooj.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fktsv.cn/Article/details/gxaicclqc.sHtML

[B09] break 与 continue
来源：http://baike.yfazqb.com/Article/details/gmruogcvj.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.bbcook.cn/Article/details/guuhjvphm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/gzfbckhsg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/giijwdgvb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/giuoitgzk.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gixzlggrp.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fktsv.cn/Article/details/gulmfeskj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fktsv.cn/Article/details/gsdeitbin.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gjyhdzgjo.sHtML

[B10] 遍历同时拿索引
来源：http://baike.sjlbkw.cn/Article/details/ggidwzelu.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.vehdjk.com/Article/details/glpgmvarg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.yfazqb.com/Article/details/gjcvhgvfo.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.yfazqb.com/Article/details/gdrwbylkd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.tarul.cn/Article/details/gacypltyc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.fktsv.cn/Article/details/gvtkatgjf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fktsv.cn/Article/details/gpafyzjvw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.tarul.cn/Article/details/gsgoipwdj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.sjlbkw.cn/Article/details/garzvttbi.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.sjlbkw.cn/Article/details/ggxlbulim.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.vehdjk.com/Article/details/gakstyioo.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.tarul.cn/Article/details/gpqhcafbp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fktsv.cn/Article/details/glypjvlxa.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.tarul.cn/Article/details/gjstfjvny.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fktsv.cn/Article/details/glbqswspc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.bbcook.cn/Article/details/gjzygjajd.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.epnwcf.com/Article/details/gqtjgrpgu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.tarul.cn/Article/details/ghfddmxlx.sHtML

[B12] 跳出多层循环
来源：http://mobile.fktsv.cn/Article/details/gfixpsirg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.yfazqb.com/Article/details/gpqphcxss.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.vehdjk.com/Article/details/gtawjcxhq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/ghamzunzd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fktsv.cn/Article/details/gwbjieorg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.tarul.cn/Article/details/gtqvboxfm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.tarul.cn/Article/details/gswhethzp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fktsv.cn/Article/details/gptwhqbzh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.yfazqb.com/Article/details/gphtnhbsa.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.epnwcf.com/Article/details/gbgyymwye.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.bbcook.cn/Article/details/gsgupvxxs.sHtML

PHP:  is_numeric($x)
来源：http://baike.vehdjk.com/Article/details/gocpvggpg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fktsv.cn/Article/details/ghtiesduw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.bbcook.cn/Article/details/ghugondot.sHtML

Java: x instanceof Number
来源：http://mobile.epnwcf.com/Article/details/glqldlqea.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.tarul.cn/Article/details/gspjwsfmu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fktsv.cn/Article/details/gkwlpxtje.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.yfazqb.com/Article/details/glzysufhx.sHtML

[B14] 判断值是否在集合内
来源：http://3g.yfazqb.com/Article/details/gvcdgpxwf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.tarul.cn/Article/details/gqocaqqsy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fktsv.cn/Article/details/guoyymssd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.bbcook.cn/Article/details/gevjwfehj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.bbcook.cn/Article/details/grshqwjnm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gwlgjwiwr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.tarul.cn/Article/details/guruaptkv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.sjlbkw.cn/Article/details/gkegtsnep.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.epnwcf.com/Article/details/gbzdhgkqa.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.sjlbkw.cn/Article/details/gxabshivk.sHtML

Py:   a and b or not c
来源：http://read.share.vehdjk.com/Article/details/ghtchyjfk.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.sjlbkw.cn/Article/details/gpgqkhhhz.sHtML

JS:   a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gsczpfmmu.sHtML

TS:   a && b || !c
来源：http://baike.bbcook.cn/Article/details/gftpscsuq.sHtML

Java: a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpxhosyo.sHtML

Go:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gchkgghqj.sHtML

Ruby: a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/ghwgywhvq.sHtML

C#:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/geeluwcrf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.tarul.cn/Article/details/gqntsjdqf.sHtML

Py:   if not data: return
来源：http://blog.bbcook.cn/Article/details/gsuoimwba.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fktsv.cn/Article/details/gywwgfndl.sHtML

JS:   if (!data) return;
来源：http://m.share.yfazqb.com/Article/details/gpltlkawa.sHtML

TS:   if (!data) return;
来源：http://www.blog.epnwcf.com/Article/details/gmjttzqxb.sHtML

Java: if (data == null) return;
来源：http://wap.epnwcf.com/Article/details/gkvfqduds.sHtML

Go:   if data == nil { return }
来源：http://m.share.yfazqb.com/Article/details/gggmaqlhc.sHtML

Ruby: return if data.nil?
来源：http://m.share.fktsv.cn/Article/details/grtygngyt.sHtML

C#:   if (data == null) return;
来源：http://blog.bbcook.cn/Article/details/gpivbuwsc.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gqlfgpuln.sHtML

C. 函数与作用域
来源：http://www.blog.vehdjk.com/Article/details/gmvrmnzmg.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gfjsraish.sHtML

[C01] 定义函数
来源：http://m.share.yfazqb.com/Article/details/gfokwrask.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.vehdjk.com/Article/details/gdpetkhch.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.epnwcf.com/Article/details/gqlhleqwh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gmgqwvllg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fktsv.cn/Article/details/glbjiyckz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.vehdjk.com/Article/details/guljkvshn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.yfazqb.com/Article/details/grlpyxehl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.epnwcf.com/Article/details/gvnnbdzly.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/grpyrhxqr.sHtML

[C02] 默认参数
来源：http://www.m.share.epnwcf.com/Article/details/gddhdtmcq.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.yfazqb.com/Article/details/gpseamiej.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.vehdjk.com/Article/details/ggsutnguw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.yfazqb.com/Article/details/geptxkvhz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fktsv.cn/Article/details/goyffwbgk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.sjlbkw.cn/Article/details/gmvqucbpm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.tarul.cn/Article/details/gxflxguzx.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.tarul.cn/Article/details/gmafuzfgy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.sjlbkw.cn/Article/details/glzkkcuft.sHtML

[C03] 可变参数
来源：http://wap.yfazqb.com/Article/details/gtkzgjdus.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.vehdjk.com/Article/details/gppzimicr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fktsv.cn/Article/details/ghdhzeptx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.bbcook.cn/Article/details/gdxwfiema.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.sjlbkw.cn/Article/details/gbheloank.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.sjlbkw.cn/Article/details/gboxyrhkv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.bbcook.cn/Article/details/gtxtlkrpm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.bbcook.cn/Article/details/gxknrvzjq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.vehdjk.com/Article/details/gfqewizze.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.yfazqb.com/Article/details/grsttledw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.epnwcf.com/Article/details/gvlxqlkpi.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.sjlbkw.cn/Article/details/gjwujqody.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.tarul.cn/Article/details/gsrjnegoj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.epnwcf.com/Article/details/gorxjfkou.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.sjlbkw.cn/Article/details/gxwwtbqrd.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.sjlbkw.cn/Article/details/grggefusa.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.tarul.cn/Article/details/gowllzceo.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/gupbtixoc.sHtML

[C05] 返回多个值
来源：http://3g.sjlbkw.cn/Article/details/grmonrrcy.sHtML

Py:   return a, b
来源：http://baike.yfazqb.com/Article/details/guzzdrdei.sHtML

PHP:  return [$a, $b];
来源：http://baike.vehdjk.com/Article/details/gtjcimimy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.vehdjk.com/Article/details/gmglavycg.sHtML

TS:   return { a, b };
来源：http://3g.vehdjk.com/Article/details/gvgbgveve.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fktsv.cn/Article/details/gqzhkdgpq.sHtML

Go:   return a, b
来源：http://3g.epnwcf.com/Article/details/goibxwuqv.sHtML

Ruby: return a, b
来源：http://www.m.share.epnwcf.com/Article/details/gqwpegokx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.vehdjk.com/Article/details/gfeacozpt.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.bbcook.cn/Article/details/gowtxepav.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fktsv.cn/Article/details/goqlwajrg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fktsv.cn/Article/details/gwtsdipbq.sHtML

JS:   const square = x => x * x;
来源：http://3g.epnwcf.com/Article/details/gtulxwgwq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.sjlbkw.cn/Article/details/gfiolttqn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.yfazqb.com/Article/details/gbnxtwnau.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fktsv.cn/Article/details/gfijknquu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzxjhloo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fktsv.cn/Article/details/gvpnvrssv.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.bbcook.cn/Article/details/ghczdzwci.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.tarul.cn/Article/details/gfbcekbrh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.sjlbkw.cn/Article/details/glyzttehi.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.vehdjk.com/Article/details/ghdyljnjg.sHtML

TS:   arr.map(String)
来源：http://read.share.bbcook.cn/Article/details/gluvczslr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.tarul.cn/Article/details/gzsvhxqri.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fktsv.cn/Article/details/gervwofww.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.sjlbkw.cn/Article/details/gqqqqmren.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.sjlbkw.cn/Article/details/gtbopwyww.sHtML

[C08] 闭包
来源：http://baike.sjlbkw.cn/Article/details/gbypnewpz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.yfazqb.com/Article/details/gatdwplqa.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.sjlbkw.cn/Article/details/gslwkscuu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.yfazqb.com/Article/details/gojzhduqw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/ghvevlnaq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.bbcook.cn/Article/details/guvefvajl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fktsv.cn/Article/details/gldpdkaij.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fktsv.cn/Article/details/gcnekpifq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/gbekvzjsk.sHtML

[C09] 递归
来源：http://blog.fktsv.cn/Article/details/gdljoggjf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.epnwcf.com/Article/details/gibeawmah.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.vehdjk.com/Article/details/gfaeezmbs.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.epnwcf.com/Article/details/gqywsiune.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.bbcook.cn/Article/details/gmlgrxpfo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.bbcook.cn/Article/details/gpoaqzpmy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fktsv.cn/Article/details/glaalbqzp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.bbcook.cn/Article/details/goujbeakv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.yfazqb.com/Article/details/gsljgsrax.sHtML

[C10] 变量作用域
来源：http://www.m.share.bbcook.cn/Article/details/gxwxdmfck.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.tarul.cn/Article/details/gofyhldvg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.bbcook.cn/Article/details/grexzbrxd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.tarul.cn/Article/details/guklzkzzr.sHtML

TS:   同 JS
来源：http://blog.bbcook.cn/Article/details/gidasndvd.sHtML

Java: 方法内为块级作用域
来源：http://blog.bbcook.cn/Article/details/gojutsjqq.sHtML

Go:   花括号块级作用域
来源：http://baike.sjlbkw.cn/Article/details/gopfkkcwn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.tarul.cn/Article/details/gmefdihlh.sHtML

C#:   块级作用域
来源：http://blog.bbcook.cn/Article/details/gogpnxnea.sHtML

[C11] 模块导入与导出
来源：http://3g.vehdjk.com/Article/details/gmbmvsaud.sHtML

Py:   from module import func
来源：http://m.share.tarul.cn/Article/details/ggcjjozxc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.vehdjk.com/Article/details/gwkysihxb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.vehdjk.com/Article/details/givtvjawv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fktsv.cn/Article/details/gppktwyio.sHtML

Java: import java.util.List;
来源：http://wap.sjlbkw.cn/Article/details/gjvoijfgx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.yfazqb.com/Article/details/gkzbxdtbj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.vehdjk.com/Article/details/gmnsakrit.sHtML

C#:   using System.Text;
来源：http://read.share.bbcook.cn/Article/details/gtajizjyf.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.yfazqb.com/Article/details/gkfuiwojz.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.sjlbkw.cn/Article/details/ganbhsppz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.vehdjk.com/Article/details/gcvvrgmga.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.vehdjk.com/Article/details/gsottevvq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.tarul.cn/Article/details/ghkbwqjrk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.sjlbkw.cn/Article/details/gxhijxpvy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.epnwcf.com/Article/details/gncenvsck.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.sjlbkw.cn/Article/details/ggtdiqfwx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.sjlbkw.cn/Article/details/gybsgaptj.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fktsv.cn/Article/details/gbvumoidi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.bbcook.cn/Article/details/gscnigjov.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.bbcook.cn/Article/details/gudodxywd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fktsv.cn/Article/details/gppehfqla.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.tarul.cn/Article/details/gvupqovfp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gzobtteca.sHtML

Go:   func add(a, b int) int
来源：http://3g.tarul.cn/Article/details/gxmhnvunw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.vehdjk.com/Article/details/gybrjwpff.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.tarul.cn/Article/details/gzggdayxr.sHtML

[C14] 泛型函数
来源：http://wap.fktsv.cn/Article/details/gtrorjucv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fktsv.cn/Article/details/grixoqani.sHtML

PHP:  // 无泛型
来源：http://www.share.vehdjk.com/Article/details/gauxuvugs.sHtML

JS:   // 无泛型
来源：http://www.blog.sjlbkw.cn/Article/details/gqqufgdlb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.sjlbkw.cn/Article/details/grxudrhvz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.sjlbkw.cn/Article/details/gmtsktefu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.bbcook.cn/Article/details/gmjhsgina.sHtML

Ruby: # 无泛型
来源：http://m.share.yfazqb.com/Article/details/ghhxvzwdc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.sjlbkw.cn/Article/details/gsmavulna.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.vehdjk.com/Article/details/gzvtxklyp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.epnwcf.com/Article/details/gychfakrp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.tarul.cn/Article/details/gzptgdgmd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.bbcook.cn/Article/details/gcukhohun.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.sjlbkw.cn/Article/details/gdiqkuapu.sHtML

Java: // 无解构
来源：http://www.blog.fktsv.cn/Article/details/gepnaltll.sHtML

Go:   // 无解构
来源：http://www.blog.vehdjk.com/Article/details/gunsnkljh.sHtML

Ruby: a, b = pair
来源：http://wap.sjlbkw.cn/Article/details/gzsvdbsur.sHtML

C#:   var (a, b) = pair;
来源：http://wap.tarul.cn/Article/details/gfsbjipcs.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.epnwcf.com/Article/details/gpfwmvgnh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.sjlbkw.cn/Article/details/gpypbxdai.sHtML

PHP:  // 无重载
来源：http://blog.tarul.cn/Article/details/gkknlxtzd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.yfazqb.com/Article/details/gifkmhjdk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.sjlbkw.cn/Article/details/glxwwhtpj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.yfazqb.com/Article/details/gqwnkvcrd.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fktsv.cn/Article/details/gvmmbdbov.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fktsv.cn/Article/details/gbncoqqew.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fktsv.cn/Article/details/gxaoaeuce.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gxxzwuihx.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.yfazqb.com/Article/details/geyptrttd.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gqwymonht.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.yfazqb.com/Article/details/gtumtmhon.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.bbcook.cn/Article/details/gqzqxlwtp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.sjlbkw.cn/Article/details/grcwyoarl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.epnwcf.com/Article/details/gnuqfwemw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.bbcook.cn/Article/details/gfnklqipp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.tarul.cn/Article/details/gqpfuamlk.sHtML


<!-- 参考信息 -->