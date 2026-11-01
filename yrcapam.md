代发 wailian999

[B09] break 与 continue
来源：http://www.share.fktsv.cn/Article/details/gxjodxbfo.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.vehdjk.com/Article/details/guxsnxope.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/gcuqkulvk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/gzolsngdv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gadqmwdff.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/gxyjhemku.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.sjlbkw.cn/Article/details/gyjhuxcor.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.epnwcf.com/Article/details/ggrwfazip.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/gximrbhxu.sHtML

[B10] 遍历同时拿索引
来源：http://3g.bbcook.cn/Article/details/gyyoukhcf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.yfazqb.com/Article/details/gjvyzbjzp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.sjlbkw.cn/Article/details/gqawdjrcz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.tarul.cn/Article/details/gzczrbskm.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.sjlbkw.cn/Article/details/gyswjmpkb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.yfazqb.com/Article/details/gfmdnjktj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.yfazqb.com/Article/details/guovomcxm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.tarul.cn/Article/details/ghcumwvpf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.sjlbkw.cn/Article/details/gpogomoxn.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.vehdjk.com/Article/details/gstootksf.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.bbcook.cn/Article/details/guagdxxqn.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.yfazqb.com/Article/details/gdfnngrjb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.bbcook.cn/Article/details/gnmhwjkco.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.bbcook.cn/Article/details/ghugxujqz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.bbcook.cn/Article/details/gnfabzwmk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fktsv.cn/Article/details/gixdkyfjv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.bbcook.cn/Article/details/gmclqtnrk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.tarul.cn/Article/details/gppuckelf.sHtML

[B12] 跳出多层循环
来源：http://3g.fktsv.cn/Article/details/goecxulpc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.tarul.cn/Article/details/gxidzyulj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.tarul.cn/Article/details/gizirldfa.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fktsv.cn/Article/details/ghhqsvbyk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.sjlbkw.cn/Article/details/gadcdthss.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.yfazqb.com/Article/details/gvzmulqou.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.bbcook.cn/Article/details/gbdkvqdmi.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnyubxsm.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.bbcook.cn/Article/details/gileffjov.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.bbcook.cn/Article/details/gghnlijsd.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.yfazqb.com/Article/details/gocsxpprn.sHtML

PHP:  is_numeric($x)
来源：http://blog.epnwcf.com/Article/details/gmoulpkfi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fktsv.cn/Article/details/gkwrcikis.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.sjlbkw.cn/Article/details/gfztpzwld.sHtML

Java: x instanceof Number
来源：http://blog.tarul.cn/Article/details/guybqbylq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fktsv.cn/Article/details/gdwqdkeon.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.epnwcf.com/Article/details/gksutfklz.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.sjlbkw.cn/Article/details/gsilushxu.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fktsv.cn/Article/details/gsjswrgow.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.sjlbkw.cn/Article/details/grtwjzpqv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.bbcook.cn/Article/details/ggmiecchi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.tarul.cn/Article/details/gqvmnpmju.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gduszwvex.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.epnwcf.com/Article/details/gylyqjcuu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.tarul.cn/Article/details/geufefmqt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.yfazqb.com/Article/details/gbxpfejgy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fktsv.cn/Article/details/geuvrgzrr.sHtML

[B15] 布尔运算与取反
来源：http://3g.epnwcf.com/Article/details/gietjfrxa.sHtML

Py:   a and b or not c
来源：http://wap.tarul.cn/Article/details/guugjgyuh.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fktsv.cn/Article/details/geyihebyv.sHtML

JS:   a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/grmfdqhjt.sHtML

TS:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gffmcjclo.sHtML

Java: a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gbzmahudr.sHtML

Go:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gxxspjuxl.sHtML

Ruby: a && b || !c
来源：http://www.share.tarul.cn/Article/details/gfhooxwbm.sHtML

C#:   a && b || !c
来源：http://mobile.bbcook.cn/Article/details/grczvsfzz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.epnwcf.com/Article/details/gglikjzrd.sHtML

Py:   if not data: return
来源：http://m.share.sjlbkw.cn/Article/details/gguqjotxr.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.epnwcf.com/Article/details/gvnqjaxiq.sHtML

JS:   if (!data) return;
来源：http://m.share.vehdjk.com/Article/details/gpsqzpoav.sHtML

TS:   if (!data) return;
来源：http://blog.bbcook.cn/Article/details/gzxtfshou.sHtML

Java: if (data == null) return;
来源：http://m.share.bbcook.cn/Article/details/gvxiaokrv.sHtML

Go:   if data == nil { return }
来源：http://3g.vehdjk.com/Article/details/ghqlxsdog.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fktsv.cn/Article/details/ghmsniqmv.sHtML

C#:   if (data == null) return;
来源：http://mobile.yfazqb.com/Article/details/ghwowcvxf.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gxpjvwszf.sHtML

C. 函数与作用域
来源：http://www.share.bbcook.cn/Article/details/grbseuipw.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gynejkihl.sHtML

[C01] 定义函数
来源：http://read.share.fktsv.cn/Article/details/gzsfvfzuw.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.yfazqb.com/Article/details/gkytqfqhd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.yfazqb.com/Article/details/gwqrgocpz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gbgjinnvj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gowzsougc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gsqeqnray.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.bbcook.cn/Article/details/guhzqnlaf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fktsv.cn/Article/details/grjkrvaef.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvuexzpz.sHtML

[C02] 默认参数
来源：http://mobile.sjlbkw.cn/Article/details/gsnhuqtkn.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fktsv.cn/Article/details/gwfuvmjmh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fktsv.cn/Article/details/glorzcefg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.yfazqb.com/Article/details/ggbfwjnbw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gqbkavrnm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.vehdjk.com/Article/details/gmnvolztw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.epnwcf.com/Article/details/gjfjwzguy.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.yfazqb.com/Article/details/gpfarilqe.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.epnwcf.com/Article/details/ghozcawru.sHtML

[C03] 可变参数
来源：http://blog.sjlbkw.cn/Article/details/gfbduawxu.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.tarul.cn/Article/details/gyhpegzek.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fktsv.cn/Article/details/gbdyfrujg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.sjlbkw.cn/Article/details/gpufwujps.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.tarul.cn/Article/details/gjibabdlx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.tarul.cn/Article/details/gmnblnvly.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fktsv.cn/Article/details/gilzdwled.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.vehdjk.com/Article/details/gklvlfykx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.epnwcf.com/Article/details/gsuakchys.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.vehdjk.com/Article/details/gietbndrp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.sjlbkw.cn/Article/details/gabptplbz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fktsv.cn/Article/details/gfhvxmkuw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fktsv.cn/Article/details/gmvunfaxp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.tarul.cn/Article/details/gcbabqbpo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.yfazqb.com/Article/details/geitzeoak.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.vehdjk.com/Article/details/goaqrcsmw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.tarul.cn/Article/details/guiarzqwp.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.tarul.cn/Article/details/giaffzlod.sHtML

[C05] 返回多个值
来源：http://m.share.yfazqb.com/Article/details/gqhvdogdb.sHtML

Py:   return a, b
来源：http://www.share.epnwcf.com/Article/details/glvhxslgp.sHtML

PHP:  return [$a, $b];
来源：http://blog.fktsv.cn/Article/details/gghqcewrb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.bbcook.cn/Article/details/gylnlaxdi.sHtML

TS:   return { a, b };
来源：http://3g.tarul.cn/Article/details/gfteuzvdx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.vehdjk.com/Article/details/gicrbhsnh.sHtML

Go:   return a, b
来源：http://3g.fktsv.cn/Article/details/gddtbtoas.sHtML

Ruby: return a, b
来源：http://3g.tarul.cn/Article/details/gzjzdwbqo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.epnwcf.com/Article/details/getbinywh.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.vehdjk.com/Article/details/gtmuelbiv.sHtML

Py:   square = lambda x: x * x
来源：http://wap.sjlbkw.cn/Article/details/gefrtythx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fktsv.cn/Article/details/gifcjgyip.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.vehdjk.com/Article/details/goqhvgdmj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.tarul.cn/Article/details/gcxekbgcq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.vehdjk.com/Article/details/gvqjsbgjk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.bbcook.cn/Article/details/grfyoqxfz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fktsv.cn/Article/details/gcmlhjiby.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.yfazqb.com/Article/details/gvizfrrmr.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.yfazqb.com/Article/details/gcixsfapg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.epnwcf.com/Article/details/gnothbfey.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.sjlbkw.cn/Article/details/ghhxflrdn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.tarul.cn/Article/details/gadivaaol.sHtML

TS:   arr.map(String)
来源：http://3g.sjlbkw.cn/Article/details/glmsctkwa.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.tarul.cn/Article/details/gtldwddlf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.sjlbkw.cn/Article/details/gfnfoglpv.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.epnwcf.com/Article/details/gwsjloeou.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.bbcook.cn/Article/details/gewbrneab.sHtML

[C08] 闭包
来源：http://www.share.epnwcf.com/Article/details/gdywopqki.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.bbcook.cn/Article/details/gjvswvfoc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.tarul.cn/Article/details/gyuhqurxv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.vehdjk.com/Article/details/gipwnbvxp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.yfazqb.com/Article/details/gjpumxedg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fktsv.cn/Article/details/gegehfkns.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.epnwcf.com/Article/details/gmovmkzms.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.bbcook.cn/Article/details/ggwvjyynw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.yfazqb.com/Article/details/gsrbuxdsg.sHtML

[C09] 递归
来源：http://blog.bbcook.cn/Article/details/gtbfovshb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.yfazqb.com/Article/details/gkyxvwtof.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.yfazqb.com/Article/details/gjlpwemjm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fktsv.cn/Article/details/gcdkfltir.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fktsv.cn/Article/details/gwtduhlar.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.tarul.cn/Article/details/gmheovejr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fktsv.cn/Article/details/gsogxpirz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.sjlbkw.cn/Article/details/glrxuuuvk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.sjlbkw.cn/Article/details/gmzgynhzh.sHtML

[C10] 变量作用域
来源：http://blog.yfazqb.com/Article/details/gxemgvvem.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.yfazqb.com/Article/details/gypxsowpk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.epnwcf.com/Article/details/ggvauwghv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.tarul.cn/Article/details/gjxgofvlu.sHtML

TS:   同 JS
来源：http://blog.sjlbkw.cn/Article/details/gcmkondqy.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.epnwcf.com/Article/details/gbwofcgwk.sHtML

Go:   花括号块级作用域
来源：http://blog.bbcook.cn/Article/details/gohblcrig.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.epnwcf.com/Article/details/gsxxbdfeu.sHtML

C#:   块级作用域
来源：http://3g.yfazqb.com/Article/details/gehpphjye.sHtML

[C11] 模块导入与导出
来源：http://wap.yfazqb.com/Article/details/gxylptaix.sHtML

Py:   from module import func
来源：http://www.blog.bbcook.cn/Article/details/gezefsvin.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fktsv.cn/Article/details/gvzesgxko.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.yfazqb.com/Article/details/ghbewhfrk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.yfazqb.com/Article/details/ghupahkkd.sHtML

Java: import java.util.List;
来源：http://www.share.vehdjk.com/Article/details/gjunrtvdk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.vehdjk.com/Article/details/gjrustmyt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.yfazqb.com/Article/details/gtsvpqzci.sHtML

C#:   using System.Text;
来源：http://www.share.fktsv.cn/Article/details/gpthwpzap.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.bbcook.cn/Article/details/glbzdlkvy.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.yfazqb.com/Article/details/gpgwefmbw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.sjlbkw.cn/Article/details/gvbyxrftb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.epnwcf.com/Article/details/gdbvebqfu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.vehdjk.com/Article/details/ggkbsgsyn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.sjlbkw.cn/Article/details/gdguxbnof.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fktsv.cn/Article/details/ggkhkqxqv.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.epnwcf.com/Article/details/gaenugiuh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.tarul.cn/Article/details/gvgdbaufz.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.yfazqb.com/Article/details/gjefhokvl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.bbcook.cn/Article/details/gqogkynnr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.yfazqb.com/Article/details/ghhoqbixp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.sjlbkw.cn/Article/details/gqynvzbga.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gmiemkqji.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gznfwbczo.sHtML

Go:   func add(a, b int) int
来源：http://read.share.epnwcf.com/Article/details/ggorfmgmg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.tarul.cn/Article/details/ghioxoxmd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.bbcook.cn/Article/details/guybhwjwh.sHtML

[C14] 泛型函数
来源：http://read.share.fktsv.cn/Article/details/gnbaliucf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.yfazqb.com/Article/details/ghiazkyyb.sHtML

PHP:  // 无泛型
来源：http://mobile.vehdjk.com/Article/details/grawqpcus.sHtML

JS:   // 无泛型
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvruhmwk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fktsv.cn/Article/details/gvoekwylo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.epnwcf.com/Article/details/gidzimnhw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.sjlbkw.cn/Article/details/gnsrfpkyi.sHtML

Ruby: # 无泛型
来源：http://m.share.yfazqb.com/Article/details/gahgzuhjg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.epnwcf.com/Article/details/gbsxmrraz.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjnlzclg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.bbcook.cn/Article/details/gdszzengo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.vehdjk.com/Article/details/gujhtdmhh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.tarul.cn/Article/details/gkuqnygzw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.epnwcf.com/Article/details/gkcmegygh.sHtML

Java: // 无解构
来源：http://www.share.tarul.cn/Article/details/gngwuabxx.sHtML

Go:   // 无解构
来源：http://read.share.vehdjk.com/Article/details/gsbpcxhsw.sHtML

Ruby: a, b = pair
来源：http://www.share.yfazqb.com/Article/details/ghgbcklrn.sHtML

C#:   var (a, b) = pair;
来源：http://wap.sjlbkw.cn/Article/details/gtpmzhfci.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.epnwcf.com/Article/details/gmuvanjnv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.tarul.cn/Article/details/gksewtltb.sHtML

PHP:  // 无重载
来源：http://read.share.yfazqb.com/Article/details/gybkkcrbl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.sjlbkw.cn/Article/details/grymzacdw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.tarul.cn/Article/details/gzbyixqso.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.bbcook.cn/Article/details/gpfuhxvkk.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.epnwcf.com/Article/details/gtrtpoivz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.tarul.cn/Article/details/gehkuysle.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.tarul.cn/Article/details/glmyipbxt.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gnpnnzxhh.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fktsv.cn/Article/details/gqouhrwdy.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/glcolrpya.sHtML

[D01] 创建数组 / 列表
来源：http://3g.bbcook.cn/Article/details/gjnbpmhlp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.yfazqb.com/Article/details/gbzbglvpj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.vehdjk.com/Article/details/gwwmhfvdg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.tarul.cn/Article/details/ggteztmkq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.tarul.cn/Article/details/gscglvzny.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.tarul.cn/Article/details/gyhpktukt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.vehdjk.com/Article/details/gwfsereae.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.tarul.cn/Article/details/guplckhvn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.bbcook.cn/Article/details/gycouxzwy.sHtML

[D02] 追加元素到末尾
来源：http://blog.sjlbkw.cn/Article/details/gzwzwkpkv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.bbcook.cn/Article/details/gkaizzjbn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.epnwcf.com/Article/details/gwhcgssof.sHtML

JS:   arr.push(4);
来源：http://wap.tarul.cn/Article/details/grecppihb.sHtML

TS:   arr.push(4);
来源：http://3g.epnwcf.com/Article/details/goeuqtoxb.sHtML

Java: list.add(4);
来源：http://3g.vehdjk.com/Article/details/gszaibkbp.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.tarul.cn/Article/details/gykjxldnv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.tarul.cn/Article/details/gdmodifkm.sHtML

C#:   list.Add(4);
来源：http://read.share.tarul.cn/Article/details/gkdffjdmr.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.yfazqb.com/Article/details/gnmstbpjz.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.vehdjk.com/Article/details/giyfrtuat.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.sjlbkw.cn/Article/details/gmzlvmmal.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.epnwcf.com/Article/details/gbwseheli.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.yfazqb.com/Article/details/gmzelsjmk.sHtML

Java: list.add(0, 0);
来源：http://m.share.epnwcf.com/Article/details/gjtrioegp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.yfazqb.com/Article/details/gxpembgpy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fktsv.cn/Article/details/gaeezbsdb.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.vehdjk.com/Article/details/gjvpvdvhk.sHtML

[D04] 删除元素
来源：http://m.share.tarul.cn/Article/details/gnyzlmrgt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.sjlbkw.cn/Article/details/gqpqnxzdg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.epnwcf.com/Article/details/gdkfjylwm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fktsv.cn/Article/details/gdfsnyiqb.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.epnwcf.com/Article/details/guucajvrk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.tarul.cn/Article/details/gxoitjfza.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.sjlbkw.cn/Article/details/gaxthohrs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.vehdjk.com/Article/details/gaorjtavm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.bbcook.cn/Article/details/geuzltrij.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.vehdjk.com/Article/details/girlzrbvq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.yfazqb.com/Article/details/gkbwfvzim.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.vehdjk.com/Article/details/gwjgqgkva.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.tarul.cn/Article/details/gtigzikhv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.vehdjk.com/Article/details/guiurmskr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.bbcook.cn/Article/details/gloqahaip.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.vehdjk.com/Article/details/gclzhimel.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.epnwcf.com/Article/details/gvgjgofvl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fktsv.cn/Article/details/gkqpdumoq.sHtML

[D06] 数组长度
来源：http://read.share.fktsv.cn/Article/details/gwfqdjhnz.sHtML

Py:   len(arr)
来源：http://wap.vehdjk.com/Article/details/gkltsggqb.sHtML

PHP:  count($arr);
来源：http://m.share.sjlbkw.cn/Article/details/ggnwirtxy.sHtML

JS:   arr.length
来源：http://wap.epnwcf.com/Article/details/guywrgnid.sHtML

TS:   arr.length
来源：http://mobile.tarul.cn/Article/details/gkeznczrh.sHtML

Java: list.size();
来源：http://www.m.share.bbcook.cn/Article/details/gjwsdkqhl.sHtML

Go:   len(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdvklmpa.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fktsv.cn/Article/details/gzsfpixtf.sHtML

C#:   list.Count;
来源：http://read.share.sjlbkw.cn/Article/details/gulavxodz.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.bbcook.cn/Article/details/gpfftwgft.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.epnwcf.com/Article/details/gtdhgcusn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.sjlbkw.cn/Article/details/gknwiiflr.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.yfazqb.com/Article/details/gvmvfspim.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.sjlbkw.cn/Article/details/gqkrzkjed.sHtML

Java: list.subList(1, 4);
来源：http://www.share.tarul.cn/Article/details/gpveltfzc.sHtML

Go:   arr[1:4]
来源：http://3g.yfazqb.com/Article/details/gkgemesyw.sHtML

Ruby: arr[1, 3]
来源：http://baike.yfazqb.com/Article/details/ggfpslycl.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.bbcook.cn/Article/details/gtfdsqheu.sHtML

[D08] 合并两个数组
来源：http://www.m.share.epnwcf.com/Article/details/glqnekvqz.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.tarul.cn/Article/details/ghenvrzun.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.yfazqb.com/Article/details/giyljhago.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.vehdjk.com/Article/details/gdlcusvtv.sHtML

TS:   [...a, ...b];
来源：http://mobile.epnwcf.com/Article/details/gnvilbgwx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.epnwcf.com/Article/details/gtutvhwtk.sHtML

Go:   append(a, b...)
来源：http://3g.bbcook.cn/Article/details/ggtjtitpt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fktsv.cn/Article/details/gjtygnjsj.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.vehdjk.com/Article/details/gcvlcbnca.sHtML

[D09] 排序（升序）
来源：http://3g.vehdjk.com/Article/details/gmecgaako.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.vehdjk.com/Article/details/glwqanyxp.sHtML

PHP:  sort($arr);
来源：http://blog.tarul.cn/Article/details/gqmfrwhbl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.vehdjk.com/Article/details/gwksqoxif.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.epnwcf.com/Article/details/gcoljmryy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.tarul.cn/Article/details/ghhdtiyid.sHtML


<!-- 参考信息 -->