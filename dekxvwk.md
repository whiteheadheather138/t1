代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://read.share.vehdjk.com/Article/details/ggzbepddx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.yfazqb.com/Article/details/gigyajciu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.sjlbkw.cn/Article/details/gfsnnppjj.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.sjlbkw.cn/Article/details/gguebkomi.sHtML

[B09] break 与 continue
来源：http://3g.tarul.cn/Article/details/gxgrkabgn.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.tarul.cn/Article/details/gseiaohmc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/ggvccykan.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gvfyxksvj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gbtpefnvo.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gpynbqezk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.vehdjk.com/Article/details/glelsmiki.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.yfazqb.com/Article/details/ghaerntbq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gtfcfvtkq.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.epnwcf.com/Article/details/gssivmeqe.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fktsv.cn/Article/details/gsfvgzqgd.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.yfazqb.com/Article/details/gyjbishxp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.vehdjk.com/Article/details/gzimpxhsc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.yfazqb.com/Article/details/gqjeqhagc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.yfazqb.com/Article/details/gnbbrtndl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.bbcook.cn/Article/details/ghdlugjae.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.vehdjk.com/Article/details/glgomelcp.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.bbcook.cn/Article/details/gthfdlqzu.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.bbcook.cn/Article/details/gbbswbmzr.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.yfazqb.com/Article/details/gefrlahus.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fktsv.cn/Article/details/gorvfkoia.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.sjlbkw.cn/Article/details/grvcmhbqe.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fktsv.cn/Article/details/gkxmtlbdh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.vehdjk.com/Article/details/gmnzghzfu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.yfazqb.com/Article/details/goqzletqq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.sjlbkw.cn/Article/details/gflyuercu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.bbcook.cn/Article/details/gjdmdiseb.sHtML

[B12] 跳出多层循环
来源：http://read.share.fktsv.cn/Article/details/gbkmnenmv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fktsv.cn/Article/details/gzexnptpu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.tarul.cn/Article/details/gyszmozjn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.vehdjk.com/Article/details/gulicqlxt.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.tarul.cn/Article/details/garutjchv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.vehdjk.com/Article/details/gbngailbo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.vehdjk.com/Article/details/ghnegpueo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fktsv.cn/Article/details/getslmqhd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.bbcook.cn/Article/details/ginvcrryd.sHtML

[B13] 判断是否为数字
来源：http://wap.vehdjk.com/Article/details/guisbalnn.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.tarul.cn/Article/details/gqkpkkgla.sHtML

PHP:  is_numeric($x)
来源：http://wap.bbcook.cn/Article/details/gtkoddbag.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.yfazqb.com/Article/details/gybnchyqh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.bbcook.cn/Article/details/grbazpvte.sHtML

Java: x instanceof Number
来源：http://m.share.sjlbkw.cn/Article/details/gasalaqrn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.bbcook.cn/Article/details/gwrpxkuqt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.bbcook.cn/Article/details/gyanqmrjl.sHtML

C#:   x is int or double or decimal
来源：http://baike.sjlbkw.cn/Article/details/gdgnfgrrj.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.vehdjk.com/Article/details/gdveyancw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.vehdjk.com/Article/details/goccguikn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.vehdjk.com/Article/details/gxiweaqzp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.vehdjk.com/Article/details/gqyujgrcc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.bbcook.cn/Article/details/gbzldlfbe.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.vehdjk.com/Article/details/gxtbnfmzn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.vehdjk.com/Article/details/geyzagwzl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.epnwcf.com/Article/details/gukniazkx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/givkvimsf.sHtML

[B15] 布尔运算与取反
来源：http://wap.bbcook.cn/Article/details/gaksfgxuy.sHtML

Py:   a and b or not c
来源：http://www.share.bbcook.cn/Article/details/gwdvlvxgs.sHtML

PHP:  $a && $b || !$c
来源：http://baike.vehdjk.com/Article/details/gnsgryszn.sHtML

JS:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/glwgzuxzr.sHtML

TS:   a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gdhcyyceu.sHtML

Java: a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/ghkufjgvc.sHtML

Go:   a && b || !c
来源：http://blog.fktsv.cn/Article/details/gzswfdugp.sHtML

Ruby: a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/gmxwmwaei.sHtML

C#:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/guvlksjwl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.vehdjk.com/Article/details/gmvgwtldp.sHtML

Py:   if not data: return
来源：http://www.m.share.vehdjk.com/Article/details/gerttgssj.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.tarul.cn/Article/details/glnunaclw.sHtML

JS:   if (!data) return;
来源：http://read.share.yfazqb.com/Article/details/gezcunzud.sHtML

TS:   if (!data) return;
来源：http://mobile.tarul.cn/Article/details/gklosoanb.sHtML

Java: if (data == null) return;
来源：http://www.share.epnwcf.com/Article/details/gwlcyxtqg.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fktsv.cn/Article/details/gehqjixlu.sHtML

Ruby: return if data.nil?
来源：http://blog.yfazqb.com/Article/details/geqzshvzl.sHtML

C#:   if (data == null) return;
来源：http://m.share.bbcook.cn/Article/details/gajvrgcon.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gsglkhhdw.sHtML

C. 函数与作用域
来源：http://www.m.share.vehdjk.com/Article/details/gagrojcaj.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gwbavahgb.sHtML

[C01] 定义函数
来源：http://mobile.vehdjk.com/Article/details/grjneovjs.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.epnwcf.com/Article/details/gpmlqrtby.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gzzsavtpp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gqilbbizi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gtgzelefu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/guhguqfhf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.yfazqb.com/Article/details/gvklxfjvy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fktsv.cn/Article/details/gtvyqqyfy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gtgysrqls.sHtML

[C02] 默认参数
来源：http://mobile.tarul.cn/Article/details/gslzkpeid.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.yfazqb.com/Article/details/grctrtgnb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.vehdjk.com/Article/details/gqvvxdonr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.bbcook.cn/Article/details/gareunqhy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.epnwcf.com/Article/details/gxtvtmmgb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.vehdjk.com/Article/details/gnmwhgfdd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.epnwcf.com/Article/details/gsytycptn.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.bbcook.cn/Article/details/gqfsyirij.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fktsv.cn/Article/details/gpvffzpko.sHtML

[C03] 可变参数
来源：http://3g.sjlbkw.cn/Article/details/ggamsswrt.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fktsv.cn/Article/details/gpjphikne.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.tarul.cn/Article/details/guahonbck.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.sjlbkw.cn/Article/details/glhioujcc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.bbcook.cn/Article/details/gcsjccnhc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.epnwcf.com/Article/details/gsohvgvtb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.epnwcf.com/Article/details/gcbcazofb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.sjlbkw.cn/Article/details/gkdkrtdek.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fktsv.cn/Article/details/gpxwtemhj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.sjlbkw.cn/Article/details/gkiqlksmd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.tarul.cn/Article/details/gbrxsevve.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fktsv.cn/Article/details/gnwgudrfw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.tarul.cn/Article/details/gxhgfymag.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.tarul.cn/Article/details/geajfvzpe.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.sjlbkw.cn/Article/details/gsjbezrxl.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.yfazqb.com/Article/details/gmprwoaba.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.tarul.cn/Article/details/gcncwpdon.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.vehdjk.com/Article/details/ghjvwjvzl.sHtML

[C05] 返回多个值
来源：http://www.m.share.tarul.cn/Article/details/gpqfcmvai.sHtML

Py:   return a, b
来源：http://baike.bbcook.cn/Article/details/ggowhmzpi.sHtML

PHP:  return [$a, $b];
来源：http://mobile.epnwcf.com/Article/details/gvhpmxiqw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.epnwcf.com/Article/details/gnaintqzh.sHtML

TS:   return { a, b };
来源：http://mobile.sjlbkw.cn/Article/details/gsledtzqp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.sjlbkw.cn/Article/details/gvhgphorz.sHtML

Go:   return a, b
来源：http://3g.yfazqb.com/Article/details/gpsizjnll.sHtML

Ruby: return a, b
来源：http://www.m.share.epnwcf.com/Article/details/gyzcjbivv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.vehdjk.com/Article/details/gsuzihzde.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.tarul.cn/Article/details/ggakqkadl.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.sjlbkw.cn/Article/details/gkzeaejqn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fktsv.cn/Article/details/gxummuvdq.sHtML

JS:   const square = x => x * x;
来源：http://m.share.bbcook.cn/Article/details/ghqgdnfmp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.epnwcf.com/Article/details/gggoybpwh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.epnwcf.com/Article/details/gjytuxysp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.vehdjk.com/Article/details/gwykhsktd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.tarul.cn/Article/details/gzrthbimm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.bbcook.cn/Article/details/gxdcmdrbq.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.epnwcf.com/Article/details/gcchowjdq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fktsv.cn/Article/details/gaunnkhrv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fktsv.cn/Article/details/ggogumnuw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.sjlbkw.cn/Article/details/gelwzgswq.sHtML

TS:   arr.map(String)
来源：http://blog.sjlbkw.cn/Article/details/gzwmxhwan.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.yfazqb.com/Article/details/gacqmprxc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.bbcook.cn/Article/details/guysqmsyq.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fktsv.cn/Article/details/gqyxasmne.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.sjlbkw.cn/Article/details/gqvtfsntl.sHtML

[C08] 闭包
来源：http://www.m.share.vehdjk.com/Article/details/gckltigwd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.vehdjk.com/Article/details/gondodetd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.vehdjk.com/Article/details/gqucaeaao.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.vehdjk.com/Article/details/gnqwmnesv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.yfazqb.com/Article/details/gqytrzmtk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.sjlbkw.cn/Article/details/ggvucgyjr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fktsv.cn/Article/details/ghrdxaijg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.sjlbkw.cn/Article/details/grxbunbnd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fktsv.cn/Article/details/gfnpsmubk.sHtML

[C09] 递归
来源：http://www.share.fktsv.cn/Article/details/gashicrib.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fktsv.cn/Article/details/glhagdbks.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gizynqkmu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.vehdjk.com/Article/details/grefnmznt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.epnwcf.com/Article/details/glrvsyynb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.vehdjk.com/Article/details/gzcojnnah.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.yfazqb.com/Article/details/gbbbxkewn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.epnwcf.com/Article/details/gnwbznaon.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fktsv.cn/Article/details/gsbekysgi.sHtML

[C10] 变量作用域
来源：http://3g.bbcook.cn/Article/details/gyeaikqpu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.vehdjk.com/Article/details/gjapcpdhe.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.vehdjk.com/Article/details/gebqhhlyc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.epnwcf.com/Article/details/gfslcpqdg.sHtML

TS:   同 JS
来源：http://read.share.vehdjk.com/Article/details/glkcybcsb.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fktsv.cn/Article/details/gohtoibgw.sHtML

Go:   花括号块级作用域
来源：http://blog.epnwcf.com/Article/details/glftkijcp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.vehdjk.com/Article/details/gazibkaak.sHtML

C#:   块级作用域
来源：http://www.share.sjlbkw.cn/Article/details/gryhiqchr.sHtML

[C11] 模块导入与导出
来源：http://read.share.fktsv.cn/Article/details/gpbarjkbd.sHtML

Py:   from module import func
来源：http://blog.epnwcf.com/Article/details/gdrmeprix.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.bbcook.cn/Article/details/gyiyafmbg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fktsv.cn/Article/details/glczuuenv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.tarul.cn/Article/details/gnqnpwqwo.sHtML

Java: import java.util.List;
来源：http://www.blog.bbcook.cn/Article/details/gkbilqbim.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.epnwcf.com/Article/details/gotebrvap.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.sjlbkw.cn/Article/details/gkqrxzdno.sHtML

C#:   using System.Text;
来源：http://www.m.share.epnwcf.com/Article/details/gnbhnyrrh.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.vehdjk.com/Article/details/gdzqzjuxu.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.epnwcf.com/Article/details/gqiutzlme.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.epnwcf.com/Article/details/gnequovnk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.vehdjk.com/Article/details/ghhwcfwzj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.tarul.cn/Article/details/gdixbpqex.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.vehdjk.com/Article/details/gjkkjtvfn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fktsv.cn/Article/details/gslnikpnm.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fktsv.cn/Article/details/gexuejxmf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.vehdjk.com/Article/details/glabktxfa.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.bbcook.cn/Article/details/gwltqlnqu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.vehdjk.com/Article/details/gheftxqrn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/gtznsomik.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.tarul.cn/Article/details/gwhmqnori.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gtmzngoif.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gvnqocthr.sHtML

Go:   func add(a, b int) int
来源：http://blog.vehdjk.com/Article/details/gyolyudcu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.yfazqb.com/Article/details/gmbuwtgea.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.sjlbkw.cn/Article/details/gegwarheu.sHtML

[C14] 泛型函数
来源：http://read.share.sjlbkw.cn/Article/details/gjpbnoaxy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.vehdjk.com/Article/details/gmzygwwfq.sHtML

PHP:  // 无泛型
来源：http://wap.sjlbkw.cn/Article/details/gtrnpkahs.sHtML

JS:   // 无泛型
来源：http://www.share.vehdjk.com/Article/details/ghkaooeic.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.vehdjk.com/Article/details/gayumxekj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.bbcook.cn/Article/details/grrcfquag.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.yfazqb.com/Article/details/gnhlclssd.sHtML

Ruby: # 无泛型
来源：http://blog.tarul.cn/Article/details/gsuawfjve.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.epnwcf.com/Article/details/guvvhyhqm.sHtML

[C15] 解构 / 展开参数
来源：http://baike.yfazqb.com/Article/details/gfjutluem.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.epnwcf.com/Article/details/gjmslgazf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.epnwcf.com/Article/details/gjkqkakaj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gjcwvsycb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.yfazqb.com/Article/details/gpmymbsqp.sHtML

Java: // 无解构
来源：http://www.m.share.bbcook.cn/Article/details/giqcxokri.sHtML

Go:   // 无解构
来源：http://blog.yfazqb.com/Article/details/gxzvxrufk.sHtML

Ruby: a, b = pair
来源：http://3g.bbcook.cn/Article/details/gmpwcjjbb.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.tarul.cn/Article/details/gbesltywb.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.sjlbkw.cn/Article/details/glhvtwczg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.yfazqb.com/Article/details/gjlzdknra.sHtML

PHP:  // 无重载
来源：http://www.blog.epnwcf.com/Article/details/ggdwpwzme.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.tarul.cn/Article/details/gfdjsaqln.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.yfazqb.com/Article/details/gnwmkqwdy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.vehdjk.com/Article/details/gazcdwvfi.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.yfazqb.com/Article/details/gocsrcvnv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fktsv.cn/Article/details/gkjzhqksu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.yfazqb.com/Article/details/gruwsrkzt.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gqmendeon.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.sjlbkw.cn/Article/details/gfewxypqi.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gnfeznopy.sHtML

[D01] 创建数组 / 列表
来源：http://blog.bbcook.cn/Article/details/gfksbdrgl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.vehdjk.com/Article/details/gzuwyfilh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.tarul.cn/Article/details/galmrnigx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.tarul.cn/Article/details/ggkfiispi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.yfazqb.com/Article/details/gwfgmlmnu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fktsv.cn/Article/details/gajzcdoxu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fktsv.cn/Article/details/grvpnnyum.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.epnwcf.com/Article/details/ghwylwtug.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.bbcook.cn/Article/details/ggmpxhokd.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fktsv.cn/Article/details/gnbshubyw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.epnwcf.com/Article/details/gdefqjewt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.epnwcf.com/Article/details/gwwjetuhk.sHtML

JS:   arr.push(4);
来源：http://baike.tarul.cn/Article/details/gqnjfplkq.sHtML

TS:   arr.push(4);
来源：http://baike.sjlbkw.cn/Article/details/gafjrqihh.sHtML

Java: list.add(4);
来源：http://www.m.share.yfazqb.com/Article/details/gnbgmpaeq.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.yfazqb.com/Article/details/ghaqmxure.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fktsv.cn/Article/details/gdbrujvow.sHtML

C#:   list.Add(4);
来源：http://read.share.sjlbkw.cn/Article/details/gsmboutna.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fktsv.cn/Article/details/gghuqkmxs.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gkcyxyotl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fktsv.cn/Article/details/gmueurkbl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.sjlbkw.cn/Article/details/gmmayjuia.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.sjlbkw.cn/Article/details/gjdblylqn.sHtML

Java: list.add(0, 0);
来源：http://wap.bbcook.cn/Article/details/gsqdjtsch.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.sjlbkw.cn/Article/details/gdtjorzgf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.tarul.cn/Article/details/gmmcraong.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.tarul.cn/Article/details/gesguotxb.sHtML

[D04] 删除元素
来源：http://m.share.fktsv.cn/Article/details/gemdkhaoh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.vehdjk.com/Article/details/gxcyjfckv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gdqakrmli.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fktsv.cn/Article/details/gzbromonm.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.epnwcf.com/Article/details/ghovroeab.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.vehdjk.com/Article/details/gcvmzxneo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.bbcook.cn/Article/details/gyrlxgjox.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.bbcook.cn/Article/details/ggiezyvag.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.sjlbkw.cn/Article/details/gkzycbbbo.sHtML

[D05] 访问与修改元素
来源：http://mobile.epnwcf.com/Article/details/guuplvjwf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/gzyinxnxh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fktsv.cn/Article/details/ghyapgzcm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.yfazqb.com/Article/details/gvzsiflla.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.yfazqb.com/Article/details/gxrjkunya.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.yfazqb.com/Article/details/gvphxbdsc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.yfazqb.com/Article/details/gtqbrwftp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fktsv.cn/Article/details/guxpftzoq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.bbcook.cn/Article/details/ggqvbdtvl.sHtML

[D06] 数组长度
来源：http://m.share.fktsv.cn/Article/details/grplxofka.sHtML

Py:   len(arr)
来源：http://3g.vehdjk.com/Article/details/gankniofb.sHtML

PHP:  count($arr);
来源：http://m.share.tarul.cn/Article/details/gboqxkhxz.sHtML

JS:   arr.length
来源：http://wap.tarul.cn/Article/details/gfynuvsiu.sHtML

TS:   arr.length
来源：http://blog.fktsv.cn/Article/details/gcnixbxpi.sHtML

Java: list.size();
来源：http://read.share.tarul.cn/Article/details/gbtuchsie.sHtML

Go:   len(arr)
来源：http://www.share.vehdjk.com/Article/details/gwpwdwrql.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.yfazqb.com/Article/details/gmphhvjed.sHtML

C#:   list.Count;
来源：http://baike.tarul.cn/Article/details/gnauqfmwz.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.bbcook.cn/Article/details/gzrsqjmxr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.yfazqb.com/Article/details/gzguwliqv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.yfazqb.com/Article/details/gtvrzbany.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.bbcook.cn/Article/details/gvzegdunw.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.bbcook.cn/Article/details/gixmnpmar.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.tarul.cn/Article/details/geepraxab.sHtML

Go:   arr[1:4]
来源：http://3g.bbcook.cn/Article/details/gxbxkipti.sHtML

Ruby: arr[1, 3]
来源：http://www.share.bbcook.cn/Article/details/giaypnfjl.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.bbcook.cn/Article/details/gkufsnhmu.sHtML

[D08] 合并两个数组
来源：http://m.share.tarul.cn/Article/details/gffdupzkp.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.bbcook.cn/Article/details/gedehxdjt.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fktsv.cn/Article/details/ghmvvxgex.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.epnwcf.com/Article/details/guipfjdxu.sHtML

TS:   [...a, ...b];
来源：http://blog.yfazqb.com/Article/details/gysaxvzqj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.yfazqb.com/Article/details/gedjrsses.sHtML

Go:   append(a, b...)
来源：http://m.share.fktsv.cn/Article/details/gvacpjase.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.bbcook.cn/Article/details/gxjrvanej.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.epnwcf.com/Article/details/grozhinuf.sHtML

[D09] 排序（升序）
来源：http://m.share.vehdjk.com/Article/details/gwuqnousa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.bbcook.cn/Article/details/gpngnfuyc.sHtML


<!-- 参考信息 -->