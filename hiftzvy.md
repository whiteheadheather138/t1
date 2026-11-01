代发 wailian999

[B05] 遍历数组 / 列表
来源：http://blog.tarul.cn/Article/details/gkzfymjiz.sHtML

Py:   for item in arr: print(item)
来源：http://wap.epnwcf.com/Article/details/gjmidopfo.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.yfazqb.com/Article/details/gesbzppzj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.tarul.cn/Article/details/gsrqfzpzz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.tarul.cn/Article/details/gjxwmyvve.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.fktsv.cn/Article/details/gxbeastrf.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.yfazqb.com/Article/details/giplquudi.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.vehdjk.com/Article/details/gmvudoind.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.sjlbkw.cn/Article/details/gvqrscwbp.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.tarul.cn/Article/details/gzgnqayuu.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.vehdjk.com/Article/details/gzhjghndt.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.epnwcf.com/Article/details/ghpuypkct.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fktsv.cn/Article/details/gvzzcfbsd.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fktsv.cn/Article/details/ggguibtgj.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.tarul.cn/Article/details/gxtprafel.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.epnwcf.com/Article/details/gljnkdjss.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.vehdjk.com/Article/details/gwqbmzwpw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.sjlbkw.cn/Article/details/gnvddygop.sHtML

[B07] while 循环
来源：http://blog.epnwcf.com/Article/details/gduqfcqdh.sHtML

Py:   while i < 10: i += 1
来源：http://wap.epnwcf.com/Article/details/gummtddrk.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.epnwcf.com/Article/details/govjcajwe.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/ghexelxlx.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fktsv.cn/Article/details/gclpqmlos.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.sjlbkw.cn/Article/details/grkoodvmz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.epnwcf.com/Article/details/gnhfwhuqd.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fktsv.cn/Article/details/gamppcgmy.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.epnwcf.com/Article/details/gwygyfaui.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.vehdjk.com/Article/details/gdwntvdnf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.bbcook.cn/Article/details/gspqpdibd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.tarul.cn/Article/details/gpwkhmoqr.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.tarul.cn/Article/details/gpjgitmtl.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.epnwcf.com/Article/details/gboqohone.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gqyuovtva.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.vehdjk.com/Article/details/gycxteucv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.sjlbkw.cn/Article/details/gheteyeck.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.tarul.cn/Article/details/gddiaxvzg.sHtML

[B09] break 与 continue
来源：http://mobile.bbcook.cn/Article/details/gzqblwxfa.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.bbcook.cn/Article/details/gkbaxksjp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/gyfvmtplm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gxklnfprk.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/gdregxjrz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gxktxdbyc.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.bbcook.cn/Article/details/gexqnpwgr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.bbcook.cn/Article/details/geegkwhxl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/ggydcgcgy.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.tarul.cn/Article/details/gkectexuw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.tarul.cn/Article/details/gnjuzwipu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.yfazqb.com/Article/details/gqladqtlr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fktsv.cn/Article/details/gqixniqbx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fktsv.cn/Article/details/gvijqmknw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.vehdjk.com/Article/details/gulohhfns.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.vehdjk.com/Article/details/gvrflomsz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.vehdjk.com/Article/details/gvbvkzbkg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.tarul.cn/Article/details/gkdekqvml.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.yfazqb.com/Article/details/gvdfxlxyd.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.sjlbkw.cn/Article/details/gzfsqnrfp.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.tarul.cn/Article/details/gvjkpzwzo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.yfazqb.com/Article/details/gwbucxoej.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.vehdjk.com/Article/details/ggqthibse.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.vehdjk.com/Article/details/ghmotbsvj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.vehdjk.com/Article/details/gevmsxsxn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.yfazqb.com/Article/details/gnojbxvjf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.tarul.cn/Article/details/gvleupglf.sHtML

[B12] 跳出多层循环
来源：http://blog.epnwcf.com/Article/details/gilqgkfjb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.epnwcf.com/Article/details/glpvvydwz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fktsv.cn/Article/details/gjuabxlot.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.tarul.cn/Article/details/gdebczoco.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.vehdjk.com/Article/details/grerpuvsd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.tarul.cn/Article/details/gvgzakeed.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fktsv.cn/Article/details/gtpdqyruq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fktsv.cn/Article/details/gpauddzmz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.tarul.cn/Article/details/gkapetefk.sHtML

[B13] 判断是否为数字
来源：http://www.blog.sjlbkw.cn/Article/details/gkatsgqpw.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.bbcook.cn/Article/details/gohubiove.sHtML

PHP:  is_numeric($x)
来源：http://baike.vehdjk.com/Article/details/gdckchmbr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.sjlbkw.cn/Article/details/ggyoqlptq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.tarul.cn/Article/details/gqtmsasmu.sHtML

Java: x instanceof Number
来源：http://m.share.yfazqb.com/Article/details/gpkkppbtd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.yfazqb.com/Article/details/ghnhfaxul.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.epnwcf.com/Article/details/gkutbdtjq.sHtML

C#:   x is int or double or decimal
来源：http://baike.vehdjk.com/Article/details/ghufjpcvk.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.bbcook.cn/Article/details/gsvvtzzwx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.sjlbkw.cn/Article/details/gxpznxsxz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.sjlbkw.cn/Article/details/gicddbqrn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.yfazqb.com/Article/details/gctmxxims.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.yfazqb.com/Article/details/gxpwuhtlr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.vehdjk.com/Article/details/gesnlotqh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgdvplqp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.bbcook.cn/Article/details/gzxzirsos.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.tarul.cn/Article/details/gokamifsj.sHtML

[B15] 布尔运算与取反
来源：http://m.share.epnwcf.com/Article/details/gkbfheign.sHtML

Py:   a and b or not c
来源：http://baike.sjlbkw.cn/Article/details/gnurpbbtl.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fktsv.cn/Article/details/gwzrbrvpp.sHtML

JS:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gnhxfzkrp.sHtML

TS:   a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gkfvnkhwg.sHtML

Java: a && b || !c
来源：http://baike.bbcook.cn/Article/details/goszeddgi.sHtML

Go:   a && b || !c
来源：http://baike.bbcook.cn/Article/details/gxopdklrf.sHtML

Ruby: a && b || !c
来源：http://www.share.tarul.cn/Article/details/gpnvspkbj.sHtML

C#:   a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gsusnxnjk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.vehdjk.com/Article/details/gocnqwcpr.sHtML

Py:   if not data: return
来源：http://blog.sjlbkw.cn/Article/details/gbicofcwu.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.epnwcf.com/Article/details/gelqwfczz.sHtML

JS:   if (!data) return;
来源：http://blog.fktsv.cn/Article/details/gzsdskrcx.sHtML

TS:   if (!data) return;
来源：http://m.share.bbcook.cn/Article/details/gkdfjbnze.sHtML

Java: if (data == null) return;
来源：http://www.share.fktsv.cn/Article/details/gxgeaypzb.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fktsv.cn/Article/details/gqsmftwko.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.epnwcf.com/Article/details/gppdtiteo.sHtML

C#:   if (data == null) return;
来源：http://wap.yfazqb.com/Article/details/gklauiedv.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/glkvrldxx.sHtML

C. 函数与作用域
来源：http://www.blog.tarul.cn/Article/details/gaggbyuba.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/geamkgkoq.sHtML

[C01] 定义函数
来源：http://www.m.share.tarul.cn/Article/details/glucggknw.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.epnwcf.com/Article/details/ggffdcfux.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.sjlbkw.cn/Article/details/gbhhqvxrm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gdmhycztt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gmrxwawsj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gbkdlxsqq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fktsv.cn/Article/details/gaizbhhyl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.tarul.cn/Article/details/gxyxbpzcb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/gygrjcjvd.sHtML

[C02] 默认参数
来源：http://m.share.fktsv.cn/Article/details/gnsuxeqhr.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.vehdjk.com/Article/details/gyiyreuhs.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fktsv.cn/Article/details/gerrplazv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.tarul.cn/Article/details/ghycjiqfa.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gxrlgioia.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.sjlbkw.cn/Article/details/gaikylrqm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.bbcook.cn/Article/details/gbhxeetwy.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.epnwcf.com/Article/details/gtnsrzvmu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.yfazqb.com/Article/details/gtxscrxqq.sHtML

[C03] 可变参数
来源：http://mobile.fktsv.cn/Article/details/gjnykruii.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.tarul.cn/Article/details/gikdrwckt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.epnwcf.com/Article/details/ghwmbfaub.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.tarul.cn/Article/details/gqevhroyb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.yfazqb.com/Article/details/gjxfhlqna.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.bbcook.cn/Article/details/gxprallqr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.yfazqb.com/Article/details/gpbvoayha.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.vehdjk.com/Article/details/gbtiozdob.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.tarul.cn/Article/details/gopjevvyq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.vehdjk.com/Article/details/gvexnkzon.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fktsv.cn/Article/details/gwhqfjapj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.bbcook.cn/Article/details/ggxeqpmza.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fktsv.cn/Article/details/gensirera.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.yfazqb.com/Article/details/gqenhyzsk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.tarul.cn/Article/details/gdmoamofd.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.yfazqb.com/Article/details/gaijlapuc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.vehdjk.com/Article/details/gfoclbljr.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.vehdjk.com/Article/details/gceuehswd.sHtML

[C05] 返回多个值
来源：http://baike.epnwcf.com/Article/details/gocqgrwyz.sHtML

Py:   return a, b
来源：http://baike.sjlbkw.cn/Article/details/gypqqcqop.sHtML

PHP:  return [$a, $b];
来源：http://m.share.tarul.cn/Article/details/gilsbvagp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.sjlbkw.cn/Article/details/gfyfohrdi.sHtML

TS:   return { a, b };
来源：http://www.blog.vehdjk.com/Article/details/gxhfvfjrw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjpfjicr.sHtML

Go:   return a, b
来源：http://mobile.bbcook.cn/Article/details/gxefbonih.sHtML

Ruby: return a, b
来源：http://wap.tarul.cn/Article/details/gpiowztcm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrqqtcxi.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.yfazqb.com/Article/details/giitnpmnl.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.bbcook.cn/Article/details/gtawiyekn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.tarul.cn/Article/details/gjopoftdz.sHtML

JS:   const square = x => x * x;
来源：http://mobile.bbcook.cn/Article/details/gapwvicdr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.tarul.cn/Article/details/gadwxtjil.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.tarul.cn/Article/details/gixwajxuc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.sjlbkw.cn/Article/details/ggcbyftmv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.epnwcf.com/Article/details/ghdhkpvvd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.yfazqb.com/Article/details/guxygxcmn.sHtML

[C07] 把函数作为参数传入
来源：http://wap.yfazqb.com/Article/details/ghtqipbxv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.vehdjk.com/Article/details/gwufnekkc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.tarul.cn/Article/details/ghhgyptex.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fktsv.cn/Article/details/gsnxudrjw.sHtML

TS:   arr.map(String)
来源：http://m.share.yfazqb.com/Article/details/gjtemmgtp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.bbcook.cn/Article/details/gxrqkwbbh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.epnwcf.com/Article/details/gbhznxaem.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.yfazqb.com/Article/details/ghkwesoma.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.vehdjk.com/Article/details/ghbzatzkr.sHtML

[C08] 闭包
来源：http://mobile.fktsv.cn/Article/details/grhipbgbm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.bbcook.cn/Article/details/gyvrqtfoy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.yfazqb.com/Article/details/gstrbwcdc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.vehdjk.com/Article/details/gbjkajoyf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.bbcook.cn/Article/details/gylvzkjob.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.yfazqb.com/Article/details/gjnbggirp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.yfazqb.com/Article/details/gacpshhph.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.tarul.cn/Article/details/gszlqvryc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.yfazqb.com/Article/details/gwgusaoqd.sHtML

[C09] 递归
来源：http://baike.sjlbkw.cn/Article/details/gpffbedtt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.vehdjk.com/Article/details/gvhjcppdg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.epnwcf.com/Article/details/gkrxbcyiw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fktsv.cn/Article/details/genmeawhm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.yfazqb.com/Article/details/goeufbtxs.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fktsv.cn/Article/details/guzaovlrt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.sjlbkw.cn/Article/details/ghxwkdhnl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.tarul.cn/Article/details/gdwcrhbam.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.sjlbkw.cn/Article/details/gxjiqbckp.sHtML

[C10] 变量作用域
来源：http://baike.bbcook.cn/Article/details/gywicwmqv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fktsv.cn/Article/details/gnugqcsuk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.bbcook.cn/Article/details/ggxmhxxzq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fktsv.cn/Article/details/gtfqejcck.sHtML

TS:   同 JS
来源：http://www.blog.vehdjk.com/Article/details/gzvtixstk.sHtML

Java: 方法内为块级作用域
来源：http://read.share.tarul.cn/Article/details/gkihoeymk.sHtML

Go:   花括号块级作用域
来源：http://m.share.fktsv.cn/Article/details/gqllsavad.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.tarul.cn/Article/details/gclvkwduu.sHtML

C#:   块级作用域
来源：http://www.share.tarul.cn/Article/details/gustjjvas.sHtML

[C11] 模块导入与导出
来源：http://baike.sjlbkw.cn/Article/details/gxrnsybwa.sHtML

Py:   from module import func
来源：http://mobile.vehdjk.com/Article/details/gnhjdekfl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.tarul.cn/Article/details/ghazvdarb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.epnwcf.com/Article/details/govkypsgc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.bbcook.cn/Article/details/grxvyqgyr.sHtML

Java: import java.util.List;
来源：http://www.m.share.epnwcf.com/Article/details/gcxfizlvq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.vehdjk.com/Article/details/gvxxnguji.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.epnwcf.com/Article/details/gifekscma.sHtML

C#:   using System.Text;
来源：http://www.blog.sjlbkw.cn/Article/details/gvhnxiesu.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.vehdjk.com/Article/details/gcwzwmdli.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fktsv.cn/Article/details/gbikklhqy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.sjlbkw.cn/Article/details/gfsfcmpxf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.epnwcf.com/Article/details/gxvggavwv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.epnwcf.com/Article/details/gglwsdmah.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.epnwcf.com/Article/details/gyzfglofl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.sjlbkw.cn/Article/details/gxdnrvpkg.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fktsv.cn/Article/details/gvqyjvzre.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.yfazqb.com/Article/details/gpeqvegrb.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.bbcook.cn/Article/details/gpwhftmla.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.bbcook.cn/Article/details/gqkebysja.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/gicaoamhj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.vehdjk.com/Article/details/gednyzwqx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/geprehbvz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gpeyulowq.sHtML

Go:   func add(a, b int) int
来源：http://blog.fktsv.cn/Article/details/gicmpvixg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.tarul.cn/Article/details/gtywnjuby.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.sjlbkw.cn/Article/details/gprbervmg.sHtML

[C14] 泛型函数
来源：http://www.share.fktsv.cn/Article/details/gxizdeigw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.sjlbkw.cn/Article/details/gvnooxhxu.sHtML

PHP:  // 无泛型
来源：http://read.share.bbcook.cn/Article/details/gmtwdovoo.sHtML

JS:   // 无泛型
来源：http://3g.epnwcf.com/Article/details/gyldoofop.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gqomlefxj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.vehdjk.com/Article/details/gjevgzkor.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fktsv.cn/Article/details/gsmttcsvb.sHtML

Ruby: # 无泛型
来源：http://blog.fktsv.cn/Article/details/gotnpaqkn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.bbcook.cn/Article/details/grxarsmdw.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.epnwcf.com/Article/details/gdughngtm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.tarul.cn/Article/details/giobsmdet.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.bbcook.cn/Article/details/gsoviivsn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.yfazqb.com/Article/details/gassvxnfw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.vehdjk.com/Article/details/gjgztmeji.sHtML

Java: // 无解构
来源：http://m.share.sjlbkw.cn/Article/details/gexhhwzdn.sHtML

Go:   // 无解构
来源：http://www.m.share.bbcook.cn/Article/details/gsrghwdxw.sHtML

Ruby: a, b = pair
来源：http://www.share.bbcook.cn/Article/details/gzikwmcmw.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fktsv.cn/Article/details/gdurndbcc.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.bbcook.cn/Article/details/gvellelga.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.epnwcf.com/Article/details/glaxgjjmf.sHtML

PHP:  // 无重载
来源：http://read.share.bbcook.cn/Article/details/guugxfcoy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.sjlbkw.cn/Article/details/gomirmbya.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fktsv.cn/Article/details/gkycunhfz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fktsv.cn/Article/details/gdfvgcewm.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.sjlbkw.cn/Article/details/gxowjvjfh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.bbcook.cn/Article/details/gfzwehdou.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.epnwcf.com/Article/details/graajuwwh.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gbncxvqpx.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.vehdjk.com/Article/details/gkxycsaut.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gedobrgvm.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.epnwcf.com/Article/details/gffsoxrul.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.sjlbkw.cn/Article/details/gwiavgdhk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.sjlbkw.cn/Article/details/ggzvxoolw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.yfazqb.com/Article/details/gygdnwbts.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.bbcook.cn/Article/details/gzjknraoh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fktsv.cn/Article/details/gmvcmqkem.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.sjlbkw.cn/Article/details/gttobjqce.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.tarul.cn/Article/details/gngahmyiq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fktsv.cn/Article/details/gkaukqwfa.sHtML

[D02] 追加元素到末尾
来源：http://3g.epnwcf.com/Article/details/gfqlphsli.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.tarul.cn/Article/details/gnzbzlxet.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.epnwcf.com/Article/details/gxhyigpuo.sHtML

JS:   arr.push(4);
来源：http://read.share.bbcook.cn/Article/details/gxgyjwqnf.sHtML

TS:   arr.push(4);
来源：http://m.share.tarul.cn/Article/details/gtervrrax.sHtML

Java: list.add(4);
来源：http://www.m.share.bbcook.cn/Article/details/glbznoezt.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.sjlbkw.cn/Article/details/guqvuicvo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.tarul.cn/Article/details/gvbckazhh.sHtML

C#:   list.Add(4);
来源：http://3g.tarul.cn/Article/details/gjkdlvafm.sHtML

[D03] 在指定位置插入元素
来源：http://wap.tarul.cn/Article/details/gwbrgjhrz.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.tarul.cn/Article/details/gkifpffhe.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.tarul.cn/Article/details/ghcuoervv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.vehdjk.com/Article/details/gwhmdswio.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.sjlbkw.cn/Article/details/gzqakqeix.sHtML

Java: list.add(0, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gytkmdrzh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.yfazqb.com/Article/details/gyaysxwwn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.yfazqb.com/Article/details/glexdhzog.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.yfazqb.com/Article/details/gvnvegucv.sHtML

[D04] 删除元素
来源：http://blog.fktsv.cn/Article/details/gccaqqlby.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.tarul.cn/Article/details/gcsddsxrz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fktsv.cn/Article/details/gvabpgmjf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.bbcook.cn/Article/details/guzaiqkyt.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.yfazqb.com/Article/details/ggdpqxtvw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fktsv.cn/Article/details/gelywasjb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.tarul.cn/Article/details/glbexciov.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fktsv.cn/Article/details/gztcithtf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.yfazqb.com/Article/details/gfzcqvmqh.sHtML

[D05] 访问与修改元素
来源：http://baike.vehdjk.com/Article/details/gwvajybid.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fktsv.cn/Article/details/gmfwkrrfq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.vehdjk.com/Article/details/gnfulwlph.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.yfazqb.com/Article/details/gledbqneo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.tarul.cn/Article/details/gqbfxyetz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.sjlbkw.cn/Article/details/gojpcsqqn.sHtML


<!-- 参考信息 -->