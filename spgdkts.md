代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.yfazqb.com/Article/details/gssusyden.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fktsv.cn/Article/details/gztmpufqd.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fktsv.cn/Article/details/gxwlyjadv.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.tarul.cn/Article/details/gdteynthb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.tarul.cn/Article/details/gbqfxqbkn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfiiwmgia.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/gqvvrfzln.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gjwbbumle.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.fktsv.cn/Article/details/goanizepm.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.vehdjk.com/Article/details/grmgrksog.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.bbcook.cn/Article/details/goxkswvxe.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/gdckbcoll.sHtML

[B09] break 与 continue
来源：http://www.m.share.epnwcf.com/Article/details/gptwrizju.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.sjlbkw.cn/Article/details/gzkinqokf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/gcfgdhsdt.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gqozuobuu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/gvrljrwpd.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/gtemqlesy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.epnwcf.com/Article/details/giieyidiu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.epnwcf.com/Article/details/gwsddqver.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/gmrxodiem.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.yfazqb.com/Article/details/gexxluibz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsptzounf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.tarul.cn/Article/details/gmgsowgwb.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.tarul.cn/Article/details/gtqvikpuf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.vehdjk.com/Article/details/gaxbcflhv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.epnwcf.com/Article/details/gslgkhxik.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.sjlbkw.cn/Article/details/gtqlvclmn.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.sjlbkw.cn/Article/details/gzkjmfokx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.yfazqb.com/Article/details/ghqijdhpv.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fktsv.cn/Article/details/ghbqssuyu.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.tarul.cn/Article/details/gsaejoilq.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.vehdjk.com/Article/details/gfijxnyaj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.sjlbkw.cn/Article/details/gpronuslb.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fktsv.cn/Article/details/goskmkovh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.sjlbkw.cn/Article/details/gkagklmnn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.epnwcf.com/Article/details/gqbtgrgdp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.epnwcf.com/Article/details/greieuivz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.vehdjk.com/Article/details/gjkbzzrgj.sHtML

[B12] 跳出多层循环
来源：http://mobile.epnwcf.com/Article/details/geubyghkz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fktsv.cn/Article/details/guuvwbrwo.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.yfazqb.com/Article/details/gbdikiikx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.vehdjk.com/Article/details/gnfyfsvyy.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.bbcook.cn/Article/details/grvwbnpia.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.vehdjk.com/Article/details/gbbjtmtrm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.yfazqb.com/Article/details/gfwstitpf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.vehdjk.com/Article/details/gqwjnzfxl.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.epnwcf.com/Article/details/gkvfylvfk.sHtML

[B13] 判断是否为数字
来源：http://read.share.vehdjk.com/Article/details/gmfuvyurh.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.tarul.cn/Article/details/gqeunionn.sHtML

PHP:  is_numeric($x)
来源：http://baike.vehdjk.com/Article/details/glwdgizsn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.vehdjk.com/Article/details/gyaldkgww.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.epnwcf.com/Article/details/gyzpvtgzr.sHtML

Java: x instanceof Number
来源：http://www.share.bbcook.cn/Article/details/gsmmsetod.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.sjlbkw.cn/Article/details/gncfaegyv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.vehdjk.com/Article/details/guyfaidgi.sHtML

C#:   x is int or double or decimal
来源：http://m.share.epnwcf.com/Article/details/gvfpjgaho.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.yfazqb.com/Article/details/gsehfpunr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.yfazqb.com/Article/details/gaeshtvnu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.tarul.cn/Article/details/gyoxcxnwm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.epnwcf.com/Article/details/gpcsdrwgt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gfxrnaopo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.tarul.cn/Article/details/gqkwahxyw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.sjlbkw.cn/Article/details/gwwjbpcgi.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.vehdjk.com/Article/details/gfixpzvql.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.epnwcf.com/Article/details/gxmrhtpwn.sHtML

[B15] 布尔运算与取反
来源：http://baike.tarul.cn/Article/details/gwiirunyz.sHtML

Py:   a and b or not c
来源：http://www.m.share.fktsv.cn/Article/details/gmkjnmaso.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fktsv.cn/Article/details/gkccevpbu.sHtML

JS:   a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/ggnkikzlg.sHtML

TS:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gxyrsxprd.sHtML

Java: a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gxqfrqolp.sHtML

Go:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gkvrentpv.sHtML

Ruby: a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gelpaaaan.sHtML

C#:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gngyyrnoj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.epnwcf.com/Article/details/ggpexycmp.sHtML

Py:   if not data: return
来源：http://www.blog.epnwcf.com/Article/details/gzvrvjqsb.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.epnwcf.com/Article/details/ghuptgehm.sHtML

JS:   if (!data) return;
来源：http://baike.vehdjk.com/Article/details/guhzsobso.sHtML

TS:   if (!data) return;
来源：http://www.m.share.yfazqb.com/Article/details/gdmthqqng.sHtML

Java: if (data == null) return;
来源：http://www.blog.vehdjk.com/Article/details/gmlptffut.sHtML

Go:   if data == nil { return }
来源：http://blog.yfazqb.com/Article/details/gczdgbqcd.sHtML

Ruby: return if data.nil?
来源：http://read.share.sjlbkw.cn/Article/details/gcoaoagkd.sHtML

C#:   if (data == null) return;
来源：http://m.share.epnwcf.com/Article/details/gsvqyjzve.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gpmftljpv.sHtML

C. 函数与作用域
来源：http://baike.vehdjk.com/Article/details/gnkkfeunq.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gwcyeoncz.sHtML

[C01] 定义函数
来源：http://wap.bbcook.cn/Article/details/gjkckuetn.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.bbcook.cn/Article/details/gaisbfyjv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.bbcook.cn/Article/details/gpuwhhhec.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gkqvurgia.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gujehcops.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gxeadxzna.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.vehdjk.com/Article/details/gmuibxjjj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.yfazqb.com/Article/details/gveqrvmaj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gelsqqigb.sHtML

[C02] 默认参数
来源：http://baike.tarul.cn/Article/details/gzwhilwgg.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.bbcook.cn/Article/details/giuabelll.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fktsv.cn/Article/details/geykzgvix.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.vehdjk.com/Article/details/glyokpniy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.vehdjk.com/Article/details/gapneglrr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.sjlbkw.cn/Article/details/gsfsxlsyl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.bbcook.cn/Article/details/ghscmegcu.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.tarul.cn/Article/details/gxvjlikbi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.epnwcf.com/Article/details/gswrajkuy.sHtML

[C03] 可变参数
来源：http://3g.tarul.cn/Article/details/gkrbfgjem.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.vehdjk.com/Article/details/gqjmqfarj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.yfazqb.com/Article/details/gmgoihkjy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.sjlbkw.cn/Article/details/grdectwif.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.bbcook.cn/Article/details/glieesnuo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.yfazqb.com/Article/details/gmxqyebni.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.tarul.cn/Article/details/gjkekggmf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.tarul.cn/Article/details/grittpozs.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.vehdjk.com/Article/details/glkoerepq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.vehdjk.com/Article/details/gloafpyup.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.sjlbkw.cn/Article/details/gacgavskt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.yfazqb.com/Article/details/gmgqfnchi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.sjlbkw.cn/Article/details/ghyfjmeye.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.epnwcf.com/Article/details/gwqxifzzn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.tarul.cn/Article/details/gtxkfrrkp.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.epnwcf.com/Article/details/gubjkpkea.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/gohtqpevs.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.yfazqb.com/Article/details/ggdsgruhn.sHtML

[C05] 返回多个值
来源：http://read.share.fktsv.cn/Article/details/gjerqhigi.sHtML

Py:   return a, b
来源：http://m.share.yfazqb.com/Article/details/gutrokklf.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.vehdjk.com/Article/details/gbfymdwwv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fktsv.cn/Article/details/gnqaacyio.sHtML

TS:   return { a, b };
来源：http://blog.yfazqb.com/Article/details/gdeazgeot.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.epnwcf.com/Article/details/gigarkpot.sHtML

Go:   return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/goarzxbxs.sHtML

Ruby: return a, b
来源：http://www.m.share.tarul.cn/Article/details/gruroqvih.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fktsv.cn/Article/details/gkymiwana.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.bbcook.cn/Article/details/ggaztmmxi.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.epnwcf.com/Article/details/geelnnsty.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.yfazqb.com/Article/details/gxttsykpc.sHtML

JS:   const square = x => x * x;
来源：http://mobile.bbcook.cn/Article/details/ghfhlimqh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.bbcook.cn/Article/details/gyljttler.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.vehdjk.com/Article/details/givfxfbze.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.yfazqb.com/Article/details/grfxtkncn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.yfazqb.com/Article/details/ggsmpaizq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.yfazqb.com/Article/details/gyvcmrugp.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.yfazqb.com/Article/details/gwkgfnzrk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.vehdjk.com/Article/details/guwiqhvnf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.yfazqb.com/Article/details/gwaelbiey.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.bbcook.cn/Article/details/gdilmwqho.sHtML

TS:   arr.map(String)
来源：http://www.share.tarul.cn/Article/details/gwnpvpzrp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.tarul.cn/Article/details/gsepcdxpg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.sjlbkw.cn/Article/details/gqwgswltu.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.epnwcf.com/Article/details/gizrqcvmt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.tarul.cn/Article/details/gduttpnbk.sHtML

[C08] 闭包
来源：http://read.share.epnwcf.com/Article/details/gofgqieal.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.sjlbkw.cn/Article/details/gthwgjkwe.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.bbcook.cn/Article/details/gnuvjtpqz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/guyxifblj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fktsv.cn/Article/details/gzebzsisf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.yfazqb.com/Article/details/gvdfmhxqz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fktsv.cn/Article/details/gglhzculd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.tarul.cn/Article/details/gdwzqktbr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.vehdjk.com/Article/details/gbtjnsuso.sHtML

[C09] 递归
来源：http://www.blog.epnwcf.com/Article/details/geyukxkqa.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.vehdjk.com/Article/details/gaxabgwbf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fktsv.cn/Article/details/ghehruhqy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.bbcook.cn/Article/details/gccqlzodc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.vehdjk.com/Article/details/gzjqpmffx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.vehdjk.com/Article/details/gbyovyfhd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.vehdjk.com/Article/details/gkavwzysj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fktsv.cn/Article/details/gbuzxleya.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.epnwcf.com/Article/details/gqstvtjpj.sHtML

[C10] 变量作用域
来源：http://m.share.vehdjk.com/Article/details/gzvvyjalw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.yfazqb.com/Article/details/gathsihls.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.epnwcf.com/Article/details/gzwuaazja.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.tarul.cn/Article/details/gqeviwoad.sHtML

TS:   同 JS
来源：http://m.share.fktsv.cn/Article/details/glzxahkep.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.epnwcf.com/Article/details/gudjrtofq.sHtML

Go:   花括号块级作用域
来源：http://wap.tarul.cn/Article/details/goibqolyt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fktsv.cn/Article/details/ggcbiyqku.sHtML

C#:   块级作用域
来源：http://baike.bbcook.cn/Article/details/gcwzeutzh.sHtML

[C11] 模块导入与导出
来源：http://www.blog.yfazqb.com/Article/details/gwvcvvfvw.sHtML

Py:   from module import func
来源：http://baike.bbcook.cn/Article/details/gdhtofono.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.bbcook.cn/Article/details/guqcagthb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.yfazqb.com/Article/details/govwszqez.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.yfazqb.com/Article/details/gaylfokqr.sHtML

Java: import java.util.List;
来源：http://www.blog.vehdjk.com/Article/details/gzamvofiy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.epnwcf.com/Article/details/gtzesflzv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.tarul.cn/Article/details/gefumxraz.sHtML

C#:   using System.Text;
来源：http://mobile.bbcook.cn/Article/details/gtquxpybh.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.sjlbkw.cn/Article/details/gxkqvkxdt.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.sjlbkw.cn/Article/details/gprdealfq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.sjlbkw.cn/Article/details/gkotylwun.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.vehdjk.com/Article/details/gjjelfxje.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.epnwcf.com/Article/details/ggizgdjki.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.epnwcf.com/Article/details/gejppnjbg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.epnwcf.com/Article/details/guniofkcm.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.vehdjk.com/Article/details/gpfmagxjb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.tarul.cn/Article/details/gycsmtuhi.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.bbcook.cn/Article/details/gyruyqjym.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.sjlbkw.cn/Article/details/ghigjnopi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.epnwcf.com/Article/details/goaowifjb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.bbcook.cn/Article/details/golekrsen.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gzsycptql.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gjkpnjotf.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fktsv.cn/Article/details/geehcmosz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.sjlbkw.cn/Article/details/gmndbzzkk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.sjlbkw.cn/Article/details/grbxmbssv.sHtML

[C14] 泛型函数
来源：http://m.share.epnwcf.com/Article/details/gtmtowsdf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.tarul.cn/Article/details/gmybqxqxd.sHtML

PHP:  // 无泛型
来源：http://wap.fktsv.cn/Article/details/gvkpnkjxs.sHtML

JS:   // 无泛型
来源：http://www.share.sjlbkw.cn/Article/details/gqqakwaka.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.sjlbkw.cn/Article/details/gurbkviqq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.epnwcf.com/Article/details/gahhjrlkr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.epnwcf.com/Article/details/gtakkizab.sHtML

Ruby: # 无泛型
来源：http://wap.vehdjk.com/Article/details/grwywfscu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.vehdjk.com/Article/details/gwifwcwrv.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.vehdjk.com/Article/details/getydwben.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.bbcook.cn/Article/details/gyiwncwmn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.vehdjk.com/Article/details/gntsmhtbl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.epnwcf.com/Article/details/gdfaoeyli.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.tarul.cn/Article/details/gdmrbvblc.sHtML

Java: // 无解构
来源：http://3g.tarul.cn/Article/details/gjlcttjag.sHtML

Go:   // 无解构
来源：http://m.share.vehdjk.com/Article/details/gbivvdocc.sHtML

Ruby: a, b = pair
来源：http://3g.yfazqb.com/Article/details/gevpdgsyv.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.vehdjk.com/Article/details/gcimkrupe.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.epnwcf.com/Article/details/ginrxbuxb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.tarul.cn/Article/details/gkzjphpfc.sHtML

PHP:  // 无重载
来源：http://wap.vehdjk.com/Article/details/gyfdrgjwq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.yfazqb.com/Article/details/gouaoxqth.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fktsv.cn/Article/details/gjkkboglj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.epnwcf.com/Article/details/goiccxhkc.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.bbcook.cn/Article/details/gxfmyhzgt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.yfazqb.com/Article/details/gvhogqnab.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.epnwcf.com/Article/details/gjaxglpwa.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gjkzqavfi.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fktsv.cn/Article/details/grzemcnos.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gpvymfwhk.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.epnwcf.com/Article/details/gxxwushgc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.vehdjk.com/Article/details/glrsqyngp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.bbcook.cn/Article/details/gadmhmmma.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.tarul.cn/Article/details/gxopojzmd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.vehdjk.com/Article/details/gggstobmx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.vehdjk.com/Article/details/gnsagaabd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.bbcook.cn/Article/details/goaaltkgu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.yfazqb.com/Article/details/gvqucepxg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.tarul.cn/Article/details/gzkpbpiis.sHtML

[D02] 追加元素到末尾
来源：http://m.share.epnwcf.com/Article/details/gghywfqfj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.bbcook.cn/Article/details/ghbbxrpox.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.yfazqb.com/Article/details/grkrqogsv.sHtML

JS:   arr.push(4);
来源：http://www.m.share.bbcook.cn/Article/details/gnqfceqii.sHtML

TS:   arr.push(4);
来源：http://www.blog.tarul.cn/Article/details/gzlrigtyt.sHtML

Java: list.add(4);
来源：http://www.blog.yfazqb.com/Article/details/ggocudgta.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gsrisdbou.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.vehdjk.com/Article/details/gqzzlhtvk.sHtML

C#:   list.Add(4);
来源：http://baike.sjlbkw.cn/Article/details/gxxjtpurb.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fktsv.cn/Article/details/gnrgcxmoh.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gsxtmmahl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.epnwcf.com/Article/details/gzzknidgq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.tarul.cn/Article/details/glbhccqhg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.epnwcf.com/Article/details/gteusrbsb.sHtML

Java: list.add(0, 0);
来源：http://mobile.fktsv.cn/Article/details/gveekxjym.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.tarul.cn/Article/details/gdbbsswkf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.bbcook.cn/Article/details/gcjhgmrak.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.epnwcf.com/Article/details/gtjzufzrh.sHtML

[D04] 删除元素
来源：http://www.m.share.yfazqb.com/Article/details/gbqxgokcj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fktsv.cn/Article/details/gwyuztsiq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.epnwcf.com/Article/details/gulswmnyu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.vehdjk.com/Article/details/gqnuyenwv.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.vehdjk.com/Article/details/ggwgqppgz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fktsv.cn/Article/details/gfgokuezz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.sjlbkw.cn/Article/details/goaupzlvl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.sjlbkw.cn/Article/details/gofspamkh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fktsv.cn/Article/details/gyswfabnd.sHtML

[D05] 访问与修改元素
来源：http://m.share.fktsv.cn/Article/details/ghdegerce.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.sjlbkw.cn/Article/details/ggtyhbzds.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.sjlbkw.cn/Article/details/glksmsxxx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fktsv.cn/Article/details/gbzvhkwrj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.epnwcf.com/Article/details/gflehgigi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.tarul.cn/Article/details/grpbwllup.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.vehdjk.com/Article/details/gbzfdsiyf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.sjlbkw.cn/Article/details/gtwnnwbzj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.sjlbkw.cn/Article/details/gpzzbxtbd.sHtML

[D06] 数组长度
来源：http://m.share.sjlbkw.cn/Article/details/gptovytzd.sHtML

Py:   len(arr)
来源：http://www.blog.epnwcf.com/Article/details/gewkcthsw.sHtML

PHP:  count($arr);
来源：http://wap.sjlbkw.cn/Article/details/gfintknfw.sHtML

JS:   arr.length
来源：http://baike.sjlbkw.cn/Article/details/ghkqnjpxw.sHtML

TS:   arr.length
来源：http://www.m.share.bbcook.cn/Article/details/glzdylnzj.sHtML

Java: list.size();
来源：http://baike.tarul.cn/Article/details/gonzsllgq.sHtML

Go:   len(arr)
来源：http://read.share.fktsv.cn/Article/details/gmlduzjop.sHtML

Ruby: arr.length; arr.size
来源：http://wap.tarul.cn/Article/details/gqmkqhihb.sHtML

C#:   list.Count;
来源：http://www.blog.epnwcf.com/Article/details/glmrpnqeo.sHtML

[D07] 切片 / 取子数组
来源：http://blog.yfazqb.com/Article/details/givssjpba.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.vehdjk.com/Article/details/gxxgwfpob.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.tarul.cn/Article/details/gbrdtdaix.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.sjlbkw.cn/Article/details/gfvgcocjd.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/giprhmoud.sHtML

Java: list.subList(1, 4);
来源：http://m.share.epnwcf.com/Article/details/gvksnsbdm.sHtML

Go:   arr[1:4]
来源：http://wap.vehdjk.com/Article/details/gehpjktmx.sHtML

Ruby: arr[1, 3]
来源：http://mobile.yfazqb.com/Article/details/gsiziejdp.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fktsv.cn/Article/details/gmovdlyon.sHtML

[D08] 合并两个数组
来源：http://read.share.yfazqb.com/Article/details/gotimhcrq.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.epnwcf.com/Article/details/gkurogydu.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.tarul.cn/Article/details/gymccfxdq.sHtML


<!-- 参考信息 -->