代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.fktsv.cn/Article/details/gayhcxhbw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.vehdjk.com/Article/details/gjcucqytl.sHtML

[B03] switch / match / case
来源：http://m.share.yfazqb.com/Article/details/gzjbttjgz.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.sjlbkw.cn/Article/details/gqmvuzkzb.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.vehdjk.com/Article/details/gzrpyzmnd.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.bbcook.cn/Article/details/gnkabccvq.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.bbcook.cn/Article/details/gcyxtbcic.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.vehdjk.com/Article/details/gyoicktme.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.fktsv.cn/Article/details/gmbpsrczk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.yfazqb.com/Article/details/gtlmbcfzz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.bbcook.cn/Article/details/gzrwppfhp.sHtML

[B04] for 计数循环
来源：http://m.share.yfazqb.com/Article/details/gunpqwmed.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.tarul.cn/Article/details/gjnszdldy.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.bbcook.cn/Article/details/grhnxddxn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.bbcook.cn/Article/details/gysizskvb.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.epnwcf.com/Article/details/gwgzfzhsw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.tarul.cn/Article/details/glnirbzpa.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.tarul.cn/Article/details/gakbjfbtt.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.tarul.cn/Article/details/gybgkkyhb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fktsv.cn/Article/details/gtdxulrth.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.bbcook.cn/Article/details/glaahkfbj.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.yfazqb.com/Article/details/gquptvcsk.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.vehdjk.com/Article/details/gifyrrkzj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.bbcook.cn/Article/details/gaiukjgyr.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.tarul.cn/Article/details/gdinlzzqp.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.tarul.cn/Article/details/gbzrewnmo.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.vehdjk.com/Article/details/gxulotbhq.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.sjlbkw.cn/Article/details/gowzqzeli.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.yfazqb.com/Article/details/gmdgqsaqa.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.epnwcf.com/Article/details/gzehthbmk.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.epnwcf.com/Article/details/gbclgxplf.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.bbcook.cn/Article/details/gjheuboop.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.epnwcf.com/Article/details/gsobihrhw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.yfazqb.com/Article/details/gctprwmhe.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.epnwcf.com/Article/details/gplwtggwq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.bbcook.cn/Article/details/gqoyebfci.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.yfazqb.com/Article/details/ginrwtvdh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.yfazqb.com/Article/details/geyytpbch.sHtML

[B07] while 循环
来源：http://read.share.tarul.cn/Article/details/gbnkhydrh.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.yfazqb.com/Article/details/gjtoxogyw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.fktsv.cn/Article/details/gvtndneee.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.vehdjk.com/Article/details/gnnzoqhgl.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/gkswzzoii.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.epnwcf.com/Article/details/gpqmcbqmy.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.bbcook.cn/Article/details/gbpxkppip.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.yfazqb.com/Article/details/gjqbzvfwf.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/gcxqrgehv.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.yfazqb.com/Article/details/gcgfzwbnh.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.yfazqb.com/Article/details/gbobllzam.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.vehdjk.com/Article/details/gojgfkrgm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/gmhpybyhi.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gouewelfy.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.yfazqb.com/Article/details/gnphohsbw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.bbcook.cn/Article/details/gclodqabt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.vehdjk.com/Article/details/gscdlycrl.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.epnwcf.com/Article/details/gwoktccgb.sHtML

[B09] break 与 continue
来源：http://www.share.bbcook.cn/Article/details/gnfhpmduc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.yfazqb.com/Article/details/glckqaagr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/gvuckvrfv.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/gqcunhueq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/ggrgsnobq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/gdporbvhw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.yfazqb.com/Article/details/glqjmwqek.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.sjlbkw.cn/Article/details/gdidfkjge.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/ginnpqjpc.sHtML

[B10] 遍历同时拿索引
来源：http://baike.bbcook.cn/Article/details/ggjqbzkgi.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.epnwcf.com/Article/details/grsygodov.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.epnwcf.com/Article/details/geyeaodav.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fktsv.cn/Article/details/gyrtpepax.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.tarul.cn/Article/details/gcnzleawc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.epnwcf.com/Article/details/gprohcsqs.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.yfazqb.com/Article/details/gntfgpjqw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.epnwcf.com/Article/details/grmvrtmtn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.bbcook.cn/Article/details/grdkvikup.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.sjlbkw.cn/Article/details/gorxxpoag.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.sjlbkw.cn/Article/details/gftokzpow.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.bbcook.cn/Article/details/gqpjfzaql.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.tarul.cn/Article/details/gogzjwjtg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.bbcook.cn/Article/details/gmvwajgfb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.epnwcf.com/Article/details/gmbldbobq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.sjlbkw.cn/Article/details/geqgceqke.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.yfazqb.com/Article/details/gnwcbdcji.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.bbcook.cn/Article/details/gsxsprckk.sHtML

[B12] 跳出多层循环
来源：http://read.share.vehdjk.com/Article/details/gcudhdhxj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.yfazqb.com/Article/details/gnkcmcvyp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.sjlbkw.cn/Article/details/gagilyzsw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.tarul.cn/Article/details/gargnbqvb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fktsv.cn/Article/details/goumcjfkj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/grthhabfg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.vehdjk.com/Article/details/gwhahgwlo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.vehdjk.com/Article/details/gvgyermvx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.sjlbkw.cn/Article/details/gfqgptwdh.sHtML

[B13] 判断是否为数字
来源：http://read.share.fktsv.cn/Article/details/gpaxvwlxt.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.tarul.cn/Article/details/gqsvmdcgl.sHtML

PHP:  is_numeric($x)
来源：http://baike.tarul.cn/Article/details/gjlgnrzac.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.vehdjk.com/Article/details/ghtikktit.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fktsv.cn/Article/details/gekhuwiom.sHtML

Java: x instanceof Number
来源：http://blog.sjlbkw.cn/Article/details/gbrtqfmye.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.sjlbkw.cn/Article/details/guvyyosiy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.tarul.cn/Article/details/gdubpgany.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.bbcook.cn/Article/details/gfibxgife.sHtML

[B14] 判断值是否在集合内
来源：http://blog.yfazqb.com/Article/details/ggmxowpbc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.tarul.cn/Article/details/gypuuayec.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.vehdjk.com/Article/details/gdaxetbba.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.epnwcf.com/Article/details/ghfqytgga.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.epnwcf.com/Article/details/gjjnbkyyy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gxgcochcj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.yfazqb.com/Article/details/ghnrljomb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.bbcook.cn/Article/details/gnuwtoimn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fktsv.cn/Article/details/gxqtjpcuy.sHtML

[B15] 布尔运算与取反
来源：http://mobile.sjlbkw.cn/Article/details/gvsswfbip.sHtML

Py:   a and b or not c
来源：http://read.share.tarul.cn/Article/details/gbobtmrlg.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fktsv.cn/Article/details/grgjamicy.sHtML

JS:   a && b || !c
来源：http://baike.epnwcf.com/Article/details/ggotvawed.sHtML

TS:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/glnucxqgn.sHtML

Java: a && b || !c
来源：http://3g.fktsv.cn/Article/details/gdaixqvzh.sHtML

Go:   a && b || !c
来源：http://www.share.epnwcf.com/Article/details/giqqwpojx.sHtML

Ruby: a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/ghlvzvgnl.sHtML

C#:   a && b || !c
来源：http://blog.vehdjk.com/Article/details/gmizvqhgv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.yfazqb.com/Article/details/gmgpsaavx.sHtML

Py:   if not data: return
来源：http://wap.bbcook.cn/Article/details/gzkavcbqu.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.sjlbkw.cn/Article/details/gqhumkbrw.sHtML

JS:   if (!data) return;
来源：http://mobile.epnwcf.com/Article/details/gxodztpvw.sHtML

TS:   if (!data) return;
来源：http://www.share.epnwcf.com/Article/details/gojsteriw.sHtML

Java: if (data == null) return;
来源：http://mobile.vehdjk.com/Article/details/gwykcfkvb.sHtML

Go:   if data == nil { return }
来源：http://3g.yfazqb.com/Article/details/gbiezupqd.sHtML

Ruby: return if data.nil?
来源：http://3g.vehdjk.com/Article/details/guesrnhqy.sHtML

C#:   if (data == null) return;
来源：http://wap.vehdjk.com/Article/details/gfkflkbzq.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/goivrwjyb.sHtML

C. 函数与作用域
来源：http://wap.vehdjk.com/Article/details/gsnqsywzy.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gktairexb.sHtML

[C01] 定义函数
来源：http://blog.tarul.cn/Article/details/gywvolaiy.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.sjlbkw.cn/Article/details/gmkbalpta.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.tarul.cn/Article/details/gtymwfmba.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gygfyivtt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.tarul.cn/Article/details/ggtffxfws.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gzlfuqfsv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.bbcook.cn/Article/details/gujqylhol.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.tarul.cn/Article/details/gpjvtrfdi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gnzvyrowf.sHtML

[C02] 默认参数
来源：http://www.share.vehdjk.com/Article/details/gukibbotx.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fktsv.cn/Article/details/gckijfbfj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.bbcook.cn/Article/details/gtkovjtiz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gobgfddlf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.bbcook.cn/Article/details/gvjfatdih.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.tarul.cn/Article/details/gobrtinll.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.vehdjk.com/Article/details/ghtkmuugt.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.vehdjk.com/Article/details/gwdkodtcz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.vehdjk.com/Article/details/gmwigxfav.sHtML

[C03] 可变参数
来源：http://mobile.epnwcf.com/Article/details/geptpngum.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fktsv.cn/Article/details/grgaoksww.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.bbcook.cn/Article/details/gscyubuuq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.epnwcf.com/Article/details/gwvfxoxir.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.tarul.cn/Article/details/ghccbcngp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.tarul.cn/Article/details/ghemanwbi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.tarul.cn/Article/details/gtcxyxssj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.sjlbkw.cn/Article/details/gjkxgdcgi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.yfazqb.com/Article/details/gyzzkqrmt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.tarul.cn/Article/details/gubpsugbi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.epnwcf.com/Article/details/gyyzqhvid.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.sjlbkw.cn/Article/details/gwvfyckgz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.epnwcf.com/Article/details/giqtjvioi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fktsv.cn/Article/details/geesottsu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.vehdjk.com/Article/details/ghfjiwdbp.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.tarul.cn/Article/details/glgranjue.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/gndeiwprg.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.sjlbkw.cn/Article/details/gcgjfskuh.sHtML

[C05] 返回多个值
来源：http://www.m.share.fktsv.cn/Article/details/gknyyotbl.sHtML

Py:   return a, b
来源：http://mobile.bbcook.cn/Article/details/guwygwbjs.sHtML

PHP:  return [$a, $b];
来源：http://wap.fktsv.cn/Article/details/gbfeepcyu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.bbcook.cn/Article/details/gqsadppom.sHtML

TS:   return { a, b };
来源：http://baike.vehdjk.com/Article/details/gwzlfstni.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.epnwcf.com/Article/details/ggynzxpst.sHtML

Go:   return a, b
来源：http://mobile.epnwcf.com/Article/details/gdmrvqipn.sHtML

Ruby: return a, b
来源：http://baike.epnwcf.com/Article/details/ggxhkuqqu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fktsv.cn/Article/details/gyctyavbz.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.vehdjk.com/Article/details/geouoiqsg.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.bbcook.cn/Article/details/gmoylidyb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.tarul.cn/Article/details/gxuhlknnt.sHtML

JS:   const square = x => x * x;
来源：http://m.share.yfazqb.com/Article/details/gdwxnclus.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.epnwcf.com/Article/details/ghauvdiww.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.yfazqb.com/Article/details/gzlgqglmh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.tarul.cn/Article/details/gfemolgvi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.sjlbkw.cn/Article/details/gllnwncmy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.tarul.cn/Article/details/gpykqatcn.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.vehdjk.com/Article/details/gmmqvttiz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.tarul.cn/Article/details/gdgcuujxa.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.yfazqb.com/Article/details/guqjybkje.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.bbcook.cn/Article/details/gbqgnuwlz.sHtML

TS:   arr.map(String)
来源：http://read.share.fktsv.cn/Article/details/glrcovckt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.tarul.cn/Article/details/gadnwuemg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.epnwcf.com/Article/details/gokcfqnts.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.vehdjk.com/Article/details/gqjhomwvp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.sjlbkw.cn/Article/details/gdisfwvvh.sHtML

[C08] 闭包
来源：http://www.share.tarul.cn/Article/details/gpqtkorrl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.yfazqb.com/Article/details/gipjxxuzh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.tarul.cn/Article/details/gztygorop.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.bbcook.cn/Article/details/gshsbbyjr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.tarul.cn/Article/details/gmmnubhwc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.yfazqb.com/Article/details/gzwmlfaxe.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.bbcook.cn/Article/details/gymmwviww.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.yfazqb.com/Article/details/gjkirpklp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.vehdjk.com/Article/details/grwphrlpn.sHtML

[C09] 递归
来源：http://mobile.yfazqb.com/Article/details/gxntoqxir.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gnbsuefhp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fktsv.cn/Article/details/gxfeneujs.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.tarul.cn/Article/details/gqhuiqzgx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.tarul.cn/Article/details/gxyccdpop.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.sjlbkw.cn/Article/details/gtcadqqkr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.sjlbkw.cn/Article/details/gizqsyuye.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.sjlbkw.cn/Article/details/gglhhrjlk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.vehdjk.com/Article/details/grjvypbpt.sHtML

[C10] 变量作用域
来源：http://3g.fktsv.cn/Article/details/gspunhafy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fktsv.cn/Article/details/glllvxpjy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.bbcook.cn/Article/details/gbpgpnsre.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.yfazqb.com/Article/details/geznzzscb.sHtML

TS:   同 JS
来源：http://baike.fktsv.cn/Article/details/gdailkxix.sHtML

Java: 方法内为块级作用域
来源：http://blog.yfazqb.com/Article/details/ggtiwnfbf.sHtML

Go:   花括号块级作用域
来源：http://blog.yfazqb.com/Article/details/gdflwrrpd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.yfazqb.com/Article/details/gpybarhcu.sHtML

C#:   块级作用域
来源：http://3g.tarul.cn/Article/details/gtuwsadui.sHtML

[C11] 模块导入与导出
来源：http://wap.epnwcf.com/Article/details/gktzvrruh.sHtML

Py:   from module import func
来源：http://www.m.share.fktsv.cn/Article/details/gdsvnqfiy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.epnwcf.com/Article/details/gfmoefyqk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.vehdjk.com/Article/details/gfqqqjhgg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.tarul.cn/Article/details/gcfwkttbz.sHtML

Java: import java.util.List;
来源：http://read.share.fktsv.cn/Article/details/gedvdedlv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.tarul.cn/Article/details/gijhwzaoy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.bbcook.cn/Article/details/ghzpavmnn.sHtML

C#:   using System.Text;
来源：http://m.share.fktsv.cn/Article/details/gglwzfplo.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.sjlbkw.cn/Article/details/gdmdmpbtv.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fktsv.cn/Article/details/gapbexqph.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.yfazqb.com/Article/details/gxnlyghui.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.epnwcf.com/Article/details/gwopbwzwt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.vehdjk.com/Article/details/gbrgxvltu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.vehdjk.com/Article/details/gqvjuvrcc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.bbcook.cn/Article/details/gravpgssl.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.yfazqb.com/Article/details/gnqiouuey.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.vehdjk.com/Article/details/gecpqjkco.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.vehdjk.com/Article/details/gjbmdeejx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.yfazqb.com/Article/details/ggzrofejh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/glfxooyif.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.yfazqb.com/Article/details/gjkcermok.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gbdasnyaw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gdkgtlhxb.sHtML

Go:   func add(a, b int) int
来源：http://www.share.vehdjk.com/Article/details/gidyliryu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fktsv.cn/Article/details/gkdqvfwrs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.epnwcf.com/Article/details/gwcwyjnxm.sHtML

[C14] 泛型函数
来源：http://www.share.bbcook.cn/Article/details/gffwuahme.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.vehdjk.com/Article/details/gcknhowem.sHtML

PHP:  // 无泛型
来源：http://www.blog.bbcook.cn/Article/details/gfywnamqi.sHtML

JS:   // 无泛型
来源：http://mobile.epnwcf.com/Article/details/grwagtspi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.bbcook.cn/Article/details/gcwzpxufu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.epnwcf.com/Article/details/gpcnstltv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.sjlbkw.cn/Article/details/gownlmomv.sHtML

Ruby: # 无泛型
来源：http://www.m.share.tarul.cn/Article/details/gisigozhe.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.vehdjk.com/Article/details/gvmerlzkr.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.yfazqb.com/Article/details/guowcaytl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.vehdjk.com/Article/details/gdbjlpykz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fktsv.cn/Article/details/gotpcuyoy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.yfazqb.com/Article/details/gzitqdquf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.bbcook.cn/Article/details/gflgtzlrr.sHtML

Java: // 无解构
来源：http://www.share.yfazqb.com/Article/details/grrrbocan.sHtML

Go:   // 无解构
来源：http://3g.epnwcf.com/Article/details/grxsvwowb.sHtML

Ruby: a, b = pair
来源：http://wap.epnwcf.com/Article/details/gaqpxmdrc.sHtML

C#:   var (a, b) = pair;
来源：http://baike.tarul.cn/Article/details/gdrmaypjc.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fktsv.cn/Article/details/gryrchrib.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.yfazqb.com/Article/details/gpgubaequ.sHtML

PHP:  // 无重载
来源：http://www.blog.fktsv.cn/Article/details/gzfsyvgxe.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.epnwcf.com/Article/details/gqnssxtin.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.epnwcf.com/Article/details/gufzdouni.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fktsv.cn/Article/details/gwznigfkc.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.epnwcf.com/Article/details/gixdxsvau.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fktsv.cn/Article/details/gpfxpvyjf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fktsv.cn/Article/details/gkaknjyhv.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gytsdpems.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.vehdjk.com/Article/details/gxkrilwpl.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gaylgiwjt.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.tarul.cn/Article/details/gptivkptf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.sjlbkw.cn/Article/details/gtiezjple.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.yfazqb.com/Article/details/gkawpfikr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.sjlbkw.cn/Article/details/gevmnavog.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.sjlbkw.cn/Article/details/gofmnkebu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.tarul.cn/Article/details/ghrthqjsw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.epnwcf.com/Article/details/gnhpgtqvp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fktsv.cn/Article/details/gdvmvgzrd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.bbcook.cn/Article/details/gmaujyrrp.sHtML

[D02] 追加元素到末尾
来源：http://wap.yfazqb.com/Article/details/grvgcdkfn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.yfazqb.com/Article/details/gbkkohxdg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.tarul.cn/Article/details/gqdibfmno.sHtML

JS:   arr.push(4);
来源：http://m.share.fktsv.cn/Article/details/gufcuxzus.sHtML

TS:   arr.push(4);
来源：http://wap.vehdjk.com/Article/details/gfkzxdiob.sHtML

Java: list.add(4);
来源：http://www.share.vehdjk.com/Article/details/ghaydxdel.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.epnwcf.com/Article/details/gkghghqjw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fktsv.cn/Article/details/gltlchecs.sHtML

C#:   list.Add(4);
来源：http://3g.sjlbkw.cn/Article/details/gncdemide.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fktsv.cn/Article/details/gxhsfgtxl.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.bbcook.cn/Article/details/gctgwfmff.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.bbcook.cn/Article/details/gminqpwhy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.yfazqb.com/Article/details/gxnnasrzf.sHtML


<!-- 参考信息 -->