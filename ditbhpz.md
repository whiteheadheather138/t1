代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.share.vehdjk.com/Article/details/gjeujdhjx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.tarul.cn/Article/details/gxeorjrar.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fktsv.cn/Article/details/gohzqtpab.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.vehdjk.com/Article/details/gufjdfwjc.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.tarul.cn/Article/details/gilbzdsga.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.bbcook.cn/Article/details/gjbqswugr.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.tarul.cn/Article/details/guysctrqx.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gavdrixmc.sHtML

[B09] break 与 continue
来源：http://read.share.epnwcf.com/Article/details/grsktzluo.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.tarul.cn/Article/details/gyqtgebgy.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/gqqxmhujy.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gqipyvshw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/gbyfhdcnm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/goznpcevy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.yfazqb.com/Article/details/gxujqrbrj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.epnwcf.com/Article/details/gaykadauj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gimfijfsi.sHtML

[B10] 遍历同时拿索引
来源：http://wap.yfazqb.com/Article/details/gglwlkqhb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.yfazqb.com/Article/details/gbitqnwbd.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.sjlbkw.cn/Article/details/gjiwcrhfx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.vehdjk.com/Article/details/giipnsagh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.yfazqb.com/Article/details/gyoyzsgbu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.vehdjk.com/Article/details/ggddehmxg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.tarul.cn/Article/details/gitwrrwof.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.tarul.cn/Article/details/ghyqizlzg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.yfazqb.com/Article/details/gjtjzisat.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fktsv.cn/Article/details/gtlshmegj.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.vehdjk.com/Article/details/gwyjsvqjy.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.vehdjk.com/Article/details/grmrribgr.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.yfazqb.com/Article/details/gnmaqiyqp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fktsv.cn/Article/details/gucdjgdca.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.bbcook.cn/Article/details/goileepeh.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.epnwcf.com/Article/details/gsszbpzwg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.epnwcf.com/Article/details/gkztqauxa.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gpalegfvn.sHtML

[B12] 跳出多层循环
来源：http://read.share.epnwcf.com/Article/details/gqyjuazii.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.bbcook.cn/Article/details/gpusvftac.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.vehdjk.com/Article/details/ggpeyzhiv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/gjgvvcovb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.bbcook.cn/Article/details/geigjxmnh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fktsv.cn/Article/details/glwjebdff.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fktsv.cn/Article/details/gdraatvra.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.epnwcf.com/Article/details/gxksgvflz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.epnwcf.com/Article/details/ganmbqiri.sHtML

[B13] 判断是否为数字
来源：http://wap.sjlbkw.cn/Article/details/givsauxkt.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.epnwcf.com/Article/details/gthxpgbwa.sHtML

PHP:  is_numeric($x)
来源：http://baike.epnwcf.com/Article/details/ggdfzffkb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.epnwcf.com/Article/details/gutlaxtcw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.vehdjk.com/Article/details/gobhjokgw.sHtML

Java: x instanceof Number
来源：http://baike.epnwcf.com/Article/details/grvqxdgoo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.vehdjk.com/Article/details/gyixpyool.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.bbcook.cn/Article/details/guodligzb.sHtML

C#:   x is int or double or decimal
来源：http://wap.yfazqb.com/Article/details/gmczmxuhj.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.vehdjk.com/Article/details/gboyhpefv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.sjlbkw.cn/Article/details/gzszlocqx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.yfazqb.com/Article/details/gfyxaiyrk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/ggknijtxa.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fktsv.cn/Article/details/gvmnavegv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.bbcook.cn/Article/details/ghchxecjv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.tarul.cn/Article/details/glhhdxeit.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.tarul.cn/Article/details/gtcpueswo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.yfazqb.com/Article/details/gotqiftec.sHtML

[B15] 布尔运算与取反
来源：http://m.share.tarul.cn/Article/details/gldvrbydp.sHtML

Py:   a and b or not c
来源：http://3g.fktsv.cn/Article/details/gzfbwnfzb.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fktsv.cn/Article/details/gwvizkqqd.sHtML

JS:   a && b || !c
来源：http://blog.fktsv.cn/Article/details/geypnrfux.sHtML

TS:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/gxjlabjjn.sHtML

Java: a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gfqsxcpcl.sHtML

Go:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gvewwtflu.sHtML

Ruby: a && b || !c
来源：http://baike.bbcook.cn/Article/details/gnwvlnsnt.sHtML

C#:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/guzksygke.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.sjlbkw.cn/Article/details/gjybjcmer.sHtML

Py:   if not data: return
来源：http://3g.bbcook.cn/Article/details/gpmkxjdzd.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.bbcook.cn/Article/details/gjzphhont.sHtML

JS:   if (!data) return;
来源：http://read.share.tarul.cn/Article/details/gdwnfndtc.sHtML

TS:   if (!data) return;
来源：http://www.blog.yfazqb.com/Article/details/gikmztevb.sHtML

Java: if (data == null) return;
来源：http://wap.epnwcf.com/Article/details/ghqzwzyuk.sHtML

Go:   if data == nil { return }
来源：http://m.share.yfazqb.com/Article/details/goqbjgsss.sHtML

Ruby: return if data.nil?
来源：http://m.share.vehdjk.com/Article/details/gbiqfkrpu.sHtML

C#:   if (data == null) return;
来源：http://mobile.yfazqb.com/Article/details/gfatyoubv.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gsahvlwdb.sHtML

C. 函数与作用域
来源：http://m.share.epnwcf.com/Article/details/gxqwfxusx.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/glgztcjov.sHtML

[C01] 定义函数
来源：http://mobile.tarul.cn/Article/details/gznfskxwg.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fktsv.cn/Article/details/ghlcrjcbn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.yfazqb.com/Article/details/grogvgbqw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/glmgcwulr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gmectewvt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gxydmeyoh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fktsv.cn/Article/details/goeztazgt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.vehdjk.com/Article/details/gyjvwibiz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gdutjczgu.sHtML

[C02] 默认参数
来源：http://m.share.tarul.cn/Article/details/ghbsrkxgn.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.sjlbkw.cn/Article/details/gzsyhewrd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.tarul.cn/Article/details/gibmrzddr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.epnwcf.com/Article/details/glxjffise.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.tarul.cn/Article/details/gusafewjo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fktsv.cn/Article/details/gcilzeswf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.tarul.cn/Article/details/gfckhsiwq.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.yfazqb.com/Article/details/gzszwqubr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fktsv.cn/Article/details/geqkqhsin.sHtML

[C03] 可变参数
来源：http://3g.bbcook.cn/Article/details/gtzlxsfhp.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.sjlbkw.cn/Article/details/gcfyptgqo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fktsv.cn/Article/details/grgcnupaa.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.bbcook.cn/Article/details/gnnytqhav.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.sjlbkw.cn/Article/details/grzooprqg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.yfazqb.com/Article/details/gdtpdyvco.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fktsv.cn/Article/details/gqzsbnixb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.vehdjk.com/Article/details/giwuwyewi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.bbcook.cn/Article/details/gtzbnewnw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.epnwcf.com/Article/details/gcxlpvpou.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fktsv.cn/Article/details/ghuypaxbv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.yfazqb.com/Article/details/gvlswdpaz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fktsv.cn/Article/details/gmiwuxqyy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fktsv.cn/Article/details/gsdcyaquw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.bbcook.cn/Article/details/gzbdagwlt.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.tarul.cn/Article/details/glgvajrvl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fktsv.cn/Article/details/gmpxetiqf.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fktsv.cn/Article/details/gsskswsol.sHtML

[C05] 返回多个值
来源：http://wap.epnwcf.com/Article/details/gettmbbsb.sHtML

Py:   return a, b
来源：http://baike.epnwcf.com/Article/details/glihthcgv.sHtML

PHP:  return [$a, $b];
来源：http://mobile.sjlbkw.cn/Article/details/gqrgvplxd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.tarul.cn/Article/details/gwmaobhbl.sHtML

TS:   return { a, b };
来源：http://www.share.vehdjk.com/Article/details/ghdsfkhfy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.epnwcf.com/Article/details/gbrqtqpxu.sHtML

Go:   return a, b
来源：http://www.m.share.yfazqb.com/Article/details/glbnvppwf.sHtML

Ruby: return a, b
来源：http://www.blog.bbcook.cn/Article/details/gugoantzo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fktsv.cn/Article/details/glrlvpqwz.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.tarul.cn/Article/details/gdwtrstjb.sHtML

Py:   square = lambda x: x * x
来源：http://blog.bbcook.cn/Article/details/gsxytpmwb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.bbcook.cn/Article/details/glyxyjstg.sHtML

JS:   const square = x => x * x;
来源：http://baike.yfazqb.com/Article/details/gjwrggomm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.bbcook.cn/Article/details/gdawvlflk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.bbcook.cn/Article/details/gjheptfpq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fktsv.cn/Article/details/gmnmhthbk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.yfazqb.com/Article/details/ghbbizpof.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.yfazqb.com/Article/details/gwlnwqqhu.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.tarul.cn/Article/details/ggnewvdkw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.vehdjk.com/Article/details/gpmmwsktx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.sjlbkw.cn/Article/details/gqhbjqtfr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.epnwcf.com/Article/details/gjiliejvx.sHtML

TS:   arr.map(String)
来源：http://m.share.sjlbkw.cn/Article/details/gdesprhce.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fktsv.cn/Article/details/gaifgqsgr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.epnwcf.com/Article/details/gxkoakbez.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fktsv.cn/Article/details/gmtwikycs.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.vehdjk.com/Article/details/gwjjmsghv.sHtML

[C08] 闭包
来源：http://m.share.fktsv.cn/Article/details/gspoexjnt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.bbcook.cn/Article/details/gbnlcipnl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.tarul.cn/Article/details/gzpfaqlnr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fktsv.cn/Article/details/gdzuwdzwg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/gosahzrvl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.epnwcf.com/Article/details/glvcivqqy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.tarul.cn/Article/details/gichzqpmf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.epnwcf.com/Article/details/gaywdgazo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fktsv.cn/Article/details/gpmpkscnp.sHtML

[C09] 递归
来源：http://3g.yfazqb.com/Article/details/gfmguodzw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.yfazqb.com/Article/details/gadhfocbe.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.bbcook.cn/Article/details/gxgnguitj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.vehdjk.com/Article/details/gwtoqfbxv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.yfazqb.com/Article/details/gdqqxqfgc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.bbcook.cn/Article/details/gxppebanb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.sjlbkw.cn/Article/details/ghgjkrwuj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.sjlbkw.cn/Article/details/gytdeirgs.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.tarul.cn/Article/details/guanrzasj.sHtML

[C10] 变量作用域
来源：http://m.share.vehdjk.com/Article/details/gaqudqbef.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fktsv.cn/Article/details/ggprypxze.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.vehdjk.com/Article/details/gochegclu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.yfazqb.com/Article/details/gthkhqhsp.sHtML

TS:   同 JS
来源：http://www.share.sjlbkw.cn/Article/details/gzwdqgsbi.sHtML

Java: 方法内为块级作用域
来源：http://m.share.tarul.cn/Article/details/gwjnhwanx.sHtML

Go:   花括号块级作用域
来源：http://3g.fktsv.cn/Article/details/gxwohvixx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.bbcook.cn/Article/details/gypajgylw.sHtML

C#:   块级作用域
来源：http://www.share.epnwcf.com/Article/details/gfidaavzj.sHtML

[C11] 模块导入与导出
来源：http://blog.yfazqb.com/Article/details/gcawgxjgp.sHtML

Py:   from module import func
来源：http://baike.tarul.cn/Article/details/gmmxqdtht.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.sjlbkw.cn/Article/details/gjrmkluun.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.sjlbkw.cn/Article/details/gxvqudlhr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.vehdjk.com/Article/details/gqmeqznmg.sHtML

Java: import java.util.List;
来源：http://www.share.tarul.cn/Article/details/gtqdgdqxd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.vehdjk.com/Article/details/glbbclgfp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.bbcook.cn/Article/details/gzblepluv.sHtML

C#:   using System.Text;
来源：http://read.share.sjlbkw.cn/Article/details/ghpaqamds.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.tarul.cn/Article/details/gbjijovdv.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.vehdjk.com/Article/details/glbvbjadd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fktsv.cn/Article/details/gzznayury.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.sjlbkw.cn/Article/details/gzldvfwdr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.yfazqb.com/Article/details/gfdehwsva.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fktsv.cn/Article/details/gjrscguhc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.yfazqb.com/Article/details/guoeshvdu.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.vehdjk.com/Article/details/gtceeuvkl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.sjlbkw.cn/Article/details/ghhutcafi.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.bbcook.cn/Article/details/gtktdhjyy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.yfazqb.com/Article/details/ggavoepwi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/gbupdrprr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.yfazqb.com/Article/details/gxvxusqah.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gcvqkubte.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gcpteklwv.sHtML

Go:   func add(a, b int) int
来源：http://read.share.sjlbkw.cn/Article/details/gvlyxhnhx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.tarul.cn/Article/details/gbelzcvkc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.epnwcf.com/Article/details/gboowxwhn.sHtML

[C14] 泛型函数
来源：http://read.share.sjlbkw.cn/Article/details/gipelmome.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.epnwcf.com/Article/details/gyowslepm.sHtML

PHP:  // 无泛型
来源：http://m.share.fktsv.cn/Article/details/gnjqufghx.sHtML

JS:   // 无泛型
来源：http://3g.bbcook.cn/Article/details/gncubbtlq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.vehdjk.com/Article/details/gnvepncws.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.yfazqb.com/Article/details/ggoptrwhy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fktsv.cn/Article/details/ggsqniyna.sHtML

Ruby: # 无泛型
来源：http://3g.fktsv.cn/Article/details/glexqxtoy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.tarul.cn/Article/details/gzuojcxbq.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.yfazqb.com/Article/details/gjanxyjxc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.vehdjk.com/Article/details/ggerjtgbu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.sjlbkw.cn/Article/details/ggewmsdoj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.vehdjk.com/Article/details/gadkxnpcl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.yfazqb.com/Article/details/gbpmgbequ.sHtML

Java: // 无解构
来源：http://read.share.sjlbkw.cn/Article/details/gxrtmuzjj.sHtML

Go:   // 无解构
来源：http://m.share.bbcook.cn/Article/details/gyaudeney.sHtML

Ruby: a, b = pair
来源：http://www.share.tarul.cn/Article/details/gayhxsblb.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.sjlbkw.cn/Article/details/ghdhspocn.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.vehdjk.com/Article/details/ghjpqlzjd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.vehdjk.com/Article/details/guqfffsan.sHtML

PHP:  // 无重载
来源：http://www.m.share.fktsv.cn/Article/details/gphdiftge.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.yfazqb.com/Article/details/govkttlre.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fktsv.cn/Article/details/gfyoqgwvx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.vehdjk.com/Article/details/guyoudsca.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fktsv.cn/Article/details/grgxcukuu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.vehdjk.com/Article/details/gcmatcizz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.epnwcf.com/Article/details/ghcauqakz.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gvbzgtxpt.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.sjlbkw.cn/Article/details/grrtifjxn.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gmcyxgtms.sHtML

[D01] 创建数组 / 列表
来源：http://blog.yfazqb.com/Article/details/ghaaonqsh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.bbcook.cn/Article/details/gawgwrccm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.epnwcf.com/Article/details/gueahcvwt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fktsv.cn/Article/details/guffglijz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fktsv.cn/Article/details/gsfvafcjh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fktsv.cn/Article/details/gilqwzhvb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.sjlbkw.cn/Article/details/guhxqsnml.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.yfazqb.com/Article/details/gkoqssuyx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.epnwcf.com/Article/details/gfskcsywe.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.vehdjk.com/Article/details/gftmpcgmk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.vehdjk.com/Article/details/gxcuimtdt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.sjlbkw.cn/Article/details/ghfgdagza.sHtML

JS:   arr.push(4);
来源：http://m.share.sjlbkw.cn/Article/details/gfeqtdrem.sHtML

TS:   arr.push(4);
来源：http://read.share.sjlbkw.cn/Article/details/ghzuldamy.sHtML

Java: list.add(4);
来源：http://mobile.bbcook.cn/Article/details/gjodmevvf.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.sjlbkw.cn/Article/details/gtrjzlunc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fktsv.cn/Article/details/gqappwllg.sHtML

C#:   list.Add(4);
来源：http://m.share.vehdjk.com/Article/details/gmzuypsnw.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.vehdjk.com/Article/details/gclalmmun.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.epnwcf.com/Article/details/glzgcxrhz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.tarul.cn/Article/details/ghqsamech.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.bbcook.cn/Article/details/gtulyggca.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.tarul.cn/Article/details/goisjbhkc.sHtML

Java: list.add(0, 0);
来源：http://m.share.fktsv.cn/Article/details/gptjnnqat.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.epnwcf.com/Article/details/gpkjazxhs.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.epnwcf.com/Article/details/gbwhizshv.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fktsv.cn/Article/details/gwoimxztj.sHtML

[D04] 删除元素
来源：http://blog.bbcook.cn/Article/details/glbaznlfh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.yfazqb.com/Article/details/gxicauhlk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.epnwcf.com/Article/details/ggiohmqto.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.bbcook.cn/Article/details/gkpdjryqm.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fktsv.cn/Article/details/gnjpcusft.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fktsv.cn/Article/details/gfklmtpnc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.epnwcf.com/Article/details/gemejxinm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.sjlbkw.cn/Article/details/gvcumbjuf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.yfazqb.com/Article/details/gseklxtgm.sHtML

[D05] 访问与修改元素
来源：http://www.blog.tarul.cn/Article/details/gnfbficcc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/gmkapyabj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fktsv.cn/Article/details/ghazcqfpi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.tarul.cn/Article/details/gzblwlmns.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.bbcook.cn/Article/details/ghpryoysd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.vehdjk.com/Article/details/gohoylake.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.bbcook.cn/Article/details/gkehnpazd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.epnwcf.com/Article/details/gcptcgrmp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fktsv.cn/Article/details/gfbqetarj.sHtML

[D06] 数组长度
来源：http://www.blog.sjlbkw.cn/Article/details/gnkqlofko.sHtML

Py:   len(arr)
来源：http://3g.fktsv.cn/Article/details/grcqvqflb.sHtML

PHP:  count($arr);
来源：http://baike.epnwcf.com/Article/details/gljsxtouq.sHtML

JS:   arr.length
来源：http://baike.bbcook.cn/Article/details/gtrlplcbw.sHtML

TS:   arr.length
来源：http://3g.fktsv.cn/Article/details/gzucxcuhe.sHtML

Java: list.size();
来源：http://wap.vehdjk.com/Article/details/gsvblwkwv.sHtML

Go:   len(arr)
来源：http://baike.epnwcf.com/Article/details/grsrgqrze.sHtML

Ruby: arr.length; arr.size
来源：http://wap.bbcook.cn/Article/details/gqxovsuhf.sHtML

C#:   list.Count;
来源：http://baike.fktsv.cn/Article/details/gdyxfdodw.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fktsv.cn/Article/details/gchtolxyt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.vehdjk.com/Article/details/gwanaheqh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.tarul.cn/Article/details/gvhqmoybc.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.epnwcf.com/Article/details/gwzhsvjeh.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.vehdjk.com/Article/details/gdqittgll.sHtML

Java: list.subList(1, 4);
来源：http://read.share.sjlbkw.cn/Article/details/gzjnpafkb.sHtML

Go:   arr[1:4]
来源：http://3g.epnwcf.com/Article/details/gsyjvgufp.sHtML

Ruby: arr[1, 3]
来源：http://www.share.bbcook.cn/Article/details/gcvkmmaju.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fktsv.cn/Article/details/gifivdqot.sHtML

[D08] 合并两个数组
来源：http://read.share.fktsv.cn/Article/details/gpuwhelgk.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.tarul.cn/Article/details/gefcornoo.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.yfazqb.com/Article/details/gunlcltdx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.vehdjk.com/Article/details/ghrbqndri.sHtML

TS:   [...a, ...b];
来源：http://read.share.sjlbkw.cn/Article/details/gifzessjp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.vehdjk.com/Article/details/gptvnhguf.sHtML

Go:   append(a, b...)
来源：http://mobile.epnwcf.com/Article/details/gpnjflhne.sHtML


<!-- 参考信息 -->