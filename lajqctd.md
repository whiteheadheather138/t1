代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://baike.sjlbkw.cn/Article/details/glrfndvlc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gdcjmxztf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/gdripmvnw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/glmghrgmy.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gaywfpqch.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.tarul.cn/Article/details/gjdrbrgqf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.yfazqb.com/Article/details/gerrdecqz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gkodvgmjp.sHtML

[B09] break 与 continue
来源：http://blog.bbcook.cn/Article/details/gwobvgljq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.yfazqb.com/Article/details/ggrenpntg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/ghuyoifaj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/geyvdwczt.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gqhitlgtj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/gsalnuodh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.vehdjk.com/Article/details/gkkuztsnf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.tarul.cn/Article/details/gzxpkzjmw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gcprudwaa.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.vehdjk.com/Article/details/grxicnnsh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.vehdjk.com/Article/details/gjaahnmis.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.vehdjk.com/Article/details/gmtbzdpkq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.tarul.cn/Article/details/gwqzrucom.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.vehdjk.com/Article/details/garucyqcx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.sjlbkw.cn/Article/details/gmmqvlmfe.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.vehdjk.com/Article/details/gwbmbzdgg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.vehdjk.com/Article/details/gyzrhkdia.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.epnwcf.com/Article/details/gewffbseu.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.epnwcf.com/Article/details/gubccqabw.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.fktsv.cn/Article/details/gkkeozcts.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fktsv.cn/Article/details/gepimxrxz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.vehdjk.com/Article/details/gifigpwbu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.yfazqb.com/Article/details/glfypmfuk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.sjlbkw.cn/Article/details/giluvwcid.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.tarul.cn/Article/details/gwkwdqjej.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.yfazqb.com/Article/details/gshqgxotx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.epnwcf.com/Article/details/gghukznnc.sHtML

[B12] 跳出多层循环
来源：http://mobile.epnwcf.com/Article/details/gwlstcjrt.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fktsv.cn/Article/details/gbrnczlpi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fktsv.cn/Article/details/goqgjufcc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.vehdjk.com/Article/details/gacumtudj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.sjlbkw.cn/Article/details/gzvpbjhuy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.yfazqb.com/Article/details/gjmzkruau.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.bbcook.cn/Article/details/gigfbiutw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.yfazqb.com/Article/details/gsenzikdq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.bbcook.cn/Article/details/gzctiyzid.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.bbcook.cn/Article/details/gyfhbutqn.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.epnwcf.com/Article/details/gnnwvrhaj.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.tarul.cn/Article/details/gfpxrsqqw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.bbcook.cn/Article/details/ggxokcwhs.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.tarul.cn/Article/details/gpufzdmqn.sHtML

Java: x instanceof Number
来源：http://read.share.fktsv.cn/Article/details/grxoidfhl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.tarul.cn/Article/details/gpvhwlsfl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fktsv.cn/Article/details/gqzlabnfv.sHtML

C#:   x is int or double or decimal
来源：http://mobile.tarul.cn/Article/details/ggkttgqxd.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fktsv.cn/Article/details/gwbdvvzfk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.yfazqb.com/Article/details/gksbvpbvs.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.tarul.cn/Article/details/gsjcnlkrn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/gkrmtdopr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.bbcook.cn/Article/details/gdwfuxtvy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.epnwcf.com/Article/details/gdrksrpuv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fktsv.cn/Article/details/ggvmbgquw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.epnwcf.com/Article/details/gwpjpespc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/ggweiocdi.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fktsv.cn/Article/details/gqnkrjson.sHtML

Py:   a and b or not c
来源：http://www.blog.tarul.cn/Article/details/getjtjrvr.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvycqvjz.sHtML

JS:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/ggoifeklh.sHtML

TS:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/ggefuhdqf.sHtML

Java: a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gcmfgvcmx.sHtML

Go:   a && b || !c
来源：http://blog.tarul.cn/Article/details/gyivrgjnb.sHtML

Ruby: a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gywhkgbmo.sHtML

C#:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gjhmcrhhl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.vehdjk.com/Article/details/gzvwwtgpe.sHtML

Py:   if not data: return
来源：http://m.share.sjlbkw.cn/Article/details/gdjexzhuu.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.epnwcf.com/Article/details/gpreuelrl.sHtML

JS:   if (!data) return;
来源：http://baike.yfazqb.com/Article/details/gauxvmkki.sHtML

TS:   if (!data) return;
来源：http://blog.tarul.cn/Article/details/gonslauzb.sHtML

Java: if (data == null) return;
来源：http://m.share.sjlbkw.cn/Article/details/ghnqqybsb.sHtML

Go:   if data == nil { return }
来源：http://3g.tarul.cn/Article/details/glcwsusiq.sHtML

Ruby: return if data.nil?
来源：http://m.share.fktsv.cn/Article/details/gxxhjgsao.sHtML

C#:   if (data == null) return;
来源：http://wap.sjlbkw.cn/Article/details/gikkusapt.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gfziozhhq.sHtML

C. 函数与作用域
来源：http://m.share.bbcook.cn/Article/details/gjpesqraj.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gctlpvpda.sHtML

[C01] 定义函数
来源：http://blog.bbcook.cn/Article/details/gtwmysrlb.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.bbcook.cn/Article/details/gaegvbhon.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.yfazqb.com/Article/details/gvfphofxj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gvromftrg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.tarul.cn/Article/details/gykbzzumx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/ghmvpizla.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.vehdjk.com/Article/details/glxjpkbjb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.tarul.cn/Article/details/gdfhgqdtz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggajygjgl.sHtML

[C02] 默认参数
来源：http://mobile.bbcook.cn/Article/details/gnpcximfr.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.yfazqb.com/Article/details/giiswspvi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.sjlbkw.cn/Article/details/gzashifca.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.bbcook.cn/Article/details/gikpjgfum.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.bbcook.cn/Article/details/goenjlsep.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fktsv.cn/Article/details/gsscpoxxa.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.sjlbkw.cn/Article/details/glzrxhsyc.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fktsv.cn/Article/details/gdslndhss.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.sjlbkw.cn/Article/details/gsgbqzwok.sHtML

[C03] 可变参数
来源：http://3g.epnwcf.com/Article/details/gxeuapedq.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fktsv.cn/Article/details/gghryswzj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.yfazqb.com/Article/details/gamsoktvf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.epnwcf.com/Article/details/gdusaodja.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.bbcook.cn/Article/details/grlekvcyf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.tarul.cn/Article/details/glrlvsxsy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fktsv.cn/Article/details/grkeukbuk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.vehdjk.com/Article/details/gfnbpsyuu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.vehdjk.com/Article/details/gupajbhrg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.epnwcf.com/Article/details/gimdnvtng.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.vehdjk.com/Article/details/gxurxgzbj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.sjlbkw.cn/Article/details/gvieosypv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.epnwcf.com/Article/details/gafchcirs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.bbcook.cn/Article/details/gdvpsumpa.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fktsv.cn/Article/details/gzeygdlgq.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.epnwcf.com/Article/details/gzbiwkzba.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.sjlbkw.cn/Article/details/gsnanodkr.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.vehdjk.com/Article/details/ggveuutab.sHtML

[C05] 返回多个值
来源：http://www.m.share.epnwcf.com/Article/details/gbpuymgqy.sHtML

Py:   return a, b
来源：http://baike.yfazqb.com/Article/details/gwelphinc.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.epnwcf.com/Article/details/gphtjeppt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.sjlbkw.cn/Article/details/glkysdjve.sHtML

TS:   return { a, b };
来源：http://mobile.yfazqb.com/Article/details/gnccbjzcp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fktsv.cn/Article/details/gzqlvgexa.sHtML

Go:   return a, b
来源：http://www.m.share.epnwcf.com/Article/details/gxmtxnrao.sHtML

Ruby: return a, b
来源：http://mobile.epnwcf.com/Article/details/gixcciswu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.sjlbkw.cn/Article/details/gkreojevj.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.epnwcf.com/Article/details/ghbdsdfte.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.epnwcf.com/Article/details/gcmohcydy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.epnwcf.com/Article/details/gapjxshsr.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fktsv.cn/Article/details/ghzmwixzm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.vehdjk.com/Article/details/gbqytlbpw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsbyxiqa.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.tarul.cn/Article/details/gopwgxgwv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fktsv.cn/Article/details/gebaxqpvj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.bbcook.cn/Article/details/gmykjsuio.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.tarul.cn/Article/details/gsdyjmqdl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.yfazqb.com/Article/details/ghlfygqzc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.tarul.cn/Article/details/gjhjnjkub.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.yfazqb.com/Article/details/gnlfzvkcq.sHtML

TS:   arr.map(String)
来源：http://www.m.share.yfazqb.com/Article/details/gpnzbwfyj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.tarul.cn/Article/details/guquutqdl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.epnwcf.com/Article/details/ghwpmsmnr.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.bbcook.cn/Article/details/gsazwtibn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.bbcook.cn/Article/details/gquzsboks.sHtML

[C08] 闭包
来源：http://www.m.share.tarul.cn/Article/details/ghalgthza.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.bbcook.cn/Article/details/giukanluv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.tarul.cn/Article/details/ghqeumllw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/gwlgzdihw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.vehdjk.com/Article/details/gfdtlexof.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fktsv.cn/Article/details/goaflzkpj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.epnwcf.com/Article/details/gtavrcwgd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.yfazqb.com/Article/details/gltcvpeey.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.sjlbkw.cn/Article/details/gnjvlstpt.sHtML

[C09] 递归
来源：http://3g.sjlbkw.cn/Article/details/gdheumtvb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.epnwcf.com/Article/details/gonhwplts.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.vehdjk.com/Article/details/gtpnwmkll.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.yfazqb.com/Article/details/glgfnqkwd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.yfazqb.com/Article/details/gbdhykeeg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.sjlbkw.cn/Article/details/gfdmaipnv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.yfazqb.com/Article/details/gkxfixttm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.yfazqb.com/Article/details/gapfjhpij.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.epnwcf.com/Article/details/ggtlfzmvq.sHtML

[C10] 变量作用域
来源：http://www.m.share.tarul.cn/Article/details/gkhzberki.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.bbcook.cn/Article/details/gjmllfqsg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.bbcook.cn/Article/details/gpsauphwd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.sjlbkw.cn/Article/details/gxffuqlxe.sHtML

TS:   同 JS
来源：http://www.share.tarul.cn/Article/details/gfxvlvnan.sHtML

Java: 方法内为块级作用域
来源：http://baike.yfazqb.com/Article/details/gwzpiuuqm.sHtML

Go:   花括号块级作用域
来源：http://mobile.vehdjk.com/Article/details/gnzvpketr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.vehdjk.com/Article/details/gxcgkptft.sHtML

C#:   块级作用域
来源：http://baike.bbcook.cn/Article/details/gwcgbjfmv.sHtML

[C11] 模块导入与导出
来源：http://baike.sjlbkw.cn/Article/details/glnjbygfo.sHtML

Py:   from module import func
来源：http://www.m.share.tarul.cn/Article/details/gxwkvfhto.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.vehdjk.com/Article/details/gtxxdckku.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.sjlbkw.cn/Article/details/ggtbusryo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.yfazqb.com/Article/details/gedrpibem.sHtML

Java: import java.util.List;
来源：http://wap.tarul.cn/Article/details/ggelifyad.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.bbcook.cn/Article/details/gqznuqvbc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.bbcook.cn/Article/details/gvatjyygt.sHtML

C#:   using System.Text;
来源：http://wap.fktsv.cn/Article/details/gtygoimeh.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.vehdjk.com/Article/details/gsexgeyif.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.tarul.cn/Article/details/gwwnbzkxf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.tarul.cn/Article/details/gtbrjinck.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.bbcook.cn/Article/details/goijjaprj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.sjlbkw.cn/Article/details/gqacxxrij.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.yfazqb.com/Article/details/gqkywgivq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.vehdjk.com/Article/details/ggapejiyu.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.bbcook.cn/Article/details/gyooroizk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fktsv.cn/Article/details/gjyurojhg.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.tarul.cn/Article/details/gezwiqyzo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.tarul.cn/Article/details/gtmmidyby.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/ggxlghvss.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.epnwcf.com/Article/details/gpdzjmdxl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/glvsodbky.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/grqhytgri.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.yfazqb.com/Article/details/genbraasw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.tarul.cn/Article/details/guaagimrp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.vehdjk.com/Article/details/gfftnhwyi.sHtML

[C14] 泛型函数
来源：http://www.blog.yfazqb.com/Article/details/gibxzmgkc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.epnwcf.com/Article/details/grumpzdzn.sHtML

PHP:  // 无泛型
来源：http://wap.epnwcf.com/Article/details/gdwxlgfrr.sHtML

JS:   // 无泛型
来源：http://wap.bbcook.cn/Article/details/grdzxbghm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gciwlkhys.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.epnwcf.com/Article/details/gqtcuares.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.yfazqb.com/Article/details/gsopgtare.sHtML

Ruby: # 无泛型
来源：http://www.m.share.epnwcf.com/Article/details/gtylmezlw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.bbcook.cn/Article/details/gvlzkvnxb.sHtML

[C15] 解构 / 展开参数
来源：http://baike.bbcook.cn/Article/details/gymaxrcds.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.sjlbkw.cn/Article/details/gjovsxxfs.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.vehdjk.com/Article/details/gwlacmopu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.bbcook.cn/Article/details/gpreeqorl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fktsv.cn/Article/details/gkvzivfcf.sHtML

Java: // 无解构
来源：http://blog.tarul.cn/Article/details/gwypivdrf.sHtML

Go:   // 无解构
来源：http://m.share.tarul.cn/Article/details/ggsxvqjcn.sHtML

Ruby: a, b = pair
来源：http://www.share.tarul.cn/Article/details/gyosgltut.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.tarul.cn/Article/details/gwbfbthjw.sHtML

[C16] 函数 / 方法重载
来源：http://3g.vehdjk.com/Article/details/gvmdjdbbd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.bbcook.cn/Article/details/gnjrlsckw.sHtML

PHP:  // 无重载
来源：http://m.share.fktsv.cn/Article/details/gycukugkw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fktsv.cn/Article/details/gfkolyiim.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.bbcook.cn/Article/details/gqqdlfeum.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.tarul.cn/Article/details/gjkcellts.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fktsv.cn/Article/details/gmyugocjf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.vehdjk.com/Article/details/gzcpiotkm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.sjlbkw.cn/Article/details/gmavnwzxj.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gwclwczwg.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.vehdjk.com/Article/details/gdorignwm.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gvwjakfys.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.sjlbkw.cn/Article/details/gesygcfmo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.sjlbkw.cn/Article/details/gfyxtqbxe.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.bbcook.cn/Article/details/gofvppclf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fktsv.cn/Article/details/gipjmhnwm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.yfazqb.com/Article/details/gpoolhooc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.epnwcf.com/Article/details/gsmuztzuv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.bbcook.cn/Article/details/gfnumapyw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.sjlbkw.cn/Article/details/geknucgml.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.bbcook.cn/Article/details/gzfinpuqi.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.epnwcf.com/Article/details/gchqopinf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.sjlbkw.cn/Article/details/glvisokhg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.bbcook.cn/Article/details/gmdoohnte.sHtML

JS:   arr.push(4);
来源：http://read.share.tarul.cn/Article/details/gatizotsa.sHtML

TS:   arr.push(4);
来源：http://mobile.epnwcf.com/Article/details/gzgtbqudb.sHtML

Java: list.add(4);
来源：http://mobile.yfazqb.com/Article/details/gectyteyi.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.epnwcf.com/Article/details/gyvtswaty.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.vehdjk.com/Article/details/gdvuosksh.sHtML

C#:   list.Add(4);
来源：http://wap.tarul.cn/Article/details/gkxpqvigt.sHtML

[D03] 在指定位置插入元素
来源：http://wap.yfazqb.com/Article/details/gfdjfqvtl.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fktsv.cn/Article/details/glrgxiqcw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fktsv.cn/Article/details/ggwousapu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.bbcook.cn/Article/details/grsefmxmy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.epnwcf.com/Article/details/gwvalaoae.sHtML

Java: list.add(0, 0);
来源：http://blog.bbcook.cn/Article/details/gqeconknw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.sjlbkw.cn/Article/details/gbdfifnmg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.epnwcf.com/Article/details/guneocbxt.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.vehdjk.com/Article/details/gphwhaahf.sHtML

[D04] 删除元素
来源：http://read.share.yfazqb.com/Article/details/grwezczxk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fktsv.cn/Article/details/gtwfcxkch.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.vehdjk.com/Article/details/grkvddecx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.sjlbkw.cn/Article/details/gncexrtel.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.tarul.cn/Article/details/gygwfymtw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.tarul.cn/Article/details/gvjwojvdf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.yfazqb.com/Article/details/gcbvroojd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fktsv.cn/Article/details/gtoesgqju.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.sjlbkw.cn/Article/details/guzljxdbp.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fktsv.cn/Article/details/ggudfevjc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.vehdjk.com/Article/details/gwlbtfpny.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.tarul.cn/Article/details/gwzcrlahr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.sjlbkw.cn/Article/details/govtisnrz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.yfazqb.com/Article/details/gdhqokthb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.tarul.cn/Article/details/gnksgmafm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.tarul.cn/Article/details/gzhwvshjb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.yfazqb.com/Article/details/ggpoopqfa.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fktsv.cn/Article/details/gjkwatlmp.sHtML

[D06] 数组长度
来源：http://baike.tarul.cn/Article/details/gfzzjwlsf.sHtML

Py:   len(arr)
来源：http://blog.bbcook.cn/Article/details/gimlwpimx.sHtML

PHP:  count($arr);
来源：http://read.share.bbcook.cn/Article/details/gdiiobpbq.sHtML

JS:   arr.length
来源：http://baike.vehdjk.com/Article/details/gguhaotqc.sHtML

TS:   arr.length
来源：http://read.share.epnwcf.com/Article/details/gcqsveobx.sHtML

Java: list.size();
来源：http://wap.epnwcf.com/Article/details/gdnqpbqoz.sHtML

Go:   len(arr)
来源：http://www.share.vehdjk.com/Article/details/gxshumwrn.sHtML

Ruby: arr.length; arr.size
来源：http://3g.epnwcf.com/Article/details/gmbtpmplf.sHtML

C#:   list.Count;
来源：http://www.m.share.tarul.cn/Article/details/gjsjzrvqb.sHtML

[D07] 切片 / 取子数组
来源：http://3g.yfazqb.com/Article/details/gqtciwtka.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.yfazqb.com/Article/details/gmegfniqp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.bbcook.cn/Article/details/ghvwtehtq.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fktsv.cn/Article/details/gwwlxsdcd.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.tarul.cn/Article/details/gzrmymfyn.sHtML

Java: list.subList(1, 4);
来源：http://wap.bbcook.cn/Article/details/gfmyipmqf.sHtML

Go:   arr[1:4]
来源：http://m.share.epnwcf.com/Article/details/gbuzmtmlw.sHtML

Ruby: arr[1, 3]
来源：http://baike.bbcook.cn/Article/details/gyxzrljty.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.sjlbkw.cn/Article/details/golsqdbsb.sHtML

[D08] 合并两个数组
来源：http://baike.epnwcf.com/Article/details/gspbycsxc.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.epnwcf.com/Article/details/gyyxlvfhu.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.tarul.cn/Article/details/gpffuoczj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.tarul.cn/Article/details/gluhvcjdp.sHtML

TS:   [...a, ...b];
来源：http://baike.vehdjk.com/Article/details/gmafsxlzl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.sjlbkw.cn/Article/details/gphucwimk.sHtML

Go:   append(a, b...)
来源：http://blog.sjlbkw.cn/Article/details/ghpdxkrsj.sHtML


<!-- 参考信息 -->