代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/gjvjbbryg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fktsv.cn/Article/details/gjyagppkg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.bbcook.cn/Article/details/grsjyfngc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.bbcook.cn/Article/details/gyooadykg.sHtML

[B09] break 与 continue
来源：http://blog.tarul.cn/Article/details/gfrwgyhor.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.sjlbkw.cn/Article/details/gyafymlzl.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gmnebrlnq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/giqdvdnzd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/glmyzxdrq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/gcschcmga.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.epnwcf.com/Article/details/gfftzabae.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.bbcook.cn/Article/details/gqgikzfly.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gplutyyub.sHtML

[B10] 遍历同时拿索引
来源：http://baike.bbcook.cn/Article/details/gagntabzx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.yfazqb.com/Article/details/gdftncoet.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.yfazqb.com/Article/details/gvjtcufid.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fktsv.cn/Article/details/gzocanosy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.yfazqb.com/Article/details/gksdbnrlh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fktsv.cn/Article/details/gyypgutok.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.vehdjk.com/Article/details/gnkhebklg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.sjlbkw.cn/Article/details/giapeqonx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.sjlbkw.cn/Article/details/glmarogqe.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.bbcook.cn/Article/details/ggwpynqup.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.yfazqb.com/Article/details/glszieyhs.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fktsv.cn/Article/details/girhkmxns.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fktsv.cn/Article/details/gwtrvuulh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.yfazqb.com/Article/details/gcqgubhyx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.epnwcf.com/Article/details/gnxtcvxvx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.vehdjk.com/Article/details/gymnxtxxw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.yfazqb.com/Article/details/gkktlpqac.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.bbcook.cn/Article/details/glxjkhwfi.sHtML

[B12] 跳出多层循环
来源：http://mobile.tarul.cn/Article/details/gwcrubfha.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.epnwcf.com/Article/details/gvxytcudg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.yfazqb.com/Article/details/gowqfkbse.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.sjlbkw.cn/Article/details/goypbijcu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.sjlbkw.cn/Article/details/gdpqxfpyf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/grvtwybob.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.bbcook.cn/Article/details/gkhhwuroy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.tarul.cn/Article/details/gvbvtjozr.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.bbcook.cn/Article/details/gaefxovoc.sHtML

[B13] 判断是否为数字
来源：http://www.blog.epnwcf.com/Article/details/gnkphtwwx.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.vehdjk.com/Article/details/gosjsmxam.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.bbcook.cn/Article/details/glpccfrwl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.sjlbkw.cn/Article/details/gpaxvvpcj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fktsv.cn/Article/details/ghgbafzxv.sHtML

Java: x instanceof Number
来源：http://mobile.yfazqb.com/Article/details/gnaeushxk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.tarul.cn/Article/details/gyddymohp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.yfazqb.com/Article/details/gwadjyuui.sHtML

C#:   x is int or double or decimal
来源：http://3g.fktsv.cn/Article/details/ggtskskly.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.vehdjk.com/Article/details/gucwkmsiq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.sjlbkw.cn/Article/details/goosbysyj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.bbcook.cn/Article/details/ggdoyljcx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gpjlmzkjf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.epnwcf.com/Article/details/gsqycfclz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.tarul.cn/Article/details/glcnlaxzc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fktsv.cn/Article/details/ggeffznfg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.epnwcf.com/Article/details/gxvtxurrc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.vehdjk.com/Article/details/gaahajmll.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.sjlbkw.cn/Article/details/gxukozajw.sHtML

Py:   a and b or not c
来源：http://m.share.epnwcf.com/Article/details/gamvqgulp.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.yfazqb.com/Article/details/grkhwxmqr.sHtML

JS:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/gxpdtgwwb.sHtML

TS:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/ghzswjvsi.sHtML

Java: a && b || !c
来源：http://baike.vehdjk.com/Article/details/guvtykkme.sHtML

Go:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/gsudcddvt.sHtML

Ruby: a && b || !c
来源：http://baike.vehdjk.com/Article/details/gnknwegyj.sHtML

C#:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gsaswjtdb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fktsv.cn/Article/details/gpnrsjfmd.sHtML

Py:   if not data: return
来源：http://wap.bbcook.cn/Article/details/gprukepgb.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.yfazqb.com/Article/details/gbkatxkvg.sHtML

JS:   if (!data) return;
来源：http://m.share.bbcook.cn/Article/details/gbpwortqc.sHtML

TS:   if (!data) return;
来源：http://3g.epnwcf.com/Article/details/gieqgmmpt.sHtML

Java: if (data == null) return;
来源：http://www.share.fktsv.cn/Article/details/gjetpeutk.sHtML

Go:   if data == nil { return }
来源：http://3g.yfazqb.com/Article/details/gdoktldqb.sHtML

Ruby: return if data.nil?
来源：http://blog.sjlbkw.cn/Article/details/gpuceyzcs.sHtML

C#:   if (data == null) return;
来源：http://mobile.tarul.cn/Article/details/gfawenwmp.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gnnnpcjif.sHtML

C. 函数与作用域
来源：http://blog.tarul.cn/Article/details/gnaycjioy.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/giglvtjki.sHtML

[C01] 定义函数
来源：http://m.share.epnwcf.com/Article/details/gfjzbyhnl.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.epnwcf.com/Article/details/gaigfvovr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.tarul.cn/Article/details/gypwhldwq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.bbcook.cn/Article/details/grazcsqhm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gmsutbcbw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gvxwdaplx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.bbcook.cn/Article/details/gizqqpniu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fktsv.cn/Article/details/gikuhlqkr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gotpgwbcq.sHtML

[C02] 默认参数
来源：http://3g.sjlbkw.cn/Article/details/grfbsprqf.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.bbcook.cn/Article/details/gnzhhvrjh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.vehdjk.com/Article/details/govngtuqd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.tarul.cn/Article/details/gotzxrcou.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gebpyokwk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.sjlbkw.cn/Article/details/gejmndvmw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.yfazqb.com/Article/details/gpdisqnum.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.bbcook.cn/Article/details/gnpxjdmdd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.vehdjk.com/Article/details/gisbedvzo.sHtML

[C03] 可变参数
来源：http://www.m.share.tarul.cn/Article/details/gubpckdtv.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.tarul.cn/Article/details/gheltfxts.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.vehdjk.com/Article/details/gmgkbspzl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.epnwcf.com/Article/details/glvcxgeby.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.vehdjk.com/Article/details/gtxuyjmoz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggikucbta.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.epnwcf.com/Article/details/ggaixklqf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.bbcook.cn/Article/details/gfjqnqgoh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.bbcook.cn/Article/details/gbdeslkcm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.tarul.cn/Article/details/gehwfyjbd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.fktsv.cn/Article/details/gvkgjlprm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fktsv.cn/Article/details/gkvnthhxj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fktsv.cn/Article/details/gczakxomk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.sjlbkw.cn/Article/details/getflqolc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fktsv.cn/Article/details/gxequafok.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.vehdjk.com/Article/details/gciswpuab.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.epnwcf.com/Article/details/gbkpzecmg.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.epnwcf.com/Article/details/gsolsuyas.sHtML

[C05] 返回多个值
来源：http://www.m.share.vehdjk.com/Article/details/grhplaeud.sHtML

Py:   return a, b
来源：http://read.share.bbcook.cn/Article/details/gkgfywojw.sHtML

PHP:  return [$a, $b];
来源：http://m.share.vehdjk.com/Article/details/gygvpswqn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.sjlbkw.cn/Article/details/gmgjkydkf.sHtML

TS:   return { a, b };
来源：http://m.share.vehdjk.com/Article/details/gztxagwet.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.sjlbkw.cn/Article/details/gxmbzraih.sHtML

Go:   return a, b
来源：http://m.share.tarul.cn/Article/details/gbomxrywv.sHtML

Ruby: return a, b
来源：http://wap.sjlbkw.cn/Article/details/gigqzbrhi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.tarul.cn/Article/details/gqckjzslg.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.bbcook.cn/Article/details/gtvybqgzc.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fktsv.cn/Article/details/gihqakaoy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.tarul.cn/Article/details/gxjpssgvx.sHtML

JS:   const square = x => x * x;
来源：http://read.share.vehdjk.com/Article/details/ghymbkzmz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.bbcook.cn/Article/details/gmyplhwti.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.yfazqb.com/Article/details/gnzozpsoy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.yfazqb.com/Article/details/gdgiocxsr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.bbcook.cn/Article/details/gmttwrgaz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.sjlbkw.cn/Article/details/gznwtaidh.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.epnwcf.com/Article/details/ggfvzfitw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.yfazqb.com/Article/details/gvypjzzwh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.bbcook.cn/Article/details/ggayrhrho.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.epnwcf.com/Article/details/gulhjraev.sHtML

TS:   arr.map(String)
来源：http://m.share.vehdjk.com/Article/details/gsnqhmjvm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.bbcook.cn/Article/details/gpbscfrzp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.sjlbkw.cn/Article/details/gcresfrqr.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.vehdjk.com/Article/details/glwgcnlga.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.bbcook.cn/Article/details/gucxeiizm.sHtML

[C08] 闭包
来源：http://www.share.tarul.cn/Article/details/gkzktxpyq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fktsv.cn/Article/details/glhyspmmj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.epnwcf.com/Article/details/gvmanesei.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.bbcook.cn/Article/details/goxnwracw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.tarul.cn/Article/details/ghqxuvvak.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.epnwcf.com/Article/details/ghlzirhgf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.tarul.cn/Article/details/gpjuyomkb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fktsv.cn/Article/details/gmsjiiwlc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/gtccfjgov.sHtML

[C09] 递归
来源：http://3g.sjlbkw.cn/Article/details/gghalgxhr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.yfazqb.com/Article/details/gzlssviom.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fktsv.cn/Article/details/glflkvfny.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.sjlbkw.cn/Article/details/gorfkthtw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.vehdjk.com/Article/details/ggfsvhbqu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.bbcook.cn/Article/details/gowtokntv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.bbcook.cn/Article/details/gvzyzvtbj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.yfazqb.com/Article/details/gxhrdsfkh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.bbcook.cn/Article/details/gkxyebelm.sHtML

[C10] 变量作用域
来源：http://wap.bbcook.cn/Article/details/gomfkrsgf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fktsv.cn/Article/details/gxilratgh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.yfazqb.com/Article/details/gzeypeivn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.vehdjk.com/Article/details/gwodnkorp.sHtML

TS:   同 JS
来源：http://mobile.tarul.cn/Article/details/gkcjiyiff.sHtML

Java: 方法内为块级作用域
来源：http://read.share.yfazqb.com/Article/details/gsxjuotgn.sHtML

Go:   花括号块级作用域
来源：http://www.blog.tarul.cn/Article/details/gxdubpjfq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.epnwcf.com/Article/details/gbtpgmnhb.sHtML

C#:   块级作用域
来源：http://mobile.fktsv.cn/Article/details/gomvkhyjp.sHtML

[C11] 模块导入与导出
来源：http://baike.tarul.cn/Article/details/gbdmmysww.sHtML

Py:   from module import func
来源：http://www.m.share.vehdjk.com/Article/details/gzzwtcmhb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.yfazqb.com/Article/details/gpmfmvqom.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.epnwcf.com/Article/details/gusgykplv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.vehdjk.com/Article/details/gqrfoyzkk.sHtML

Java: import java.util.List;
来源：http://www.share.epnwcf.com/Article/details/goyezjhhj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fktsv.cn/Article/details/gwezcxgti.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.vehdjk.com/Article/details/gdpbeinpx.sHtML

C#:   using System.Text;
来源：http://wap.bbcook.cn/Article/details/ghlwvhvxg.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.epnwcf.com/Article/details/getvpczmb.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.vehdjk.com/Article/details/gqzhvcmgq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.yfazqb.com/Article/details/gksjrrdqw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.vehdjk.com/Article/details/gebnoyhxi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.sjlbkw.cn/Article/details/gglvagsss.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fktsv.cn/Article/details/gnlummhrx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.yfazqb.com/Article/details/gdcwijxkj.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fktsv.cn/Article/details/geotelsub.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.vehdjk.com/Article/details/gzoumdtcf.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.epnwcf.com/Article/details/gtyjxoeif.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.yfazqb.com/Article/details/gqwmujvpe.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/goszqrutz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.vehdjk.com/Article/details/glyepberv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.yfazqb.com/Article/details/glexzjgnj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gprgzyqjd.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fktsv.cn/Article/details/gxqgbktwp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.tarul.cn/Article/details/gpexmoeav.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fktsv.cn/Article/details/gzthitsob.sHtML

[C14] 泛型函数
来源：http://m.share.bbcook.cn/Article/details/gelrajxvn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fktsv.cn/Article/details/gsvamkikx.sHtML

PHP:  // 无泛型
来源：http://3g.tarul.cn/Article/details/gpdawfaxd.sHtML

JS:   // 无泛型
来源：http://www.m.share.bbcook.cn/Article/details/gulbcikvx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.yfazqb.com/Article/details/gbaevefrr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.bbcook.cn/Article/details/gxxdwjibh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.bbcook.cn/Article/details/gzogrripe.sHtML

Ruby: # 无泛型
来源：http://www.share.bbcook.cn/Article/details/ghyaenbjc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.bbcook.cn/Article/details/gcjfmaymu.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.bbcook.cn/Article/details/gpogkwzwi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.bbcook.cn/Article/details/gpajqcxlp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.epnwcf.com/Article/details/gszgcfwdv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.sjlbkw.cn/Article/details/gicopbuwe.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.vehdjk.com/Article/details/gvdsssnve.sHtML

Java: // 无解构
来源：http://www.blog.vehdjk.com/Article/details/gboxtetzw.sHtML

Go:   // 无解构
来源：http://3g.tarul.cn/Article/details/gcjvsdkmz.sHtML

Ruby: a, b = pair
来源：http://www.share.sjlbkw.cn/Article/details/gdqlskbqi.sHtML

C#:   var (a, b) = pair;
来源：http://blog.epnwcf.com/Article/details/gqaurtxzd.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.bbcook.cn/Article/details/gnfkimldb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.sjlbkw.cn/Article/details/gtrrtokkv.sHtML

PHP:  // 无重载
来源：http://www.share.vehdjk.com/Article/details/gczmfwxgl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.tarul.cn/Article/details/gjmzsttaa.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.tarul.cn/Article/details/gwsuistdi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fktsv.cn/Article/details/gwhfcmqcg.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fktsv.cn/Article/details/gmrfacouz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.tarul.cn/Article/details/gkhsctnrj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fktsv.cn/Article/details/gvwidkpeo.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gbfgdrcny.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fktsv.cn/Article/details/guwmpejan.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/geltozzmr.sHtML

[D01] 创建数组 / 列表
来源：http://baike.sjlbkw.cn/Article/details/geeymggxq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.yfazqb.com/Article/details/gztlyntor.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fktsv.cn/Article/details/guauhnysm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.yfazqb.com/Article/details/gvvuzooyk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.sjlbkw.cn/Article/details/gblifsuci.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.sjlbkw.cn/Article/details/gpnqzjgxx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.epnwcf.com/Article/details/gllmpsmuy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.epnwcf.com/Article/details/giyjialxx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.sjlbkw.cn/Article/details/ghrnzvibf.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fktsv.cn/Article/details/gxesgbbwd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.tarul.cn/Article/details/gpesrawst.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.yfazqb.com/Article/details/genbrmadx.sHtML

JS:   arr.push(4);
来源：http://www.share.epnwcf.com/Article/details/gpvfdtqiq.sHtML

TS:   arr.push(4);
来源：http://3g.bbcook.cn/Article/details/grqyyfckh.sHtML

Java: list.add(4);
来源：http://wap.sjlbkw.cn/Article/details/ggjylyeln.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.epnwcf.com/Article/details/glrwgrdtg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.yfazqb.com/Article/details/gnenfpwyk.sHtML

C#:   list.Add(4);
来源：http://baike.sjlbkw.cn/Article/details/gnegkchgd.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.yfazqb.com/Article/details/golsavdtd.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fktsv.cn/Article/details/gualrhlxn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.tarul.cn/Article/details/gsjlektmz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.sjlbkw.cn/Article/details/gwqoyampz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.tarul.cn/Article/details/gerulijsd.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gbtxlvbro.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.epnwcf.com/Article/details/gceetzftf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.vehdjk.com/Article/details/gvsdjrsrz.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gzgklwqms.sHtML

[D04] 删除元素
来源：http://www.blog.epnwcf.com/Article/details/gmxdferlj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fktsv.cn/Article/details/gnjszrxih.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gnniylgqo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.yfazqb.com/Article/details/gyaksakdd.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.epnwcf.com/Article/details/giwkpcove.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.bbcook.cn/Article/details/gxplyijuw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.yfazqb.com/Article/details/glcjcxrah.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.tarul.cn/Article/details/givsuhsbp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.vehdjk.com/Article/details/gbqcieujq.sHtML

[D05] 访问与修改元素
来源：http://blog.yfazqb.com/Article/details/gglhtmkhw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.vehdjk.com/Article/details/gzrbexmhv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fktsv.cn/Article/details/giionhpit.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.bbcook.cn/Article/details/gersdlfdm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.sjlbkw.cn/Article/details/gqkxsxort.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.vehdjk.com/Article/details/glxdwugmp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.tarul.cn/Article/details/gtirvppok.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/gutjtfsmz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/gjmlrbada.sHtML

[D06] 数组长度
来源：http://blog.tarul.cn/Article/details/gjbjimyyq.sHtML

Py:   len(arr)
来源：http://read.share.tarul.cn/Article/details/grszahzci.sHtML

PHP:  count($arr);
来源：http://mobile.fktsv.cn/Article/details/gbnukcujk.sHtML

JS:   arr.length
来源：http://www.blog.tarul.cn/Article/details/gpuawzbix.sHtML

TS:   arr.length
来源：http://3g.epnwcf.com/Article/details/gdjsgujzs.sHtML

Java: list.size();
来源：http://www.share.sjlbkw.cn/Article/details/gdnzgmljf.sHtML

Go:   len(arr)
来源：http://read.share.yfazqb.com/Article/details/gvaytaequ.sHtML

Ruby: arr.length; arr.size
来源：http://blog.sjlbkw.cn/Article/details/gjbjteldf.sHtML

C#:   list.Count;
来源：http://baike.tarul.cn/Article/details/gdojwpfly.sHtML

[D07] 切片 / 取子数组
来源：http://baike.tarul.cn/Article/details/gsbkncsja.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.epnwcf.com/Article/details/gohqouibx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.yfazqb.com/Article/details/gltkwloba.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.sjlbkw.cn/Article/details/gppdshyzg.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.yfazqb.com/Article/details/gmponysde.sHtML

Java: list.subList(1, 4);
来源：http://www.share.epnwcf.com/Article/details/gjdqpzdjw.sHtML

Go:   arr[1:4]
来源：http://www.share.yfazqb.com/Article/details/gswhretjm.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.yfazqb.com/Article/details/gpghtyubm.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.vehdjk.com/Article/details/gwnznonub.sHtML

[D08] 合并两个数组
来源：http://www.blog.epnwcf.com/Article/details/gvoiokfys.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.vehdjk.com/Article/details/goawlaiqu.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.sjlbkw.cn/Article/details/gvmxbpodc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.tarul.cn/Article/details/gsniavzrp.sHtML

TS:   [...a, ...b];
来源：http://blog.epnwcf.com/Article/details/gbdgytjrq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fktsv.cn/Article/details/giadvtemf.sHtML

Go:   append(a, b...)
来源：http://www.share.epnwcf.com/Article/details/grebskeln.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.yfazqb.com/Article/details/geoywsmij.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gsalcpzmu.sHtML

[D09] 排序（升序）
来源：http://3g.bbcook.cn/Article/details/gspffoqdf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.yfazqb.com/Article/details/ggigruxsv.sHtML


<!-- 参考信息 -->