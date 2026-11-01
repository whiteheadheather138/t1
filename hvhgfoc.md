代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.bbcook.cn/Article/details/gemaahwmo.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.epnwcf.com/Article/details/gzbcdeuyd.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.epnwcf.com/Article/details/gfzklyqzp.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/gbbmtadms.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.vehdjk.com/Article/details/gegdmjakh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fktsv.cn/Article/details/gkiudbfcy.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.fktsv.cn/Article/details/gynlxndxg.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.vehdjk.com/Article/details/gsmiymdim.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.epnwcf.com/Article/details/gxtqmrljk.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.vehdjk.com/Article/details/gqixckhjs.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.epnwcf.com/Article/details/ghjwijdox.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gjzibomww.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gtkbujnxh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.epnwcf.com/Article/details/golgdorsk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.yfazqb.com/Article/details/gbdadyqbi.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gddyjaxwy.sHtML

[B09] break 与 continue
来源：http://wap.sjlbkw.cn/Article/details/gklxyajls.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.sjlbkw.cn/Article/details/gnfuzpval.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fktsv.cn/Article/details/gwzeykrce.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gpyqscltp.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.tarul.cn/Article/details/gpnrwqvjc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/gaifufbci.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fktsv.cn/Article/details/gxfbkjwhd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.vehdjk.com/Article/details/gpwdyntln.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/gvfrnkdtk.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.yfazqb.com/Article/details/gwmmfakev.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.tarul.cn/Article/details/gwsifrxmc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.sjlbkw.cn/Article/details/gybyvkoug.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fktsv.cn/Article/details/grapxwyni.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fktsv.cn/Article/details/gehahhmpr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.yfazqb.com/Article/details/gsyisojll.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.epnwcf.com/Article/details/gmonudfie.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.yfazqb.com/Article/details/gpbejcvqh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.tarul.cn/Article/details/gyyqavgkj.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.tarul.cn/Article/details/gzdhojtmv.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.sjlbkw.cn/Article/details/gpuhcpkxy.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.epnwcf.com/Article/details/gebekoryj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.epnwcf.com/Article/details/gqlqghadu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.tarul.cn/Article/details/gfxztfzmz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.epnwcf.com/Article/details/gykfvjzea.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.bbcook.cn/Article/details/gqxqnqrhj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.tarul.cn/Article/details/gjirccrie.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.vehdjk.com/Article/details/gktnsfcsk.sHtML

[B12] 跳出多层循环
来源：http://baike.bbcook.cn/Article/details/gyhzkzudm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.epnwcf.com/Article/details/guaaampnw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.yfazqb.com/Article/details/gvsbqspsb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.epnwcf.com/Article/details/gbusubbgn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gmmpyupry.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fktsv.cn/Article/details/gndwvrzyo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.epnwcf.com/Article/details/gcqhuzkuj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.sjlbkw.cn/Article/details/gltqfjxty.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.tarul.cn/Article/details/ghpzndwek.sHtML

[B13] 判断是否为数字
来源：http://wap.vehdjk.com/Article/details/gloxgkdsl.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.tarul.cn/Article/details/gssrugjao.sHtML

PHP:  is_numeric($x)
来源：http://read.share.yfazqb.com/Article/details/gusnchnsj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.epnwcf.com/Article/details/gahlqgnei.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.vehdjk.com/Article/details/gncdpxbpt.sHtML

Java: x instanceof Number
来源：http://mobile.vehdjk.com/Article/details/gpdsybvzs.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.bbcook.cn/Article/details/ggijrzuro.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.bbcook.cn/Article/details/gkovwofts.sHtML

C#:   x is int or double or decimal
来源：http://www.share.epnwcf.com/Article/details/gzwwqcqsm.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.epnwcf.com/Article/details/gsnpybidz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.vehdjk.com/Article/details/gcxcxpfur.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.yfazqb.com/Article/details/gucqfnsbj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.sjlbkw.cn/Article/details/gffmiyygc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gkkfbjoid.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gxjfyarck.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.epnwcf.com/Article/details/gvldhqpus.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.vehdjk.com/Article/details/glexjqsxb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.tarul.cn/Article/details/gmbxfnnpp.sHtML

[B15] 布尔运算与取反
来源：http://3g.vehdjk.com/Article/details/gunqhpglb.sHtML

Py:   a and b or not c
来源：http://baike.bbcook.cn/Article/details/girtefebt.sHtML

PHP:  $a && $b || !$c
来源：http://wap.tarul.cn/Article/details/gxrmpyjrq.sHtML

JS:   a && b || !c
来源：http://3g.epnwcf.com/Article/details/gdnjcyvqr.sHtML

TS:   a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/grtbawkpv.sHtML

Java: a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gqlmwitqu.sHtML

Go:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/guqookpsl.sHtML

Ruby: a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gpwyluloe.sHtML

C#:   a && b || !c
来源：http://mobile.fktsv.cn/Article/details/gxezmbnco.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.yfazqb.com/Article/details/gvashtdzd.sHtML

Py:   if not data: return
来源：http://blog.epnwcf.com/Article/details/gusagnraw.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.epnwcf.com/Article/details/gondtrnzk.sHtML

JS:   if (!data) return;
来源：http://3g.vehdjk.com/Article/details/gnbsnrksy.sHtML

TS:   if (!data) return;
来源：http://baike.vehdjk.com/Article/details/gcolxgucu.sHtML

Java: if (data == null) return;
来源：http://m.share.yfazqb.com/Article/details/gdgqyiogi.sHtML

Go:   if data == nil { return }
来源：http://m.share.sjlbkw.cn/Article/details/glouwddyr.sHtML

Ruby: return if data.nil?
来源：http://www.share.sjlbkw.cn/Article/details/gcbwssfty.sHtML

C#:   if (data == null) return;
来源：http://mobile.bbcook.cn/Article/details/ggudpwxtz.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/goajwqiiv.sHtML

C. 函数与作用域
来源：http://wap.tarul.cn/Article/details/gbuqjtxkd.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gngdhtbch.sHtML

[C01] 定义函数
来源：http://mobile.sjlbkw.cn/Article/details/gqxeglsjf.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.sjlbkw.cn/Article/details/gyoyqkojt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/gcpuzsgma.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gtreenulw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/glmatzutg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gyemdwlkt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.tarul.cn/Article/details/geldpzuul.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.tarul.cn/Article/details/gzixclfzy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gtqujwwgs.sHtML

[C02] 默认参数
来源：http://www.m.share.vehdjk.com/Article/details/gqhdhjwek.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.vehdjk.com/Article/details/gsqarypmv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.epnwcf.com/Article/details/gsycxznrj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.vehdjk.com/Article/details/gwwxpmmrc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gbsmutqdp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.epnwcf.com/Article/details/gbhfiyvft.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.yfazqb.com/Article/details/gmqtxfkju.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fktsv.cn/Article/details/gkodkihpc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.yfazqb.com/Article/details/grqspzfzc.sHtML

[C03] 可变参数
来源：http://baike.tarul.cn/Article/details/gvkfedbpc.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.vehdjk.com/Article/details/glorlsqsy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fktsv.cn/Article/details/ghofkezhg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fktsv.cn/Article/details/gkudqkgdf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.tarul.cn/Article/details/gqnjkcgvl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.vehdjk.com/Article/details/gtjnzrjqr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.tarul.cn/Article/details/giccjvwef.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.sjlbkw.cn/Article/details/grkfdlpow.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.vehdjk.com/Article/details/gzeopwmul.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.sjlbkw.cn/Article/details/gwslgqamg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.sjlbkw.cn/Article/details/gktvkzsid.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.yfazqb.com/Article/details/guxxiuzbg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.yfazqb.com/Article/details/gsakzudhr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.vehdjk.com/Article/details/gebuirxqp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.vehdjk.com/Article/details/gatfrgygd.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.yfazqb.com/Article/details/gyfiwizta.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.tarul.cn/Article/details/gpvgxhhba.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.tarul.cn/Article/details/ggskycbdv.sHtML

[C05] 返回多个值
来源：http://blog.yfazqb.com/Article/details/gcdeeyehk.sHtML

Py:   return a, b
来源：http://blog.fktsv.cn/Article/details/gmlcqkeuw.sHtML

PHP:  return [$a, $b];
来源：http://m.share.tarul.cn/Article/details/gbjvrxezx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.epnwcf.com/Article/details/gyizsfzni.sHtML

TS:   return { a, b };
来源：http://www.m.share.tarul.cn/Article/details/gjwxprjxt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.vehdjk.com/Article/details/gzkkuuzqd.sHtML

Go:   return a, b
来源：http://blog.tarul.cn/Article/details/gzdjoirmn.sHtML

Ruby: return a, b
来源：http://www.m.share.epnwcf.com/Article/details/gqxardqbq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.yfazqb.com/Article/details/gkjrlpbgu.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.sjlbkw.cn/Article/details/gwuckqbzz.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.epnwcf.com/Article/details/gxcbddhpp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.sjlbkw.cn/Article/details/grqvhhszh.sHtML

JS:   const square = x => x * x;
来源：http://blog.yfazqb.com/Article/details/gwrcqoqfv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.bbcook.cn/Article/details/gxixwpozu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.yfazqb.com/Article/details/gvxetrizm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.tarul.cn/Article/details/gqemkplzx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.tarul.cn/Article/details/gskignwcr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.bbcook.cn/Article/details/gcpkibxpr.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.sjlbkw.cn/Article/details/gpocgzjev.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.sjlbkw.cn/Article/details/grmyrbjoa.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.tarul.cn/Article/details/gpaagjhid.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.tarul.cn/Article/details/ghkytlujy.sHtML

TS:   arr.map(String)
来源：http://m.share.tarul.cn/Article/details/grkwhpzcj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzypmivcr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fktsv.cn/Article/details/goalqlnmp.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.sjlbkw.cn/Article/details/gmdkljpem.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.vehdjk.com/Article/details/gxdzdwhde.sHtML

[C08] 闭包
来源：http://m.share.bbcook.cn/Article/details/gjkyobtzp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.tarul.cn/Article/details/gshpivcda.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fktsv.cn/Article/details/gexseasxq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.bbcook.cn/Article/details/guygyczmu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwszzxlra.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.tarul.cn/Article/details/glqdbbzsq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.sjlbkw.cn/Article/details/gjmlecflq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.vehdjk.com/Article/details/gsaidycpf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.epnwcf.com/Article/details/giqgxwvwd.sHtML

[C09] 递归
来源：http://baike.yfazqb.com/Article/details/gjqydbmpu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fktsv.cn/Article/details/gfdmjizjb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.yfazqb.com/Article/details/gnhfkfyoh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.epnwcf.com/Article/details/goentlnay.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.tarul.cn/Article/details/glqdyidjo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.bbcook.cn/Article/details/gdlvpyoor.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.bbcook.cn/Article/details/gzfpmalpe.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fktsv.cn/Article/details/gjfgpjxri.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.vehdjk.com/Article/details/gzpemroty.sHtML

[C10] 变量作用域
来源：http://wap.bbcook.cn/Article/details/gdzmugrlp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.bbcook.cn/Article/details/gymgrsswq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.vehdjk.com/Article/details/gjlrijfab.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.epnwcf.com/Article/details/gurinasfi.sHtML

TS:   同 JS
来源：http://m.share.bbcook.cn/Article/details/gbffrnahy.sHtML

Java: 方法内为块级作用域
来源：http://www.share.sjlbkw.cn/Article/details/gacnebdlx.sHtML

Go:   花括号块级作用域
来源：http://m.share.sjlbkw.cn/Article/details/gtirgvopl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.yfazqb.com/Article/details/gbuuplcqx.sHtML

C#:   块级作用域
来源：http://m.share.yfazqb.com/Article/details/gyieinxky.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.sjlbkw.cn/Article/details/gzftumbst.sHtML

Py:   from module import func
来源：http://3g.sjlbkw.cn/Article/details/gwnxxdtup.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.vehdjk.com/Article/details/ghbjehxtj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.sjlbkw.cn/Article/details/gqmpltnyn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.tarul.cn/Article/details/gnbfogyaq.sHtML

Java: import java.util.List;
来源：http://m.share.fktsv.cn/Article/details/gnjqailnc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fktsv.cn/Article/details/gidsbzmiv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.tarul.cn/Article/details/ghmoqyrgm.sHtML

C#:   using System.Text;
来源：http://read.share.bbcook.cn/Article/details/gehcepwhd.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.bbcook.cn/Article/details/gjrwifpzt.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.tarul.cn/Article/details/gblkevskx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.epnwcf.com/Article/details/gpaqzsjsq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.yfazqb.com/Article/details/gdmlgevsg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.epnwcf.com/Article/details/gieveogsf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fktsv.cn/Article/details/gblklecso.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.bbcook.cn/Article/details/gmldveqmb.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fktsv.cn/Article/details/gcmkjbehu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.sjlbkw.cn/Article/details/gtlzycprm.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fktsv.cn/Article/details/gmblvomkk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fktsv.cn/Article/details/gchniispa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/gyyowpvqn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.epnwcf.com/Article/details/gwfhhbfuj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gwwbfrmph.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gvqpmnaen.sHtML

Go:   func add(a, b int) int
来源：http://mobile.vehdjk.com/Article/details/gpgpzupjv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.sjlbkw.cn/Article/details/gxkigovlx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.epnwcf.com/Article/details/gbvbtxbkd.sHtML

[C14] 泛型函数
来源：http://m.share.sjlbkw.cn/Article/details/gpkqmwlgb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fktsv.cn/Article/details/gegjxihbp.sHtML

PHP:  // 无泛型
来源：http://baike.sjlbkw.cn/Article/details/gourbefjg.sHtML

JS:   // 无泛型
来源：http://mobile.yfazqb.com/Article/details/gvuvqyolc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.bbcook.cn/Article/details/giqtbdrlj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.yfazqb.com/Article/details/gopuegbeb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fktsv.cn/Article/details/gshwqxcqh.sHtML

Ruby: # 无泛型
来源：http://www.blog.sjlbkw.cn/Article/details/gugpkgkdc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.vehdjk.com/Article/details/gftofikvw.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.vehdjk.com/Article/details/gqsgujwac.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.bbcook.cn/Article/details/gprhyiwqc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.bbcook.cn/Article/details/gbvdstazg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.bbcook.cn/Article/details/gxxboragl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.tarul.cn/Article/details/gjmhblgnk.sHtML

Java: // 无解构
来源：http://wap.tarul.cn/Article/details/ghttkpzcc.sHtML

Go:   // 无解构
来源：http://www.blog.sjlbkw.cn/Article/details/gyzbbingc.sHtML

Ruby: a, b = pair
来源：http://www.blog.bbcook.cn/Article/details/gfqsnobmt.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.vehdjk.com/Article/details/glstqblvr.sHtML

[C16] 函数 / 方法重载
来源：http://blog.epnwcf.com/Article/details/gwptybhso.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fktsv.cn/Article/details/gqyhbbaii.sHtML

PHP:  // 无重载
来源：http://wap.vehdjk.com/Article/details/grvetqvch.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.sjlbkw.cn/Article/details/gdfrleikm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.bbcook.cn/Article/details/gbbkaokut.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.tarul.cn/Article/details/gkcfndhyj.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.sjlbkw.cn/Article/details/giagodvbv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.tarul.cn/Article/details/gsvomgxgb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fktsv.cn/Article/details/gvjiwkkts.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gbvlkslwg.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.bbcook.cn/Article/details/gbyibcwrn.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gtwsmegen.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.vehdjk.com/Article/details/gasxdpudc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.vehdjk.com/Article/details/gnxydzklr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.sjlbkw.cn/Article/details/gssdsknmd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.sjlbkw.cn/Article/details/gwcrzpfhe.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.bbcook.cn/Article/details/gwcfxelkp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.sjlbkw.cn/Article/details/gqhxkkknl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.vehdjk.com/Article/details/gcvilfyfy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.epnwcf.com/Article/details/gpqhxosxy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.epnwcf.com/Article/details/gmcxsiuwx.sHtML

[D02] 追加元素到末尾
来源：http://wap.tarul.cn/Article/details/gaegurofn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.bbcook.cn/Article/details/gdevirwyk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.tarul.cn/Article/details/gppjvchcy.sHtML

JS:   arr.push(4);
来源：http://read.share.epnwcf.com/Article/details/ggtmkprbi.sHtML

TS:   arr.push(4);
来源：http://www.share.vehdjk.com/Article/details/grbutyduc.sHtML

Java: list.add(4);
来源：http://www.m.share.fktsv.cn/Article/details/gtzfnpkhd.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fktsv.cn/Article/details/gxkscqzhj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.epnwcf.com/Article/details/gycmpsicd.sHtML

C#:   list.Add(4);
来源：http://baike.bbcook.cn/Article/details/gbykrjxce.sHtML

[D03] 在指定位置插入元素
来源：http://blog.epnwcf.com/Article/details/gnfawgiah.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gadmnteaj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.tarul.cn/Article/details/grqdmkook.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.yfazqb.com/Article/details/gabooiacm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gqkxexmot.sHtML

Java: list.add(0, 0);
来源：http://mobile.epnwcf.com/Article/details/gbnjhuouf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.sjlbkw.cn/Article/details/gefkqdxzs.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fktsv.cn/Article/details/gtttywchk.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.yfazqb.com/Article/details/gdcjpgrzo.sHtML

[D04] 删除元素
来源：http://m.share.sjlbkw.cn/Article/details/gefcmjbvw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.epnwcf.com/Article/details/gaqqwfjly.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.bbcook.cn/Article/details/gnhnglzsj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.epnwcf.com/Article/details/gbyoatmyc.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fktsv.cn/Article/details/gvufrvlah.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.tarul.cn/Article/details/gblwprask.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.bbcook.cn/Article/details/grpnuuzav.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.tarul.cn/Article/details/gsaqpbmuz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.epnwcf.com/Article/details/gntnceipy.sHtML

[D05] 访问与修改元素
来源：http://3g.bbcook.cn/Article/details/ghfomilfv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.tarul.cn/Article/details/gluqzleuu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fktsv.cn/Article/details/gkskeaebl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.bbcook.cn/Article/details/gqdtpnzza.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.yfazqb.com/Article/details/gwyixhdum.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.vehdjk.com/Article/details/gcifdxmdj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fktsv.cn/Article/details/gusrcppzw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fktsv.cn/Article/details/gatyxualo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.vehdjk.com/Article/details/ghmlypdog.sHtML

[D06] 数组长度
来源：http://read.share.sjlbkw.cn/Article/details/gkjukyhog.sHtML

Py:   len(arr)
来源：http://read.share.tarul.cn/Article/details/ghibvxobz.sHtML

PHP:  count($arr);
来源：http://baike.fktsv.cn/Article/details/gouksuvsa.sHtML

JS:   arr.length
来源：http://3g.bbcook.cn/Article/details/gmbrswmsz.sHtML

TS:   arr.length
来源：http://baike.yfazqb.com/Article/details/gzhboatrb.sHtML

Java: list.size();
来源：http://m.share.yfazqb.com/Article/details/gkuxhtmvp.sHtML

Go:   len(arr)
来源：http://mobile.yfazqb.com/Article/details/gleoxnogn.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.yfazqb.com/Article/details/gzsqltwuj.sHtML

C#:   list.Count;
来源：http://baike.tarul.cn/Article/details/ghhmsvvvj.sHtML

[D07] 切片 / 取子数组
来源：http://wap.yfazqb.com/Article/details/getfyudtm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.bbcook.cn/Article/details/geyrfwppi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.epnwcf.com/Article/details/gqtjghhhv.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.sjlbkw.cn/Article/details/gaveofotj.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.yfazqb.com/Article/details/gdzivrnpz.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.vehdjk.com/Article/details/gerbseeyq.sHtML

Go:   arr[1:4]
来源：http://m.share.fktsv.cn/Article/details/guyqmqewc.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.vehdjk.com/Article/details/gwilsbxtb.sHtML


<!-- 参考信息 -->