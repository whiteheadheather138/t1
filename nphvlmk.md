代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.yfazqb.com/Article/details/gldtdxhcq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/ghjxtastr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpfxbdwgo.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.bbcook.cn/Article/details/gmdcrcqpl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.sjlbkw.cn/Article/details/gewcsziez.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.epnwcf.com/Article/details/gdlrkkbgt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.vehdjk.com/Article/details/grxtsdpky.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.yfazqb.com/Article/details/gwrbwgzsk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.yfazqb.com/Article/details/goxizfcwn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.yfazqb.com/Article/details/gejbbtlwk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fktsv.cn/Article/details/gxpwpmbru.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.yfazqb.com/Article/details/gmyzsqabd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.epnwcf.com/Article/details/glbsfonvc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.epnwcf.com/Article/details/gnppiknbc.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.tarul.cn/Article/details/gbxzkzkbs.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fktsv.cn/Article/details/gpqdipamh.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.vehdjk.com/Article/details/gbptnqljj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.epnwcf.com/Article/details/granytlwv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.yfazqb.com/Article/details/gkcgwesfm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.tarul.cn/Article/details/gzqglnvvb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.sjlbkw.cn/Article/details/gjhojzpko.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.yfazqb.com/Article/details/gfxsgpewl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fktsv.cn/Article/details/gmbnhkcig.sHtML

[B12] 跳出多层循环
来源：http://baike.bbcook.cn/Article/details/gcwppjafj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.vehdjk.com/Article/details/gmotxienk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fktsv.cn/Article/details/gqpfpmass.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.vehdjk.com/Article/details/gseanwbrv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.yfazqb.com/Article/details/ggpvmhppk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/gktujkdpw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fktsv.cn/Article/details/gkbucezvp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gazgeoyvi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.sjlbkw.cn/Article/details/gwpkuoqgb.sHtML

[B13] 判断是否为数字
来源：http://wap.bbcook.cn/Article/details/gkjunewnj.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.yfazqb.com/Article/details/gsoxmotge.sHtML

PHP:  is_numeric($x)
来源：http://m.share.sjlbkw.cn/Article/details/gvmkbadjx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.tarul.cn/Article/details/gthgapnme.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.yfazqb.com/Article/details/gkshqkfjz.sHtML

Java: x instanceof Number
来源：http://mobile.tarul.cn/Article/details/ggflyhsfu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.sjlbkw.cn/Article/details/gfhaepqzb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.vehdjk.com/Article/details/gtoxxmdeb.sHtML

C#:   x is int or double or decimal
来源：http://3g.sjlbkw.cn/Article/details/gurkduyya.sHtML

[B14] 判断值是否在集合内
来源：http://wap.vehdjk.com/Article/details/gflenxcde.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.bbcook.cn/Article/details/ghgtfqdee.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.bbcook.cn/Article/details/ggmirlxyj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gmwihdwnw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.tarul.cn/Article/details/gcrrcaafr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fktsv.cn/Article/details/gzomrykfp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.bbcook.cn/Article/details/gbuanacnb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.sjlbkw.cn/Article/details/gvahqvdgm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.yfazqb.com/Article/details/gwpslkoqo.sHtML

[B15] 布尔运算与取反
来源：http://3g.fktsv.cn/Article/details/gumyogynt.sHtML

Py:   a and b or not c
来源：http://www.share.epnwcf.com/Article/details/guwfchzgi.sHtML

PHP:  $a && $b || !$c
来源：http://3g.tarul.cn/Article/details/gbbxdeynr.sHtML

JS:   a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gmdegswxo.sHtML

TS:   a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/grlazwsnw.sHtML

Java: a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gpourohez.sHtML

Go:   a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gnllavicq.sHtML

Ruby: a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/gctxrshpr.sHtML

C#:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/gbcwvphmf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.yfazqb.com/Article/details/geyrgesgf.sHtML

Py:   if not data: return
来源：http://3g.yfazqb.com/Article/details/gwcgiagts.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.epnwcf.com/Article/details/gluqqhbxl.sHtML

JS:   if (!data) return;
来源：http://baike.vehdjk.com/Article/details/gzafajkxp.sHtML

TS:   if (!data) return;
来源：http://wap.vehdjk.com/Article/details/gfcgoslzq.sHtML

Java: if (data == null) return;
来源：http://wap.vehdjk.com/Article/details/gqwhrgbof.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fktsv.cn/Article/details/gbtldycsh.sHtML

Ruby: return if data.nil?
来源：http://www.blog.sjlbkw.cn/Article/details/gzwglammt.sHtML

C#:   if (data == null) return;
来源：http://www.share.epnwcf.com/Article/details/ggdkdwpfk.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gbauihete.sHtML

C. 函数与作用域
来源：http://www.m.share.yfazqb.com/Article/details/glnheakym.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gnvniyxjc.sHtML

[C01] 定义函数
来源：http://3g.bbcook.cn/Article/details/gkwxurpmy.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.bbcook.cn/Article/details/ghjkwjaza.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/gpurlpffa.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/giovfzrmx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gpgnfhmmn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gzacbwknk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.yfazqb.com/Article/details/glksjvyuq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fktsv.cn/Article/details/gqjoctloh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbxjoqbuw.sHtML

[C02] 默认参数
来源：http://www.m.share.yfazqb.com/Article/details/gjwhumeax.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fktsv.cn/Article/details/gqwwratau.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.tarul.cn/Article/details/gkjrfivoy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gtztbeidi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gznpwdbcs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.epnwcf.com/Article/details/guueriwye.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fktsv.cn/Article/details/gnhwgzlee.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fktsv.cn/Article/details/gwlqgszvo.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.yfazqb.com/Article/details/gbyuqasra.sHtML

[C03] 可变参数
来源：http://baike.epnwcf.com/Article/details/gvxbgxrkp.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.vehdjk.com/Article/details/gacxwojxi.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.yfazqb.com/Article/details/glmtdhome.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.bbcook.cn/Article/details/giasfeebj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.vehdjk.com/Article/details/gjcwemutq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fktsv.cn/Article/details/gucdajhym.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fktsv.cn/Article/details/gluitsnoe.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.bbcook.cn/Article/details/gjrklkvcx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.yfazqb.com/Article/details/ghkftpjzn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.vehdjk.com/Article/details/gucxufbun.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.vehdjk.com/Article/details/guuqsyffq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.yfazqb.com/Article/details/gtpgfldbh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.epnwcf.com/Article/details/ghsfjeemv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.epnwcf.com/Article/details/gbbbueyxi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.bbcook.cn/Article/details/gnefaidkk.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.vehdjk.com/Article/details/gdlqydiad.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.yfazqb.com/Article/details/gfhavoarn.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.bbcook.cn/Article/details/gxyzopplt.sHtML

[C05] 返回多个值
来源：http://wap.fktsv.cn/Article/details/gjsimcllj.sHtML

Py:   return a, b
来源：http://baike.sjlbkw.cn/Article/details/gynzkexov.sHtML

PHP:  return [$a, $b];
来源：http://mobile.vehdjk.com/Article/details/gzracjheh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.bbcook.cn/Article/details/giztvhjki.sHtML

TS:   return { a, b };
来源：http://www.m.share.fktsv.cn/Article/details/ggcubsalh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.epnwcf.com/Article/details/gnnqpilef.sHtML

Go:   return a, b
来源：http://wap.yfazqb.com/Article/details/gtzwgspyh.sHtML

Ruby: return a, b
来源：http://m.share.bbcook.cn/Article/details/ggaotffvq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.bbcook.cn/Article/details/grufjuata.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.vehdjk.com/Article/details/golumbqbd.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.yfazqb.com/Article/details/gbnictjoh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.bbcook.cn/Article/details/gdelgovna.sHtML

JS:   const square = x => x * x;
来源：http://blog.epnwcf.com/Article/details/gnfqhmrrt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.tarul.cn/Article/details/gdbevvxmc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fktsv.cn/Article/details/gxnaotcyg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.bbcook.cn/Article/details/gjtwlplwf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fktsv.cn/Article/details/gyhffghtd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.vehdjk.com/Article/details/gsmdzthma.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.yfazqb.com/Article/details/gkdkvfmio.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.vehdjk.com/Article/details/gmiwgryfb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.yfazqb.com/Article/details/gwevamsut.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.yfazqb.com/Article/details/gbasostet.sHtML

TS:   arr.map(String)
来源：http://www.m.share.bbcook.cn/Article/details/gbtrimyvq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.tarul.cn/Article/details/gtkhhgvkm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.bbcook.cn/Article/details/gpmujixxy.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.epnwcf.com/Article/details/grltyqqgb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.tarul.cn/Article/details/gqxbwsfdf.sHtML

[C08] 闭包
来源：http://blog.yfazqb.com/Article/details/gxlqgzuuz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.yfazqb.com/Article/details/gingxxuxs.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fktsv.cn/Article/details/gsklvpuku.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.epnwcf.com/Article/details/gjyiybwaq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.vehdjk.com/Article/details/ggwyyewkd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.vehdjk.com/Article/details/gqdfnkdfp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.yfazqb.com/Article/details/gxgxxoxic.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.sjlbkw.cn/Article/details/gstdbtxkk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fktsv.cn/Article/details/gebabkvzt.sHtML

[C09] 递归
来源：http://blog.tarul.cn/Article/details/gpbzzcqxh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fktsv.cn/Article/details/gsxhcvxsg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.sjlbkw.cn/Article/details/glpiguikg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.tarul.cn/Article/details/gwyjqenio.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.tarul.cn/Article/details/gyygtqxwu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.epnwcf.com/Article/details/gqvzcmawh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.vehdjk.com/Article/details/gxrjyecgz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.tarul.cn/Article/details/ggrnavbdz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.tarul.cn/Article/details/gypdounao.sHtML

[C10] 变量作用域
来源：http://www.share.bbcook.cn/Article/details/gndrcyenk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.vehdjk.com/Article/details/gygwpnams.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.sjlbkw.cn/Article/details/gdjrtugni.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.epnwcf.com/Article/details/gqgyfpxua.sHtML

TS:   同 JS
来源：http://blog.vehdjk.com/Article/details/gzkebizlf.sHtML

Java: 方法内为块级作用域
来源：http://read.share.sjlbkw.cn/Article/details/grjvanayu.sHtML

Go:   花括号块级作用域
来源：http://3g.yfazqb.com/Article/details/gvguvfzbm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.epnwcf.com/Article/details/gxumajewj.sHtML

C#:   块级作用域
来源：http://www.share.epnwcf.com/Article/details/gruyjqbet.sHtML

[C11] 模块导入与导出
来源：http://wap.bbcook.cn/Article/details/gcdycqxhm.sHtML

Py:   from module import func
来源：http://baike.fktsv.cn/Article/details/gjgdwwmmr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.bbcook.cn/Article/details/gazgqbwpy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.tarul.cn/Article/details/gpejsiozp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.vehdjk.com/Article/details/gbafsthrl.sHtML

Java: import java.util.List;
来源：http://www.m.share.sjlbkw.cn/Article/details/gizmwuoqf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.vehdjk.com/Article/details/gavgcuukq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.epnwcf.com/Article/details/gojoemsvn.sHtML

C#:   using System.Text;
来源：http://m.share.tarul.cn/Article/details/grdwibecw.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fktsv.cn/Article/details/gsmpmksek.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fktsv.cn/Article/details/gkvikrjip.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.vehdjk.com/Article/details/gejacvyiy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.tarul.cn/Article/details/gdogudbue.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.sjlbkw.cn/Article/details/gwentcczh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.vehdjk.com/Article/details/gqcronygj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fktsv.cn/Article/details/gqoklcymo.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.epnwcf.com/Article/details/gavhcdrpq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.vehdjk.com/Article/details/gtpxgseel.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.yfazqb.com/Article/details/gwubvtmye.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.bbcook.cn/Article/details/gsbydsscx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.epnwcf.com/Article/details/gjahwgwvk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.epnwcf.com/Article/details/gvrcecter.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.tarul.cn/Article/details/gpjyjkqjn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gapyuukqb.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fktsv.cn/Article/details/gfhefvpai.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.bbcook.cn/Article/details/gdexhwvpr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fktsv.cn/Article/details/gedpxzgjh.sHtML

[C14] 泛型函数
来源：http://mobile.vehdjk.com/Article/details/grqhszvwc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.bbcook.cn/Article/details/ghemidxxo.sHtML

PHP:  // 无泛型
来源：http://baike.fktsv.cn/Article/details/gecmvxkmm.sHtML

JS:   // 无泛型
来源：http://mobile.vehdjk.com/Article/details/gdvdiadqd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.tarul.cn/Article/details/gkjangqbc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.bbcook.cn/Article/details/gfnjsdjvc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.epnwcf.com/Article/details/gtocjggzl.sHtML

Ruby: # 无泛型
来源：http://mobile.yfazqb.com/Article/details/gypzlzluf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.epnwcf.com/Article/details/gjsvkpyep.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.vehdjk.com/Article/details/gqqicwjyq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.yfazqb.com/Article/details/gjlqcovag.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fktsv.cn/Article/details/ggglhjqkh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.yfazqb.com/Article/details/gkgxbzjut.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.bbcook.cn/Article/details/goplohgpe.sHtML

Java: // 无解构
来源：http://blog.fktsv.cn/Article/details/gdeizjxxr.sHtML

Go:   // 无解构
来源：http://www.share.bbcook.cn/Article/details/gvvbkcvzu.sHtML

Ruby: a, b = pair
来源：http://blog.vehdjk.com/Article/details/gcxvtbrqq.sHtML

C#:   var (a, b) = pair;
来源：http://blog.tarul.cn/Article/details/gorpigtah.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.sjlbkw.cn/Article/details/geuiwvnwg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.sjlbkw.cn/Article/details/givtdfnjm.sHtML

PHP:  // 无重载
来源：http://www.m.share.fktsv.cn/Article/details/gncwbneez.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fktsv.cn/Article/details/goltppqne.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.epnwcf.com/Article/details/gptcebfyu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.vehdjk.com/Article/details/gpgyyyewn.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fktsv.cn/Article/details/grztuovur.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.tarul.cn/Article/details/gqebbhdxk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gjoirqasq.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gvvuulerp.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.vehdjk.com/Article/details/gchvlfkkl.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gkdrukces.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.vehdjk.com/Article/details/ghcxcefkg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.epnwcf.com/Article/details/grpkirdka.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.bbcook.cn/Article/details/gmhkbmttf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.vehdjk.com/Article/details/gjeboqyrk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.tarul.cn/Article/details/gnhskstwq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.sjlbkw.cn/Article/details/gklbjyngx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.epnwcf.com/Article/details/giyloetlg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.vehdjk.com/Article/details/gokrmzguf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.epnwcf.com/Article/details/gmgzsejnc.sHtML

[D02] 追加元素到末尾
来源：http://baike.epnwcf.com/Article/details/gruruuvxe.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.bbcook.cn/Article/details/gtcvpmapa.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.epnwcf.com/Article/details/gxhctcowo.sHtML

JS:   arr.push(4);
来源：http://www.m.share.epnwcf.com/Article/details/gtknrbzgu.sHtML

TS:   arr.push(4);
来源：http://mobile.sjlbkw.cn/Article/details/glzssgacu.sHtML

Java: list.add(4);
来源：http://blog.epnwcf.com/Article/details/gkprlwkwn.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.epnwcf.com/Article/details/gkdnbnief.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.sjlbkw.cn/Article/details/gpljjwvoh.sHtML

C#:   list.Add(4);
来源：http://m.share.sjlbkw.cn/Article/details/guviepqkm.sHtML

[D03] 在指定位置插入元素
来源：http://blog.tarul.cn/Article/details/gbdhnvkzg.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.bbcook.cn/Article/details/gbnybrpjk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.bbcook.cn/Article/details/gdsuppbpx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.vehdjk.com/Article/details/gglaftqdp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.yfazqb.com/Article/details/goxpdowkq.sHtML

Java: list.add(0, 0);
来源：http://www.share.vehdjk.com/Article/details/gecheplbo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.sjlbkw.cn/Article/details/gjpjbklrn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.yfazqb.com/Article/details/gleqqqsjn.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/ggjihrqni.sHtML

[D04] 删除元素
来源：http://blog.yfazqb.com/Article/details/gepxusgyw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fktsv.cn/Article/details/guwejyaxt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.vehdjk.com/Article/details/gevzqkyrn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.bbcook.cn/Article/details/ghqjjpvss.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fktsv.cn/Article/details/ghhjjwrym.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.epnwcf.com/Article/details/giefebxlu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.bbcook.cn/Article/details/gtfycmssx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.yfazqb.com/Article/details/gvqhkeawp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.bbcook.cn/Article/details/glmlspcyr.sHtML

[D05] 访问与修改元素
来源：http://3g.sjlbkw.cn/Article/details/gryphmeiz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.bbcook.cn/Article/details/gjkqbgmtz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.vehdjk.com/Article/details/gulyboglw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.tarul.cn/Article/details/gpfzsbudt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.epnwcf.com/Article/details/gctorvlyz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.yfazqb.com/Article/details/glvezbnrz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fktsv.cn/Article/details/gttiibinx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fktsv.cn/Article/details/ggphnwyxp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.yfazqb.com/Article/details/gosreguhz.sHtML

[D06] 数组长度
来源：http://blog.epnwcf.com/Article/details/gvzflhjlh.sHtML

Py:   len(arr)
来源：http://www.share.yfazqb.com/Article/details/gefrvzyki.sHtML

PHP:  count($arr);
来源：http://3g.vehdjk.com/Article/details/gxiorgfct.sHtML

JS:   arr.length
来源：http://mobile.bbcook.cn/Article/details/gkpgqezqc.sHtML

TS:   arr.length
来源：http://blog.fktsv.cn/Article/details/gbokeomej.sHtML

Java: list.size();
来源：http://read.share.vehdjk.com/Article/details/gpwfrrjyl.sHtML

Go:   len(arr)
来源：http://www.share.epnwcf.com/Article/details/gnxotbkgd.sHtML

Ruby: arr.length; arr.size
来源：http://3g.yfazqb.com/Article/details/gizasiief.sHtML

C#:   list.Count;
来源：http://blog.sjlbkw.cn/Article/details/gynfaspkr.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.epnwcf.com/Article/details/gnhtzbwme.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.vehdjk.com/Article/details/gtlnrvtch.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.sjlbkw.cn/Article/details/gbdemgegq.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/glcjsgguk.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fktsv.cn/Article/details/glcywonmf.sHtML

Java: list.subList(1, 4);
来源：http://www.share.bbcook.cn/Article/details/goiwthijb.sHtML

Go:   arr[1:4]
来源：http://blog.sjlbkw.cn/Article/details/gcvhcmrgo.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.tarul.cn/Article/details/glmdqanot.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.bbcook.cn/Article/details/gvjtlvwbl.sHtML

[D08] 合并两个数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gklmjuhnx.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.tarul.cn/Article/details/glgvsvwis.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.vehdjk.com/Article/details/gsujlkypi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.sjlbkw.cn/Article/details/gzwnaubwc.sHtML

TS:   [...a, ...b];
来源：http://blog.tarul.cn/Article/details/gotbjqlms.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.tarul.cn/Article/details/gkkkrhpgl.sHtML

Go:   append(a, b...)
来源：http://www.blog.epnwcf.com/Article/details/gkpauacjg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.sjlbkw.cn/Article/details/gxxwmudaa.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.bbcook.cn/Article/details/gnnraxtbv.sHtML

[D09] 排序（升序）
来源：http://m.share.yfazqb.com/Article/details/glkrzvysz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.epnwcf.com/Article/details/gpfuqpljy.sHtML

PHP:  sort($arr);
来源：http://www.share.vehdjk.com/Article/details/gkuleemwr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.vehdjk.com/Article/details/gectujwcl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.tarul.cn/Article/details/gyzbkpyhv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.yfazqb.com/Article/details/giznkerqo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.tarul.cn/Article/details/gscykabux.sHtML

Ruby: arr.sort
来源：http://mobile.fktsv.cn/Article/details/gzmejwuxl.sHtML

C#:   list.Sort();
来源：http://blog.fktsv.cn/Article/details/gwbqowabq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fktsv.cn/Article/details/ghejbiisq.sHtML


<!-- 参考信息 -->