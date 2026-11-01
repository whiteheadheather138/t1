代发 wailian999

[B09] break 与 continue
来源：http://3g.fktsv.cn/Article/details/ghpdvaayy.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gwzpkcjql.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gczxghszr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.yfazqb.com/Article/details/gxfcfzlef.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.vehdjk.com/Article/details/gccxpljde.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gsbuhisdp.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.tarul.cn/Article/details/guwkxiirg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.yfazqb.com/Article/details/gylxwuckm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/gzcpdmdto.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fktsv.cn/Article/details/gczvuqifo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.bbcook.cn/Article/details/gzwskphcy.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.vehdjk.com/Article/details/gsjwuxyno.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.vehdjk.com/Article/details/gocsglnlq.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fktsv.cn/Article/details/gqmqdbevn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.yfazqb.com/Article/details/gwdpqzgeg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.sjlbkw.cn/Article/details/glqbwpiiy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fktsv.cn/Article/details/gupkevqko.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.tarul.cn/Article/details/gjxziamsv.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.yfazqb.com/Article/details/gcqkyjntc.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.epnwcf.com/Article/details/grqcciycv.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.tarul.cn/Article/details/gbgfcqqoa.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.vehdjk.com/Article/details/gryadhuqt.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fktsv.cn/Article/details/gclfkkryq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.yfazqb.com/Article/details/gmptscoho.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.yfazqb.com/Article/details/grtuddwka.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.tarul.cn/Article/details/gmdbykiao.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.sjlbkw.cn/Article/details/ggeapbwgx.sHtML

[B12] 跳出多层循环
来源：http://mobile.sjlbkw.cn/Article/details/gkuzzzqso.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fktsv.cn/Article/details/gutylndeq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.epnwcf.com/Article/details/gtkpoenjm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/gzaurrrbj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.vehdjk.com/Article/details/gaynhwdjo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.bbcook.cn/Article/details/gvjewdlhx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.yfazqb.com/Article/details/gzojvjuhw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fktsv.cn/Article/details/gkohqfkmo.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.vehdjk.com/Article/details/gpruvfphh.sHtML

[B13] 判断是否为数字
来源：http://read.share.fktsv.cn/Article/details/gfvlrmnjd.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fktsv.cn/Article/details/gvfqodbrf.sHtML

PHP:  is_numeric($x)
来源：http://baike.bbcook.cn/Article/details/gbwihhrsx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.tarul.cn/Article/details/gayewgoqz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.sjlbkw.cn/Article/details/gqpvbchxn.sHtML

Java: x instanceof Number
来源：http://www.blog.vehdjk.com/Article/details/ggujpyewc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.fktsv.cn/Article/details/gssgywgcu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.epnwcf.com/Article/details/gugkzknpf.sHtML

C#:   x is int or double or decimal
来源：http://www.share.vehdjk.com/Article/details/gnwtdbjfo.sHtML

[B14] 判断值是否在集合内
来源：http://baike.sjlbkw.cn/Article/details/gmgdcqwiu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fktsv.cn/Article/details/gzwofaorx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fktsv.cn/Article/details/glqqqdwfa.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.epnwcf.com/Article/details/gtkbfzvsr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.tarul.cn/Article/details/gutydhmde.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdtmquha.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fktsv.cn/Article/details/glbvwpydv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.bbcook.cn/Article/details/gaijddgrf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.sjlbkw.cn/Article/details/getqkxoss.sHtML

[B15] 布尔运算与取反
来源：http://mobile.tarul.cn/Article/details/gymalhvsa.sHtML

Py:   a and b or not c
来源：http://baike.vehdjk.com/Article/details/gsrqabtfo.sHtML

PHP:  $a && $b || !$c
来源：http://3g.sjlbkw.cn/Article/details/gulpkmzbi.sHtML

JS:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gbcagdgtz.sHtML

TS:   a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gayyttipq.sHtML

Java: a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gbzmurbiz.sHtML

Go:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/grylowtrf.sHtML

Ruby: a && b || !c
来源：http://baike.yfazqb.com/Article/details/gkjfqcpyh.sHtML

C#:   a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gzalxgfls.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.tarul.cn/Article/details/gdbotnelm.sHtML

Py:   if not data: return
来源：http://m.share.tarul.cn/Article/details/grxnioskx.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.yfazqb.com/Article/details/gasnvhfjk.sHtML

JS:   if (!data) return;
来源：http://read.share.yfazqb.com/Article/details/gmjufqdgq.sHtML

TS:   if (!data) return;
来源：http://wap.fktsv.cn/Article/details/gmypdhuve.sHtML

Java: if (data == null) return;
来源：http://m.share.sjlbkw.cn/Article/details/glxcsdwks.sHtML

Go:   if data == nil { return }
来源：http://m.share.fktsv.cn/Article/details/ghzbzdzbe.sHtML

Ruby: return if data.nil?
来源：http://baike.fktsv.cn/Article/details/gnuweyxan.sHtML

C#:   if (data == null) return;
来源：http://www.share.bbcook.cn/Article/details/giuuqtwxq.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gcxxzzgyh.sHtML

C. 函数与作用域
来源：http://www.share.vehdjk.com/Article/details/gdtiejfzb.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/grfyihcfa.sHtML

[C01] 定义函数
来源：http://www.share.vehdjk.com/Article/details/gnigyeszu.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.tarul.cn/Article/details/gnkxpfuly.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/gvprvytll.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gbgdkqxxm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gowkelska.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/ggwbtovod.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.epnwcf.com/Article/details/gmfqwvbol.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.bbcook.cn/Article/details/gouspkdot.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gqsxvczpl.sHtML

[C02] 默认参数
来源：http://www.blog.bbcook.cn/Article/details/glrqaydae.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.sjlbkw.cn/Article/details/gkeqgsudu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.epnwcf.com/Article/details/gegmqvldz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.tarul.cn/Article/details/ghjpdhekk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fktsv.cn/Article/details/gipzbnusq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.sjlbkw.cn/Article/details/gpfqhfrmo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.bbcook.cn/Article/details/gjzlwlubq.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.tarul.cn/Article/details/gnvhdchin.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.tarul.cn/Article/details/gbtstllgi.sHtML

[C03] 可变参数
来源：http://wap.fktsv.cn/Article/details/gefnzkzcw.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.vehdjk.com/Article/details/gqpscuznq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.epnwcf.com/Article/details/gvgktvggf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.bbcook.cn/Article/details/guisqwzkr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.vehdjk.com/Article/details/gexnnoauj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fktsv.cn/Article/details/glcxqknqa.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.yfazqb.com/Article/details/gutltfqik.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.vehdjk.com/Article/details/gjxqpadri.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.yfazqb.com/Article/details/gbcrlkcof.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.tarul.cn/Article/details/ggwxocjpp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fktsv.cn/Article/details/gdvrsvhlm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.tarul.cn/Article/details/ggfyqzyvb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.tarul.cn/Article/details/gltbftghb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.vehdjk.com/Article/details/ghyiamtxk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fktsv.cn/Article/details/gbcuxhxly.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fktsv.cn/Article/details/gffvhteti.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.sjlbkw.cn/Article/details/gjxfxsqlu.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fktsv.cn/Article/details/gdhuznfeb.sHtML

[C05] 返回多个值
来源：http://3g.yfazqb.com/Article/details/giowjhdcv.sHtML

Py:   return a, b
来源：http://3g.epnwcf.com/Article/details/gokhhamvh.sHtML

PHP:  return [$a, $b];
来源：http://wap.tarul.cn/Article/details/gfozjszec.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.tarul.cn/Article/details/gxugadwxh.sHtML

TS:   return { a, b };
来源：http://read.share.vehdjk.com/Article/details/gxaqfufss.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.tarul.cn/Article/details/gfjvtgctl.sHtML

Go:   return a, b
来源：http://mobile.yfazqb.com/Article/details/gkqeyajnp.sHtML

Ruby: return a, b
来源：http://blog.epnwcf.com/Article/details/gpvowwiuz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.bbcook.cn/Article/details/gelrifqwf.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fktsv.cn/Article/details/gaftzucln.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.bbcook.cn/Article/details/gcnkbtvqp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.sjlbkw.cn/Article/details/graxktapb.sHtML

JS:   const square = x => x * x;
来源：http://www.share.tarul.cn/Article/details/guhwcrugm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.epnwcf.com/Article/details/ggqiszksg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.vehdjk.com/Article/details/gratzjsmc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.vehdjk.com/Article/details/gzcxumonb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.vehdjk.com/Article/details/gjnlfielg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.vehdjk.com/Article/details/goltktcpt.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.vehdjk.com/Article/details/gnyulqxyi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.sjlbkw.cn/Article/details/gxbzihbiu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/govdwloiy.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.bbcook.cn/Article/details/gwvemuafd.sHtML

TS:   arr.map(String)
来源：http://www.share.epnwcf.com/Article/details/gvvscbelb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fktsv.cn/Article/details/gamklsidj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.epnwcf.com/Article/details/gsaarkgpx.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.bbcook.cn/Article/details/gujpdumqu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.tarul.cn/Article/details/gsmxbdzpj.sHtML

[C08] 闭包
来源：http://www.blog.yfazqb.com/Article/details/gkiyvgkqi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fktsv.cn/Article/details/gjcxzdfug.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.vehdjk.com/Article/details/gbpoxehna.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.sjlbkw.cn/Article/details/gimivuiyy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.bbcook.cn/Article/details/gfbjtfguc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.sjlbkw.cn/Article/details/gahzpzryp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.vehdjk.com/Article/details/gthvgomao.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.bbcook.cn/Article/details/gorloyjwz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.epnwcf.com/Article/details/gjcloknsx.sHtML

[C09] 递归
来源：http://mobile.vehdjk.com/Article/details/gtjwkrurq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fktsv.cn/Article/details/gqplrtkhx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.vehdjk.com/Article/details/gflahhxdf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.sjlbkw.cn/Article/details/gxqcfpcdt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fktsv.cn/Article/details/gsldobeny.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fktsv.cn/Article/details/gkgyqiztp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.yfazqb.com/Article/details/gyccjufii.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gdwpazsas.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.vehdjk.com/Article/details/gztqscwag.sHtML

[C10] 变量作用域
来源：http://3g.tarul.cn/Article/details/grjnqizwg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.tarul.cn/Article/details/gyykxrwmp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.tarul.cn/Article/details/gwsvjakhk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.vehdjk.com/Article/details/gyvapaipb.sHtML

TS:   同 JS
来源：http://mobile.vehdjk.com/Article/details/ghmswddsc.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fktsv.cn/Article/details/gfyfsuepm.sHtML

Go:   花括号块级作用域
来源：http://3g.yfazqb.com/Article/details/gbzdxwxvt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fktsv.cn/Article/details/gtsgqylgp.sHtML

C#:   块级作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gxonpvakh.sHtML

[C11] 模块导入与导出
来源：http://baike.fktsv.cn/Article/details/guptbpvuo.sHtML

Py:   from module import func
来源：http://m.share.yfazqb.com/Article/details/gxneddeib.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.tarul.cn/Article/details/gozlroweq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.vehdjk.com/Article/details/glrkjmwra.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.epnwcf.com/Article/details/gihoeyuid.sHtML

Java: import java.util.List;
来源：http://m.share.bbcook.cn/Article/details/gwfzfblri.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.epnwcf.com/Article/details/gwwhocaor.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.yfazqb.com/Article/details/gxzgmxvbg.sHtML

C#:   using System.Text;
来源：http://blog.bbcook.cn/Article/details/gvgfmkwbe.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fktsv.cn/Article/details/ghsxobwjd.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.tarul.cn/Article/details/gtydbupmw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fktsv.cn/Article/details/gijpzltew.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.tarul.cn/Article/details/gmpcvytol.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fktsv.cn/Article/details/gesauwrwr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.vehdjk.com/Article/details/goxeyhfeg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fktsv.cn/Article/details/gfibvhejg.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.yfazqb.com/Article/details/gplmkaxmo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.yfazqb.com/Article/details/gtybmqlff.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.bbcook.cn/Article/details/grofgaehx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.vehdjk.com/Article/details/grynoyuxk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gnyygohgn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.tarul.cn/Article/details/gtbiumrlv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gwcqvvces.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gbodndgyl.sHtML

Go:   func add(a, b int) int
来源：http://blog.sjlbkw.cn/Article/details/golvpzqsi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.bbcook.cn/Article/details/gqmdpirto.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.tarul.cn/Article/details/gakxtnjxw.sHtML

[C14] 泛型函数
来源：http://wap.fktsv.cn/Article/details/gsoowkrkp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.bbcook.cn/Article/details/gfpydeabq.sHtML

PHP:  // 无泛型
来源：http://www.m.share.tarul.cn/Article/details/gnggdeovp.sHtML

JS:   // 无泛型
来源：http://blog.fktsv.cn/Article/details/giqfvittv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.tarul.cn/Article/details/gmmjmvani.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.vehdjk.com/Article/details/gbtnrjwyl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fktsv.cn/Article/details/grfemcfay.sHtML

Ruby: # 无泛型
来源：http://wap.vehdjk.com/Article/details/gebbxkryp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.yfazqb.com/Article/details/gvhxucrur.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.tarul.cn/Article/details/gtwjucteb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.epnwcf.com/Article/details/gmkxsdndl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.bbcook.cn/Article/details/gvgmgehka.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.tarul.cn/Article/details/gaefgagak.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gdwuonkfm.sHtML

Java: // 无解构
来源：http://read.share.yfazqb.com/Article/details/gouelkvvh.sHtML

Go:   // 无解构
来源：http://www.share.yfazqb.com/Article/details/gzhzcassk.sHtML

Ruby: a, b = pair
来源：http://www.blog.tarul.cn/Article/details/gareoulpt.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.bbcook.cn/Article/details/glkltcvmd.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.yfazqb.com/Article/details/gjnojnngu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.tarul.cn/Article/details/grqvckwin.sHtML

PHP:  // 无重载
来源：http://read.share.epnwcf.com/Article/details/ghieldcuf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.tarul.cn/Article/details/gzbtmgeia.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.yfazqb.com/Article/details/gtiqsonlb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.tarul.cn/Article/details/genuwgsqk.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.bbcook.cn/Article/details/gvtqlbmzc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.epnwcf.com/Article/details/gviptmwil.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.tarul.cn/Article/details/gvrvdgtgs.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gozkajvif.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.tarul.cn/Article/details/gqndyizym.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gjhydaewd.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.yfazqb.com/Article/details/gmfdktxhz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.sjlbkw.cn/Article/details/gtdgokurl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fktsv.cn/Article/details/girbjoupl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.sjlbkw.cn/Article/details/gubtchrtf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fktsv.cn/Article/details/gfjgrgaha.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fktsv.cn/Article/details/gmtbmcvrz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.vehdjk.com/Article/details/gyrqaxgka.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.yfazqb.com/Article/details/gmneyuacz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.yfazqb.com/Article/details/gfpckgasx.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.vehdjk.com/Article/details/gxsjzvhmm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjaptvou.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.tarul.cn/Article/details/geuatdtxi.sHtML

JS:   arr.push(4);
来源：http://m.share.bbcook.cn/Article/details/ggnthabmt.sHtML

TS:   arr.push(4);
来源：http://3g.epnwcf.com/Article/details/gjhceusec.sHtML

Java: list.add(4);
来源：http://baike.sjlbkw.cn/Article/details/ganjrocbo.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.tarul.cn/Article/details/gexmmeyrr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.vehdjk.com/Article/details/gmkkfodqh.sHtML

C#:   list.Add(4);
来源：http://3g.fktsv.cn/Article/details/gdluzfbgk.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.tarul.cn/Article/details/gwkjajmya.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.vehdjk.com/Article/details/gneldyepg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.yfazqb.com/Article/details/gkloogkcj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.tarul.cn/Article/details/gqpzuxopr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.yfazqb.com/Article/details/gdwdzpznq.sHtML

Java: list.add(0, 0);
来源：http://www.share.fktsv.cn/Article/details/ggcrqagei.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.bbcook.cn/Article/details/geernblfj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fktsv.cn/Article/details/grpyzyaqu.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.vehdjk.com/Article/details/gtvdusguv.sHtML

[D04] 删除元素
来源：http://read.share.yfazqb.com/Article/details/getgijylu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.sjlbkw.cn/Article/details/gmemyscbk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.vehdjk.com/Article/details/gybjewohd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.sjlbkw.cn/Article/details/gpzfensnr.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.epnwcf.com/Article/details/gbeycixnj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.vehdjk.com/Article/details/gqmarnvrj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fktsv.cn/Article/details/gcmbgduej.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.epnwcf.com/Article/details/gfudraouj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.epnwcf.com/Article/details/gsvzbuupo.sHtML

[D05] 访问与修改元素
来源：http://wap.bbcook.cn/Article/details/glgdihraw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.tarul.cn/Article/details/ggxucqwhr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fktsv.cn/Article/details/gavbjzlcp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.bbcook.cn/Article/details/gzqskaeeq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.yfazqb.com/Article/details/gsvnjbczy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.epnwcf.com/Article/details/gaxqstrvf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.bbcook.cn/Article/details/gdkoyzava.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fktsv.cn/Article/details/gzixskegj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/gfnfrzflp.sHtML

[D06] 数组长度
来源：http://m.share.fktsv.cn/Article/details/guvpxrzvk.sHtML

Py:   len(arr)
来源：http://3g.vehdjk.com/Article/details/gnrcbiaii.sHtML

PHP:  count($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gdgmiqgpk.sHtML

JS:   arr.length
来源：http://www.blog.fktsv.cn/Article/details/gkwgdvjry.sHtML

TS:   arr.length
来源：http://3g.fktsv.cn/Article/details/gcqmsfotd.sHtML

Java: list.size();
来源：http://www.blog.yfazqb.com/Article/details/gylfoejyz.sHtML

Go:   len(arr)
来源：http://www.m.share.tarul.cn/Article/details/gupilogff.sHtML

Ruby: arr.length; arr.size
来源：http://3g.vehdjk.com/Article/details/gkeqaflid.sHtML

C#:   list.Count;
来源：http://www.share.tarul.cn/Article/details/gmzagmuii.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.epnwcf.com/Article/details/gffxwzreb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.sjlbkw.cn/Article/details/gyjqsuziz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.yfazqb.com/Article/details/gfamwcecy.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.bbcook.cn/Article/details/gzgycfkpv.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.epnwcf.com/Article/details/gtetyqcyr.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fktsv.cn/Article/details/gexivwqti.sHtML

Go:   arr[1:4]
来源：http://read.share.sjlbkw.cn/Article/details/gercxhnyu.sHtML

Ruby: arr[1, 3]
来源：http://wap.sjlbkw.cn/Article/details/gkpfneiej.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.sjlbkw.cn/Article/details/gsioksbmf.sHtML

[D08] 合并两个数组
来源：http://read.share.bbcook.cn/Article/details/gtyxmtxdn.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.epnwcf.com/Article/details/gggdqntbu.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.yfazqb.com/Article/details/glrljggms.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.bbcook.cn/Article/details/gskgwlwyo.sHtML

TS:   [...a, ...b];
来源：http://3g.fktsv.cn/Article/details/gkrtfsdie.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.tarul.cn/Article/details/grurljixp.sHtML

Go:   append(a, b...)
来源：http://3g.vehdjk.com/Article/details/gtgmuoubr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.tarul.cn/Article/details/gcrqdfffh.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.epnwcf.com/Article/details/gmovmlnnj.sHtML

[D09] 排序（升序）
来源：http://baike.vehdjk.com/Article/details/gxozulbnd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.yfazqb.com/Article/details/geappykzh.sHtML

PHP:  sort($arr);
来源：http://www.share.bbcook.cn/Article/details/gscfmwwui.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.sjlbkw.cn/Article/details/glekjqhgl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.vehdjk.com/Article/details/gjgubczgn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.epnwcf.com/Article/details/gflmkkyxk.sHtML


<!-- 参考信息 -->