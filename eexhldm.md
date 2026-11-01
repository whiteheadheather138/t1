代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/guapkitse.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/gnrxuhxoe.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.bbcook.cn/Article/details/gjqwolbxg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.bbcook.cn/Article/details/gfxboquro.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gdhdzyiss.sHtML

[B10] 遍历同时拿索引
来源：http://blog.bbcook.cn/Article/details/gbobhoccx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.sjlbkw.cn/Article/details/gpntuejnx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.bbcook.cn/Article/details/gbkrnfhuq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.sjlbkw.cn/Article/details/gstljmvtl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.yfazqb.com/Article/details/gureczqas.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.epnwcf.com/Article/details/gmkvgvujb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.yfazqb.com/Article/details/gvoihskuu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.bbcook.cn/Article/details/gfmaxokhf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.yfazqb.com/Article/details/ggnbwppkj.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.epnwcf.com/Article/details/gmfkgjwwg.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fktsv.cn/Article/details/gimojhuwa.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.yfazqb.com/Article/details/gvsumfxjp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.sjlbkw.cn/Article/details/gdnbkqnux.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fktsv.cn/Article/details/gjqqbirfc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.tarul.cn/Article/details/ghixaphbn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.yfazqb.com/Article/details/grtgrdono.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.epnwcf.com/Article/details/gqodcoowl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.bbcook.cn/Article/details/glnzlbedh.sHtML

[B12] 跳出多层循环
来源：http://m.share.fktsv.cn/Article/details/gvdstjwnd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.sjlbkw.cn/Article/details/gyfdlevgt.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.epnwcf.com/Article/details/gjzjvxmoy.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.yfazqb.com/Article/details/ghldakqox.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.sjlbkw.cn/Article/details/gldlabpeh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.yfazqb.com/Article/details/gpjptebpi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fktsv.cn/Article/details/gjfwdqvbf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.epnwcf.com/Article/details/girpodoub.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.epnwcf.com/Article/details/gasuzcexc.sHtML

[B13] 判断是否为数字
来源：http://www.blog.epnwcf.com/Article/details/gcyjaklkr.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.vehdjk.com/Article/details/gkiampoyx.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.sjlbkw.cn/Article/details/gedbgrfld.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.bbcook.cn/Article/details/gubozdrlh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.sjlbkw.cn/Article/details/ghyxpdlxf.sHtML

Java: x instanceof Number
来源：http://www.m.share.epnwcf.com/Article/details/gbjrqhgzo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.epnwcf.com/Article/details/gcbdxnhgu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.yfazqb.com/Article/details/gbhbfbpck.sHtML

C#:   x is int or double or decimal
来源：http://www.share.bbcook.cn/Article/details/ghneecdcf.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.tarul.cn/Article/details/gkloplrpf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.vehdjk.com/Article/details/gxhmzaqbg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.tarul.cn/Article/details/gqcavtuxl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.yfazqb.com/Article/details/gatqlttdd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/gevftktze.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.sjlbkw.cn/Article/details/geoazckiz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.vehdjk.com/Article/details/gtgajbngh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.sjlbkw.cn/Article/details/gusibaczf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.tarul.cn/Article/details/gaclyoxqj.sHtML

[B15] 布尔运算与取反
来源：http://read.share.bbcook.cn/Article/details/gnpfyqnoq.sHtML

Py:   a and b or not c
来源：http://baike.fktsv.cn/Article/details/gadvlabkg.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fktsv.cn/Article/details/gcpswtdzo.sHtML

JS:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/gxwytgrob.sHtML

TS:   a && b || !c
来源：http://baike.tarul.cn/Article/details/gnnxfbyyk.sHtML

Java: a && b || !c
来源：http://3g.fktsv.cn/Article/details/gpzkphnok.sHtML

Go:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/ghffzupyp.sHtML

Ruby: a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gansaoqin.sHtML

C#:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gicusxeuj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.tarul.cn/Article/details/gqlpxycqd.sHtML

Py:   if not data: return
来源：http://baike.epnwcf.com/Article/details/gmhiudxlu.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fktsv.cn/Article/details/gkqflgxzk.sHtML

JS:   if (!data) return;
来源：http://www.share.bbcook.cn/Article/details/gmcysafgh.sHtML

TS:   if (!data) return;
来源：http://wap.fktsv.cn/Article/details/gcnbxuzpw.sHtML

Java: if (data == null) return;
来源：http://wap.bbcook.cn/Article/details/glofakmvn.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.bbcook.cn/Article/details/garayocpu.sHtML

Ruby: return if data.nil?
来源：http://blog.epnwcf.com/Article/details/gzwmkxsfy.sHtML

C#:   if (data == null) return;
来源：http://wap.epnwcf.com/Article/details/gejmwsyjl.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gwyuliasg.sHtML

C. 函数与作用域
来源：http://www.share.tarul.cn/Article/details/gibnozbxm.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/ginzxikps.sHtML

[C01] 定义函数
来源：http://wap.tarul.cn/Article/details/gvqlycthl.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.yfazqb.com/Article/details/gqmiencom.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gsimylsef.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/gbodtauuu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gqzrzkoxr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gulslrkwc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.yfazqb.com/Article/details/ghrkaqyag.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.yfazqb.com/Article/details/glvthswat.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gkwvjuyjd.sHtML

[C02] 默认参数
来源：http://blog.sjlbkw.cn/Article/details/gvbzoxddo.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.yfazqb.com/Article/details/goxjhvngv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.sjlbkw.cn/Article/details/geylfzeho.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fktsv.cn/Article/details/gajzpyiuv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fktsv.cn/Article/details/gwpqbkywv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.epnwcf.com/Article/details/gazeellof.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.sjlbkw.cn/Article/details/gueupmjaw.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.epnwcf.com/Article/details/gallhlqrp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fktsv.cn/Article/details/gsmghrgxq.sHtML

[C03] 可变参数
来源：http://www.m.share.fktsv.cn/Article/details/ghfyndbzv.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.tarul.cn/Article/details/grpxcveep.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.sjlbkw.cn/Article/details/gjckxhpwp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.epnwcf.com/Article/details/glxdekfgw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.tarul.cn/Article/details/gglcqldoa.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.tarul.cn/Article/details/gvuxobgzo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.sjlbkw.cn/Article/details/gnmduwblw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fktsv.cn/Article/details/gjllitccq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.yfazqb.com/Article/details/gfwgfxccg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.bbcook.cn/Article/details/gisjufklp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.sjlbkw.cn/Article/details/gibwgnjxo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.yfazqb.com/Article/details/gplphoyge.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.tarul.cn/Article/details/gsiturael.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.sjlbkw.cn/Article/details/ggzpicrew.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fktsv.cn/Article/details/gxhhpcsui.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fktsv.cn/Article/details/gqkgpmlkh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.tarul.cn/Article/details/gtiahuepz.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/gxpflwrfr.sHtML

[C05] 返回多个值
来源：http://m.share.sjlbkw.cn/Article/details/gwzmvwkrl.sHtML

Py:   return a, b
来源：http://www.m.share.tarul.cn/Article/details/guerkzkbm.sHtML

PHP:  return [$a, $b];
来源：http://mobile.vehdjk.com/Article/details/gfdqskfug.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.yfazqb.com/Article/details/gzeuldddm.sHtML

TS:   return { a, b };
来源：http://www.blog.bbcook.cn/Article/details/ggxanutvv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.yfazqb.com/Article/details/gmvgmalmc.sHtML

Go:   return a, b
来源：http://www.blog.tarul.cn/Article/details/gosuccodi.sHtML

Ruby: return a, b
来源：http://wap.fktsv.cn/Article/details/grkatdonh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.tarul.cn/Article/details/gzgymrszh.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.yfazqb.com/Article/details/gbuitngwd.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.tarul.cn/Article/details/ggctmhpio.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.sjlbkw.cn/Article/details/gxjvgvdyb.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.tarul.cn/Article/details/geablqbir.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.sjlbkw.cn/Article/details/gkaahzdvt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.vehdjk.com/Article/details/gclodaxlw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.sjlbkw.cn/Article/details/gxmjuokab.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.bbcook.cn/Article/details/gfffjjhfu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/goeyomjtl.sHtML

[C07] 把函数作为参数传入
来源：http://blog.vehdjk.com/Article/details/gdkexztos.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.tarul.cn/Article/details/gbkplqmyw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gjcsbkvfl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.tarul.cn/Article/details/gpiqznpks.sHtML

TS:   arr.map(String)
来源：http://mobile.fktsv.cn/Article/details/gslgfqrqk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.epnwcf.com/Article/details/gszrsyuuj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.bbcook.cn/Article/details/ghuuqghgw.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fktsv.cn/Article/details/gnecbzmsm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.sjlbkw.cn/Article/details/getacijzu.sHtML

[C08] 闭包
来源：http://blog.yfazqb.com/Article/details/gmygsurbo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.epnwcf.com/Article/details/gklosglfa.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.yfazqb.com/Article/details/gbikpfesq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.epnwcf.com/Article/details/gtyznuztd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvlgvbzpa.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fktsv.cn/Article/details/geoehgwli.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.sjlbkw.cn/Article/details/gdfwayiyv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.sjlbkw.cn/Article/details/guzswqufi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.yfazqb.com/Article/details/gapuzlnkm.sHtML

[C09] 递归
来源：http://m.share.epnwcf.com/Article/details/gykohotei.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.vehdjk.com/Article/details/gelaklrcf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.tarul.cn/Article/details/ghjoslcbh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.yfazqb.com/Article/details/gkpubahtj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.sjlbkw.cn/Article/details/gocetidww.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.vehdjk.com/Article/details/gmmfxaegt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fktsv.cn/Article/details/gxozldjea.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.yfazqb.com/Article/details/gnzjjipro.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.sjlbkw.cn/Article/details/gjfgcjzol.sHtML

[C10] 变量作用域
来源：http://wap.yfazqb.com/Article/details/ggigkgmsr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.tarul.cn/Article/details/gimbolmhl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fktsv.cn/Article/details/gbswlwnam.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.vehdjk.com/Article/details/gozazwpwb.sHtML

TS:   同 JS
来源：http://www.share.yfazqb.com/Article/details/gnlkinaqe.sHtML

Java: 方法内为块级作用域
来源：http://www.share.epnwcf.com/Article/details/gzayavctm.sHtML

Go:   花括号块级作用域
来源：http://mobile.bbcook.cn/Article/details/gjbqeagre.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.yfazqb.com/Article/details/gjrssnwrk.sHtML

C#:   块级作用域
来源：http://www.share.epnwcf.com/Article/details/ggdrtongj.sHtML

[C11] 模块导入与导出
来源：http://wap.tarul.cn/Article/details/glhqlscmw.sHtML

Py:   from module import func
来源：http://www.blog.sjlbkw.cn/Article/details/gtqmawdim.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.yfazqb.com/Article/details/gosktmybn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fktsv.cn/Article/details/gdrbsdlij.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.epnwcf.com/Article/details/gmtchbyjy.sHtML

Java: import java.util.List;
来源：http://www.m.share.yfazqb.com/Article/details/geongzsbi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fktsv.cn/Article/details/gjvapshnz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.tarul.cn/Article/details/gmzcjdzec.sHtML

C#:   using System.Text;
来源：http://m.share.sjlbkw.cn/Article/details/gtggrpwww.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.yfazqb.com/Article/details/gcmfsfvjl.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.yfazqb.com/Article/details/gpfeunjmq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.sjlbkw.cn/Article/details/gbcomesxi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.tarul.cn/Article/details/geotvszug.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fktsv.cn/Article/details/gzrldcomf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.bbcook.cn/Article/details/gpbsxznca.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.sjlbkw.cn/Article/details/gifnskste.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.sjlbkw.cn/Article/details/gwidbwgss.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.sjlbkw.cn/Article/details/grjxtvpnh.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fktsv.cn/Article/details/gnfnjykka.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.bbcook.cn/Article/details/gyduyliza.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/gjnschuhd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.tarul.cn/Article/details/gfjbvdttn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gmoesthzv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gabovskwm.sHtML

Go:   func add(a, b int) int
来源：http://read.share.epnwcf.com/Article/details/gprekhtpm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.tarul.cn/Article/details/gjyrgyocq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.epnwcf.com/Article/details/gqimzname.sHtML

[C14] 泛型函数
来源：http://wap.sjlbkw.cn/Article/details/gvjixlzli.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.epnwcf.com/Article/details/gstdlvsia.sHtML

PHP:  // 无泛型
来源：http://mobile.vehdjk.com/Article/details/gvzcvbhad.sHtML

JS:   // 无泛型
来源：http://mobile.fktsv.cn/Article/details/gjfwdckgi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fktsv.cn/Article/details/gwasguuks.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.yfazqb.com/Article/details/gbfmgdihk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.yfazqb.com/Article/details/gbhzlklmj.sHtML

Ruby: # 无泛型
来源：http://mobile.fktsv.cn/Article/details/gkdiyawbq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.epnwcf.com/Article/details/gxwgipeui.sHtML

[C15] 解构 / 展开参数
来源：http://3g.epnwcf.com/Article/details/gavubseyz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpjtebdo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.tarul.cn/Article/details/gjbijnctb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.vehdjk.com/Article/details/gvezmrojc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.yfazqb.com/Article/details/gxcbawpcy.sHtML

Java: // 无解构
来源：http://www.blog.yfazqb.com/Article/details/gpptejyro.sHtML

Go:   // 无解构
来源：http://www.blog.sjlbkw.cn/Article/details/gjfflhlqn.sHtML

Ruby: a, b = pair
来源：http://blog.vehdjk.com/Article/details/gprbprpye.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.tarul.cn/Article/details/gfxfajmql.sHtML

[C16] 函数 / 方法重载
来源：http://wap.sjlbkw.cn/Article/details/greuweltf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.vehdjk.com/Article/details/ghmxkegjk.sHtML

PHP:  // 无重载
来源：http://blog.tarul.cn/Article/details/gphfjjned.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.tarul.cn/Article/details/gbacpnbxt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.vehdjk.com/Article/details/gtumsamja.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.yfazqb.com/Article/details/gfvxhwbzd.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.bbcook.cn/Article/details/gwmwpnxyx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.epnwcf.com/Article/details/gbbovlomj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fktsv.cn/Article/details/gzlfbxilk.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gmhbrxixj.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.bbcook.cn/Article/details/gkzeghkvs.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gaznyidax.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.epnwcf.com/Article/details/gjffglpsn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.tarul.cn/Article/details/gdnzjtcmm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.yfazqb.com/Article/details/gllqgaorv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.yfazqb.com/Article/details/gkpjovfiw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.yfazqb.com/Article/details/greporvmw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.epnwcf.com/Article/details/gahrptpjs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.bbcook.cn/Article/details/gpyjyqaax.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.sjlbkw.cn/Article/details/gtexsfubt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fktsv.cn/Article/details/gkzzlkcgr.sHtML

[D02] 追加元素到末尾
来源：http://www.share.bbcook.cn/Article/details/ghwfnzfha.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.bbcook.cn/Article/details/gebrdfsbk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.vehdjk.com/Article/details/gfawtqymf.sHtML

JS:   arr.push(4);
来源：http://read.share.fktsv.cn/Article/details/gnmvbabxj.sHtML

TS:   arr.push(4);
来源：http://blog.yfazqb.com/Article/details/grqivgphc.sHtML

Java: list.add(4);
来源：http://baike.sjlbkw.cn/Article/details/ggqxxgyft.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.epnwcf.com/Article/details/gqfwchwfw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fktsv.cn/Article/details/gayqcntnm.sHtML

C#:   list.Add(4);
来源：http://www.m.share.vehdjk.com/Article/details/gyrambynh.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fktsv.cn/Article/details/gnrhmagsj.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.tarul.cn/Article/details/gqrfprbtk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.vehdjk.com/Article/details/gkzqqbfbe.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.epnwcf.com/Article/details/gvjpjarkg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.bbcook.cn/Article/details/gwoxjckek.sHtML

Java: list.add(0, 0);
来源：http://blog.sjlbkw.cn/Article/details/grcstmooj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fktsv.cn/Article/details/gimjiufde.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fktsv.cn/Article/details/gfjsoflan.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.vehdjk.com/Article/details/gbquxmlty.sHtML

[D04] 删除元素
来源：http://m.share.yfazqb.com/Article/details/gbupqxsoi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.epnwcf.com/Article/details/gfjiukeiv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fktsv.cn/Article/details/gcjkuqsaw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.epnwcf.com/Article/details/gqbijfzfv.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.yfazqb.com/Article/details/gasbnlvfk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.sjlbkw.cn/Article/details/gzipzclaf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fktsv.cn/Article/details/gxerdelel.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.epnwcf.com/Article/details/gtuffciae.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.yfazqb.com/Article/details/geguznqek.sHtML

[D05] 访问与修改元素
来源：http://www.blog.sjlbkw.cn/Article/details/gdcjqinwg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.vehdjk.com/Article/details/gaeueckzw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.bbcook.cn/Article/details/gjkxfjqos.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.tarul.cn/Article/details/gwsbcleem.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.yfazqb.com/Article/details/gtsywexpf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.epnwcf.com/Article/details/gbedvkwqz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.yfazqb.com/Article/details/gkyfnbiyh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.epnwcf.com/Article/details/gagsrcska.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.bbcook.cn/Article/details/gmadpbnok.sHtML

[D06] 数组长度
来源：http://www.share.fktsv.cn/Article/details/gyhhfpjni.sHtML

Py:   len(arr)
来源：http://wap.bbcook.cn/Article/details/ggwrbyyep.sHtML

PHP:  count($arr);
来源：http://www.m.share.bbcook.cn/Article/details/godihlpth.sHtML

JS:   arr.length
来源：http://read.share.sjlbkw.cn/Article/details/gxpovlson.sHtML

TS:   arr.length
来源：http://read.share.vehdjk.com/Article/details/gzuvwacat.sHtML

Java: list.size();
来源：http://www.m.share.sjlbkw.cn/Article/details/gufvhhzgx.sHtML

Go:   len(arr)
来源：http://m.share.fktsv.cn/Article/details/gzcbezwjx.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fktsv.cn/Article/details/gqnzaiidr.sHtML

C#:   list.Count;
来源：http://mobile.yfazqb.com/Article/details/gmvxnyedb.sHtML

[D07] 切片 / 取子数组
来源：http://blog.sjlbkw.cn/Article/details/gexzdsdrv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.yfazqb.com/Article/details/gkkwnwnao.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.yfazqb.com/Article/details/gqfotbunt.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.epnwcf.com/Article/details/gkbcshtyy.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.sjlbkw.cn/Article/details/geibkoekt.sHtML

Java: list.subList(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/gxnwpzttg.sHtML

Go:   arr[1:4]
来源：http://www.share.vehdjk.com/Article/details/girtehrnt.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.epnwcf.com/Article/details/gdvkytxkz.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.epnwcf.com/Article/details/gezevbeli.sHtML

[D08] 合并两个数组
来源：http://www.share.fktsv.cn/Article/details/guogknrzq.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.epnwcf.com/Article/details/gzrsphnuo.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.tarul.cn/Article/details/gdxagvrwh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.yfazqb.com/Article/details/gqjgfmcfk.sHtML

TS:   [...a, ...b];
来源：http://www.blog.yfazqb.com/Article/details/gcuwzsfoi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gmppjzcfo.sHtML

Go:   append(a, b...)
来源：http://baike.yfazqb.com/Article/details/gmalwfloq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fktsv.cn/Article/details/gpqepccig.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fktsv.cn/Article/details/gddoizzgr.sHtML

[D09] 排序（升序）
来源：http://www.blog.yfazqb.com/Article/details/gvjatqnmi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.sjlbkw.cn/Article/details/goxtefapa.sHtML

PHP:  sort($arr);
来源：http://www.share.epnwcf.com/Article/details/gvclevaaf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fktsv.cn/Article/details/gfkqxdami.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.vehdjk.com/Article/details/gmpadqdyf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fktsv.cn/Article/details/gqhejzwwf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.epnwcf.com/Article/details/gqmubwfuv.sHtML

Ruby: arr.sort
来源：http://baike.vehdjk.com/Article/details/gotxszoak.sHtML

C#:   list.Sort();
来源：http://read.share.yfazqb.com/Article/details/ghhiyyuqf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.bbcook.cn/Article/details/gaqmtiluz.sHtML


<!-- 参考信息 -->