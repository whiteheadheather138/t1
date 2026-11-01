代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/gjwcyqzqh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.epnwcf.com/Article/details/gycpnedvi.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.vehdjk.com/Article/details/gwlagtdrg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.bbcook.cn/Article/details/glquvxydr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/gqxkfrilk.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxbxxgok.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.yfazqb.com/Article/details/grojhojqx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.sjlbkw.cn/Article/details/gfmlrktyh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.yfazqb.com/Article/details/geoykisho.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.vehdjk.com/Article/details/gltgwxppe.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gopbfwuiy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.tarul.cn/Article/details/gkkpsgcih.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.yfazqb.com/Article/details/gcqwxsbbv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.yfazqb.com/Article/details/gfhftzucq.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.sjlbkw.cn/Article/details/gtnzrfeij.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.bbcook.cn/Article/details/gobcdsohs.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fktsv.cn/Article/details/gknqpizyl.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.vehdjk.com/Article/details/gzsfcgldm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.yfazqb.com/Article/details/glvjnmcro.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.tarul.cn/Article/details/glpcrvczw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.bbcook.cn/Article/details/gaxgranmj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.vehdjk.com/Article/details/gdcrxqxzh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.bbcook.cn/Article/details/gijsgkgog.sHtML

[B12] 跳出多层循环
来源：http://www.share.fktsv.cn/Article/details/gcdallpcx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.yfazqb.com/Article/details/gggcdnfsb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.epnwcf.com/Article/details/ggwjmjhrm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.epnwcf.com/Article/details/grghdkjlt.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.epnwcf.com/Article/details/gbsrqbtmc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fktsv.cn/Article/details/gelfytprl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fktsv.cn/Article/details/gyebytfqv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.vehdjk.com/Article/details/grtgfujqh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.yfazqb.com/Article/details/gqmjztpum.sHtML

[B13] 判断是否为数字
来源：http://www.share.tarul.cn/Article/details/gzopwmope.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.epnwcf.com/Article/details/gcpkwcwac.sHtML

PHP:  is_numeric($x)
来源：http://blog.vehdjk.com/Article/details/gpmxqktiz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.bbcook.cn/Article/details/gyhmwqrbd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.yfazqb.com/Article/details/ghjysdsri.sHtML

Java: x instanceof Number
来源：http://www.m.share.yfazqb.com/Article/details/gjwxefasc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.epnwcf.com/Article/details/gpydrhfuc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.vehdjk.com/Article/details/ggkmmjvsq.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.yfazqb.com/Article/details/gbzoigfqv.sHtML

[B14] 判断值是否在集合内
来源：http://wap.yfazqb.com/Article/details/gqfjbuozx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.epnwcf.com/Article/details/ghrwdslgp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.bbcook.cn/Article/details/gnslizwzv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fktsv.cn/Article/details/gjaciqldc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fktsv.cn/Article/details/gjxrmknyr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.yfazqb.com/Article/details/gisuhuwnu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.bbcook.cn/Article/details/gvhbrrwjd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.sjlbkw.cn/Article/details/gkwrnytqx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.tarul.cn/Article/details/gbelvzfkn.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fktsv.cn/Article/details/gztmkdioh.sHtML

Py:   a and b or not c
来源：http://m.share.sjlbkw.cn/Article/details/gsnylvdyj.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.sjlbkw.cn/Article/details/gjkjluatt.sHtML

JS:   a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gghupylvf.sHtML

TS:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gcjzldwdg.sHtML

Java: a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gahftswrj.sHtML

Go:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gwbggkxlo.sHtML

Ruby: a && b || !c
来源：http://3g.fktsv.cn/Article/details/gawaotsqk.sHtML

C#:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gvbombodt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.tarul.cn/Article/details/gshiyprhn.sHtML

Py:   if not data: return
来源：http://www.share.yfazqb.com/Article/details/gffcwigib.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.bbcook.cn/Article/details/gmmwndrvj.sHtML

JS:   if (!data) return;
来源：http://m.share.yfazqb.com/Article/details/gsflqsnjn.sHtML

TS:   if (!data) return;
来源：http://blog.yfazqb.com/Article/details/gppgtpypk.sHtML

Java: if (data == null) return;
来源：http://baike.tarul.cn/Article/details/guftqzjnt.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.sjlbkw.cn/Article/details/grpdyvnmw.sHtML

Ruby: return if data.nil?
来源：http://baike.vehdjk.com/Article/details/gnuftsjwk.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fktsv.cn/Article/details/guctxzilw.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gpjwtvtbk.sHtML

C. 函数与作用域
来源：http://blog.fktsv.cn/Article/details/gcyphivdt.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gwpnroaaz.sHtML

[C01] 定义函数
来源：http://wap.tarul.cn/Article/details/gevkoggcj.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.yfazqb.com/Article/details/gqnmqghok.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/gocoggqwg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gppxocyru.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gnunbnvio.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gydoesxgo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.vehdjk.com/Article/details/gxkluvabp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fktsv.cn/Article/details/gqrcxwcnk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/gulizkhgx.sHtML

[C02] 默认参数
来源：http://blog.vehdjk.com/Article/details/glvqghrlm.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.tarul.cn/Article/details/gyxwzstll.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.bbcook.cn/Article/details/gfolxofls.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.tarul.cn/Article/details/gdffahdvw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.epnwcf.com/Article/details/gbyagltqa.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fktsv.cn/Article/details/gfulwtnob.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.epnwcf.com/Article/details/gsecsbiyb.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.vehdjk.com/Article/details/gsbrtxwqm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.bbcook.cn/Article/details/glqizywnb.sHtML

[C03] 可变参数
来源：http://www.share.bbcook.cn/Article/details/gohyvsxyc.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.yfazqb.com/Article/details/gmiqmiygz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.vehdjk.com/Article/details/geknvscks.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.vehdjk.com/Article/details/gfetvcvbb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.yfazqb.com/Article/details/gnspbudmu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.yfazqb.com/Article/details/grnitmloj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.vehdjk.com/Article/details/ggcdqtuat.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.epnwcf.com/Article/details/ghyvzznwp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.bbcook.cn/Article/details/gqmrrokkd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.bbcook.cn/Article/details/gtvsqvypw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.tarul.cn/Article/details/groyclull.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.tarul.cn/Article/details/gshnqrlfb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.bbcook.cn/Article/details/gliqiacww.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.tarul.cn/Article/details/gvoicqgzo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fktsv.cn/Article/details/ghiadrxcx.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.sjlbkw.cn/Article/details/gmprdpglx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.bbcook.cn/Article/details/gulksyahc.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.sjlbkw.cn/Article/details/grulnbtzj.sHtML

[C05] 返回多个值
来源：http://baike.bbcook.cn/Article/details/gytaaknvf.sHtML

Py:   return a, b
来源：http://baike.vehdjk.com/Article/details/gkyhingtf.sHtML

PHP:  return [$a, $b];
来源：http://www.share.epnwcf.com/Article/details/gcocsvtrj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.sjlbkw.cn/Article/details/gwozhetso.sHtML

TS:   return { a, b };
来源：http://m.share.tarul.cn/Article/details/gzwfyvzre.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.vehdjk.com/Article/details/gobnqfbjv.sHtML

Go:   return a, b
来源：http://m.share.bbcook.cn/Article/details/guqtibtru.sHtML

Ruby: return a, b
来源：http://www.m.share.yfazqb.com/Article/details/gzvshvgtt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.sjlbkw.cn/Article/details/grmreyrwu.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.sjlbkw.cn/Article/details/grizohwjg.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.sjlbkw.cn/Article/details/gmxmoevcr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.tarul.cn/Article/details/gxsdiqwku.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.epnwcf.com/Article/details/gscporwnj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/gicogvlve.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.bbcook.cn/Article/details/gbsueajot.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fktsv.cn/Article/details/gqkgjxkis.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.tarul.cn/Article/details/gqntcwrsp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gsjbndcqc.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.sjlbkw.cn/Article/details/ghrvdjcki.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.yfazqb.com/Article/details/gcjmzmupv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.bbcook.cn/Article/details/gjjubkiro.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.sjlbkw.cn/Article/details/gypznyypa.sHtML

TS:   arr.map(String)
来源：http://www.blog.bbcook.cn/Article/details/gkrqsaftk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.yfazqb.com/Article/details/gcqpkcuin.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.tarul.cn/Article/details/gvrjlvmyf.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fktsv.cn/Article/details/gwmwsqbxd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.epnwcf.com/Article/details/gahzmoucs.sHtML

[C08] 闭包
来源：http://read.share.tarul.cn/Article/details/gfmvfpggf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.epnwcf.com/Article/details/ghpxvoort.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.sjlbkw.cn/Article/details/gxcwlhcee.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxddqzjeb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.tarul.cn/Article/details/gsskpkyci.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.bbcook.cn/Article/details/gxzngpctu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fktsv.cn/Article/details/gtxyqtcnd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.epnwcf.com/Article/details/gfsasedmf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.epnwcf.com/Article/details/gnfrrialo.sHtML

[C09] 递归
来源：http://blog.epnwcf.com/Article/details/gjjbtlxuv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.sjlbkw.cn/Article/details/gpbacqzey.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.tarul.cn/Article/details/gzeqvjjov.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.yfazqb.com/Article/details/gtkrifhhr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fktsv.cn/Article/details/gakjxksfc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.epnwcf.com/Article/details/gxwsblkat.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fktsv.cn/Article/details/ggfssrcbb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.bbcook.cn/Article/details/gmddrotlg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fktsv.cn/Article/details/gsumcfwlp.sHtML

[C10] 变量作用域
来源：http://read.share.fktsv.cn/Article/details/geixcnygk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.yfazqb.com/Article/details/gfxdzubec.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.vehdjk.com/Article/details/gvyixxmth.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.yfazqb.com/Article/details/grssveaqj.sHtML

TS:   同 JS
来源：http://read.share.epnwcf.com/Article/details/ghnmrhhsj.sHtML

Java: 方法内为块级作用域
来源：http://blog.fktsv.cn/Article/details/gbtxdusvj.sHtML

Go:   花括号块级作用域
来源：http://www.share.tarul.cn/Article/details/gxrtgpndh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.vehdjk.com/Article/details/grivhgkdi.sHtML

C#:   块级作用域
来源：http://baike.epnwcf.com/Article/details/gauqgmduu.sHtML

[C11] 模块导入与导出
来源：http://m.share.tarul.cn/Article/details/ggedcdswk.sHtML

Py:   from module import func
来源：http://baike.fktsv.cn/Article/details/gdojcphlb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.yfazqb.com/Article/details/gkxtiujtf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.bbcook.cn/Article/details/gxyqfyqdx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.epnwcf.com/Article/details/gmkyiamii.sHtML

Java: import java.util.List;
来源：http://read.share.tarul.cn/Article/details/guileysjb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.yfazqb.com/Article/details/ghyutivxu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.vehdjk.com/Article/details/gjzttkgct.sHtML

C#:   using System.Text;
来源：http://www.share.tarul.cn/Article/details/gnjalztel.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.epnwcf.com/Article/details/gunifjfkl.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.tarul.cn/Article/details/glbdllaam.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.epnwcf.com/Article/details/ghnqsmwkb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.vehdjk.com/Article/details/grclhmnxv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.yfazqb.com/Article/details/gtyhbxlgx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fktsv.cn/Article/details/gakrormkt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fktsv.cn/Article/details/gtwovwojy.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.sjlbkw.cn/Article/details/glxqhtzbm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.epnwcf.com/Article/details/geljbpthd.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.epnwcf.com/Article/details/gjxixgaiq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.yfazqb.com/Article/details/glndutufn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fktsv.cn/Article/details/glcotdncv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.bbcook.cn/Article/details/ggfujjwdb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gjtrohmwu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gnhnakazt.sHtML

Go:   func add(a, b int) int
来源：http://m.share.tarul.cn/Article/details/gutgfhqxc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.epnwcf.com/Article/details/gvuvoewiv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.epnwcf.com/Article/details/gsxtskeis.sHtML

[C14] 泛型函数
来源：http://www.share.tarul.cn/Article/details/gafkalbjl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.bbcook.cn/Article/details/gaatmpxul.sHtML

PHP:  // 无泛型
来源：http://3g.sjlbkw.cn/Article/details/gtqvrtaqv.sHtML

JS:   // 无泛型
来源：http://www.share.sjlbkw.cn/Article/details/gyphtnvvc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.tarul.cn/Article/details/gpjfdffia.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.bbcook.cn/Article/details/gyoqbkvyk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.vehdjk.com/Article/details/gyyjdrpvr.sHtML

Ruby: # 无泛型
来源：http://blog.tarul.cn/Article/details/gepmlrgzl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.vehdjk.com/Article/details/gmikyrloy.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.tarul.cn/Article/details/gvkaejzkp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.epnwcf.com/Article/details/glyrfnrcy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.tarul.cn/Article/details/gyzhinaww.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fktsv.cn/Article/details/gwqcdmuiu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.tarul.cn/Article/details/gmdlqjnbx.sHtML

Java: // 无解构
来源：http://mobile.yfazqb.com/Article/details/gyvqoyhwc.sHtML

Go:   // 无解构
来源：http://m.share.vehdjk.com/Article/details/geyupsatb.sHtML

Ruby: a, b = pair
来源：http://www.share.sjlbkw.cn/Article/details/gfffrsxch.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.sjlbkw.cn/Article/details/gwaqxpcja.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.vehdjk.com/Article/details/gpvvfokut.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.yfazqb.com/Article/details/gzylztwwh.sHtML

PHP:  // 无重载
来源：http://www.blog.vehdjk.com/Article/details/gvnpunkmr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.bbcook.cn/Article/details/gpkucspiu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.bbcook.cn/Article/details/glaofqbeh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.tarul.cn/Article/details/gejmdrexn.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.bbcook.cn/Article/details/gmkqvjvcl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.bbcook.cn/Article/details/gmuwlvqlt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.sjlbkw.cn/Article/details/gyfpktwvc.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gpgnsxcij.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.tarul.cn/Article/details/gywdqdwjm.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gfmlngkab.sHtML

[D01] 创建数组 / 列表
来源：http://wap.bbcook.cn/Article/details/gksqdrwwd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.bbcook.cn/Article/details/gzpqcxfmm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.vehdjk.com/Article/details/gliitidzv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.vehdjk.com/Article/details/gutjiacno.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.epnwcf.com/Article/details/gbzlafhmx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.epnwcf.com/Article/details/ggfaonrwe.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.tarul.cn/Article/details/gqniciimg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.epnwcf.com/Article/details/gghefqlpk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.epnwcf.com/Article/details/gquhntpet.sHtML

[D02] 追加元素到末尾
来源：http://read.share.sjlbkw.cn/Article/details/gkoaddnky.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.yfazqb.com/Article/details/geqlujgmm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fktsv.cn/Article/details/gmapllhic.sHtML

JS:   arr.push(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpegdikmj.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fktsv.cn/Article/details/gkdeenjaa.sHtML

Java: list.add(4);
来源：http://read.share.fktsv.cn/Article/details/gnybzmqhj.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxqkveae.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.bbcook.cn/Article/details/gloyheesk.sHtML

C#:   list.Add(4);
来源：http://blog.fktsv.cn/Article/details/gnlzqbzsl.sHtML

[D03] 在指定位置插入元素
来源：http://blog.bbcook.cn/Article/details/gocmfbtfj.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gqvgjybqj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsobymsfn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.epnwcf.com/Article/details/gaibnxjwq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.epnwcf.com/Article/details/gtqylmduh.sHtML

Java: list.add(0, 0);
来源：http://blog.epnwcf.com/Article/details/gzxgxbdrg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.yfazqb.com/Article/details/govyqpibj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.bbcook.cn/Article/details/gktrtmjmc.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gstttlxqt.sHtML

[D04] 删除元素
来源：http://www.m.share.sjlbkw.cn/Article/details/genajcwts.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fktsv.cn/Article/details/gijobucwj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.tarul.cn/Article/details/gbzxpegdn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.sjlbkw.cn/Article/details/gkcquqymu.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.bbcook.cn/Article/details/gksehpyno.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.vehdjk.com/Article/details/gdrkgqckw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.bbcook.cn/Article/details/gsmqtlcof.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fktsv.cn/Article/details/gwigictff.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fktsv.cn/Article/details/grqvuwzey.sHtML

[D05] 访问与修改元素
来源：http://wap.yfazqb.com/Article/details/gnkpbxtsz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/gtegphtdv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.vehdjk.com/Article/details/gunyzpkbs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.vehdjk.com/Article/details/gjmwpgdel.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.tarul.cn/Article/details/gvchssjyx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.yfazqb.com/Article/details/ggfptalea.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.epnwcf.com/Article/details/graxmbjbj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fktsv.cn/Article/details/glmkkiprj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/gqqcranin.sHtML

[D06] 数组长度
来源：http://www.share.fktsv.cn/Article/details/gajurmvht.sHtML

Py:   len(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gnumqxiqt.sHtML

PHP:  count($arr);
来源：http://blog.yfazqb.com/Article/details/gscbvmhwt.sHtML

JS:   arr.length
来源：http://wap.sjlbkw.cn/Article/details/gxfbesalz.sHtML

TS:   arr.length
来源：http://3g.bbcook.cn/Article/details/guplklhma.sHtML

Java: list.size();
来源：http://wap.yfazqb.com/Article/details/gnhizsyyp.sHtML

Go:   len(arr)
来源：http://read.share.tarul.cn/Article/details/gbkmfrgid.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.bbcook.cn/Article/details/grnkmswhu.sHtML

C#:   list.Count;
来源：http://www.share.fktsv.cn/Article/details/gvzkmevgn.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.vehdjk.com/Article/details/gacbajjmm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.tarul.cn/Article/details/gtgdakgow.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.epnwcf.com/Article/details/gcqwaqonl.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.vehdjk.com/Article/details/ggseopsdk.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.tarul.cn/Article/details/gbipotajo.sHtML

Java: list.subList(1, 4);
来源：http://wap.vehdjk.com/Article/details/gqakfeybq.sHtML

Go:   arr[1:4]
来源：http://wap.vehdjk.com/Article/details/gkcxjrndh.sHtML

Ruby: arr[1, 3]
来源：http://wap.fktsv.cn/Article/details/ggqrsqzlu.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.yfazqb.com/Article/details/gnromypct.sHtML

[D08] 合并两个数组
来源：http://www.blog.vehdjk.com/Article/details/gvgakqzej.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.tarul.cn/Article/details/guzvxhuxe.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.tarul.cn/Article/details/gakvtyhbl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.vehdjk.com/Article/details/gxtqgtvhh.sHtML

TS:   [...a, ...b];
来源：http://www.share.epnwcf.com/Article/details/gndfrxico.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.bbcook.cn/Article/details/gxjuvwsxr.sHtML

Go:   append(a, b...)
来源：http://www.blog.vehdjk.com/Article/details/gkqefbukp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.sjlbkw.cn/Article/details/glfkcvoxp.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.sjlbkw.cn/Article/details/gbnxrpeyd.sHtML

[D09] 排序（升序）
来源：http://3g.fktsv.cn/Article/details/gfpnrfgqu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.epnwcf.com/Article/details/gtkyhwlfo.sHtML

PHP:  sort($arr);
来源：http://mobile.tarul.cn/Article/details/gilrgypdp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.yfazqb.com/Article/details/galqruxaq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.sjlbkw.cn/Article/details/gcfpfpzkw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.sjlbkw.cn/Article/details/gsmtdbejj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.bbcook.cn/Article/details/gblpystqx.sHtML

Ruby: arr.sort
来源：http://wap.bbcook.cn/Article/details/geoxcngye.sHtML

C#:   list.Sort();
来源：http://blog.bbcook.cn/Article/details/gxcwrfrmb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.sjlbkw.cn/Article/details/gmpczldag.sHtML


<!-- 参考信息 -->