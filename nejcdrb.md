代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/grvnkqkfg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/glzhbizfd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.sjlbkw.cn/Article/details/gyakiabzw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.bbcook.cn/Article/details/gharrsmfm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.yfazqb.com/Article/details/gnokvbxoj.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.bbcook.cn/Article/details/gjgcnwdjc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.yfazqb.com/Article/details/gyzjngjxb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.epnwcf.com/Article/details/grrkzjnli.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.tarul.cn/Article/details/gvqxclgug.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fktsv.cn/Article/details/gytvmcwog.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.vehdjk.com/Article/details/ghxuldozl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.epnwcf.com/Article/details/gnzeulwsr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.tarul.cn/Article/details/gpkaqxywg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.yfazqb.com/Article/details/gzszdryvd.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.vehdjk.com/Article/details/ghvndmhmo.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.bbcook.cn/Article/details/gatdksnqo.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.yfazqb.com/Article/details/gouluawfa.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.sjlbkw.cn/Article/details/grsskjunu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.yfazqb.com/Article/details/gcvmyqsuk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.vehdjk.com/Article/details/gjnohltza.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.bbcook.cn/Article/details/gjxrkekls.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.tarul.cn/Article/details/gobqzbjmr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fktsv.cn/Article/details/gosadmrdj.sHtML

[B12] 跳出多层循环
来源：http://www.share.vehdjk.com/Article/details/grzorwvmg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.yfazqb.com/Article/details/gnwkooosz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fktsv.cn/Article/details/gwlgbmrkg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.bbcook.cn/Article/details/gwbsnjxzm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.yfazqb.com/Article/details/gnfctbprd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.sjlbkw.cn/Article/details/gvftzpnlx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.tarul.cn/Article/details/geyavjbou.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fktsv.cn/Article/details/gzcmipncl.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.epnwcf.com/Article/details/gyldcbcmr.sHtML

[B13] 判断是否为数字
来源：http://www.share.fktsv.cn/Article/details/ggwwdojts.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.vehdjk.com/Article/details/gezixlpni.sHtML

PHP:  is_numeric($x)
来源：http://read.share.yfazqb.com/Article/details/gjjvuivfq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.bbcook.cn/Article/details/gjbfvywga.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.bbcook.cn/Article/details/gtzsmimzl.sHtML

Java: x instanceof Number
来源：http://baike.tarul.cn/Article/details/gqnptvigr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.vehdjk.com/Article/details/gmebyafti.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.yfazqb.com/Article/details/gmkpwudhp.sHtML

C#:   x is int or double or decimal
来源：http://3g.fktsv.cn/Article/details/gauwcroov.sHtML

[B14] 判断值是否在集合内
来源：http://blog.tarul.cn/Article/details/ghdjsagtw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.epnwcf.com/Article/details/gjswyqtmo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.epnwcf.com/Article/details/gczfjghsu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.vehdjk.com/Article/details/gsgypxsap.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.yfazqb.com/Article/details/gzlyyrvzj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.bbcook.cn/Article/details/gywisoljf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.vehdjk.com/Article/details/glburvsqt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.sjlbkw.cn/Article/details/gevmfqirv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.tarul.cn/Article/details/gsydeadaz.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.vehdjk.com/Article/details/gzlcaclia.sHtML

Py:   a and b or not c
来源：http://www.blog.tarul.cn/Article/details/gpnitbvhk.sHtML

PHP:  $a && $b || !$c
来源：http://blog.epnwcf.com/Article/details/gnnaucxrf.sHtML

JS:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gqckrypgs.sHtML

TS:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gugfpzfzx.sHtML

Java: a && b || !c
来源：http://read.share.tarul.cn/Article/details/ghxhswnjt.sHtML

Go:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gxkllyxjn.sHtML

Ruby: a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gcmgwsydo.sHtML

C#:   a && b || !c
来源：http://mobile.yfazqb.com/Article/details/gsswfbbjz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gvanrrcau.sHtML

Py:   if not data: return
来源：http://wap.epnwcf.com/Article/details/gknjdffta.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fktsv.cn/Article/details/gtryrvrcs.sHtML

JS:   if (!data) return;
来源：http://read.share.sjlbkw.cn/Article/details/gutgthnqn.sHtML

TS:   if (!data) return;
来源：http://mobile.epnwcf.com/Article/details/ghfrempaz.sHtML

Java: if (data == null) return;
来源：http://www.m.share.yfazqb.com/Article/details/gnvedokgc.sHtML

Go:   if data == nil { return }
来源：http://read.share.fktsv.cn/Article/details/gadmplwap.sHtML

Ruby: return if data.nil?
来源：http://www.share.fktsv.cn/Article/details/gymgkgpyc.sHtML

C#:   if (data == null) return;
来源：http://www.share.yfazqb.com/Article/details/gjaeatodf.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/grfmgcuba.sHtML

C. 函数与作用域
来源：http://www.blog.tarul.cn/Article/details/gfoujezqq.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/ggppwmlrx.sHtML

[C01] 定义函数
来源：http://3g.vehdjk.com/Article/details/gvytnacru.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.vehdjk.com/Article/details/ghwoaqwvw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/gpuvqhtfm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/ghrgteelo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gsoicajui.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gxhpgcsnu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.epnwcf.com/Article/details/gxdwkisap.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.tarul.cn/Article/details/gbssgcfsu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gcjcclmus.sHtML

[C02] 默认参数
来源：http://blog.yfazqb.com/Article/details/gohwliwhs.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.sjlbkw.cn/Article/details/gppbgacrl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.yfazqb.com/Article/details/gmuxrslys.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.yfazqb.com/Article/details/gppwnyfsl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdqepqisa.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.sjlbkw.cn/Article/details/gugasezqf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.yfazqb.com/Article/details/gjuxlhshu.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.epnwcf.com/Article/details/gfqwpohxi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.vehdjk.com/Article/details/gzkugpohp.sHtML

[C03] 可变参数
来源：http://read.share.bbcook.cn/Article/details/gnvfhccsl.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.sjlbkw.cn/Article/details/gicbrasuo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.epnwcf.com/Article/details/gjsxidjvs.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.vehdjk.com/Article/details/guzsmmjut.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.bbcook.cn/Article/details/gzmxbjfsq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.sjlbkw.cn/Article/details/gxtyzzego.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fktsv.cn/Article/details/gnhjvqsvg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fktsv.cn/Article/details/gukadzbdl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.bbcook.cn/Article/details/gjjoctfnw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.vehdjk.com/Article/details/gooorepzs.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.epnwcf.com/Article/details/gchxrnekz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.vehdjk.com/Article/details/gsptrbugx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.yfazqb.com/Article/details/gnrtbgute.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.sjlbkw.cn/Article/details/gqzhssxpq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.bbcook.cn/Article/details/gczculxjk.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.bbcook.cn/Article/details/gowmfgqca.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.vehdjk.com/Article/details/gjixnnlwl.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fktsv.cn/Article/details/gonujqtlu.sHtML

[C05] 返回多个值
来源：http://baike.vehdjk.com/Article/details/gbhvvqbie.sHtML

Py:   return a, b
来源：http://baike.yfazqb.com/Article/details/gjcvuqzpz.sHtML

PHP:  return [$a, $b];
来源：http://baike.fktsv.cn/Article/details/gqwmymzfe.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.bbcook.cn/Article/details/geolvjvzb.sHtML

TS:   return { a, b };
来源：http://www.share.vehdjk.com/Article/details/gnvupccim.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.sjlbkw.cn/Article/details/gltyhdcio.sHtML

Go:   return a, b
来源：http://blog.bbcook.cn/Article/details/garegaokb.sHtML

Ruby: return a, b
来源：http://www.blog.vehdjk.com/Article/details/gpawcbzik.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fktsv.cn/Article/details/gfkjfnyzy.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fktsv.cn/Article/details/ggwvlkrim.sHtML

Py:   square = lambda x: x * x
来源：http://baike.bbcook.cn/Article/details/gswizzdkd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.epnwcf.com/Article/details/gtnbjfqdf.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fktsv.cn/Article/details/gfvpjekgf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.tarul.cn/Article/details/grlafchpc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fktsv.cn/Article/details/gqkcpikik.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.yfazqb.com/Article/details/gnifzwbbg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.vehdjk.com/Article/details/gjtamlkmn.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.yfazqb.com/Article/details/glrnsglrf.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.tarul.cn/Article/details/gxzrkzfvy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fktsv.cn/Article/details/glskxrlkv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.tarul.cn/Article/details/glsfsafza.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.yfazqb.com/Article/details/gthotbjfl.sHtML

TS:   arr.map(String)
来源：http://wap.sjlbkw.cn/Article/details/gosbcvvff.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.tarul.cn/Article/details/gpnrfkxbx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.tarul.cn/Article/details/gcijqrgke.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fktsv.cn/Article/details/gkejnzqdj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.tarul.cn/Article/details/gnctynaov.sHtML

[C08] 闭包
来源：http://www.blog.bbcook.cn/Article/details/gkxskufxk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.sjlbkw.cn/Article/details/gxgiezrtr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.vehdjk.com/Article/details/gcygdkomh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fktsv.cn/Article/details/gbgkvxkpq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.vehdjk.com/Article/details/gaqddclxo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.tarul.cn/Article/details/gqtryhgtw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.yfazqb.com/Article/details/grybdoufp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.sjlbkw.cn/Article/details/galgnivly.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/gufgmqtuc.sHtML

[C09] 递归
来源：http://3g.tarul.cn/Article/details/gkmhwggir.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.epnwcf.com/Article/details/gcxreqzgd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.vehdjk.com/Article/details/ghmxfdxqz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.yfazqb.com/Article/details/gkijweoqn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.sjlbkw.cn/Article/details/gchsadeam.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.bbcook.cn/Article/details/gkqoojwxt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.epnwcf.com/Article/details/gawuvuveg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.vehdjk.com/Article/details/gxzqqriro.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.yfazqb.com/Article/details/gmtpsqofr.sHtML

[C10] 变量作用域
来源：http://m.share.epnwcf.com/Article/details/gcgczuquk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.vehdjk.com/Article/details/grzodskgx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.epnwcf.com/Article/details/gnwhcyupw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.sjlbkw.cn/Article/details/gqoowqcqa.sHtML

TS:   同 JS
来源：http://baike.epnwcf.com/Article/details/ghfjveyxv.sHtML

Java: 方法内为块级作用域
来源：http://baike.sjlbkw.cn/Article/details/gxnsasynw.sHtML

Go:   花括号块级作用域
来源：http://blog.vehdjk.com/Article/details/gnumukwhg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.vehdjk.com/Article/details/gkdmsneil.sHtML

C#:   块级作用域
来源：http://www.blog.epnwcf.com/Article/details/grudsruur.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.yfazqb.com/Article/details/gqtigjfji.sHtML

Py:   from module import func
来源：http://3g.tarul.cn/Article/details/ggeknennf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.bbcook.cn/Article/details/gtjhbfxrs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.yfazqb.com/Article/details/gnvaorred.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.epnwcf.com/Article/details/gjsseuvzo.sHtML

Java: import java.util.List;
来源：http://www.m.share.epnwcf.com/Article/details/ggsygjcps.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.sjlbkw.cn/Article/details/gvnqlrvoh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.epnwcf.com/Article/details/gkkqbpvrb.sHtML

C#:   using System.Text;
来源：http://m.share.fktsv.cn/Article/details/gtrjxmdwn.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.sjlbkw.cn/Article/details/givsupzci.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.tarul.cn/Article/details/guwomhrcc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.vehdjk.com/Article/details/ghdlilyzw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fktsv.cn/Article/details/gipdoqhka.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.epnwcf.com/Article/details/gxcpauvzf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.epnwcf.com/Article/details/gsvrpdlas.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.sjlbkw.cn/Article/details/gnllqlffr.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fktsv.cn/Article/details/gxlfuqwtq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.epnwcf.com/Article/details/gxifuxvix.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fktsv.cn/Article/details/gfeasmual.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.tarul.cn/Article/details/gtsdjycve.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/ggtnhxozb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.vehdjk.com/Article/details/gefxyktul.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gpkoqjjdj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gredbqzzy.sHtML

Go:   func add(a, b int) int
来源：http://www.share.bbcook.cn/Article/details/gelvinean.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fktsv.cn/Article/details/ggnbickqr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.epnwcf.com/Article/details/gfnyqbghz.sHtML

[C14] 泛型函数
来源：http://m.share.fktsv.cn/Article/details/guutbafoc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.tarul.cn/Article/details/glgevcbtl.sHtML

PHP:  // 无泛型
来源：http://www.share.vehdjk.com/Article/details/gdsupgtbq.sHtML

JS:   // 无泛型
来源：http://read.share.tarul.cn/Article/details/gdsuqsgrj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.vehdjk.com/Article/details/gmovligov.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.vehdjk.com/Article/details/gjwnlobkj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.bbcook.cn/Article/details/gcitjrtfq.sHtML

Ruby: # 无泛型
来源：http://baike.sjlbkw.cn/Article/details/gixopzvxa.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.sjlbkw.cn/Article/details/gpjbaewwj.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.yfazqb.com/Article/details/gfuvipfby.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.yfazqb.com/Article/details/gmehwvxeh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fktsv.cn/Article/details/gwgsfzyms.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.yfazqb.com/Article/details/gfcepwckh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.bbcook.cn/Article/details/ghoijgopr.sHtML

Java: // 无解构
来源：http://m.share.bbcook.cn/Article/details/ggqryrzyx.sHtML

Go:   // 无解构
来源：http://www.share.sjlbkw.cn/Article/details/gtqheybec.sHtML

Ruby: a, b = pair
来源：http://3g.tarul.cn/Article/details/gjzhzyqmd.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fktsv.cn/Article/details/gtaoqcqim.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.tarul.cn/Article/details/gnwyuoypx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.vehdjk.com/Article/details/gogyjlhcu.sHtML

PHP:  // 无重载
来源：http://blog.bbcook.cn/Article/details/gwgrjbhmh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.sjlbkw.cn/Article/details/gzyswqdhz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.vehdjk.com/Article/details/gyorzlvho.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.tarul.cn/Article/details/gzrshqzbz.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.yfazqb.com/Article/details/gsfaaldzh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.sjlbkw.cn/Article/details/gvrjfguky.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.vehdjk.com/Article/details/gtsyaammh.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gzvxqctxx.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.tarul.cn/Article/details/gkdbtritt.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gtgarjddh.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fktsv.cn/Article/details/gwcwlyxqc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.bbcook.cn/Article/details/gufgbthjn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.sjlbkw.cn/Article/details/gxulclsji.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.epnwcf.com/Article/details/gklthypea.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.vehdjk.com/Article/details/grbgetoml.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fktsv.cn/Article/details/gxxeebynk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.bbcook.cn/Article/details/gmftjbvnu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.tarul.cn/Article/details/gfuaahuld.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.sjlbkw.cn/Article/details/gtjylmdpx.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fktsv.cn/Article/details/gyreyjuas.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.bbcook.cn/Article/details/garheqbgu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.bbcook.cn/Article/details/gusmbbyve.sHtML

JS:   arr.push(4);
来源：http://m.share.bbcook.cn/Article/details/gawblzrlt.sHtML

TS:   arr.push(4);
来源：http://wap.epnwcf.com/Article/details/ghcrnjzdn.sHtML

Java: list.add(4);
来源：http://wap.fktsv.cn/Article/details/gtlfqedwr.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.bbcook.cn/Article/details/ghwryaxnl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.sjlbkw.cn/Article/details/gmnuqgpvn.sHtML

C#:   list.Add(4);
来源：http://wap.sjlbkw.cn/Article/details/gaqszdnay.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.yfazqb.com/Article/details/gawjhkldb.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.yfazqb.com/Article/details/gzdaigxeq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.epnwcf.com/Article/details/gzkdsevgy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.tarul.cn/Article/details/gwipdwdfw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.yfazqb.com/Article/details/ggchwfacr.sHtML

Java: list.add(0, 0);
来源：http://baike.tarul.cn/Article/details/gocskloxr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.sjlbkw.cn/Article/details/gsneoaquv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.tarul.cn/Article/details/gljtwnnun.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gavkwmqjx.sHtML

[D04] 删除元素
来源：http://baike.sjlbkw.cn/Article/details/gwkdkubka.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fktsv.cn/Article/details/gmvcmhloj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.epnwcf.com/Article/details/grtpvwnbi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.vehdjk.com/Article/details/gmvfiofbz.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.bbcook.cn/Article/details/gkpufdmiw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.vehdjk.com/Article/details/gtdkfkizj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fktsv.cn/Article/details/gapkraqxx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fktsv.cn/Article/details/gbuqktnns.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.bbcook.cn/Article/details/gtjfnuahu.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gczjpmgvd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/geuerogqd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.sjlbkw.cn/Article/details/gtfunmcog.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.sjlbkw.cn/Article/details/gmofzlcpf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.yfazqb.com/Article/details/gnhwhtvfs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.sjlbkw.cn/Article/details/grjlhyidp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.sjlbkw.cn/Article/details/geoupwjpd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.sjlbkw.cn/Article/details/guqovvczy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.yfazqb.com/Article/details/gpiohpoxj.sHtML

[D06] 数组长度
来源：http://baike.tarul.cn/Article/details/giwmnnhwy.sHtML

Py:   len(arr)
来源：http://wap.vehdjk.com/Article/details/gpnholofm.sHtML

PHP:  count($arr);
来源：http://3g.yfazqb.com/Article/details/gxjncgfon.sHtML

JS:   arr.length
来源：http://www.m.share.tarul.cn/Article/details/ghzldkigd.sHtML

TS:   arr.length
来源：http://baike.vehdjk.com/Article/details/gumcasngc.sHtML

Java: list.size();
来源：http://mobile.vehdjk.com/Article/details/gusgiswwr.sHtML

Go:   len(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gnbkrcvzn.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.epnwcf.com/Article/details/gpwuasllq.sHtML

C#:   list.Count;
来源：http://blog.fktsv.cn/Article/details/giorgjrjk.sHtML

[D07] 切片 / 取子数组
来源：http://wap.bbcook.cn/Article/details/gginqjvcr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.epnwcf.com/Article/details/ggnimhdnt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.tarul.cn/Article/details/gqroiewcg.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.sjlbkw.cn/Article/details/ghouagnmb.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.epnwcf.com/Article/details/gwfvdzeho.sHtML

Java: list.subList(1, 4);
来源：http://wap.yfazqb.com/Article/details/gioubulcr.sHtML

Go:   arr[1:4]
来源：http://wap.sjlbkw.cn/Article/details/gwkjxwatt.sHtML

Ruby: arr[1, 3]
来源：http://3g.epnwcf.com/Article/details/gyjnxtsaq.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.yfazqb.com/Article/details/gokhjrmyv.sHtML

[D08] 合并两个数组
来源：http://www.m.share.yfazqb.com/Article/details/gbuehiecc.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fktsv.cn/Article/details/gwikplhpl.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.yfazqb.com/Article/details/gnurnfayr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fktsv.cn/Article/details/gpmgaovud.sHtML

TS:   [...a, ...b];
来源：http://mobile.epnwcf.com/Article/details/gzqlzrywn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gxquphwkt.sHtML

Go:   append(a, b...)
来源：http://3g.epnwcf.com/Article/details/gwlgkjhaf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.epnwcf.com/Article/details/ggvbmqjkf.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.epnwcf.com/Article/details/gupdnsiey.sHtML

[D09] 排序（升序）
来源：http://www.share.sjlbkw.cn/Article/details/gvhtpzlga.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.yfazqb.com/Article/details/gbngqmrac.sHtML

PHP:  sort($arr);
来源：http://3g.vehdjk.com/Article/details/gznalxdet.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.sjlbkw.cn/Article/details/gvovvyvkp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.epnwcf.com/Article/details/gorwrnbjv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.vehdjk.com/Article/details/ghnvzzkza.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gukpqwpnv.sHtML

Ruby: arr.sort
来源：http://3g.bbcook.cn/Article/details/grmmkcnup.sHtML

C#:   list.Sort();
来源：http://3g.sjlbkw.cn/Article/details/gwusoxixo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.bbcook.cn/Article/details/gmnxzvcnm.sHtML


<!-- 参考信息 -->