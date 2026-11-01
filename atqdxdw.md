代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.sjlbkw.cn/Article/details/gqdtnwogc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.yfazqb.com/Article/details/gagvakztc.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/gwdezjzns.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.tarul.cn/Article/details/guskdwbqt.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.bbcook.cn/Article/details/gybopvjos.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.yfazqb.com/Article/details/gwqgvggaf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.epnwcf.com/Article/details/gjzheyfdu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.fktsv.cn/Article/details/gxgzaoidg.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/gxzhgvzlm.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.sjlbkw.cn/Article/details/gacamfset.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.tarul.cn/Article/details/gqfsubrlp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.bbcook.cn/Article/details/gkujgmulp.sHtML

[B09] break 与 continue
来源：http://wap.fktsv.cn/Article/details/garuyeuco.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.bbcook.cn/Article/details/gqetvitlt.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/gndgzomxs.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.yfazqb.com/Article/details/gfueskcpt.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/gpdexmevw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.epnwcf.com/Article/details/gtzzgsnrj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.vehdjk.com/Article/details/gzieepkmj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.sjlbkw.cn/Article/details/ghhrewour.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.yfazqb.com/Article/details/glmbbpldn.sHtML

[B10] 遍历同时拿索引
来源：http://blog.vehdjk.com/Article/details/gkpywlvlt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.epnwcf.com/Article/details/gkuamhenh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.epnwcf.com/Article/details/guqpidyam.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fktsv.cn/Article/details/gwjvomuxj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.bbcook.cn/Article/details/gtsovrtho.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.yfazqb.com/Article/details/gdekdfnag.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.bbcook.cn/Article/details/gssktkdhd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.tarul.cn/Article/details/gvggadmhe.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.epnwcf.com/Article/details/gwpzdyxts.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fktsv.cn/Article/details/gqxrmtooy.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.bbcook.cn/Article/details/glyccmnpq.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.vehdjk.com/Article/details/gdoyhoxtl.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.vehdjk.com/Article/details/gidkwnena.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.sjlbkw.cn/Article/details/gnogybetu.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fktsv.cn/Article/details/gtiwjbauy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.bbcook.cn/Article/details/gpdwszmer.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.vehdjk.com/Article/details/gcrtpeihe.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fktsv.cn/Article/details/gvdqyuyoi.sHtML

[B12] 跳出多层循环
来源：http://3g.yfazqb.com/Article/details/gdlulvkxl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.bbcook.cn/Article/details/ghotrsdcx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.yfazqb.com/Article/details/gquxsztur.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsioqdfpg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.tarul.cn/Article/details/gfjfkqyth.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.yfazqb.com/Article/details/gvilcwuhx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.vehdjk.com/Article/details/gubviwepp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.sjlbkw.cn/Article/details/gtylcoxwz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.bbcook.cn/Article/details/goamcmvcn.sHtML

[B13] 判断是否为数字
来源：http://read.share.sjlbkw.cn/Article/details/gmwrnvwpm.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.epnwcf.com/Article/details/gynbiajmn.sHtML

PHP:  is_numeric($x)
来源：http://mobile.epnwcf.com/Article/details/guyjkwrsq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fktsv.cn/Article/details/gnhdpmoxz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.bbcook.cn/Article/details/gahyyksjj.sHtML

Java: x instanceof Number
来源：http://www.m.share.vehdjk.com/Article/details/gxaebgrnn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.tarul.cn/Article/details/gyvmiszta.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.epnwcf.com/Article/details/gaehtojro.sHtML

C#:   x is int or double or decimal
来源：http://blog.epnwcf.com/Article/details/ghvwggith.sHtML

[B14] 判断值是否在集合内
来源：http://3g.bbcook.cn/Article/details/gqdixeoyf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.vehdjk.com/Article/details/gxjhxaouc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.yfazqb.com/Article/details/gxtmrhgvz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.yfazqb.com/Article/details/gkbydkyxr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.bbcook.cn/Article/details/gntujzlba.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/gqaezqezh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.vehdjk.com/Article/details/gbsqelfwc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.vehdjk.com/Article/details/gvorijxem.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.sjlbkw.cn/Article/details/gcewkchgp.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.yfazqb.com/Article/details/gdcjirjzq.sHtML

Py:   a and b or not c
来源：http://wap.epnwcf.com/Article/details/gsecqfnnb.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.vehdjk.com/Article/details/gtmljigtl.sHtML

JS:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gpfxofamn.sHtML

TS:   a && b || !c
来源：http://baike.fktsv.cn/Article/details/gqnjoqjui.sHtML

Java: a && b || !c
来源：http://blog.epnwcf.com/Article/details/gsdjziqip.sHtML

Go:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gfnixougv.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/guecphsls.sHtML

C#:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gscffqhdf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.tarul.cn/Article/details/govcrnsjv.sHtML

Py:   if not data: return
来源：http://3g.bbcook.cn/Article/details/gbkxjtswt.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.sjlbkw.cn/Article/details/gvplmavby.sHtML

JS:   if (!data) return;
来源：http://mobile.epnwcf.com/Article/details/gpajcibbn.sHtML

TS:   if (!data) return;
来源：http://wap.yfazqb.com/Article/details/glueuizao.sHtML

Java: if (data == null) return;
来源：http://3g.fktsv.cn/Article/details/gmpqccduh.sHtML

Go:   if data == nil { return }
来源：http://m.share.vehdjk.com/Article/details/gatthqnau.sHtML

Ruby: return if data.nil?
来源：http://mobile.vehdjk.com/Article/details/gdzmoaiyi.sHtML

C#:   if (data == null) return;
来源：http://m.share.epnwcf.com/Article/details/gavyxbphc.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gfetafofy.sHtML

C. 函数与作用域
来源：http://www.blog.epnwcf.com/Article/details/gjewyvoyy.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gfnjvwupc.sHtML

[C01] 定义函数
来源：http://wap.tarul.cn/Article/details/gefzyoykk.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.yfazqb.com/Article/details/gcwyrayxl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/grqurxynw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/giihdzuyl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gvfykbwyf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gungicxru.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.epnwcf.com/Article/details/guronalru.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.epnwcf.com/Article/details/gtpzzvdos.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/ghouvypkx.sHtML

[C02] 默认参数
来源：http://blog.bbcook.cn/Article/details/girunogbg.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.bbcook.cn/Article/details/gkuacknay.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.tarul.cn/Article/details/gownaycnp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/grnbiojtv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fktsv.cn/Article/details/gcmketgjs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.bbcook.cn/Article/details/gawlevreg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.vehdjk.com/Article/details/gjtrzokue.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.sjlbkw.cn/Article/details/gcgnktapx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.bbcook.cn/Article/details/ghlpdzier.sHtML

[C03] 可变参数
来源：http://mobile.epnwcf.com/Article/details/gcoemcqcd.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.bbcook.cn/Article/details/guxbsqhba.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.bbcook.cn/Article/details/guetflbrx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.tarul.cn/Article/details/gatynmmvs.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.yfazqb.com/Article/details/grzkwxrlv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fktsv.cn/Article/details/ghldgsnos.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.yfazqb.com/Article/details/gzyfzweft.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.yfazqb.com/Article/details/grjqclxsr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.bbcook.cn/Article/details/gkcgpxgbw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.sjlbkw.cn/Article/details/gvajlceor.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.yfazqb.com/Article/details/gemvapuxp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.bbcook.cn/Article/details/ggpqmhgxo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.sjlbkw.cn/Article/details/ghalxocuz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.epnwcf.com/Article/details/ghwayksmk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.epnwcf.com/Article/details/gzhlewiha.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.yfazqb.com/Article/details/ggtjtasds.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.vehdjk.com/Article/details/gorblidom.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fktsv.cn/Article/details/gqaidqrus.sHtML

[C05] 返回多个值
来源：http://www.blog.vehdjk.com/Article/details/ghtdgcywd.sHtML

Py:   return a, b
来源：http://3g.fktsv.cn/Article/details/gmxzcfxxh.sHtML

PHP:  return [$a, $b];
来源：http://m.share.vehdjk.com/Article/details/gnbepkrtx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.sjlbkw.cn/Article/details/gagsqecki.sHtML

TS:   return { a, b };
来源：http://www.share.fktsv.cn/Article/details/gvyciyiip.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.tarul.cn/Article/details/gblxvixnx.sHtML

Go:   return a, b
来源：http://www.blog.bbcook.cn/Article/details/gqmhwdhoa.sHtML

Ruby: return a, b
来源：http://m.share.bbcook.cn/Article/details/guqppodlt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.bbcook.cn/Article/details/gwliykjwh.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.bbcook.cn/Article/details/gwdrnwwyl.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.sjlbkw.cn/Article/details/ghkprqniv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fktsv.cn/Article/details/gsfacfbva.sHtML

JS:   const square = x => x * x;
来源：http://mobile.vehdjk.com/Article/details/gkunsvrfs.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.epnwcf.com/Article/details/gmzwshvru.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.bbcook.cn/Article/details/gdwrsvfcu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.yfazqb.com/Article/details/gogfhzsfm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.sjlbkw.cn/Article/details/gxdttudjv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.bbcook.cn/Article/details/gjesgfdvd.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.epnwcf.com/Article/details/glrcftgla.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.sjlbkw.cn/Article/details/gnyzyyxqw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.tarul.cn/Article/details/ghtskjtjq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.sjlbkw.cn/Article/details/gojvnhaos.sHtML

TS:   arr.map(String)
来源：http://baike.yfazqb.com/Article/details/gowgcayei.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.vehdjk.com/Article/details/gdnrrnfde.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.epnwcf.com/Article/details/gddjragbv.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.yfazqb.com/Article/details/gqyqjqstv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.tarul.cn/Article/details/gqpgrvqqr.sHtML

[C08] 闭包
来源：http://blog.tarul.cn/Article/details/goulhmesl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.epnwcf.com/Article/details/grrfxxryf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fktsv.cn/Article/details/gfgzebjxt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.bbcook.cn/Article/details/gomtdmpim.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.bbcook.cn/Article/details/gwlmyvcrn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fktsv.cn/Article/details/ginybcahe.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.vehdjk.com/Article/details/gnpqfxphi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.bbcook.cn/Article/details/gxxiaaoph.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.epnwcf.com/Article/details/gcctmsaii.sHtML

[C09] 递归
来源：http://www.blog.fktsv.cn/Article/details/geeazfzei.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.yfazqb.com/Article/details/gmlfigsgd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fktsv.cn/Article/details/geqqqgszk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.yfazqb.com/Article/details/gtzhgbxhj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.vehdjk.com/Article/details/gdummqldg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.yfazqb.com/Article/details/gajfigcpf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.tarul.cn/Article/details/gcmqyqchm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.vehdjk.com/Article/details/gedaxfrut.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.tarul.cn/Article/details/gcmztgdvo.sHtML

[C10] 变量作用域
来源：http://www.share.tarul.cn/Article/details/gjhbqopzh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.epnwcf.com/Article/details/gcrldytcx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.vehdjk.com/Article/details/gemqwsefu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.bbcook.cn/Article/details/gckxavkxu.sHtML

TS:   同 JS
来源：http://www.share.yfazqb.com/Article/details/gshzafqyu.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fktsv.cn/Article/details/gbzxgoivc.sHtML

Go:   花括号块级作用域
来源：http://3g.vehdjk.com/Article/details/gmtqsvkob.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.bbcook.cn/Article/details/gjbxawtdi.sHtML

C#:   块级作用域
来源：http://www.m.share.fktsv.cn/Article/details/glqswwqjj.sHtML

[C11] 模块导入与导出
来源：http://baike.fktsv.cn/Article/details/gphasjlmg.sHtML

Py:   from module import func
来源：http://3g.sjlbkw.cn/Article/details/gdbsgejxo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.epnwcf.com/Article/details/ghdqwracm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.sjlbkw.cn/Article/details/ghtwipehf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.tarul.cn/Article/details/gjxajryda.sHtML

Java: import java.util.List;
来源：http://3g.fktsv.cn/Article/details/gmnzyyuwy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.sjlbkw.cn/Article/details/gdvpkgbah.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.bbcook.cn/Article/details/gfxpokhgs.sHtML

C#:   using System.Text;
来源：http://www.share.vehdjk.com/Article/details/gqewjmrxd.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fktsv.cn/Article/details/gcuokjsuy.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.sjlbkw.cn/Article/details/gpigibycp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fktsv.cn/Article/details/gfosflfpv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.yfazqb.com/Article/details/gyuvsowzt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.sjlbkw.cn/Article/details/gpxjlqalw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.bbcook.cn/Article/details/gohwswios.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.yfazqb.com/Article/details/ggsyofojk.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.sjlbkw.cn/Article/details/gootaahup.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.tarul.cn/Article/details/gumtftvei.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.vehdjk.com/Article/details/gtwfwdikc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.tarul.cn/Article/details/gacxtslza.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/gfnhiyeiw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.vehdjk.com/Article/details/gylocesks.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gwmuyjrda.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gxlaamnbt.sHtML

Go:   func add(a, b int) int
来源：http://3g.yfazqb.com/Article/details/grhhxteah.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.vehdjk.com/Article/details/gyvgmtrkb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.tarul.cn/Article/details/gpdvibxpe.sHtML

[C14] 泛型函数
来源：http://blog.sjlbkw.cn/Article/details/gelroircv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.tarul.cn/Article/details/genqedovi.sHtML

PHP:  // 无泛型
来源：http://www.share.yfazqb.com/Article/details/gcexbwery.sHtML

JS:   // 无泛型
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmoanrls.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.sjlbkw.cn/Article/details/gvybbzhuv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.vehdjk.com/Article/details/gvjdvbofd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.tarul.cn/Article/details/gdsmdrziw.sHtML

Ruby: # 无泛型
来源：http://m.share.fktsv.cn/Article/details/gchrfeiyq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.sjlbkw.cn/Article/details/gozbsqqcs.sHtML

[C15] 解构 / 展开参数
来源：http://blog.sjlbkw.cn/Article/details/gugytxthi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.vehdjk.com/Article/details/ghxdchypo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.vehdjk.com/Article/details/gxzbqwjve.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.sjlbkw.cn/Article/details/gxotceooc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.sjlbkw.cn/Article/details/gagmnepvp.sHtML

Java: // 无解构
来源：http://www.share.fktsv.cn/Article/details/gqdrhsqsf.sHtML

Go:   // 无解构
来源：http://www.share.sjlbkw.cn/Article/details/gxeirpxxx.sHtML

Ruby: a, b = pair
来源：http://www.m.share.yfazqb.com/Article/details/gfkjmwzwj.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.yfazqb.com/Article/details/ggmjctnev.sHtML

[C16] 函数 / 方法重载
来源：http://blog.epnwcf.com/Article/details/gpydniydc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.epnwcf.com/Article/details/gzivopmnb.sHtML

PHP:  // 无重载
来源：http://blog.sjlbkw.cn/Article/details/gtvqpacau.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fktsv.cn/Article/details/ghikvvmnq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.tarul.cn/Article/details/gjhomleha.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.sjlbkw.cn/Article/details/gvhpcduhd.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.vehdjk.com/Article/details/gmcdlxuri.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.epnwcf.com/Article/details/gansfoxbo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.yfazqb.com/Article/details/gxgqvuowh.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gzcylegqn.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.yfazqb.com/Article/details/glgldsdrk.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gccgawwzl.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fktsv.cn/Article/details/gdkpgrpyp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.epnwcf.com/Article/details/ghohnafab.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.vehdjk.com/Article/details/gljataznf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.yfazqb.com/Article/details/gqpzenimu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fktsv.cn/Article/details/gcktfnyge.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.epnwcf.com/Article/details/goadlmhvg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.vehdjk.com/Article/details/gcsfxktff.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.epnwcf.com/Article/details/giaqvwuvq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.sjlbkw.cn/Article/details/gagjcbxqs.sHtML

[D02] 追加元素到末尾
来源：http://wap.yfazqb.com/Article/details/gxfyolepz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.vehdjk.com/Article/details/goocnzenz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.tarul.cn/Article/details/gtmfzlzhj.sHtML

JS:   arr.push(4);
来源：http://www.share.tarul.cn/Article/details/ggikansti.sHtML

TS:   arr.push(4);
来源：http://read.share.sjlbkw.cn/Article/details/gsngycbta.sHtML

Java: list.add(4);
来源：http://www.blog.tarul.cn/Article/details/gtqgjxrrx.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.bbcook.cn/Article/details/gnvoppess.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.yfazqb.com/Article/details/gogjbghpn.sHtML

C#:   list.Add(4);
来源：http://baike.bbcook.cn/Article/details/gkicliwaj.sHtML

[D03] 在指定位置插入元素
来源：http://wap.bbcook.cn/Article/details/geooetwjv.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.yfazqb.com/Article/details/gomrjjrbw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.tarul.cn/Article/details/gpikdzqge.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.epnwcf.com/Article/details/grkhglauc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.tarul.cn/Article/details/gfdmewrgd.sHtML

Java: list.add(0, 0);
来源：http://wap.sjlbkw.cn/Article/details/gzscgzlfc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.sjlbkw.cn/Article/details/gpbgqpakz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fktsv.cn/Article/details/gisqznvzz.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gelmicxds.sHtML

[D04] 删除元素
来源：http://m.share.yfazqb.com/Article/details/glxvkhiou.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.tarul.cn/Article/details/guhuiszlj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.tarul.cn/Article/details/grdvazuuh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.sjlbkw.cn/Article/details/gqkugmeww.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.vehdjk.com/Article/details/gmrwhiywt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbfmzoxd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.yfazqb.com/Article/details/guwnjmucu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.epnwcf.com/Article/details/gxpoxljmt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.bbcook.cn/Article/details/gzhhtxxlx.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.vehdjk.com/Article/details/gvszwkgon.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.vehdjk.com/Article/details/gjcplogvq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.tarul.cn/Article/details/gsfxknwgl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.epnwcf.com/Article/details/gfbrtcahp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.tarul.cn/Article/details/gplptkntc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.epnwcf.com/Article/details/gdqpbtxyb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.bbcook.cn/Article/details/gduoyoutb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/glkpyqncy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.bbcook.cn/Article/details/gxagxcfxl.sHtML

[D06] 数组长度
来源：http://mobile.bbcook.cn/Article/details/gzhcsmrsd.sHtML

Py:   len(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gzmmezpwo.sHtML

PHP:  count($arr);
来源：http://www.m.share.tarul.cn/Article/details/gvwprjnsq.sHtML

JS:   arr.length
来源：http://www.blog.vehdjk.com/Article/details/gpljaweic.sHtML

TS:   arr.length
来源：http://www.m.share.vehdjk.com/Article/details/gqpgvyagb.sHtML

Java: list.size();
来源：http://baike.fktsv.cn/Article/details/gwepedbpb.sHtML

Go:   len(arr)
来源：http://read.share.fktsv.cn/Article/details/gxljnkjos.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fktsv.cn/Article/details/gdcfpivec.sHtML

C#:   list.Count;
来源：http://3g.fktsv.cn/Article/details/grzqdipdq.sHtML

[D07] 切片 / 取子数组
来源：http://3g.epnwcf.com/Article/details/gkotndqtj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fktsv.cn/Article/details/gbkrmlxcr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fktsv.cn/Article/details/gaabcdnjq.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.sjlbkw.cn/Article/details/gtnfbcxes.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.epnwcf.com/Article/details/gxmjdlkev.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fktsv.cn/Article/details/gzwdkxshc.sHtML

Go:   arr[1:4]
来源：http://read.share.tarul.cn/Article/details/gunobjdjd.sHtML

Ruby: arr[1, 3]
来源：http://wap.vehdjk.com/Article/details/gztrvodec.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.bbcook.cn/Article/details/gdvspzokg.sHtML

[D08] 合并两个数组
来源：http://blog.bbcook.cn/Article/details/gezlvrhbu.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fktsv.cn/Article/details/gsqnycucr.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.bbcook.cn/Article/details/gzonrrhkl.sHtML


<!-- 参考信息 -->