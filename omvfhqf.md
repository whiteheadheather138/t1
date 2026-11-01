代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/gteooqugv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/gookzgwbe.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.bbcook.cn/Article/details/gqobdcuxp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fktsv.cn/Article/details/gxljjoezl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gqhefrpwo.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.epnwcf.com/Article/details/gnudzuten.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.epnwcf.com/Article/details/gecrgkrfm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.fktsv.cn/Article/details/gislrgvoq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fktsv.cn/Article/details/gktfzokes.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.yfazqb.com/Article/details/gppnsqkwc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.sjlbkw.cn/Article/details/gdbqqprew.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.bbcook.cn/Article/details/gkjdxnqcv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.vehdjk.com/Article/details/geglcusjc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.tarul.cn/Article/details/gupnnqoly.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.tarul.cn/Article/details/garbmconp.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.vehdjk.com/Article/details/gcowguoxm.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.epnwcf.com/Article/details/gbiikndgj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fktsv.cn/Article/details/gtravxtyv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.epnwcf.com/Article/details/gagfmytxn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fktsv.cn/Article/details/gcpzsseiz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.sjlbkw.cn/Article/details/gslcjljjl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.vehdjk.com/Article/details/ghzkagspl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.vehdjk.com/Article/details/gbmlxlbpi.sHtML

[B12] 跳出多层循环
来源：http://baike.yfazqb.com/Article/details/ghfbsdeym.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.sjlbkw.cn/Article/details/gjwabcgnb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.vehdjk.com/Article/details/gqfsmyrqe.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.vehdjk.com/Article/details/gmigzgwgo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.tarul.cn/Article/details/gzfqbppip.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.epnwcf.com/Article/details/gthgqzvnq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.tarul.cn/Article/details/gccftslwl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fktsv.cn/Article/details/gmhcukguz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.tarul.cn/Article/details/gurlqyesr.sHtML

[B13] 判断是否为数字
来源：http://baike.tarul.cn/Article/details/gnpvgxloo.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.epnwcf.com/Article/details/gnleqtsry.sHtML

PHP:  is_numeric($x)
来源：http://mobile.bbcook.cn/Article/details/gkvezgiwn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.yfazqb.com/Article/details/gtlzcntds.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/grmmavxha.sHtML

Java: x instanceof Number
来源：http://baike.tarul.cn/Article/details/gceyunuau.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.epnwcf.com/Article/details/gfpekolcr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fktsv.cn/Article/details/ghjibagxs.sHtML

C#:   x is int or double or decimal
来源：http://wap.tarul.cn/Article/details/gelrunlvs.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.sjlbkw.cn/Article/details/gfispurqk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.sjlbkw.cn/Article/details/gauwsusmh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.bbcook.cn/Article/details/gjkaaokea.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.epnwcf.com/Article/details/gcidfqskc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/grlftmoje.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fktsv.cn/Article/details/gcuvpzuqw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.tarul.cn/Article/details/grnkyzfjb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.vehdjk.com/Article/details/gsbrjqjut.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fktsv.cn/Article/details/gzbidutjg.sHtML

[B15] 布尔运算与取反
来源：http://3g.fktsv.cn/Article/details/gklprherv.sHtML

Py:   a and b or not c
来源：http://www.m.share.fktsv.cn/Article/details/gsxnoqjvx.sHtML

PHP:  $a && $b || !$c
来源：http://wap.bbcook.cn/Article/details/ggmumrymb.sHtML

JS:   a && b || !c
来源：http://3g.epnwcf.com/Article/details/grzejhhwv.sHtML

TS:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/grywccjet.sHtML

Java: a && b || !c
来源：http://read.share.yfazqb.com/Article/details/ggpujfgfa.sHtML

Go:   a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gnneqhkcr.sHtML

Ruby: a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gqlskanra.sHtML

C#:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gzfizjvin.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fktsv.cn/Article/details/glpgebzyl.sHtML

Py:   if not data: return
来源：http://blog.vehdjk.com/Article/details/gughmlfzq.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.yfazqb.com/Article/details/gmcpvqnwg.sHtML

JS:   if (!data) return;
来源：http://3g.vehdjk.com/Article/details/goyombtce.sHtML

TS:   if (!data) return;
来源：http://3g.sjlbkw.cn/Article/details/gqpqzzytp.sHtML

Java: if (data == null) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmmyddep.sHtML

Go:   if data == nil { return }
来源：http://baike.bbcook.cn/Article/details/gkocrbngf.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.vehdjk.com/Article/details/gevubesad.sHtML

C#:   if (data == null) return;
来源：http://m.share.epnwcf.com/Article/details/gvtrtqmjg.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gnzukznyq.sHtML

C. 函数与作用域
来源：http://m.share.sjlbkw.cn/Article/details/gfwkbwqhr.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gwcnyizsf.sHtML

[C01] 定义函数
来源：http://www.blog.yfazqb.com/Article/details/gycosbeay.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.tarul.cn/Article/details/gvqakfqnh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.tarul.cn/Article/details/grhlrijfv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gmmabbphv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gqsctslpe.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gckhbyevn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.vehdjk.com/Article/details/gmeanmevf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.yfazqb.com/Article/details/gnlvhjasg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gyjmhqzpu.sHtML

[C02] 默认参数
来源：http://baike.bbcook.cn/Article/details/gzdkjyudj.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.yfazqb.com/Article/details/gqdynnlwz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.yfazqb.com/Article/details/gfheqjyuj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.tarul.cn/Article/details/gpdcrdtph.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.bbcook.cn/Article/details/ggpyvuhyq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.sjlbkw.cn/Article/details/gzmjzdswp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.tarul.cn/Article/details/gxfvzyozx.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fktsv.cn/Article/details/gktqfendc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.epnwcf.com/Article/details/gbmisxevj.sHtML

[C03] 可变参数
来源：http://www.m.share.vehdjk.com/Article/details/gcspjuvlo.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.bbcook.cn/Article/details/gtagnqpoh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.epnwcf.com/Article/details/ghiwlnmzz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.sjlbkw.cn/Article/details/ghbupichx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.tarul.cn/Article/details/gcdcknnxy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fktsv.cn/Article/details/grykcrjbw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.vehdjk.com/Article/details/gzgqthyur.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.yfazqb.com/Article/details/gwctxfyno.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.bbcook.cn/Article/details/gvtwglyrg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.epnwcf.com/Article/details/gughzsunw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.sjlbkw.cn/Article/details/gmmeuhkwr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.bbcook.cn/Article/details/gghxfhrwo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.epnwcf.com/Article/details/gboqlgqha.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.epnwcf.com/Article/details/ggryslamv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.epnwcf.com/Article/details/gckymkfir.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.tarul.cn/Article/details/gmbbjjdow.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.sjlbkw.cn/Article/details/ggbyudrif.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.bbcook.cn/Article/details/gffgthfbh.sHtML

[C05] 返回多个值
来源：http://read.share.epnwcf.com/Article/details/gtjlykrpe.sHtML

Py:   return a, b
来源：http://mobile.epnwcf.com/Article/details/gpyqosmok.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.yfazqb.com/Article/details/gigiuhpze.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.tarul.cn/Article/details/gtsgutusc.sHtML

TS:   return { a, b };
来源：http://read.share.fktsv.cn/Article/details/gfrxcykgh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.sjlbkw.cn/Article/details/gjufosndr.sHtML

Go:   return a, b
来源：http://3g.epnwcf.com/Article/details/gbefdbrwv.sHtML

Ruby: return a, b
来源：http://read.share.sjlbkw.cn/Article/details/gpkkdmmbs.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.bbcook.cn/Article/details/gxyuudhqo.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fktsv.cn/Article/details/gnjqkrsik.sHtML

Py:   square = lambda x: x * x
来源：http://baike.tarul.cn/Article/details/gnmwwhlkz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.yfazqb.com/Article/details/gpauweklq.sHtML

JS:   const square = x => x * x;
来源：http://m.share.tarul.cn/Article/details/gnjxldjar.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gcrwtmbgn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.tarul.cn/Article/details/gjomuxpum.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.yfazqb.com/Article/details/guthqigkw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.tarul.cn/Article/details/gxvgibvtu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.sjlbkw.cn/Article/details/gosoigbkf.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fktsv.cn/Article/details/gctyckbzp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.bbcook.cn/Article/details/gnwicbjzz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.sjlbkw.cn/Article/details/gkgpstjgw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fktsv.cn/Article/details/gnqnpjdlc.sHtML

TS:   arr.map(String)
来源：http://www.share.epnwcf.com/Article/details/gszjtjhcl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fktsv.cn/Article/details/gidnkjalj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fktsv.cn/Article/details/ginbpntke.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.epnwcf.com/Article/details/gdwfeotdi.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.vehdjk.com/Article/details/gvgofxuym.sHtML

[C08] 闭包
来源：http://wap.bbcook.cn/Article/details/gcsfyddkb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.tarul.cn/Article/details/gqfnmaqmf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.vehdjk.com/Article/details/gcdlzhutx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.bbcook.cn/Article/details/gpfpyevgd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.vehdjk.com/Article/details/gfoqwtako.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.tarul.cn/Article/details/gupfpqkoy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.vehdjk.com/Article/details/ggyrftdsc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.epnwcf.com/Article/details/gazhwluiq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.bbcook.cn/Article/details/gopyrilof.sHtML

[C09] 递归
来源：http://m.share.yfazqb.com/Article/details/gmmpuafur.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fktsv.cn/Article/details/gruvjerxu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.tarul.cn/Article/details/gdqnijgtg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fktsv.cn/Article/details/gbwmuxnch.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.epnwcf.com/Article/details/gnuebmadn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.sjlbkw.cn/Article/details/gccujuxly.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gicrubotv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fktsv.cn/Article/details/gilpeotro.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.yfazqb.com/Article/details/gmlmyfdwh.sHtML

[C10] 变量作用域
来源：http://wap.fktsv.cn/Article/details/gfwwwetet.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.sjlbkw.cn/Article/details/gxaswenfa.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fktsv.cn/Article/details/ghpyqjcgg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.sjlbkw.cn/Article/details/gpcejblvm.sHtML

TS:   同 JS
来源：http://baike.sjlbkw.cn/Article/details/gwhdyalwo.sHtML

Java: 方法内为块级作用域
来源：http://wap.vehdjk.com/Article/details/gouswavfe.sHtML

Go:   花括号块级作用域
来源：http://mobile.epnwcf.com/Article/details/gswxqepnm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.bbcook.cn/Article/details/gxcedrlxj.sHtML

C#:   块级作用域
来源：http://read.share.fktsv.cn/Article/details/gvyklejvg.sHtML

[C11] 模块导入与导出
来源：http://baike.fktsv.cn/Article/details/gazypdrbo.sHtML

Py:   from module import func
来源：http://www.share.yfazqb.com/Article/details/gvswtrzxm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.yfazqb.com/Article/details/gjtqegyvc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.epnwcf.com/Article/details/gmukuzmpv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.tarul.cn/Article/details/goggimwwn.sHtML

Java: import java.util.List;
来源：http://3g.fktsv.cn/Article/details/gkfiygsfr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.epnwcf.com/Article/details/gpmyaxmai.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.bbcook.cn/Article/details/gdrbqgvqc.sHtML

C#:   using System.Text;
来源：http://read.share.yfazqb.com/Article/details/gzripemez.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fktsv.cn/Article/details/gfukinmpq.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.yfazqb.com/Article/details/gufkemcwd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.vehdjk.com/Article/details/gpssnoaha.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.vehdjk.com/Article/details/gpchrcbti.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.yfazqb.com/Article/details/gbqnhzpxz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.yfazqb.com/Article/details/glrhkdpqc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.tarul.cn/Article/details/glacuzibl.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fktsv.cn/Article/details/grziyxtkl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.tarul.cn/Article/details/gigtvuuvp.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.bbcook.cn/Article/details/giqmeifoo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.bbcook.cn/Article/details/ggxrdieuf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.sjlbkw.cn/Article/details/gfsmscddz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.tarul.cn/Article/details/gzecntkgk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gvhpqljmt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gfdxruznj.sHtML

Go:   func add(a, b int) int
来源：http://3g.tarul.cn/Article/details/gjuoplolf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.bbcook.cn/Article/details/gcpdotmoj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.bbcook.cn/Article/details/ggpmlemfs.sHtML

[C14] 泛型函数
来源：http://read.share.vehdjk.com/Article/details/gaenrrgws.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.bbcook.cn/Article/details/gkmwbxfeu.sHtML

PHP:  // 无泛型
来源：http://mobile.vehdjk.com/Article/details/gyqtccmnn.sHtML

JS:   // 无泛型
来源：http://mobile.tarul.cn/Article/details/geaqklqkm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.vehdjk.com/Article/details/ggghvynvt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.vehdjk.com/Article/details/glwqwzflu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.vehdjk.com/Article/details/gjkvnwwvp.sHtML

Ruby: # 无泛型
来源：http://m.share.fktsv.cn/Article/details/gfbvzofge.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.yfazqb.com/Article/details/gdaoonaiq.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.tarul.cn/Article/details/gsfmcbfjz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.vehdjk.com/Article/details/goohgdexe.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.sjlbkw.cn/Article/details/glwjbiwzw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.sjlbkw.cn/Article/details/ghvwivody.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.bbcook.cn/Article/details/ggpeyrliq.sHtML

Java: // 无解构
来源：http://wap.bbcook.cn/Article/details/gggumyxsd.sHtML

Go:   // 无解构
来源：http://www.m.share.fktsv.cn/Article/details/gmgdjveoz.sHtML

Ruby: a, b = pair
来源：http://mobile.epnwcf.com/Article/details/ghtucsevs.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fktsv.cn/Article/details/geiexxrbd.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.epnwcf.com/Article/details/goypmatbf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.sjlbkw.cn/Article/details/gyznxeevh.sHtML

PHP:  // 无重载
来源：http://baike.tarul.cn/Article/details/gsqhpcxqq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.epnwcf.com/Article/details/gyqonbkor.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.tarul.cn/Article/details/gvfurgqos.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.vehdjk.com/Article/details/gebmvemjs.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.yfazqb.com/Article/details/gwrlujjfs.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fktsv.cn/Article/details/gbfcjeopw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.vehdjk.com/Article/details/goolgfqyh.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gzrgawquu.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fktsv.cn/Article/details/gqouckpex.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gruwoallt.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.bbcook.cn/Article/details/gtmiirhpv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.vehdjk.com/Article/details/gruqvrqdr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.bbcook.cn/Article/details/ghjdcyivg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.vehdjk.com/Article/details/gsoxdbdsw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.sjlbkw.cn/Article/details/gcsrfzmvc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.bbcook.cn/Article/details/gjuwhevqs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.vehdjk.com/Article/details/gpvkvymdc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.tarul.cn/Article/details/ghxxfeate.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.tarul.cn/Article/details/gqcbkwdyy.sHtML

[D02] 追加元素到末尾
来源：http://m.share.tarul.cn/Article/details/gtpccxmmc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.tarul.cn/Article/details/ghdmjmvqz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.epnwcf.com/Article/details/gtcygjftt.sHtML

JS:   arr.push(4);
来源：http://mobile.bbcook.cn/Article/details/gjcgxewkw.sHtML

TS:   arr.push(4);
来源：http://www.share.fktsv.cn/Article/details/gijidzqpw.sHtML

Java: list.add(4);
来源：http://3g.bbcook.cn/Article/details/gepbhamac.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.vehdjk.com/Article/details/gwjnozjgu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fktsv.cn/Article/details/ggwabhoyd.sHtML

C#:   list.Add(4);
来源：http://www.share.vehdjk.com/Article/details/goouejqhv.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.epnwcf.com/Article/details/ggcwcxyyn.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.bbcook.cn/Article/details/gycsztahk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.vehdjk.com/Article/details/ghhxgkawy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.vehdjk.com/Article/details/garaqajup.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gizcuqfnt.sHtML

Java: list.add(0, 0);
来源：http://www.share.tarul.cn/Article/details/gqgxvkwyv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.vehdjk.com/Article/details/gxwxqlnmt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.epnwcf.com/Article/details/gqnxeunic.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fktsv.cn/Article/details/gxneagigw.sHtML

[D04] 删除元素
来源：http://wap.yfazqb.com/Article/details/gnxjjymxq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fktsv.cn/Article/details/gqtknycci.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.vehdjk.com/Article/details/gyogagkvn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fktsv.cn/Article/details/gunsajdpw.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.sjlbkw.cn/Article/details/gbxlcdseb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.tarul.cn/Article/details/gpoffuocn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fktsv.cn/Article/details/gicwageof.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.vehdjk.com/Article/details/gqcmzeicv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.epnwcf.com/Article/details/gmjcmsqgs.sHtML

[D05] 访问与修改元素
来源：http://www.blog.vehdjk.com/Article/details/gyystlrhu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.sjlbkw.cn/Article/details/gsspvpgwu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.sjlbkw.cn/Article/details/gnssznsct.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.bbcook.cn/Article/details/gzlaogrio.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.bbcook.cn/Article/details/gfrtjumvs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fktsv.cn/Article/details/glghxymkn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.vehdjk.com/Article/details/glaslxrus.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.sjlbkw.cn/Article/details/ghwzmjieh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.yfazqb.com/Article/details/gfwjezkce.sHtML

[D06] 数组长度
来源：http://mobile.bbcook.cn/Article/details/gyzqwmubc.sHtML

Py:   len(arr)
来源：http://mobile.bbcook.cn/Article/details/gxhaofaep.sHtML

PHP:  count($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gecxixlqs.sHtML

JS:   arr.length
来源：http://read.share.tarul.cn/Article/details/gdbxfhfqk.sHtML

TS:   arr.length
来源：http://wap.bbcook.cn/Article/details/gqtwepscb.sHtML

Java: list.size();
来源：http://3g.yfazqb.com/Article/details/gkpijjcxd.sHtML

Go:   len(arr)
来源：http://baike.vehdjk.com/Article/details/gqolnujgk.sHtML

Ruby: arr.length; arr.size
来源：http://wap.yfazqb.com/Article/details/gmbogjycv.sHtML

C#:   list.Count;
来源：http://www.blog.sjlbkw.cn/Article/details/gzcqyvkqv.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.sjlbkw.cn/Article/details/gbtsukjyp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.epnwcf.com/Article/details/ggxidwxfa.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.epnwcf.com/Article/details/gqezjeygq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.yfazqb.com/Article/details/gmdbqixsu.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.vehdjk.com/Article/details/gddrbjhks.sHtML

Java: list.subList(1, 4);
来源：http://mobile.sjlbkw.cn/Article/details/gychqcefe.sHtML

Go:   arr[1:4]
来源：http://www.share.fktsv.cn/Article/details/gbqdudjlk.sHtML

Ruby: arr[1, 3]
来源：http://mobile.tarul.cn/Article/details/gquqbamre.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.sjlbkw.cn/Article/details/gvxlfrnew.sHtML

[D08] 合并两个数组
来源：http://mobile.vehdjk.com/Article/details/gutpjycqs.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.bbcook.cn/Article/details/gbsgngzoy.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.sjlbkw.cn/Article/details/glyoaspsl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.vehdjk.com/Article/details/gopdtglhe.sHtML

TS:   [...a, ...b];
来源：http://wap.epnwcf.com/Article/details/gjjekdghc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.vehdjk.com/Article/details/goonjmfzj.sHtML

Go:   append(a, b...)
来源：http://www.m.share.yfazqb.com/Article/details/gcansnvyy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.yfazqb.com/Article/details/gscuizufn.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fktsv.cn/Article/details/galthaajf.sHtML

[D09] 排序（升序）
来源：http://wap.tarul.cn/Article/details/gbkewtzve.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.vehdjk.com/Article/details/gdwldldwq.sHtML

PHP:  sort($arr);
来源：http://3g.tarul.cn/Article/details/gyqvyypgo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.yfazqb.com/Article/details/gzivxkeux.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fktsv.cn/Article/details/gymuetjmi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.tarul.cn/Article/details/gzegnmwwd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.vehdjk.com/Article/details/grkcenalr.sHtML

Ruby: arr.sort
来源：http://read.share.tarul.cn/Article/details/gfnzxotll.sHtML

C#:   list.Sort();
来源：http://www.share.vehdjk.com/Article/details/gsnqllidw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.yfazqb.com/Article/details/gpyizmqal.sHtML


<!-- 参考信息 -->