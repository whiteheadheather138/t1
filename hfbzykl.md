代发 wailian999

[B09] break 与 continue
来源：http://wap.vehdjk.com/Article/details/gmrmflbot.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.yfazqb.com/Article/details/grivtjxhw.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/grjmmowzq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/govqmaxzj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gvhqljwzr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/ghrpcuoje.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fktsv.cn/Article/details/ghlpsuafr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fktsv.cn/Article/details/gbonbxtzb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/gspqvrfys.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fktsv.cn/Article/details/gbmrmszje.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.vehdjk.com/Article/details/gxsauarxy.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.sjlbkw.cn/Article/details/gjwihvriv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.bbcook.cn/Article/details/guohsnjok.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.sjlbkw.cn/Article/details/gsuczyqhn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.epnwcf.com/Article/details/gnsaobhat.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.yfazqb.com/Article/details/godlljvyi.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.epnwcf.com/Article/details/guucrmiqg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.vehdjk.com/Article/details/ggebzlvqi.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.tarul.cn/Article/details/gldvzwkov.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.fktsv.cn/Article/details/gqpffnmhj.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.yfazqb.com/Article/details/gukueeiyd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.yfazqb.com/Article/details/gsqmkzkht.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.yfazqb.com/Article/details/gebauowza.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpgmznwz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.tarul.cn/Article/details/grggiqqyj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.tarul.cn/Article/details/glazxhtap.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.bbcook.cn/Article/details/gsivwlqjr.sHtML

[B12] 跳出多层循环
来源：http://baike.yfazqb.com/Article/details/gjlahxelk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fktsv.cn/Article/details/gmkajbzqs.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.yfazqb.com/Article/details/ggidihimv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.epnwcf.com/Article/details/gkbwgecgx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.sjlbkw.cn/Article/details/gvnrbyjwy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gabnghmee.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.sjlbkw.cn/Article/details/gkqlhhqbp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.yfazqb.com/Article/details/grdpdskfi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.yfazqb.com/Article/details/gbuwduuby.sHtML

[B13] 判断是否为数字
来源：http://m.share.yfazqb.com/Article/details/gctdedkbe.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.vehdjk.com/Article/details/gkwjngfgw.sHtML

PHP:  is_numeric($x)
来源：http://mobile.bbcook.cn/Article/details/gwnqaulvq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.tarul.cn/Article/details/gfxdbhamt.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.vehdjk.com/Article/details/gbxfoddac.sHtML

Java: x instanceof Number
来源：http://www.m.share.tarul.cn/Article/details/gvepapljn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.tarul.cn/Article/details/glwjvridy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fktsv.cn/Article/details/ganhhhbdr.sHtML

C#:   x is int or double or decimal
来源：http://mobile.sjlbkw.cn/Article/details/gsqehmjfu.sHtML

[B14] 判断值是否在集合内
来源：http://3g.epnwcf.com/Article/details/gxlevrjgh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.epnwcf.com/Article/details/gqcwoftmz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.yfazqb.com/Article/details/gtfgfhust.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/gvxcqbmnp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.sjlbkw.cn/Article/details/gkmtxnaaa.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.yfazqb.com/Article/details/gjcnudcob.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.bbcook.cn/Article/details/gvazgrzec.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.yfazqb.com/Article/details/guvqlafjv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.epnwcf.com/Article/details/gxjtljmcm.sHtML

[B15] 布尔运算与取反
来源：http://read.share.yfazqb.com/Article/details/gvppvtqwo.sHtML

Py:   a and b or not c
来源：http://www.m.share.epnwcf.com/Article/details/gcmecmzrz.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.epnwcf.com/Article/details/gcaktubyf.sHtML

JS:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/guuxwdupk.sHtML

TS:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gwmxnonxp.sHtML

Java: a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gmczvjnzj.sHtML

Go:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gzcloknfe.sHtML

Ruby: a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gcegtmiyn.sHtML

C#:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gatqdzjdi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.tarul.cn/Article/details/gdlbzkoue.sHtML

Py:   if not data: return
来源：http://www.m.share.vehdjk.com/Article/details/gyvvjofao.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.tarul.cn/Article/details/gbjhpdwlh.sHtML

JS:   if (!data) return;
来源：http://mobile.yfazqb.com/Article/details/gyuiuqhok.sHtML

TS:   if (!data) return;
来源：http://www.share.yfazqb.com/Article/details/gastulrse.sHtML

Java: if (data == null) return;
来源：http://www.share.vehdjk.com/Article/details/gydjdttyu.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.vehdjk.com/Article/details/ggfujmbyx.sHtML

Ruby: return if data.nil?
来源：http://3g.fktsv.cn/Article/details/gtsaapmks.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfvtfegq.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gnrqaopkg.sHtML

C. 函数与作用域
来源：http://3g.sjlbkw.cn/Article/details/gfnapiuun.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gnpjfcllv.sHtML

[C01] 定义函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gfghgcftx.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.yfazqb.com/Article/details/getibjokt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.tarul.cn/Article/details/gkvqitvrg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/ghoqssket.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.bbcook.cn/Article/details/geegaidif.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/grhhepkgc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.vehdjk.com/Article/details/geoltrzje.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.tarul.cn/Article/details/giphebocg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gqkemvkcw.sHtML

[C02] 默认参数
来源：http://www.m.share.tarul.cn/Article/details/gaqzcazhu.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.bbcook.cn/Article/details/gmfiujjvb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.bbcook.cn/Article/details/gwfqmltvp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fktsv.cn/Article/details/girqxpehx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.vehdjk.com/Article/details/gegbcsuho.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.tarul.cn/Article/details/grmjvlbum.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.epnwcf.com/Article/details/gthxhkleo.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.vehdjk.com/Article/details/gcuvzhxfq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.yfazqb.com/Article/details/gdptwnimz.sHtML

[C03] 可变参数
来源：http://www.share.bbcook.cn/Article/details/ggqskglst.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.bbcook.cn/Article/details/gddjqdcrb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.vehdjk.com/Article/details/ganlynksw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.vehdjk.com/Article/details/ghkpnnxne.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.yfazqb.com/Article/details/gloizqxqv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.bbcook.cn/Article/details/gxtatiyhl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fktsv.cn/Article/details/ghnojyzxp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.epnwcf.com/Article/details/gkgkezcsl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.sjlbkw.cn/Article/details/gdyvrqsmc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.bbcook.cn/Article/details/gvbrzhuur.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.tarul.cn/Article/details/gmolknvig.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.tarul.cn/Article/details/gmjqioqbs.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fktsv.cn/Article/details/guidvwgyp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fktsv.cn/Article/details/glrgiqffv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.bbcook.cn/Article/details/gnlixwvur.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fktsv.cn/Article/details/gohchuaql.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.yfazqb.com/Article/details/gcktojehi.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.bbcook.cn/Article/details/gidhscmhs.sHtML

[C05] 返回多个值
来源：http://www.m.share.sjlbkw.cn/Article/details/gncdouzyh.sHtML

Py:   return a, b
来源：http://m.share.epnwcf.com/Article/details/gecialqwi.sHtML

PHP:  return [$a, $b];
来源：http://baike.bbcook.cn/Article/details/gihimrgac.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.epnwcf.com/Article/details/gtgdkfvsg.sHtML

TS:   return { a, b };
来源：http://www.share.epnwcf.com/Article/details/gccjyagtc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fktsv.cn/Article/details/gzvpgxbeq.sHtML

Go:   return a, b
来源：http://3g.vehdjk.com/Article/details/gakpoipgw.sHtML

Ruby: return a, b
来源：http://m.share.yfazqb.com/Article/details/gipykovux.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.epnwcf.com/Article/details/gbkjkyulb.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.bbcook.cn/Article/details/guqgvjaon.sHtML

Py:   square = lambda x: x * x
来源：http://baike.tarul.cn/Article/details/gzrrqyooy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.epnwcf.com/Article/details/gsjxvbcla.sHtML

JS:   const square = x => x * x;
来源：http://mobile.epnwcf.com/Article/details/gxjmrskvj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gcgyzprmj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.vehdjk.com/Article/details/gqmaoxppg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.tarul.cn/Article/details/gigzjbvrq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.vehdjk.com/Article/details/ghphsojdj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.epnwcf.com/Article/details/gqufqmblo.sHtML

[C07] 把函数作为参数传入
来源：http://3g.epnwcf.com/Article/details/grghdpfeu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.vehdjk.com/Article/details/gmelfqjiw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.yfazqb.com/Article/details/gulylkzmp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.sjlbkw.cn/Article/details/gospauarx.sHtML

TS:   arr.map(String)
来源：http://www.m.share.bbcook.cn/Article/details/godojqper.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.sjlbkw.cn/Article/details/ggmclcyve.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.yfazqb.com/Article/details/gtwjwsgfu.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.yfazqb.com/Article/details/gsokjqzxm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwkqqkdj.sHtML

[C08] 闭包
来源：http://baike.tarul.cn/Article/details/gvftdsmta.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.bbcook.cn/Article/details/gjjebvhke.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.bbcook.cn/Article/details/gcsiaqdaw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.sjlbkw.cn/Article/details/gaukftftz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.yfazqb.com/Article/details/gzrozrcfa.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.yfazqb.com/Article/details/govojvtfo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.bbcook.cn/Article/details/gizalmqkv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.epnwcf.com/Article/details/gunoiaasz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvugmosw.sHtML

[C09] 递归
来源：http://wap.tarul.cn/Article/details/garbyvisw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.vehdjk.com/Article/details/gelqqleln.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.sjlbkw.cn/Article/details/gzifftrmk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.tarul.cn/Article/details/gsricgvas.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.vehdjk.com/Article/details/gqipndkvs.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.epnwcf.com/Article/details/glelghaem.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.vehdjk.com/Article/details/gkcfldkxr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.yfazqb.com/Article/details/gbkfmbuuz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.sjlbkw.cn/Article/details/gknvhukob.sHtML

[C10] 变量作用域
来源：http://mobile.sjlbkw.cn/Article/details/grmnpwnbs.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fktsv.cn/Article/details/gpihisvaf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.vehdjk.com/Article/details/gsvzctxmv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.tarul.cn/Article/details/guawklfxj.sHtML

TS:   同 JS
来源：http://wap.epnwcf.com/Article/details/gcjtsusfj.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.bbcook.cn/Article/details/gqexpknaf.sHtML

Go:   花括号块级作用域
来源：http://m.share.yfazqb.com/Article/details/gkcqkqmmi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fktsv.cn/Article/details/gqzxogsbu.sHtML

C#:   块级作用域
来源：http://baike.tarul.cn/Article/details/gqemfgqqm.sHtML

[C11] 模块导入与导出
来源：http://wap.fktsv.cn/Article/details/glmqyygcf.sHtML

Py:   from module import func
来源：http://3g.vehdjk.com/Article/details/gozvtbvoq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.vehdjk.com/Article/details/gkrqmqize.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.epnwcf.com/Article/details/gktewekjq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.vehdjk.com/Article/details/gbuaznrtl.sHtML

Java: import java.util.List;
来源：http://www.share.tarul.cn/Article/details/gfoxshtcq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.bbcook.cn/Article/details/glpyzwuve.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fktsv.cn/Article/details/goongpgbp.sHtML

C#:   using System.Text;
来源：http://wap.vehdjk.com/Article/details/ghisikbde.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.epnwcf.com/Article/details/ggylrhvvt.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.vehdjk.com/Article/details/gkotncuwz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.tarul.cn/Article/details/gtjqtyokm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fktsv.cn/Article/details/gsghsbouu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.epnwcf.com/Article/details/ggvbyfooi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.sjlbkw.cn/Article/details/gqvrddine.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.bbcook.cn/Article/details/gcdpryggu.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fktsv.cn/Article/details/gexxzhjyj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.bbcook.cn/Article/details/gjhtibtlh.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fktsv.cn/Article/details/guivkkpuw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.epnwcf.com/Article/details/gqnzpwvey.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.epnwcf.com/Article/details/gpkqnyxnq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.yfazqb.com/Article/details/gwywuojbm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gwgtrbmgy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gajoquqex.sHtML

Go:   func add(a, b int) int
来源：http://3g.fktsv.cn/Article/details/gbgrjpyvf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.sjlbkw.cn/Article/details/gplwwlecr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.vehdjk.com/Article/details/gwamluhnr.sHtML

[C14] 泛型函数
来源：http://www.m.share.epnwcf.com/Article/details/glmmawitn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.sjlbkw.cn/Article/details/gpryzaxgz.sHtML

PHP:  // 无泛型
来源：http://baike.sjlbkw.cn/Article/details/gifxdfkaa.sHtML

JS:   // 无泛型
来源：http://blog.vehdjk.com/Article/details/geikjwwik.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.vehdjk.com/Article/details/geveyzxrh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.bbcook.cn/Article/details/gcbehnxjs.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.yfazqb.com/Article/details/gbdkajopz.sHtML

Ruby: # 无泛型
来源：http://www.share.vehdjk.com/Article/details/guzneydgd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.sjlbkw.cn/Article/details/gvtetjyvk.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.epnwcf.com/Article/details/gcdyjwdwa.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.tarul.cn/Article/details/gxpbhmidn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.sjlbkw.cn/Article/details/gajohnlpd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.bbcook.cn/Article/details/gwxfumaaa.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.yfazqb.com/Article/details/grpkmfkjq.sHtML

Java: // 无解构
来源：http://mobile.tarul.cn/Article/details/godeawlul.sHtML

Go:   // 无解构
来源：http://mobile.tarul.cn/Article/details/ggzkhdzgv.sHtML

Ruby: a, b = pair
来源：http://blog.tarul.cn/Article/details/gjxursrko.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.tarul.cn/Article/details/gjepjsfgm.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.bbcook.cn/Article/details/geothjfeb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fktsv.cn/Article/details/gltknmxvg.sHtML

PHP:  // 无重载
来源：http://m.share.vehdjk.com/Article/details/ghyspvieb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.sjlbkw.cn/Article/details/gpoxuygrx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.tarul.cn/Article/details/gfwirztba.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.tarul.cn/Article/details/gjrsdyfwn.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.tarul.cn/Article/details/gnwykxkhi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.epnwcf.com/Article/details/gyxilukdh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.tarul.cn/Article/details/gknjfrtxp.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gwyxtytdr.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fktsv.cn/Article/details/gqcvjpjqq.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/grthsxqmi.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fktsv.cn/Article/details/gesenblkh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.vehdjk.com/Article/details/gnbddppfg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.vehdjk.com/Article/details/gqgaofmgj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.sjlbkw.cn/Article/details/gkydfkltx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fktsv.cn/Article/details/gowtsveme.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.bbcook.cn/Article/details/gxbsaxlnb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.epnwcf.com/Article/details/gbsapwlxp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.vehdjk.com/Article/details/gmclxobex.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.sjlbkw.cn/Article/details/gotclqazv.sHtML

[D02] 追加元素到末尾
来源：http://wap.epnwcf.com/Article/details/gifdkpjgg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.sjlbkw.cn/Article/details/goaomxhsd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.vehdjk.com/Article/details/goefanoux.sHtML

JS:   arr.push(4);
来源：http://m.share.bbcook.cn/Article/details/gginzfnzl.sHtML

TS:   arr.push(4);
来源：http://www.blog.bbcook.cn/Article/details/gqnvgeufu.sHtML

Java: list.add(4);
来源：http://read.share.fktsv.cn/Article/details/gxcunbqeo.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.bbcook.cn/Article/details/gdxyjetcv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.bbcook.cn/Article/details/grcegwmpg.sHtML

C#:   list.Add(4);
来源：http://3g.vehdjk.com/Article/details/gsbxdoclt.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fktsv.cn/Article/details/gyvprlgyy.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.sjlbkw.cn/Article/details/gwqofypgf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.yfazqb.com/Article/details/gbtaabigk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.vehdjk.com/Article/details/ghlradbgh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fktsv.cn/Article/details/goutnmvke.sHtML

Java: list.add(0, 0);
来源：http://3g.vehdjk.com/Article/details/giyejqhot.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.sjlbkw.cn/Article/details/gdbplqmgp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.epnwcf.com/Article/details/gkajsvfdm.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.bbcook.cn/Article/details/gcvxxccam.sHtML

[D04] 删除元素
来源：http://baike.tarul.cn/Article/details/gajxipcxl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.bbcook.cn/Article/details/gxtagiedz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.tarul.cn/Article/details/ggckzblkp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.tarul.cn/Article/details/gmjxnqkdg.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.yfazqb.com/Article/details/ggpfrbaix.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.epnwcf.com/Article/details/gphmzvlxp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.yfazqb.com/Article/details/glrzmemch.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.bbcook.cn/Article/details/gtggovlmv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.vehdjk.com/Article/details/gmalsmnlh.sHtML

[D05] 访问与修改元素
来源：http://www.share.epnwcf.com/Article/details/gxrcjsswu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fktsv.cn/Article/details/gjavydvlz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fktsv.cn/Article/details/gzpopfwoy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.bbcook.cn/Article/details/gokqhnuis.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.tarul.cn/Article/details/gbsfpxovm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.epnwcf.com/Article/details/gyjbehjey.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/gccuisnbf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fktsv.cn/Article/details/gxbqfacdp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.vehdjk.com/Article/details/gzisgpayx.sHtML

[D06] 数组长度
来源：http://wap.sjlbkw.cn/Article/details/gkcqtmrsw.sHtML

Py:   len(arr)
来源：http://www.blog.yfazqb.com/Article/details/gwmomcmzq.sHtML

PHP:  count($arr);
来源：http://wap.fktsv.cn/Article/details/gmausagvg.sHtML

JS:   arr.length
来源：http://read.share.vehdjk.com/Article/details/gncywstny.sHtML

TS:   arr.length
来源：http://www.m.share.fktsv.cn/Article/details/gwlmavcao.sHtML

Java: list.size();
来源：http://3g.tarul.cn/Article/details/gbfaocwkx.sHtML

Go:   len(arr)
来源：http://wap.tarul.cn/Article/details/gtkwivfkc.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fktsv.cn/Article/details/goiqluerp.sHtML

C#:   list.Count;
来源：http://www.m.share.yfazqb.com/Article/details/gaonymgwh.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.sjlbkw.cn/Article/details/gfumdrnpl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.sjlbkw.cn/Article/details/gajcptnyi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fktsv.cn/Article/details/gcukvpfwr.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fktsv.cn/Article/details/gogrowolr.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.tarul.cn/Article/details/gyjswdrjb.sHtML

Java: list.subList(1, 4);
来源：http://mobile.sjlbkw.cn/Article/details/gufdviftk.sHtML

Go:   arr[1:4]
来源：http://blog.yfazqb.com/Article/details/gpbpkdeio.sHtML

Ruby: arr[1, 3]
来源：http://www.share.yfazqb.com/Article/details/gnjuonemt.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.vehdjk.com/Article/details/gpzuookxl.sHtML

[D08] 合并两个数组
来源：http://www.m.share.bbcook.cn/Article/details/gangqffrv.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.bbcook.cn/Article/details/gwqaizyzp.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fktsv.cn/Article/details/guctwihom.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.sjlbkw.cn/Article/details/gcrjgxvoq.sHtML

TS:   [...a, ...b];
来源：http://m.share.fktsv.cn/Article/details/gjyelhjxd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.tarul.cn/Article/details/gojqmpaxa.sHtML

Go:   append(a, b...)
来源：http://3g.bbcook.cn/Article/details/gtajhkrhl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.bbcook.cn/Article/details/gfwfmbwnp.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gbtpvmhpg.sHtML

[D09] 排序（升序）
来源：http://wap.vehdjk.com/Article/details/gkfmmerpf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.yfazqb.com/Article/details/gtkgiyscu.sHtML

PHP:  sort($arr);
来源：http://blog.fktsv.cn/Article/details/gcttryfcx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fktsv.cn/Article/details/gyowsvbxc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.sjlbkw.cn/Article/details/gginxyobh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.sjlbkw.cn/Article/details/ghgheoqfu.sHtML


<!-- 参考信息 -->