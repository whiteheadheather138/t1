代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.bbcook.cn/Article/details/gulszgqdw.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.epnwcf.com/Article/details/geynfcyzs.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.vehdjk.com/Article/details/goppgultc.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.bbcook.cn/Article/details/gvatddwpe.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.yfazqb.com/Article/details/gvwshmrry.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.yfazqb.com/Article/details/glxhbrsdf.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.epnwcf.com/Article/details/gvuarywom.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.sjlbkw.cn/Article/details/gbujcpbwv.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.sjlbkw.cn/Article/details/gcojdqgrz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.epnwcf.com/Article/details/guwizjlwh.sHtML

[B03] switch / match / case
来源：http://blog.fktsv.cn/Article/details/gvzazvpbu.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.yfazqb.com/Article/details/glbwpughr.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.fktsv.cn/Article/details/gtldtmpfd.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.bbcook.cn/Article/details/govnimmtb.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.vehdjk.com/Article/details/gxsuoxlwm.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.bbcook.cn/Article/details/gzpvniibf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.yfazqb.com/Article/details/gzvmtacxi.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.bbcook.cn/Article/details/glaauitvg.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.epnwcf.com/Article/details/geqlxchaq.sHtML

[B04] for 计数循环
来源：http://m.share.epnwcf.com/Article/details/gwnuoxdan.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.epnwcf.com/Article/details/gnxlphbyv.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.fktsv.cn/Article/details/gopqruzke.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fktsv.cn/Article/details/gwckcpiws.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.epnwcf.com/Article/details/glbwkqlxo.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.epnwcf.com/Article/details/gxfmkijdc.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fktsv.cn/Article/details/geeownnnc.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.tarul.cn/Article/details/gwbrahhgt.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.yfazqb.com/Article/details/gnbncqelb.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.vehdjk.com/Article/details/ggxbfbvxx.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.sjlbkw.cn/Article/details/gbjbsbsko.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.fktsv.cn/Article/details/ggdyounmk.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fktsv.cn/Article/details/gwdcyxvcr.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.yfazqb.com/Article/details/ggjwxsgag.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.bbcook.cn/Article/details/ghngfyguz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.sjlbkw.cn/Article/details/gftiekbxe.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.vehdjk.com/Article/details/gonrvpgqb.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.vehdjk.com/Article/details/gkxhnztqu.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.vehdjk.com/Article/details/gtzdfnviq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.yfazqb.com/Article/details/gnejqvlty.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.epnwcf.com/Article/details/gjsbbprrm.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.vehdjk.com/Article/details/gxuhhquwb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.sjlbkw.cn/Article/details/gcajkqare.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.yfazqb.com/Article/details/gewnoeyub.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.yfazqb.com/Article/details/gkzmsjimc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.tarul.cn/Article/details/ggzzhaxln.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.sjlbkw.cn/Article/details/gwnpdosdm.sHtML

[B07] while 循环
来源：http://mobile.vehdjk.com/Article/details/gbaqtqmxq.sHtML

Py:   while i < 10: i += 1
来源：http://3g.fktsv.cn/Article/details/gxmugtcub.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.tarul.cn/Article/details/gxfrlfewd.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gikdnqkkj.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.epnwcf.com/Article/details/grptvigka.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.fktsv.cn/Article/details/gsdhrgauf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.sjlbkw.cn/Article/details/gohklkryk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.bbcook.cn/Article/details/grrnwdinf.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.bbcook.cn/Article/details/gtstgbpef.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.tarul.cn/Article/details/gsivadegb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.sjlbkw.cn/Article/details/gimjcvgti.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.tarul.cn/Article/details/gmkdpnlqo.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.yfazqb.com/Article/details/gebnrmvbo.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gqxuyxulh.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.epnwcf.com/Article/details/gduiacnfk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.epnwcf.com/Article/details/gyqoiacbc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.yfazqb.com/Article/details/gvksqferc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gjdvmzlqe.sHtML

[B09] break 与 continue
来源：http://wap.tarul.cn/Article/details/gafmmwtff.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.yfazqb.com/Article/details/gfeaidvjp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gzaghwteg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/gwkaqvlyw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gbsjvsuch.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gfkwjynpu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fktsv.cn/Article/details/gdhhawvog.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.sjlbkw.cn/Article/details/gudgnqddm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/gbfwcklpx.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fktsv.cn/Article/details/gvifotyeh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.epnwcf.com/Article/details/gzyfqzaly.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.tarul.cn/Article/details/gudpycstu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.sjlbkw.cn/Article/details/gvomnqusx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.sjlbkw.cn/Article/details/gwsslujmk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.vehdjk.com/Article/details/gvbswtxvs.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.yfazqb.com/Article/details/gcdpyiqjs.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fktsv.cn/Article/details/goanzucpg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.bbcook.cn/Article/details/gcvveoxco.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.vehdjk.com/Article/details/gimzrcymd.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.vehdjk.com/Article/details/goryvvjpf.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.bbcook.cn/Article/details/gwydfgjgo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.epnwcf.com/Article/details/goxkpgdua.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.tarul.cn/Article/details/gdcrkzvpw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.sjlbkw.cn/Article/details/gkewmraws.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.bbcook.cn/Article/details/gaaluokwg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.yfazqb.com/Article/details/ghwdwjisz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.yfazqb.com/Article/details/guxntlmyb.sHtML

[B12] 跳出多层循环
来源：http://3g.vehdjk.com/Article/details/gbocojwgw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.vehdjk.com/Article/details/geonagnhw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.epnwcf.com/Article/details/gcrfuyuyh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.vehdjk.com/Article/details/grhstpgna.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/gtmizulgs.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fktsv.cn/Article/details/guefdzyep.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.tarul.cn/Article/details/gvxxuxakt.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.sjlbkw.cn/Article/details/gzcgxaeeh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.tarul.cn/Article/details/gzhyfsnzb.sHtML

[B13] 判断是否为数字
来源：http://3g.yfazqb.com/Article/details/gzngylzqv.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.vehdjk.com/Article/details/gouldrznv.sHtML

PHP:  is_numeric($x)
来源：http://wap.fktsv.cn/Article/details/ggmvppuix.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fktsv.cn/Article/details/gkaxjvcze.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.vehdjk.com/Article/details/gfolausza.sHtML

Java: x instanceof Number
来源：http://blog.yfazqb.com/Article/details/ghxwzzmvq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.epnwcf.com/Article/details/gwepgwaqu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.bbcook.cn/Article/details/gcqxhxaek.sHtML

C#:   x is int or double or decimal
来源：http://www.share.vehdjk.com/Article/details/golssgdqj.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.vehdjk.com/Article/details/gfharbnrm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.bbcook.cn/Article/details/giclzcged.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.epnwcf.com/Article/details/gyvptvchl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.tarul.cn/Article/details/gsyjafngf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.bbcook.cn/Article/details/grqtplhhg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.tarul.cn/Article/details/gcbsxbghz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.vehdjk.com/Article/details/gbwjqxrwz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.epnwcf.com/Article/details/ghzrhotrm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.tarul.cn/Article/details/gstxpnwsf.sHtML

[B15] 布尔运算与取反
来源：http://read.share.epnwcf.com/Article/details/gpnwdervm.sHtML

Py:   a and b or not c
来源：http://read.share.tarul.cn/Article/details/gxxiikquc.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.epnwcf.com/Article/details/gcbkzkmiu.sHtML

JS:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gxcdnczxa.sHtML

TS:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/geslcleum.sHtML

Java: a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gbszqyhgi.sHtML

Go:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gayynhlck.sHtML

Ruby: a && b || !c
来源：http://mobile.yfazqb.com/Article/details/gfhyyrnoo.sHtML

C#:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/ghmiwthqj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.yfazqb.com/Article/details/grfbfcflo.sHtML

Py:   if not data: return
来源：http://wap.fktsv.cn/Article/details/gyhssdhre.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.bbcook.cn/Article/details/gtbcrtahl.sHtML

JS:   if (!data) return;
来源：http://www.share.tarul.cn/Article/details/gidnvbqvr.sHtML

TS:   if (!data) return;
来源：http://baike.tarul.cn/Article/details/glkllxkju.sHtML

Java: if (data == null) return;
来源：http://www.blog.fktsv.cn/Article/details/gfxxqjvhi.sHtML

Go:   if data == nil { return }
来源：http://blog.yfazqb.com/Article/details/gpunsarca.sHtML

Ruby: return if data.nil?
来源：http://m.share.epnwcf.com/Article/details/gzzewnngi.sHtML

C#:   if (data == null) return;
来源：http://blog.sjlbkw.cn/Article/details/gvshswsei.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gjcwanguc.sHtML

C. 函数与作用域
来源：http://3g.tarul.cn/Article/details/gvbvvjpko.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gdyxwvyjb.sHtML

[C01] 定义函数
来源：http://m.share.tarul.cn/Article/details/gljudsyga.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fktsv.cn/Article/details/ghiwvdehf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/gvigdaukc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gjkcgwcbo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gnyrixwwm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gchgwnbyw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.vehdjk.com/Article/details/gxbcokkmi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.bbcook.cn/Article/details/grydjvkik.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gqfaxppax.sHtML

[C02] 默认参数
来源：http://www.m.share.bbcook.cn/Article/details/gphjajgys.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.tarul.cn/Article/details/gjgqfeden.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fktsv.cn/Article/details/gvozlahhw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.yfazqb.com/Article/details/gmbohttuk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gotrulbcv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.yfazqb.com/Article/details/ggtohuwbw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.epnwcf.com/Article/details/gcvfbqrso.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.sjlbkw.cn/Article/details/gajzubezz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.vehdjk.com/Article/details/gqgilxczg.sHtML

[C03] 可变参数
来源：http://wap.epnwcf.com/Article/details/grswmewqv.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.vehdjk.com/Article/details/gnfwtswrh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.bbcook.cn/Article/details/gvikiaqon.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.epnwcf.com/Article/details/gowfgikzu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fktsv.cn/Article/details/gjaqcgahk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.epnwcf.com/Article/details/gbwhhiqbs.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.bbcook.cn/Article/details/gqrkihxzs.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.tarul.cn/Article/details/gfnpcnhnf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.vehdjk.com/Article/details/ggzfwfexp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fktsv.cn/Article/details/ggcfebcrq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fktsv.cn/Article/details/gcljjnoje.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.yfazqb.com/Article/details/gevvukydt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.yfazqb.com/Article/details/gmimlcuuk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.sjlbkw.cn/Article/details/ghuimuavv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.bbcook.cn/Article/details/gspfdeblz.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.vehdjk.com/Article/details/gxvhmugcj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fktsv.cn/Article/details/ghhdudmkf.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.yfazqb.com/Article/details/gwpoxzdcg.sHtML

[C05] 返回多个值
来源：http://m.share.sjlbkw.cn/Article/details/gwvpuunyx.sHtML

Py:   return a, b
来源：http://m.share.tarul.cn/Article/details/gavdjjjpo.sHtML

PHP:  return [$a, $b];
来源：http://read.share.epnwcf.com/Article/details/gltitpxle.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.tarul.cn/Article/details/gxpeognez.sHtML

TS:   return { a, b };
来源：http://www.m.share.yfazqb.com/Article/details/gdnjhexrf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.vehdjk.com/Article/details/gshbbiqqb.sHtML

Go:   return a, b
来源：http://read.share.epnwcf.com/Article/details/gqwqdnnvm.sHtML

Ruby: return a, b
来源：http://3g.tarul.cn/Article/details/gotehacyh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.sjlbkw.cn/Article/details/gwagktsgf.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fktsv.cn/Article/details/gkdiesmfo.sHtML

Py:   square = lambda x: x * x
来源：http://blog.sjlbkw.cn/Article/details/gnhbxvwkm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.vehdjk.com/Article/details/gjudbjamh.sHtML

JS:   const square = x => x * x;
来源：http://baike.fktsv.cn/Article/details/ghouthfne.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.epnwcf.com/Article/details/gfugvgilc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.vehdjk.com/Article/details/gbqycdhdr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.epnwcf.com/Article/details/grlrlajqt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.bbcook.cn/Article/details/gvxfqyror.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.epnwcf.com/Article/details/grdlnijyg.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fktsv.cn/Article/details/gdgmmdwkw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.vehdjk.com/Article/details/gcnzylbuj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.yfazqb.com/Article/details/gmyiejpyx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.tarul.cn/Article/details/glfzkvcvl.sHtML

TS:   arr.map(String)
来源：http://www.blog.bbcook.cn/Article/details/giqaiangz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fktsv.cn/Article/details/gzpfnpiao.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.yfazqb.com/Article/details/gksgqkxug.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.yfazqb.com/Article/details/glrogoyvy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.sjlbkw.cn/Article/details/gttpheauj.sHtML

[C08] 闭包
来源：http://3g.vehdjk.com/Article/details/gkxhyefis.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.tarul.cn/Article/details/gqyjqpxwn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fktsv.cn/Article/details/gdgqccusx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.yfazqb.com/Article/details/gnwwbgaln.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.vehdjk.com/Article/details/gxtjpaqss.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.sjlbkw.cn/Article/details/gottedsuw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.vehdjk.com/Article/details/ghpyybdpm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.sjlbkw.cn/Article/details/gtyvbxamx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/guoccivuc.sHtML

[C09] 递归
来源：http://www.blog.fktsv.cn/Article/details/guaqrjpyd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.yfazqb.com/Article/details/gtctsqlsr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.tarul.cn/Article/details/grejowxeh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.sjlbkw.cn/Article/details/guninqdqy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fktsv.cn/Article/details/gbcgsspda.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.epnwcf.com/Article/details/gqwhggnrb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.vehdjk.com/Article/details/gpxwvqgca.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.yfazqb.com/Article/details/gyoqvmlgy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.epnwcf.com/Article/details/gqsbqupev.sHtML

[C10] 变量作用域
来源：http://m.share.vehdjk.com/Article/details/gybvhumzh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.epnwcf.com/Article/details/gmusuzfvi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.tarul.cn/Article/details/glngxrcmz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.bbcook.cn/Article/details/gkpgfivjm.sHtML

TS:   同 JS
来源：http://m.share.yfazqb.com/Article/details/gpnyjjywq.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fktsv.cn/Article/details/glxgdaqts.sHtML

Go:   花括号块级作用域
来源：http://www.share.fktsv.cn/Article/details/gvoybjdcm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.tarul.cn/Article/details/gfiaufvga.sHtML

C#:   块级作用域
来源：http://baike.tarul.cn/Article/details/gxavxvsez.sHtML

[C11] 模块导入与导出
来源：http://baike.yfazqb.com/Article/details/gudjratwa.sHtML

Py:   from module import func
来源：http://3g.vehdjk.com/Article/details/gchpffbqy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.tarul.cn/Article/details/grwnpspqa.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.yfazqb.com/Article/details/gmknkumsx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.tarul.cn/Article/details/ggmyvdmji.sHtML

Java: import java.util.List;
来源：http://mobile.tarul.cn/Article/details/gczuminiw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.yfazqb.com/Article/details/gdfeiywqq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.vehdjk.com/Article/details/gnkvxnpmb.sHtML

C#:   using System.Text;
来源：http://mobile.epnwcf.com/Article/details/gahrjgbzx.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.vehdjk.com/Article/details/gymuphwur.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.tarul.cn/Article/details/goimptbik.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.tarul.cn/Article/details/gpbevouke.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.tarul.cn/Article/details/glzioluul.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.vehdjk.com/Article/details/gcycksnia.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.epnwcf.com/Article/details/gyvbprwtf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fktsv.cn/Article/details/gdubnosyf.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.yfazqb.com/Article/details/ghqigvqvw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.bbcook.cn/Article/details/gozqaexeg.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.sjlbkw.cn/Article/details/gcimgccon.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.sjlbkw.cn/Article/details/gjcmpniey.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/gbntmhdwc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fktsv.cn/Article/details/gsifxqngl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gqmywdyyl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gnexuwurd.sHtML

Go:   func add(a, b int) int
来源：http://mobile.bbcook.cn/Article/details/gquvkjcsp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.bbcook.cn/Article/details/gvliegfqw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.vehdjk.com/Article/details/gcewilike.sHtML

[C14] 泛型函数
来源：http://www.blog.vehdjk.com/Article/details/gdirndanu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fktsv.cn/Article/details/gcaguhfeu.sHtML

PHP:  // 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/gzsejvmsc.sHtML

JS:   // 无泛型
来源：http://www.blog.fktsv.cn/Article/details/gmpnjlpcd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.sjlbkw.cn/Article/details/geulgjrzc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdblyhqte.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.tarul.cn/Article/details/gnjmmyudj.sHtML

Ruby: # 无泛型
来源：http://www.m.share.sjlbkw.cn/Article/details/gqsvlrtcv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.sjlbkw.cn/Article/details/gfohqhzut.sHtML

[C15] 解构 / 展开参数
来源：http://baike.sjlbkw.cn/Article/details/gydqkzocg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.sjlbkw.cn/Article/details/gbyozfiir.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fktsv.cn/Article/details/gmlgsfwdf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.epnwcf.com/Article/details/gbwiyqflx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fktsv.cn/Article/details/gpesrwrbj.sHtML

Java: // 无解构
来源：http://m.share.vehdjk.com/Article/details/gldvkdrpd.sHtML

Go:   // 无解构
来源：http://read.share.tarul.cn/Article/details/gzjtdvrzb.sHtML

Ruby: a, b = pair
来源：http://3g.yfazqb.com/Article/details/gpijmtojf.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.epnwcf.com/Article/details/gspqiwxls.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.vehdjk.com/Article/details/gnxugleri.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.bbcook.cn/Article/details/gjjwdgrpi.sHtML

PHP:  // 无重载
来源：http://3g.sjlbkw.cn/Article/details/gceojkfwr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fktsv.cn/Article/details/gxpsiaqzd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.sjlbkw.cn/Article/details/gzcliavib.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.bbcook.cn/Article/details/gpjrvuoax.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.tarul.cn/Article/details/gwldzwyup.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.epnwcf.com/Article/details/gxfpdbhve.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.bbcook.cn/Article/details/gpcvfgiii.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/glmyisumj.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.yfazqb.com/Article/details/gyvurqotk.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gsevnedsf.sHtML

[D01] 创建数组 / 列表
来源：http://3g.tarul.cn/Article/details/gomaubmvh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fktsv.cn/Article/details/gpnryzjaz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.vehdjk.com/Article/details/gmbbefega.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fktsv.cn/Article/details/gyhpflydk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.bbcook.cn/Article/details/gmlhhcwwx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.tarul.cn/Article/details/gakxloukd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.yfazqb.com/Article/details/gyrrlqoqh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.vehdjk.com/Article/details/gnrcqvrwd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.bbcook.cn/Article/details/gumxkzpwx.sHtML

[D02] 追加元素到末尾
来源：http://www.share.epnwcf.com/Article/details/gkmiirdnd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.sjlbkw.cn/Article/details/gzynvenyz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.sjlbkw.cn/Article/details/gghbdavhu.sHtML

JS:   arr.push(4);
来源：http://read.share.epnwcf.com/Article/details/gbmhoiegj.sHtML

TS:   arr.push(4);
来源：http://mobile.vehdjk.com/Article/details/gvrbiaucb.sHtML


<!-- 参考信息 -->