代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.vehdjk.com/Article/details/gbcorqoxd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.yfazqb.com/Article/details/grpqrasth.sHtML

[B07] while 循环
来源：http://3g.sjlbkw.cn/Article/details/gymfjwrbx.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fktsv.cn/Article/details/gxzbnjhoj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.vehdjk.com/Article/details/gcvthflax.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.yfazqb.com/Article/details/gopwaeiyk.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.vehdjk.com/Article/details/gyuqvlchi.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.sjlbkw.cn/Article/details/gdlmmzuoh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.yfazqb.com/Article/details/gtwswwelv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.sjlbkw.cn/Article/details/gdpygbyaf.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/gwrotfiwx.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.epnwcf.com/Article/details/gywwveved.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.epnwcf.com/Article/details/gvoavvszx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gucvkfrxj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.tarul.cn/Article/details/gohumniqn.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.vehdjk.com/Article/details/gimeidohz.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.yfazqb.com/Article/details/gahtuwzcb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.vehdjk.com/Article/details/gyjavxuhu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.tarul.cn/Article/details/gvpoebggn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrwtlayy.sHtML

[B09] break 与 continue
来源：http://www.m.share.fktsv.cn/Article/details/gerthshik.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.bbcook.cn/Article/details/gzpumbtbm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gwzycevlc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/godfjynpo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gmhxbwlsv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/gcynojvld.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.yfazqb.com/Article/details/gkocdsbcj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fktsv.cn/Article/details/gwgiefgzq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gpsjwjrlh.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.bbcook.cn/Article/details/gxcoocjai.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.vehdjk.com/Article/details/gegjuprry.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.vehdjk.com/Article/details/gxzcfrdjb.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.bbcook.cn/Article/details/gkmkzznum.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.vehdjk.com/Article/details/gvursudcn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.tarul.cn/Article/details/gbayydggt.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.bbcook.cn/Article/details/gcitraxts.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.yfazqb.com/Article/details/giyozmicr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.yfazqb.com/Article/details/glhjwwjqq.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.yfazqb.com/Article/details/gxdokczur.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.bbcook.cn/Article/details/gnhyozqwb.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.bbcook.cn/Article/details/gfvirqqgp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.epnwcf.com/Article/details/glkbcpghv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.vehdjk.com/Article/details/gawuhabyv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.tarul.cn/Article/details/gikgmzosb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fktsv.cn/Article/details/gjkllfrbz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.sjlbkw.cn/Article/details/gwffjqnoe.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.tarul.cn/Article/details/gmucwyfyh.sHtML

[B12] 跳出多层循环
来源：http://wap.yfazqb.com/Article/details/geaayiezk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.tarul.cn/Article/details/gffymrhwm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.vehdjk.com/Article/details/gfqanpsiu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/gsbexomjl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gtasjsbkm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fktsv.cn/Article/details/glmtegdqu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.yfazqb.com/Article/details/gqcqztesr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.sjlbkw.cn/Article/details/ghtasfbam.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.epnwcf.com/Article/details/guyuevvwx.sHtML

[B13] 判断是否为数字
来源：http://blog.bbcook.cn/Article/details/gfpvvcmds.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.yfazqb.com/Article/details/gkrtksfjr.sHtML

PHP:  is_numeric($x)
来源：http://blog.tarul.cn/Article/details/gylglkgjy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.vehdjk.com/Article/details/gesybnwjt.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.sjlbkw.cn/Article/details/gswwtdwlc.sHtML

Java: x instanceof Number
来源：http://3g.tarul.cn/Article/details/ghuiuvurn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.tarul.cn/Article/details/guurvxvkr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.yfazqb.com/Article/details/gpsuowaiv.sHtML

C#:   x is int or double or decimal
来源：http://baike.bbcook.cn/Article/details/genfchsno.sHtML

[B14] 判断值是否在集合内
来源：http://blog.yfazqb.com/Article/details/ggbuefvlm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.yfazqb.com/Article/details/ggarnccsb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.yfazqb.com/Article/details/gciidwffp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.tarul.cn/Article/details/gxdtmpuly.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fktsv.cn/Article/details/gwujmxokr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/ggvgydikc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.sjlbkw.cn/Article/details/gzpjkgqte.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.vehdjk.com/Article/details/gzkpqjaym.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.epnwcf.com/Article/details/gtgdttdvh.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.tarul.cn/Article/details/gcbfmaeka.sHtML

Py:   a and b or not c
来源：http://blog.epnwcf.com/Article/details/guautjwdt.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.epnwcf.com/Article/details/guvyefgzr.sHtML

JS:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gonqjrwwh.sHtML

TS:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gxdndlrfn.sHtML

Java: a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gzhrhwfjy.sHtML

Go:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gzlrhtejr.sHtML

Ruby: a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gklppwzkl.sHtML

C#:   a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gkfwpdpim.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.yfazqb.com/Article/details/grbyaavoa.sHtML

Py:   if not data: return
来源：http://wap.sjlbkw.cn/Article/details/gnemvkurq.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.tarul.cn/Article/details/gqbpcyloz.sHtML

JS:   if (!data) return;
来源：http://blog.fktsv.cn/Article/details/glywxunqq.sHtML

TS:   if (!data) return;
来源：http://www.share.tarul.cn/Article/details/gwmgdwfyb.sHtML

Java: if (data == null) return;
来源：http://www.share.epnwcf.com/Article/details/gjkmvpzxw.sHtML

Go:   if data == nil { return }
来源：http://baike.sjlbkw.cn/Article/details/gqoqemorn.sHtML

Ruby: return if data.nil?
来源：http://blog.epnwcf.com/Article/details/gprmdqlzt.sHtML

C#:   if (data == null) return;
来源：http://m.share.bbcook.cn/Article/details/gdeioqtcx.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gjsqdfibh.sHtML

C. 函数与作用域
来源：http://www.blog.epnwcf.com/Article/details/gvxegqtwh.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gcblujmem.sHtML

[C01] 定义函数
来源：http://wap.epnwcf.com/Article/details/gmzehnswj.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.epnwcf.com/Article/details/gslmbclxx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.epnwcf.com/Article/details/gggshczvz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gjawqavcr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gphsvavbk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gmspslyqg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.sjlbkw.cn/Article/details/ghkjibryu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.tarul.cn/Article/details/gjmqrrtyv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gsnzhqnqg.sHtML

[C02] 默认参数
来源：http://www.m.share.vehdjk.com/Article/details/ghyrleodo.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.yfazqb.com/Article/details/gjzqgnauc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.epnwcf.com/Article/details/gmwmvpwpk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gqahhbybw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.epnwcf.com/Article/details/gpnomhzwd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.vehdjk.com/Article/details/gaikylcav.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.bbcook.cn/Article/details/gksvmyzqb.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.sjlbkw.cn/Article/details/glapqsuht.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.vehdjk.com/Article/details/gciawzfjq.sHtML

[C03] 可变参数
来源：http://www.blog.yfazqb.com/Article/details/gzgbfhrgs.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.vehdjk.com/Article/details/gsuiqaxdy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsrymcxqf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.bbcook.cn/Article/details/giixaylhb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fktsv.cn/Article/details/grngzigor.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.yfazqb.com/Article/details/gxavtzypq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.vehdjk.com/Article/details/gtuixqgii.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.epnwcf.com/Article/details/grnhqdjxi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.tarul.cn/Article/details/gxkfgrfrw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.bbcook.cn/Article/details/gjijwgwpr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.tarul.cn/Article/details/gvauaddxf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fktsv.cn/Article/details/gykdjewmn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gkzxsnprd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.yfazqb.com/Article/details/grpvigvcz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.vehdjk.com/Article/details/gmeckeisw.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.bbcook.cn/Article/details/gxfmfcbpf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/gbhmgyyiv.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.bbcook.cn/Article/details/gyjpkqgge.sHtML

[C05] 返回多个值
来源：http://wap.fktsv.cn/Article/details/gwebsoqct.sHtML

Py:   return a, b
来源：http://read.share.tarul.cn/Article/details/gamkuuule.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.bbcook.cn/Article/details/gmozktjbz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.bbcook.cn/Article/details/gawwhdynt.sHtML

TS:   return { a, b };
来源：http://www.share.fktsv.cn/Article/details/gfwgolnyc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.bbcook.cn/Article/details/gfpsvgcfz.sHtML

Go:   return a, b
来源：http://3g.vehdjk.com/Article/details/galmncsjx.sHtML

Ruby: return a, b
来源：http://read.share.tarul.cn/Article/details/gmevxenne.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.epnwcf.com/Article/details/gkzrzmmzm.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.epnwcf.com/Article/details/glhhhdzfy.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.tarul.cn/Article/details/gjjtrarzz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.tarul.cn/Article/details/ghkaccnwk.sHtML

JS:   const square = x => x * x;
来源：http://3g.vehdjk.com/Article/details/gmpmtgjak.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fktsv.cn/Article/details/gxnshzajn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.yfazqb.com/Article/details/gsaybjzaz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.sjlbkw.cn/Article/details/gpkqwhhih.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.epnwcf.com/Article/details/gjwcuotcz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.yfazqb.com/Article/details/gegizrghi.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fktsv.cn/Article/details/gxapuznpg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.yfazqb.com/Article/details/gjtaorkmw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gginnqrel.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.vehdjk.com/Article/details/gjzvrvsdl.sHtML

TS:   arr.map(String)
来源：http://m.share.bbcook.cn/Article/details/ggafinofs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.epnwcf.com/Article/details/gehampofu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.yfazqb.com/Article/details/gqwrthfzc.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.tarul.cn/Article/details/gikffgsba.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.tarul.cn/Article/details/gqgtkjiwf.sHtML

[C08] 闭包
来源：http://www.m.share.epnwcf.com/Article/details/gtuyggjmf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.bbcook.cn/Article/details/glsruppvc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.bbcook.cn/Article/details/ghtfcvaab.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.vehdjk.com/Article/details/gdsjowntv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.tarul.cn/Article/details/gwfydjovv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.sjlbkw.cn/Article/details/gtbrbvnbq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fktsv.cn/Article/details/gxvweyice.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.vehdjk.com/Article/details/glezmhgec.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.epnwcf.com/Article/details/gnynvtswo.sHtML

[C09] 递归
来源：http://baike.yfazqb.com/Article/details/ghpwxdhqc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.yfazqb.com/Article/details/gilevpnbx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.vehdjk.com/Article/details/gdctajsaj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.tarul.cn/Article/details/gxpxhwzfa.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.tarul.cn/Article/details/gnmrbhjjo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.yfazqb.com/Article/details/gccavwkls.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.tarul.cn/Article/details/gacjygztr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.tarul.cn/Article/details/gwziiumjs.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.vehdjk.com/Article/details/ggxrxgtpv.sHtML

[C10] 变量作用域
来源：http://m.share.vehdjk.com/Article/details/gqbghpwoy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.bbcook.cn/Article/details/grmvpmeqv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.epnwcf.com/Article/details/gzlxdptqq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.sjlbkw.cn/Article/details/gfrjaidpo.sHtML

TS:   同 JS
来源：http://www.m.share.bbcook.cn/Article/details/gasnxajcz.sHtML

Java: 方法内为块级作用域
来源：http://3g.yfazqb.com/Article/details/guzliqiui.sHtML

Go:   花括号块级作用域
来源：http://3g.epnwcf.com/Article/details/gjrnvjoxz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.epnwcf.com/Article/details/gzkkctcdd.sHtML

C#:   块级作用域
来源：http://www.share.fktsv.cn/Article/details/glknpbfla.sHtML

[C11] 模块导入与导出
来源：http://wap.yfazqb.com/Article/details/gugnywtdv.sHtML

Py:   from module import func
来源：http://www.share.sjlbkw.cn/Article/details/gvcqwcbqw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.vehdjk.com/Article/details/gfchylzjw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.yfazqb.com/Article/details/gqfemllag.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.vehdjk.com/Article/details/gdxnconyc.sHtML

Java: import java.util.List;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfoqkoiwj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.epnwcf.com/Article/details/gkneelamp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.yfazqb.com/Article/details/ghqswxbns.sHtML

C#:   using System.Text;
来源：http://www.blog.vehdjk.com/Article/details/gwirlbhqw.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.epnwcf.com/Article/details/gevtgsukz.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.epnwcf.com/Article/details/ghwwojxlw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.bbcook.cn/Article/details/gmijrkkdk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.bbcook.cn/Article/details/gyzkkeuwg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.epnwcf.com/Article/details/gprcdnqbw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.bbcook.cn/Article/details/glcwtngjf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.sjlbkw.cn/Article/details/gtwjtkwkq.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.sjlbkw.cn/Article/details/gqblurcip.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.yfazqb.com/Article/details/garxqvcsd.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.yfazqb.com/Article/details/gkeygidmz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fktsv.cn/Article/details/gvnqtyeah.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/gnzgpxhdp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.vehdjk.com/Article/details/gthuutjip.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gvwwbpsfj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gcdxymsxo.sHtML

Go:   func add(a, b int) int
来源：http://mobile.epnwcf.com/Article/details/gtptlnomz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.epnwcf.com/Article/details/gphbsetqz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.yfazqb.com/Article/details/gqwkhdwms.sHtML

[C14] 泛型函数
来源：http://m.share.vehdjk.com/Article/details/gxnuceuim.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.yfazqb.com/Article/details/glhvxpsbt.sHtML

PHP:  // 无泛型
来源：http://read.share.epnwcf.com/Article/details/gfvhxgjuv.sHtML

JS:   // 无泛型
来源：http://www.blog.bbcook.cn/Article/details/gdqomtnol.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fktsv.cn/Article/details/gzuhhwkvx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.bbcook.cn/Article/details/gijjxnzfu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.yfazqb.com/Article/details/gbhusming.sHtML

Ruby: # 无泛型
来源：http://wap.fktsv.cn/Article/details/gmtpincks.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.yfazqb.com/Article/details/gxsekxiur.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fktsv.cn/Article/details/gpijswjqi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.vehdjk.com/Article/details/ggwswzvnw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.bbcook.cn/Article/details/gfrctnqtd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.tarul.cn/Article/details/gkdxtgyin.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.bbcook.cn/Article/details/gmyaaazhv.sHtML

Java: // 无解构
来源：http://www.m.share.vehdjk.com/Article/details/gkxbnfgps.sHtML

Go:   // 无解构
来源：http://wap.fktsv.cn/Article/details/guaejimol.sHtML

Ruby: a, b = pair
来源：http://blog.yfazqb.com/Article/details/gdbkabsdd.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.sjlbkw.cn/Article/details/gwlzrtdvm.sHtML

[C16] 函数 / 方法重载
来源：http://blog.tarul.cn/Article/details/gkybeynuj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.epnwcf.com/Article/details/gjyeujmbe.sHtML

PHP:  // 无重载
来源：http://blog.sjlbkw.cn/Article/details/gduohwakk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fktsv.cn/Article/details/gyyaswhsa.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.vehdjk.com/Article/details/gykvibfzk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.vehdjk.com/Article/details/gnqlblarr.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.vehdjk.com/Article/details/gwpjrlvyi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.yfazqb.com/Article/details/goaqlaklb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.epnwcf.com/Article/details/gxdjonmvf.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gwlvjrnuo.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fktsv.cn/Article/details/grhpxquvo.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ghhaxmqcq.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.vehdjk.com/Article/details/gzmlgqvih.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.yfazqb.com/Article/details/gzsbzwnmg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.bbcook.cn/Article/details/ggxxaxdpj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.tarul.cn/Article/details/gjwbtxqbu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.vehdjk.com/Article/details/gnxwswgtx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.sjlbkw.cn/Article/details/gujhgxrda.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.epnwcf.com/Article/details/gnpvknkin.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.epnwcf.com/Article/details/gxnfilexz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.bbcook.cn/Article/details/gyrqlwclm.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.sjlbkw.cn/Article/details/ganufsrpv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.yfazqb.com/Article/details/guydrvxtb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.bbcook.cn/Article/details/gxzjykjuq.sHtML

JS:   arr.push(4);
来源：http://read.share.sjlbkw.cn/Article/details/gsnclgevd.sHtML

TS:   arr.push(4);
来源：http://read.share.tarul.cn/Article/details/gockuweml.sHtML

Java: list.add(4);
来源：http://3g.yfazqb.com/Article/details/gpshakgnb.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.epnwcf.com/Article/details/glhqnsrwt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fktsv.cn/Article/details/goaxqiqwi.sHtML

C#:   list.Add(4);
来源：http://baike.tarul.cn/Article/details/gorkufksl.sHtML

[D03] 在指定位置插入元素
来源：http://baike.tarul.cn/Article/details/gwhpgjsuo.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.tarul.cn/Article/details/gonloebng.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.tarul.cn/Article/details/gfqmzxvfi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.vehdjk.com/Article/details/guymsgqos.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.vehdjk.com/Article/details/gfisbrhhj.sHtML

Java: list.add(0, 0);
来源：http://wap.vehdjk.com/Article/details/grredtvvp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.yfazqb.com/Article/details/gucbklowe.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.sjlbkw.cn/Article/details/guysvweri.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.bbcook.cn/Article/details/gbwbjiotn.sHtML

[D04] 删除元素
来源：http://mobile.yfazqb.com/Article/details/gmhpglnam.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.vehdjk.com/Article/details/gjzgbqnjc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.epnwcf.com/Article/details/gkeqoxhqy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.tarul.cn/Article/details/gzemxmhef.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.bbcook.cn/Article/details/goavusabp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fktsv.cn/Article/details/gjckijsoh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.vehdjk.com/Article/details/gkdaphpuh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.sjlbkw.cn/Article/details/gchhcorvk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.tarul.cn/Article/details/givmfstlk.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.tarul.cn/Article/details/gnjhoazpl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.vehdjk.com/Article/details/gxijsnmwc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.sjlbkw.cn/Article/details/gkfrvibhw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.vehdjk.com/Article/details/gabrgsnxj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.sjlbkw.cn/Article/details/gtcferapo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.bbcook.cn/Article/details/gbspcwpvo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fktsv.cn/Article/details/gartdxtfp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.tarul.cn/Article/details/gtbeuptxm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.vehdjk.com/Article/details/gbrnebkdn.sHtML

[D06] 数组长度
来源：http://3g.yfazqb.com/Article/details/gynqpfzqs.sHtML

Py:   len(arr)
来源：http://blog.yfazqb.com/Article/details/gpghoeftg.sHtML

PHP:  count($arr);
来源：http://blog.yfazqb.com/Article/details/gdfjexzrf.sHtML

JS:   arr.length
来源：http://mobile.sjlbkw.cn/Article/details/gxfilypje.sHtML

TS:   arr.length
来源：http://www.blog.tarul.cn/Article/details/gwvvdmwuo.sHtML

Java: list.size();
来源：http://m.share.yfazqb.com/Article/details/ghefxosmn.sHtML

Go:   len(arr)
来源：http://read.share.epnwcf.com/Article/details/geojljdia.sHtML

Ruby: arr.length; arr.size
来源：http://wap.epnwcf.com/Article/details/gqgnzfmqc.sHtML

C#:   list.Count;
来源：http://baike.epnwcf.com/Article/details/gcfudfato.sHtML

[D07] 切片 / 取子数组
来源：http://3g.vehdjk.com/Article/details/gaibanoar.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fktsv.cn/Article/details/gwpaetkix.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.bbcook.cn/Article/details/gllfrnftk.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.yfazqb.com/Article/details/gzpppopxd.sHtML


<!-- 参考信息 -->