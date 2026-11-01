代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.yfazqb.com/Article/details/gwtmbvzyu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.tarul.cn/Article/details/gituufkru.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.fktsv.cn/Article/details/gzvkedvnq.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.yfazqb.com/Article/details/gjbehxocp.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.bbcook.cn/Article/details/gjhingrnv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.yfazqb.com/Article/details/gyabyacek.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.epnwcf.com/Article/details/gscvvfvdw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/gijouewib.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/gcyzazchk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.yfazqb.com/Article/details/gdlitemho.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.tarul.cn/Article/details/grusnnzjb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.yfazqb.com/Article/details/gtsgoljma.sHtML

[B09] break 与 continue
来源：http://blog.vehdjk.com/Article/details/gmwravwhy.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.epnwcf.com/Article/details/gbjxfhisy.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/gptwgolhn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/gjdxguzzd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/glhbpiqgu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/gjzewejxf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fktsv.cn/Article/details/ggqnwxxrk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.epnwcf.com/Article/details/gdhnpirik.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/gozbffkhq.sHtML

[B10] 遍历同时拿索引
来源：http://blog.vehdjk.com/Article/details/gjxfusqlc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.bbcook.cn/Article/details/glgmavspq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.tarul.cn/Article/details/genesinyb.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fktsv.cn/Article/details/grghbsssp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.sjlbkw.cn/Article/details/giwevpmbr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.bbcook.cn/Article/details/gjftcezpx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.epnwcf.com/Article/details/ghgxfawbe.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.yfazqb.com/Article/details/gpgxtaskm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.fktsv.cn/Article/details/gqpnssfgf.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.epnwcf.com/Article/details/grxtvtkkj.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.sjlbkw.cn/Article/details/gxmzhaebt.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fktsv.cn/Article/details/gmwkxregp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.sjlbkw.cn/Article/details/gygcjjani.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fktsv.cn/Article/details/ghkngwjkh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fktsv.cn/Article/details/ghqvvfyys.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.vehdjk.com/Article/details/gviikvvak.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.vehdjk.com/Article/details/gvkpgbhch.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.sjlbkw.cn/Article/details/glqnzwqac.sHtML

[B12] 跳出多层循环
来源：http://baike.sjlbkw.cn/Article/details/gcivjwerb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.sjlbkw.cn/Article/details/gydsaaspv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.epnwcf.com/Article/details/giuuzthxd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fktsv.cn/Article/details/gbojrqjoc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.sjlbkw.cn/Article/details/gbknfkwiy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.epnwcf.com/Article/details/gttiauemx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.sjlbkw.cn/Article/details/gbzflbtke.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.bbcook.cn/Article/details/guikqlxxu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fktsv.cn/Article/details/gnmaqfjqh.sHtML

[B13] 判断是否为数字
来源：http://blog.vehdjk.com/Article/details/gfdbjbxmm.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.tarul.cn/Article/details/gymuxqrcm.sHtML

PHP:  is_numeric($x)
来源：http://read.share.sjlbkw.cn/Article/details/gucprjcvx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.sjlbkw.cn/Article/details/gibsqdusw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkzxptmvn.sHtML

Java: x instanceof Number
来源：http://mobile.epnwcf.com/Article/details/gsgxjxxfa.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.epnwcf.com/Article/details/gnpprybrk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.bbcook.cn/Article/details/gsmlfxqxx.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fktsv.cn/Article/details/gxqeqdqot.sHtML

[B14] 判断值是否在集合内
来源：http://3g.epnwcf.com/Article/details/gjeknelpj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.sjlbkw.cn/Article/details/gbiimqkqn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.tarul.cn/Article/details/gwxuzlepo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.bbcook.cn/Article/details/gzwnkxbyv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.vehdjk.com/Article/details/gtibmxiie.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.yfazqb.com/Article/details/gjwkfytuc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.vehdjk.com/Article/details/gmjpknqis.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.vehdjk.com/Article/details/gewahtiam.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.epnwcf.com/Article/details/gnggdrllw.sHtML

[B15] 布尔运算与取反
来源：http://wap.tarul.cn/Article/details/gpvkzljpj.sHtML

Py:   a and b or not c
来源：http://m.share.bbcook.cn/Article/details/gcubyccjv.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.vehdjk.com/Article/details/gtoiyxcbd.sHtML

JS:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/ggroipudv.sHtML

TS:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/gozlyjthq.sHtML

Java: a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gxedoquqo.sHtML

Go:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gvdujtomw.sHtML

Ruby: a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gddiezwhs.sHtML

C#:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/goszjdajd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.epnwcf.com/Article/details/gflsmakfb.sHtML

Py:   if not data: return
来源：http://mobile.sjlbkw.cn/Article/details/ghmcecadn.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.yfazqb.com/Article/details/gwxdhniyo.sHtML

JS:   if (!data) return;
来源：http://www.share.yfazqb.com/Article/details/glfiobcbc.sHtML

TS:   if (!data) return;
来源：http://wap.epnwcf.com/Article/details/gzclhucqh.sHtML

Java: if (data == null) return;
来源：http://baike.sjlbkw.cn/Article/details/grlvaoqdg.sHtML

Go:   if data == nil { return }
来源：http://baike.bbcook.cn/Article/details/gbjmjvzul.sHtML

Ruby: return if data.nil?
来源：http://m.share.epnwcf.com/Article/details/godwsvpai.sHtML

C#:   if (data == null) return;
来源：http://baike.vehdjk.com/Article/details/gddcxcbht.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gvatkkpze.sHtML

C. 函数与作用域
来源：http://3g.yfazqb.com/Article/details/gqmwhbimo.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gjskiembg.sHtML

[C01] 定义函数
来源：http://www.share.sjlbkw.cn/Article/details/getyailfj.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.bbcook.cn/Article/details/gwftcamrg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/gqfvjuvzi.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gjonhrhij.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gbyraetqy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gngbaycdg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.sjlbkw.cn/Article/details/gjrbrvrja.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.tarul.cn/Article/details/gjuzwhhnr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gdpjzfgmv.sHtML

[C02] 默认参数
来源：http://www.blog.bbcook.cn/Article/details/gziigqpwj.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.sjlbkw.cn/Article/details/glxyipeyx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.yfazqb.com/Article/details/gghtjvukv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fktsv.cn/Article/details/gxvcyaskh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.vehdjk.com/Article/details/grgzdelyw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.vehdjk.com/Article/details/gqlqbcfxz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.vehdjk.com/Article/details/ghigzwgnj.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.bbcook.cn/Article/details/gzmgpvwlz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.tarul.cn/Article/details/gsxzsmwmi.sHtML

[C03] 可变参数
来源：http://www.m.share.epnwcf.com/Article/details/gjdykclzk.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.epnwcf.com/Article/details/gkzvulyqn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.sjlbkw.cn/Article/details/gvwxtmjiv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.vehdjk.com/Article/details/gvyeyghcx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.tarul.cn/Article/details/gnspgdnve.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.sjlbkw.cn/Article/details/gmpgbildc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fktsv.cn/Article/details/ghzqfctip.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.sjlbkw.cn/Article/details/gnruquvqz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.tarul.cn/Article/details/gwysdqxbb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.vehdjk.com/Article/details/gmhllxehl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.yfazqb.com/Article/details/gyjlbbmpj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.sjlbkw.cn/Article/details/gvdnewwac.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fktsv.cn/Article/details/gndvmmiaj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.tarul.cn/Article/details/guiyxnumn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.vehdjk.com/Article/details/ghjpmerxd.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.yfazqb.com/Article/details/gissbrcoz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.sjlbkw.cn/Article/details/gqgjfznlj.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.yfazqb.com/Article/details/gtkgrttin.sHtML

[C05] 返回多个值
来源：http://blog.epnwcf.com/Article/details/gfkwittgw.sHtML

Py:   return a, b
来源：http://www.m.share.fktsv.cn/Article/details/gcqfqavtq.sHtML

PHP:  return [$a, $b];
来源：http://blog.tarul.cn/Article/details/ggwiayeqe.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.yfazqb.com/Article/details/gyihjvzpf.sHtML

TS:   return { a, b };
来源：http://blog.fktsv.cn/Article/details/gqcncmsex.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.epnwcf.com/Article/details/gvfrsyfff.sHtML

Go:   return a, b
来源：http://www.blog.yfazqb.com/Article/details/gvjviayys.sHtML

Ruby: return a, b
来源：http://www.m.share.sjlbkw.cn/Article/details/grlxmnlte.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.sjlbkw.cn/Article/details/ggxgllcfw.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.tarul.cn/Article/details/grexorgtw.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fktsv.cn/Article/details/gtsclrdzg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.bbcook.cn/Article/details/gufjltuum.sHtML

JS:   const square = x => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gniepysbz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.bbcook.cn/Article/details/govepmwvv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.yfazqb.com/Article/details/gkqmpvoab.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.sjlbkw.cn/Article/details/guziorgez.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.epnwcf.com/Article/details/gwvlpekth.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.bbcook.cn/Article/details/grcuxiwoh.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.sjlbkw.cn/Article/details/ggsvunqhc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.yfazqb.com/Article/details/gixrkbwmo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.bbcook.cn/Article/details/grngrvuqg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.sjlbkw.cn/Article/details/ggjshqwbz.sHtML

TS:   arr.map(String)
来源：http://3g.vehdjk.com/Article/details/gfnrsismj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.tarul.cn/Article/details/gysmxydrs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.vehdjk.com/Article/details/gvmapjgth.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.sjlbkw.cn/Article/details/grjlzunkr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.sjlbkw.cn/Article/details/gawegkscg.sHtML

[C08] 闭包
来源：http://3g.yfazqb.com/Article/details/gzqnjxbys.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.epnwcf.com/Article/details/gkbvfpiwj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.epnwcf.com/Article/details/ggpoiopbt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.vehdjk.com/Article/details/gfdeuqauf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/gsvdiojso.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fktsv.cn/Article/details/gbhvoeuub.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.tarul.cn/Article/details/ggxvnytuz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fktsv.cn/Article/details/gtdlxrsui.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.epnwcf.com/Article/details/gbfxcjmxa.sHtML

[C09] 递归
来源：http://3g.bbcook.cn/Article/details/gjgttehvq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.bbcook.cn/Article/details/gwmtrdlmq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.sjlbkw.cn/Article/details/gzmtkwmnh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.yfazqb.com/Article/details/gmjdhozyu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fktsv.cn/Article/details/ghkikolic.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.tarul.cn/Article/details/gnzdxnsld.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.sjlbkw.cn/Article/details/gbfffnhdn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.bbcook.cn/Article/details/gcgaavauj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.tarul.cn/Article/details/ggyhvhdtp.sHtML

[C10] 变量作用域
来源：http://www.share.epnwcf.com/Article/details/gemopnzrk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.yfazqb.com/Article/details/gjckrczmi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fktsv.cn/Article/details/gzppxbnbv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.vehdjk.com/Article/details/gtypugmbv.sHtML

TS:   同 JS
来源：http://wap.yfazqb.com/Article/details/gtwsxuamq.sHtML

Java: 方法内为块级作用域
来源：http://mobile.sjlbkw.cn/Article/details/gyxhdzgav.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fktsv.cn/Article/details/gjwfheohw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fktsv.cn/Article/details/gpmzvtvjm.sHtML

C#:   块级作用域
来源：http://www.blog.tarul.cn/Article/details/grkpkdrtb.sHtML

[C11] 模块导入与导出
来源：http://3g.tarul.cn/Article/details/gmxwdbfao.sHtML

Py:   from module import func
来源：http://www.m.share.bbcook.cn/Article/details/gmsypjjop.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.vehdjk.com/Article/details/goduzjydq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.bbcook.cn/Article/details/gtgeicyza.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fktsv.cn/Article/details/gqzdtueyx.sHtML

Java: import java.util.List;
来源：http://www.m.share.yfazqb.com/Article/details/gnrbyflsp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.tarul.cn/Article/details/gnefvaqsp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.tarul.cn/Article/details/gzbmemktz.sHtML

C#:   using System.Text;
来源：http://read.share.fktsv.cn/Article/details/gsrurgxzb.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.sjlbkw.cn/Article/details/gehzfkusa.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.tarul.cn/Article/details/grisqofjq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fktsv.cn/Article/details/gxxxdkswi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.sjlbkw.cn/Article/details/gfuxqrbtn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.bbcook.cn/Article/details/gtuthbzrw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.yfazqb.com/Article/details/ggxqvzoqu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.bbcook.cn/Article/details/gjhdvhaxg.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.vehdjk.com/Article/details/glrjmxled.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.yfazqb.com/Article/details/gfdsdgost.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.vehdjk.com/Article/details/gucudfbyi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.tarul.cn/Article/details/glsxrinpu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/gajyijhnc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.vehdjk.com/Article/details/glrofxknp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gtajmxuhd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gyumdswzo.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.yfazqb.com/Article/details/gifzgqpzs.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.bbcook.cn/Article/details/gefzbrzzo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.sjlbkw.cn/Article/details/gvdmuukjl.sHtML

[C14] 泛型函数
来源：http://wap.bbcook.cn/Article/details/gdoqbgefa.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.yfazqb.com/Article/details/gkvheztzq.sHtML

PHP:  // 无泛型
来源：http://3g.bbcook.cn/Article/details/gqowhxnhh.sHtML

JS:   // 无泛型
来源：http://www.share.sjlbkw.cn/Article/details/gqrjfrcss.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.tarul.cn/Article/details/gqklccjhx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.epnwcf.com/Article/details/gkqdblkzl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.epnwcf.com/Article/details/ginzgpwuf.sHtML

Ruby: # 无泛型
来源：http://www.share.fktsv.cn/Article/details/gksujytng.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.vehdjk.com/Article/details/gtdkmqsav.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.bbcook.cn/Article/details/gpjilutsa.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.epnwcf.com/Article/details/gypbhmuyl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.yfazqb.com/Article/details/guhurbdtk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.epnwcf.com/Article/details/gscrtsjfy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.epnwcf.com/Article/details/gdgnzwuow.sHtML

Java: // 无解构
来源：http://www.blog.yfazqb.com/Article/details/gzmdiupkx.sHtML

Go:   // 无解构
来源：http://baike.bbcook.cn/Article/details/gffvcqoyp.sHtML

Ruby: a, b = pair
来源：http://www.share.tarul.cn/Article/details/gkulwmpha.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fktsv.cn/Article/details/gzlqqmxly.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.epnwcf.com/Article/details/glxxepomu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.vehdjk.com/Article/details/gvtvuieyj.sHtML

PHP:  // 无重载
来源：http://baike.vehdjk.com/Article/details/giaroybzz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.vehdjk.com/Article/details/gbborebjh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.tarul.cn/Article/details/gjdzcxbmn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.yfazqb.com/Article/details/gmydkjkag.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fktsv.cn/Article/details/gypyhrdxt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.sjlbkw.cn/Article/details/gtairgrpf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.tarul.cn/Article/details/ghknounqd.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/glevqpjbg.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.tarul.cn/Article/details/gjzdttxdj.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gjysaqtav.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fktsv.cn/Article/details/gxlvmgnfb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.sjlbkw.cn/Article/details/gwhmgxcdt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.tarul.cn/Article/details/gpuhjukfz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.vehdjk.com/Article/details/gvzncetgm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.bbcook.cn/Article/details/gxosqguul.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fktsv.cn/Article/details/gilnhupln.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.tarul.cn/Article/details/gckbdakiy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.tarul.cn/Article/details/gilcmutpe.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.sjlbkw.cn/Article/details/gkfxotdfv.sHtML

[D02] 追加元素到末尾
来源：http://baike.yfazqb.com/Article/details/gepzuaznw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.bbcook.cn/Article/details/goaefbbdt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqilsbnr.sHtML

JS:   arr.push(4);
来源：http://m.share.vehdjk.com/Article/details/gbkhjwkgv.sHtML

TS:   arr.push(4);
来源：http://www.share.fktsv.cn/Article/details/grwxdocxc.sHtML

Java: list.add(4);
来源：http://3g.sjlbkw.cn/Article/details/gfktvbodi.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.yfazqb.com/Article/details/gnkucevlj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.epnwcf.com/Article/details/gxvriekxp.sHtML

C#:   list.Add(4);
来源：http://mobile.yfazqb.com/Article/details/gjisyslho.sHtML

[D03] 在指定位置插入元素
来源：http://blog.yfazqb.com/Article/details/gsovluoxt.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fktsv.cn/Article/details/gtskofxbv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.yfazqb.com/Article/details/gewppgjpg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.sjlbkw.cn/Article/details/gphapgovp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.vehdjk.com/Article/details/glmwldnrt.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.tarul.cn/Article/details/gdihmsubo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.epnwcf.com/Article/details/glbsgkqvm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fktsv.cn/Article/details/gysulkaho.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.yfazqb.com/Article/details/gdjqopyrm.sHtML

[D04] 删除元素
来源：http://m.share.fktsv.cn/Article/details/gncavdaca.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fktsv.cn/Article/details/gsrrbgira.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gpjhdmaas.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.epnwcf.com/Article/details/gbjjpizzl.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fktsv.cn/Article/details/gsmgytxop.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.vehdjk.com/Article/details/gqjontkye.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fktsv.cn/Article/details/gchmzzfuv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.tarul.cn/Article/details/gegqvqylr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.bbcook.cn/Article/details/ghnjqddwh.sHtML

[D05] 访问与修改元素
来源：http://read.share.sjlbkw.cn/Article/details/gftdusggd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fktsv.cn/Article/details/gudsdcquj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.epnwcf.com/Article/details/glxlcxjkc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.epnwcf.com/Article/details/gcbhgmtku.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.vehdjk.com/Article/details/gydudtgxp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.vehdjk.com/Article/details/gxqieqbyz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.tarul.cn/Article/details/gbiffdtlm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.sjlbkw.cn/Article/details/gfveeyieh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.tarul.cn/Article/details/gyxufeeuo.sHtML

[D06] 数组长度
来源：http://read.share.epnwcf.com/Article/details/gyloiomnb.sHtML

Py:   len(arr)
来源：http://www.m.share.fktsv.cn/Article/details/grzvgxxod.sHtML

PHP:  count($arr);
来源：http://wap.bbcook.cn/Article/details/gtfmwyyuz.sHtML

JS:   arr.length
来源：http://mobile.sjlbkw.cn/Article/details/grjpwghij.sHtML

TS:   arr.length
来源：http://www.share.sjlbkw.cn/Article/details/gxzfdesiq.sHtML

Java: list.size();
来源：http://3g.epnwcf.com/Article/details/gxokfwuce.sHtML

Go:   len(arr)
来源：http://baike.sjlbkw.cn/Article/details/gucucdvle.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.bbcook.cn/Article/details/gidxlrmfi.sHtML

C#:   list.Count;
来源：http://3g.vehdjk.com/Article/details/gyckakrbn.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fktsv.cn/Article/details/ggqaksqpe.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfjsmzjz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.tarul.cn/Article/details/glzkovfhw.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.epnwcf.com/Article/details/gzwyhwcpb.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.bbcook.cn/Article/details/ghgkofbcg.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fktsv.cn/Article/details/ghbjiyszu.sHtML

Go:   arr[1:4]
来源：http://www.share.fktsv.cn/Article/details/gtjqucdzl.sHtML

Ruby: arr[1, 3]
来源：http://blog.sjlbkw.cn/Article/details/gfynzirca.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.yfazqb.com/Article/details/gtfeaxrtb.sHtML

[D08] 合并两个数组
来源：http://baike.fktsv.cn/Article/details/gxjdujpsi.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.bbcook.cn/Article/details/glnakhprx.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fktsv.cn/Article/details/gktpfjrfm.sHtML


<!-- 参考信息 -->