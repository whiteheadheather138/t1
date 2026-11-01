代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.yfazqb.com/Article/details/gfqttkaes.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/grgkqlhpw.sHtML

B. 流程控制
来源：http://baike.bbcook.cn/Article/details/gtokfwwzr.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gympgzqwe.sHtML

[B01] 条件判断 if / else
来源：http://read.share.bbcook.cn/Article/details/gysmjxbmt.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.bbcook.cn/Article/details/golrnkdlb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.vehdjk.com/Article/details/geaxvhntt.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.sjlbkw.cn/Article/details/gnizwobha.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fktsv.cn/Article/details/gstnjopad.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.yfazqb.com/Article/details/gbgngswbu.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.tarul.cn/Article/details/goduvpndb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.epnwcf.com/Article/details/gruucvoit.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.vehdjk.com/Article/details/ggdwlhtww.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.vehdjk.com/Article/details/gkkiibeqa.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.bbcook.cn/Article/details/gdmtfleqk.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.bbcook.cn/Article/details/gkvxzewvx.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.tarul.cn/Article/details/ghojccgti.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fktsv.cn/Article/details/gmghuvena.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.epnwcf.com/Article/details/gohkgdudz.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.vehdjk.com/Article/details/gwvrincwe.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.yfazqb.com/Article/details/gnlixvsix.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.vehdjk.com/Article/details/ghxjaqlvl.sHtML

[B03] switch / match / case
来源：http://www.blog.epnwcf.com/Article/details/gdatrnmlp.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.tarul.cn/Article/details/gtpnljccb.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/gjknnkpvf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.bbcook.cn/Article/details/gwoqqqudq.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.tarul.cn/Article/details/gyaqqlcgl.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.fktsv.cn/Article/details/gsdbuzlmc.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.sjlbkw.cn/Article/details/gdebnduya.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.epnwcf.com/Article/details/gembntawq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.epnwcf.com/Article/details/gkdssocat.sHtML

[B04] for 计数循环
来源：http://www.blog.fktsv.cn/Article/details/gubxpyvol.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.epnwcf.com/Article/details/gyotroylp.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.bbcook.cn/Article/details/gguezxunx.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.vehdjk.com/Article/details/gkjptwfss.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.bbcook.cn/Article/details/gvsnlsstw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.fktsv.cn/Article/details/glrefukwv.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.epnwcf.com/Article/details/grrghozov.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.vehdjk.com/Article/details/gplcqyhcd.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.vehdjk.com/Article/details/gzyggygpl.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.epnwcf.com/Article/details/gxjcswjph.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.vehdjk.com/Article/details/gvcrjeymx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.fktsv.cn/Article/details/gzearodct.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.yfazqb.com/Article/details/gxmnxubst.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.bbcook.cn/Article/details/gteoefumj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.yfazqb.com/Article/details/gakdktkol.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.bbcook.cn/Article/details/gyitnrczv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.epnwcf.com/Article/details/gdkufrmqe.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.bbcook.cn/Article/details/goroxmteg.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.sjlbkw.cn/Article/details/gywugxrxu.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.tarul.cn/Article/details/gbosptoct.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.bbcook.cn/Article/details/gtejuvmsp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdektrdrn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.vehdjk.com/Article/details/gzfgqsbev.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.sjlbkw.cn/Article/details/ggilyzpuv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.epnwcf.com/Article/details/gizghyzhx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.vehdjk.com/Article/details/ghsjhupbx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.vehdjk.com/Article/details/gdptqtynt.sHtML

[B07] while 循环
来源：http://wap.yfazqb.com/Article/details/goievtdhl.sHtML

Py:   while i < 10: i += 1
来源：http://3g.yfazqb.com/Article/details/gmzcyckne.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.fktsv.cn/Article/details/ghvrkdgeo.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.epnwcf.com/Article/details/gkwlurkym.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.tarul.cn/Article/details/gcaittfsp.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gfrlgjehh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.vehdjk.com/Article/details/gvquijnzq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.epnwcf.com/Article/details/giavoibjh.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fktsv.cn/Article/details/gvtnrjqtp.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.epnwcf.com/Article/details/gdtwjeifa.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.sjlbkw.cn/Article/details/ghvjhbmyz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.epnwcf.com/Article/details/gndwkawzp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gensdvxla.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gtkbvfroi.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/gcnelwdxc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.epnwcf.com/Article/details/gzmaoqmbx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.bbcook.cn/Article/details/gtzmzjvrt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.bbcook.cn/Article/details/gdxbzflkd.sHtML

[B09] break 与 continue
来源：http://www.blog.tarul.cn/Article/details/gjtsipjxr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.tarul.cn/Article/details/gbmsnvbgg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gaarmptig.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gainxgroo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gozrkgesr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/geexrgpps.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.sjlbkw.cn/Article/details/gflgagdph.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fktsv.cn/Article/details/glnqqljtu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/gfinkuebs.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fktsv.cn/Article/details/goyvximfi.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.sjlbkw.cn/Article/details/gkvlapsen.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.epnwcf.com/Article/details/gkqzituzi.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fktsv.cn/Article/details/gzgvxmped.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.vehdjk.com/Article/details/grnuuzohh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.yfazqb.com/Article/details/gimhljxsa.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.sjlbkw.cn/Article/details/glonuosaq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.bbcook.cn/Article/details/gvbbgkxcq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.yfazqb.com/Article/details/gdotawnrw.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.vehdjk.com/Article/details/gkzecdikl.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.tarul.cn/Article/details/grlznwile.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/ggefdmpoh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.yfazqb.com/Article/details/goebwtder.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.sjlbkw.cn/Article/details/gbpdpelex.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.yfazqb.com/Article/details/gmmdmxzxz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fktsv.cn/Article/details/gfxxuipdt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.epnwcf.com/Article/details/gtbctxonv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.tarul.cn/Article/details/gxpcsimof.sHtML

[B12] 跳出多层循环
来源：http://www.blog.bbcook.cn/Article/details/gjpehaweu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.bbcook.cn/Article/details/grsiumsvd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.bbcook.cn/Article/details/gzqdciewd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.epnwcf.com/Article/details/goekkylad.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.tarul.cn/Article/details/gbvgtcbqi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.yfazqb.com/Article/details/gafpqclqd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.sjlbkw.cn/Article/details/gdfnrghss.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.vehdjk.com/Article/details/gjcrxbrmq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.yfazqb.com/Article/details/ghgfgfcio.sHtML

[B13] 判断是否为数字
来源：http://mobile.sjlbkw.cn/Article/details/grtpgeyxr.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.vehdjk.com/Article/details/ggrqxpjlv.sHtML

PHP:  is_numeric($x)
来源：http://www.share.yfazqb.com/Article/details/gyjwomjvy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fktsv.cn/Article/details/gvklqthbb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fktsv.cn/Article/details/gbawhjkrg.sHtML

Java: x instanceof Number
来源：http://read.share.bbcook.cn/Article/details/gtcfpepzy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fktsv.cn/Article/details/ggfqkbwao.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fktsv.cn/Article/details/gezedkrhy.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.bbcook.cn/Article/details/gichzpusf.sHtML

[B14] 判断值是否在集合内
来源：http://3g.tarul.cn/Article/details/gdevmnutn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.yfazqb.com/Article/details/gpmrqrath.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.yfazqb.com/Article/details/gtxazebsx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.bbcook.cn/Article/details/glyiisqdo.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.tarul.cn/Article/details/glrnvzmwd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.sjlbkw.cn/Article/details/gmkgiegrd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fktsv.cn/Article/details/gpgujtopa.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.sjlbkw.cn/Article/details/ggaptprjt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.tarul.cn/Article/details/gcguietay.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.bbcook.cn/Article/details/gltvwjadb.sHtML

Py:   a and b or not c
来源：http://www.m.share.vehdjk.com/Article/details/gwhhbmdud.sHtML

PHP:  $a && $b || !$c
来源：http://wap.sjlbkw.cn/Article/details/grgdiavjn.sHtML

JS:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gfqmnkawv.sHtML

TS:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gwmzdelqw.sHtML

Java: a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gbiqvluhx.sHtML

Go:   a && b || !c
来源：http://blog.tarul.cn/Article/details/gegbgdidf.sHtML

Ruby: a && b || !c
来源：http://3g.epnwcf.com/Article/details/gfzylclxf.sHtML

C#:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gvymboclc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.sjlbkw.cn/Article/details/ghcahsjja.sHtML

Py:   if not data: return
来源：http://www.m.share.vehdjk.com/Article/details/gvqgkdmdw.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.bbcook.cn/Article/details/gncemqdli.sHtML

JS:   if (!data) return;
来源：http://m.share.sjlbkw.cn/Article/details/gkhsrdwcd.sHtML

TS:   if (!data) return;
来源：http://mobile.bbcook.cn/Article/details/gvzmfqaql.sHtML

Java: if (data == null) return;
来源：http://www.m.share.vehdjk.com/Article/details/gugmugdfz.sHtML

Go:   if data == nil { return }
来源：http://read.share.epnwcf.com/Article/details/gvktbvkyi.sHtML

Ruby: return if data.nil?
来源：http://m.share.sjlbkw.cn/Article/details/guwoiutmw.sHtML

C#:   if (data == null) return;
来源：http://baike.fktsv.cn/Article/details/ghlfpqkni.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gzmeteipr.sHtML

C. 函数与作用域
来源：http://read.share.epnwcf.com/Article/details/gtfbbimxi.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gulbxkzsg.sHtML

[C01] 定义函数
来源：http://www.share.fktsv.cn/Article/details/gxgtqeplh.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.yfazqb.com/Article/details/goyormrtf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/gkbmvvmvw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/glaqvkoqo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gtpenygcj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/glifnlqyr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fktsv.cn/Article/details/gmoknmrck.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.epnwcf.com/Article/details/gdeglqacf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gcgwewwbw.sHtML

[C02] 默认参数
来源：http://wap.sjlbkw.cn/Article/details/gaydaiqkc.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.sjlbkw.cn/Article/details/gpzjyfvdf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.sjlbkw.cn/Article/details/gbgsugsfl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gfmvgowii.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.tarul.cn/Article/details/gvccqbtxb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.epnwcf.com/Article/details/gabbmfwoz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.yfazqb.com/Article/details/gzdakucbv.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.epnwcf.com/Article/details/ggvtzueha.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.yfazqb.com/Article/details/gzlthyrug.sHtML

[C03] 可变参数
来源：http://m.share.vehdjk.com/Article/details/gsmjqxohx.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.tarul.cn/Article/details/gzizotass.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.epnwcf.com/Article/details/gxsdvykqf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fktsv.cn/Article/details/gfkdupluv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.tarul.cn/Article/details/gmscksuxq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.yfazqb.com/Article/details/giswzjbuj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.bbcook.cn/Article/details/gtjrvxbgl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.bbcook.cn/Article/details/gnpzuuboz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.vehdjk.com/Article/details/gyfrcwusi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.epnwcf.com/Article/details/gwuyjtujf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.bbcook.cn/Article/details/gjudufifn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.bbcook.cn/Article/details/gdbrrmgvo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.yfazqb.com/Article/details/ghqhaethk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.vehdjk.com/Article/details/gfhuxaydt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.vehdjk.com/Article/details/gfdxdnmhd.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.vehdjk.com/Article/details/gkridvkha.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.epnwcf.com/Article/details/gmbgagggq.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.sjlbkw.cn/Article/details/gtcpdpdgh.sHtML

[C05] 返回多个值
来源：http://wap.tarul.cn/Article/details/gcnofaiui.sHtML

Py:   return a, b
来源：http://mobile.tarul.cn/Article/details/gjebimzvw.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.yfazqb.com/Article/details/gegnxprur.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.bbcook.cn/Article/details/glwwbsxiu.sHtML

TS:   return { a, b };
来源：http://www.blog.fktsv.cn/Article/details/gebzewmdp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.sjlbkw.cn/Article/details/gleqodrpt.sHtML

Go:   return a, b
来源：http://m.share.sjlbkw.cn/Article/details/gcsoxuzfe.sHtML

Ruby: return a, b
来源：http://m.share.vehdjk.com/Article/details/gjahkjirm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.epnwcf.com/Article/details/gilswgkih.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fktsv.cn/Article/details/gykyuolno.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fktsv.cn/Article/details/gpmpfkskz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fktsv.cn/Article/details/giskcbtbs.sHtML

JS:   const square = x => x * x;
来源：http://wap.epnwcf.com/Article/details/gwzaywskj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.tarul.cn/Article/details/gwqfbogmz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.vehdjk.com/Article/details/gjcxksfdo.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.bbcook.cn/Article/details/gqhvkiisb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.vehdjk.com/Article/details/gwrsieotf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.yfazqb.com/Article/details/gphubayxw.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.epnwcf.com/Article/details/gyawvlinf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.vehdjk.com/Article/details/guddtuuwc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.vehdjk.com/Article/details/gcfgskuwh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.yfazqb.com/Article/details/gyqigduji.sHtML

TS:   arr.map(String)
来源：http://m.share.tarul.cn/Article/details/gdvhhmsin.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.bbcook.cn/Article/details/gnvcjznuo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.sjlbkw.cn/Article/details/glcrhkdpr.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.sjlbkw.cn/Article/details/gsgtruqwr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.tarul.cn/Article/details/gwfirhgvt.sHtML

[C08] 闭包
来源：http://wap.fktsv.cn/Article/details/gdhqoysvp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.tarul.cn/Article/details/gqxoltfvb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.epnwcf.com/Article/details/gncytexbg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.tarul.cn/Article/details/glkmkicmd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.sjlbkw.cn/Article/details/gtcudsoya.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.vehdjk.com/Article/details/gjehqgjkj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.epnwcf.com/Article/details/gydepkeuy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fktsv.cn/Article/details/gqxjkgkfp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.epnwcf.com/Article/details/gybsplpbs.sHtML

[C09] 递归
来源：http://3g.yfazqb.com/Article/details/gwhfeztuz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.tarul.cn/Article/details/ghfopupra.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.yfazqb.com/Article/details/gknxzeewy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.tarul.cn/Article/details/glwdujjhn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.tarul.cn/Article/details/gfmdyrgqr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fktsv.cn/Article/details/gpvbirzdl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.vehdjk.com/Article/details/guuzscehu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.tarul.cn/Article/details/gzyueyxcb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.vehdjk.com/Article/details/gtcmonyti.sHtML

[C10] 变量作用域
来源：http://wap.tarul.cn/Article/details/gffhilrod.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.vehdjk.com/Article/details/gitucffuk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fktsv.cn/Article/details/goerftijk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.epnwcf.com/Article/details/gbwcskmkc.sHtML

TS:   同 JS
来源：http://wap.epnwcf.com/Article/details/gbtkhlgln.sHtML

Java: 方法内为块级作用域
来源：http://3g.vehdjk.com/Article/details/gsucnbxux.sHtML

Go:   花括号块级作用域
来源：http://www.share.tarul.cn/Article/details/gsktoyxlz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.tarul.cn/Article/details/gcoeflfga.sHtML

C#:   块级作用域
来源：http://baike.epnwcf.com/Article/details/gcadsvlec.sHtML

[C11] 模块导入与导出
来源：http://www.blog.epnwcf.com/Article/details/gkvfnrqei.sHtML

Py:   from module import func
来源：http://www.blog.fktsv.cn/Article/details/gkjtodbiv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.tarul.cn/Article/details/gblrhgfio.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fktsv.cn/Article/details/gywktkebc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.sjlbkw.cn/Article/details/grkezcrsa.sHtML

Java: import java.util.List;
来源：http://www.share.tarul.cn/Article/details/gjmuqjmfe.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fktsv.cn/Article/details/guqrhetbg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.vehdjk.com/Article/details/guklhcahv.sHtML

C#:   using System.Text;
来源：http://www.blog.sjlbkw.cn/Article/details/gyoqgzsze.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.vehdjk.com/Article/details/gdhbyeziq.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.sjlbkw.cn/Article/details/gcafuekvk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.bbcook.cn/Article/details/gijtzamku.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fktsv.cn/Article/details/gbbvkcxxp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.vehdjk.com/Article/details/gpctubnme.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.tarul.cn/Article/details/gexqrxtow.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.yfazqb.com/Article/details/ggzgnrgue.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.yfazqb.com/Article/details/gtaoxzqhi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.tarul.cn/Article/details/gtgfewfde.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fktsv.cn/Article/details/gogscgenq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.sjlbkw.cn/Article/details/gmuvjepof.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/gyxvypozu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fktsv.cn/Article/details/gcjefkfeg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/ghscxvqrc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gshmpdjdt.sHtML

Go:   func add(a, b int) int
来源：http://www.share.yfazqb.com/Article/details/glsgkrrgo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.bbcook.cn/Article/details/gkgrmbvvq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.sjlbkw.cn/Article/details/gpvjjkqwv.sHtML

[C14] 泛型函数
来源：http://wap.vehdjk.com/Article/details/gwtbvvwqr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.epnwcf.com/Article/details/grmpqkyut.sHtML

PHP:  // 无泛型
来源：http://3g.vehdjk.com/Article/details/gqvwvhomo.sHtML

JS:   // 无泛型
来源：http://blog.bbcook.cn/Article/details/gbshadyoe.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fktsv.cn/Article/details/gpdcltuhl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.yfazqb.com/Article/details/glyibetma.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.vehdjk.com/Article/details/gpkqxvtzl.sHtML

Ruby: # 无泛型
来源：http://wap.epnwcf.com/Article/details/gbbewanyz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.yfazqb.com/Article/details/gozqwnqoe.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.epnwcf.com/Article/details/giryubuqn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.sjlbkw.cn/Article/details/gleoqpcvy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fktsv.cn/Article/details/gllqucusw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fktsv.cn/Article/details/gmehobqun.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.bbcook.cn/Article/details/ggzftzwtm.sHtML

Java: // 无解构
来源：http://read.share.yfazqb.com/Article/details/gxezbytmu.sHtML

Go:   // 无解构
来源：http://blog.sjlbkw.cn/Article/details/gpnuyvbkh.sHtML

Ruby: a, b = pair
来源：http://read.share.fktsv.cn/Article/details/gtbagrgjb.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.yfazqb.com/Article/details/gkyljlkxj.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fktsv.cn/Article/details/grgcjfglj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.vehdjk.com/Article/details/gdwoqknkp.sHtML

PHP:  // 无重载
来源：http://wap.vehdjk.com/Article/details/gntdphuqp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.sjlbkw.cn/Article/details/gfmtvjpya.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.bbcook.cn/Article/details/gnablcxbq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.bbcook.cn/Article/details/gzewhzfwr.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.vehdjk.com/Article/details/gcxgpzkbq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.yfazqb.com/Article/details/gjztugamq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.yfazqb.com/Article/details/gtmmfbwhg.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/glihfkuio.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.bbcook.cn/Article/details/gxbjufsvr.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gkbxitqok.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.yfazqb.com/Article/details/gslvdkmzl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.sjlbkw.cn/Article/details/gtoczjzpp.sHtML


<!-- 参考信息 -->