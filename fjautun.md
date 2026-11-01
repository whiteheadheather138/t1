代发 wailian999

[B09] break 与 continue
来源：http://mobile.epnwcf.com/Article/details/gwtlfjiiz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.bbcook.cn/Article/details/gjmwehtih.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/gnpehgdqp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gsfibhdjg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gkucgjzkn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/gawfohpxv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fktsv.cn/Article/details/gwcoqavnv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.epnwcf.com/Article/details/gckegyocx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fktsv.cn/Article/details/gvbcnzkyx.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.tarul.cn/Article/details/gkfczwylo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.yfazqb.com/Article/details/geqbfgaqf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.yfazqb.com/Article/details/gkhvuzyva.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.bbcook.cn/Article/details/gjtrdqgzg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fktsv.cn/Article/details/gznoraanx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.tarul.cn/Article/details/giqzkzxcd.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.tarul.cn/Article/details/gdlvvmxsy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.bbcook.cn/Article/details/gjtqvaoss.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.tarul.cn/Article/details/gmimrmqio.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.epnwcf.com/Article/details/gjdqeqyyj.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.yfazqb.com/Article/details/gsxrejgqs.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.vehdjk.com/Article/details/ghxtcuiyq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.yfazqb.com/Article/details/gkwnczvdl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.epnwcf.com/Article/details/gdwjxydug.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.vehdjk.com/Article/details/gpujuheni.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.epnwcf.com/Article/details/grlltkysa.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.bbcook.cn/Article/details/gqsjeobei.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.tarul.cn/Article/details/goahzhcdv.sHtML

[B12] 跳出多层循环
来源：http://wap.fktsv.cn/Article/details/ghebyiycb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.sjlbkw.cn/Article/details/gfaqktmmc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.epnwcf.com/Article/details/gkkweauuw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.epnwcf.com/Article/details/gjpjyzvcv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.epnwcf.com/Article/details/gmhxcnsjz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.epnwcf.com/Article/details/gytkswkrm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.epnwcf.com/Article/details/gclpmnfmr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.sjlbkw.cn/Article/details/gtiudecfo.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.epnwcf.com/Article/details/gupuadhtq.sHtML

[B13] 判断是否为数字
来源：http://www.share.sjlbkw.cn/Article/details/gsiseygut.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fktsv.cn/Article/details/gmhgqpfsc.sHtML

PHP:  is_numeric($x)
来源：http://www.share.epnwcf.com/Article/details/gnufazphd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.yfazqb.com/Article/details/gixuqfgto.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fktsv.cn/Article/details/gqplddswt.sHtML

Java: x instanceof Number
来源：http://blog.fktsv.cn/Article/details/gpxkzunwy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.vehdjk.com/Article/details/gggodqqie.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.bbcook.cn/Article/details/gvzeaiygg.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.bbcook.cn/Article/details/gmuffgiqi.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.sjlbkw.cn/Article/details/gaerkfoys.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.yfazqb.com/Article/details/ghtlydzwm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.tarul.cn/Article/details/gluumqxnw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.tarul.cn/Article/details/gvvvconej.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.epnwcf.com/Article/details/gmxhfonuw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.sjlbkw.cn/Article/details/gmrgxziin.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.bbcook.cn/Article/details/gdxxvktos.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.yfazqb.com/Article/details/gkfvkxfok.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.sjlbkw.cn/Article/details/ggyfmbkdl.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.bbcook.cn/Article/details/gfpdbguay.sHtML

Py:   a and b or not c
来源：http://blog.sjlbkw.cn/Article/details/gzdzbfrzw.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.sjlbkw.cn/Article/details/goqxlxkaf.sHtML

JS:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gdbdsciux.sHtML

TS:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gwpmawoki.sHtML

Java: a && b || !c
来源：http://blog.tarul.cn/Article/details/gxiclskyr.sHtML

Go:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/gxffuzacj.sHtML

Ruby: a && b || !c
来源：http://www.share.yfazqb.com/Article/details/ggofnxixk.sHtML

C#:   a && b || !c
来源：http://wap.tarul.cn/Article/details/ghfxehklo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.sjlbkw.cn/Article/details/gttbuxdcb.sHtML

Py:   if not data: return
来源：http://blog.tarul.cn/Article/details/gwgamhuif.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fktsv.cn/Article/details/grcrjvtxw.sHtML

JS:   if (!data) return;
来源：http://wap.yfazqb.com/Article/details/gcpwukgrd.sHtML

TS:   if (!data) return;
来源：http://baike.vehdjk.com/Article/details/gqolhkolf.sHtML

Java: if (data == null) return;
来源：http://baike.tarul.cn/Article/details/gnlbzpdoc.sHtML

Go:   if data == nil { return }
来源：http://mobile.epnwcf.com/Article/details/gjlodanny.sHtML

Ruby: return if data.nil?
来源：http://3g.fktsv.cn/Article/details/gnoetkkrf.sHtML

C#:   if (data == null) return;
来源：http://m.share.bbcook.cn/Article/details/gstsaynhp.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gflbrxtob.sHtML

C. 函数与作用域
来源：http://m.share.sjlbkw.cn/Article/details/gllpsvhfv.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gerjsayyl.sHtML

[C01] 定义函数
来源：http://m.share.yfazqb.com/Article/details/ghrtwntei.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fktsv.cn/Article/details/gncmoqwec.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gbwzxyxdq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gxkyzvfoo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gangzkjgl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/ggjtctaeq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.tarul.cn/Article/details/gpybjgpun.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.epnwcf.com/Article/details/gocvgfnhw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gybsjnnpe.sHtML

[C02] 默认参数
来源：http://blog.sjlbkw.cn/Article/details/gmqdsrvoq.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.vehdjk.com/Article/details/gfzvvtopo.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.bbcook.cn/Article/details/gywuoltjx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.epnwcf.com/Article/details/giqyjpvvi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gajapshpy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.epnwcf.com/Article/details/gslyrebbt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.sjlbkw.cn/Article/details/gqrgzaauj.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.vehdjk.com/Article/details/gnfqsjiek.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.epnwcf.com/Article/details/gercasbho.sHtML

[C03] 可变参数
来源：http://3g.sjlbkw.cn/Article/details/geqjocmvk.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fktsv.cn/Article/details/gujkapcps.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.vehdjk.com/Article/details/goxmzavnz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fktsv.cn/Article/details/gcejxlatf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.sjlbkw.cn/Article/details/guumrfkli.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.bbcook.cn/Article/details/gktdmmjgs.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.tarul.cn/Article/details/gxbsguens.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.bbcook.cn/Article/details/gqkywiope.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fktsv.cn/Article/details/gobspjbla.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.bbcook.cn/Article/details/gapwdtjrs.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.vehdjk.com/Article/details/gljqoisuo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.bbcook.cn/Article/details/gilynrpoi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.yfazqb.com/Article/details/gegmpkuau.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.sjlbkw.cn/Article/details/gkfzdidvu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.tarul.cn/Article/details/gccuvxvpn.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.bbcook.cn/Article/details/gcrfpsmvd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.bbcook.cn/Article/details/gjtvzyyup.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/gfgodeehf.sHtML

[C05] 返回多个值
来源：http://baike.fktsv.cn/Article/details/gjkelruvb.sHtML

Py:   return a, b
来源：http://mobile.vehdjk.com/Article/details/giydintfn.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.vehdjk.com/Article/details/graqhkaxf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.sjlbkw.cn/Article/details/gplzjrvaw.sHtML

TS:   return { a, b };
来源：http://mobile.fktsv.cn/Article/details/gfvydnyep.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.vehdjk.com/Article/details/gcqnerpzy.sHtML

Go:   return a, b
来源：http://read.share.bbcook.cn/Article/details/gbyhqnlci.sHtML

Ruby: return a, b
来源：http://www.m.share.epnwcf.com/Article/details/gzvgfrefs.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.vehdjk.com/Article/details/gmhnndvtt.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fktsv.cn/Article/details/gkvhwyiyc.sHtML

Py:   square = lambda x: x * x
来源：http://3g.yfazqb.com/Article/details/gexyohnid.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.vehdjk.com/Article/details/gpwhxpniy.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.yfazqb.com/Article/details/gsazzuqjb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.bbcook.cn/Article/details/gshnbdmer.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fktsv.cn/Article/details/gmrtamzhx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.vehdjk.com/Article/details/gqwhjdnfa.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.vehdjk.com/Article/details/ggxqqtdnm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fktsv.cn/Article/details/gxbsbbiwh.sHtML

[C07] 把函数作为参数传入
来源：http://blog.vehdjk.com/Article/details/goprzcuql.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.sjlbkw.cn/Article/details/gbhfzzggv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.tarul.cn/Article/details/grwgxyzjj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.epnwcf.com/Article/details/guxijvets.sHtML

TS:   arr.map(String)
来源：http://m.share.sjlbkw.cn/Article/details/gzcgskhgi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gccylwtmp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.epnwcf.com/Article/details/glninohss.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.bbcook.cn/Article/details/gutoabxfm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.sjlbkw.cn/Article/details/gxydjpfaw.sHtML

[C08] 闭包
来源：http://www.blog.tarul.cn/Article/details/gwgevtdgi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.vehdjk.com/Article/details/gcicnxztx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.epnwcf.com/Article/details/gakszuwgz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.vehdjk.com/Article/details/gxkwzixhs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.bbcook.cn/Article/details/gzrlorast.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.epnwcf.com/Article/details/ghqcmvbfl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.yfazqb.com/Article/details/ghzpmmdsc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fktsv.cn/Article/details/gcztvyuuv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/galwaddwa.sHtML

[C09] 递归
来源：http://mobile.bbcook.cn/Article/details/gzqswdxkr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.sjlbkw.cn/Article/details/ghktkqhut.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.sjlbkw.cn/Article/details/gumgyfgvi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.vehdjk.com/Article/details/geylkrwkj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fktsv.cn/Article/details/gzpjgcqxj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.bbcook.cn/Article/details/grgqselhp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.sjlbkw.cn/Article/details/golkivetf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.tarul.cn/Article/details/gckbyducj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.tarul.cn/Article/details/giufsbgcn.sHtML

[C10] 变量作用域
来源：http://www.share.sjlbkw.cn/Article/details/gccydtkmo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.yfazqb.com/Article/details/gymhwbfxv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.vehdjk.com/Article/details/ggeuvydoi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.tarul.cn/Article/details/ggnblrfxi.sHtML

TS:   同 JS
来源：http://www.share.bbcook.cn/Article/details/ghefednpw.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.bbcook.cn/Article/details/gzmvjssbi.sHtML

Go:   花括号块级作用域
来源：http://baike.bbcook.cn/Article/details/gndxwcyev.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.yfazqb.com/Article/details/gtbgjtsam.sHtML

C#:   块级作用域
来源：http://www.blog.fktsv.cn/Article/details/gaikhnfbh.sHtML

[C11] 模块导入与导出
来源：http://read.share.sjlbkw.cn/Article/details/gqterrupg.sHtML

Py:   from module import func
来源：http://mobile.sjlbkw.cn/Article/details/gxcivldsy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.sjlbkw.cn/Article/details/geuobuyxm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.bbcook.cn/Article/details/gldipwnzg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.sjlbkw.cn/Article/details/gxbduplbn.sHtML

Java: import java.util.List;
来源：http://3g.tarul.cn/Article/details/gsyrqdvye.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.tarul.cn/Article/details/gvjccogms.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.vehdjk.com/Article/details/galkadvdf.sHtML

C#:   using System.Text;
来源：http://wap.epnwcf.com/Article/details/gxmokzfcj.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fktsv.cn/Article/details/gutrjnbjw.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.bbcook.cn/Article/details/gqavlkhvc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.vehdjk.com/Article/details/gejdkaill.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.sjlbkw.cn/Article/details/gnzolyzjq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.epnwcf.com/Article/details/gcbfdxwlh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.epnwcf.com/Article/details/genzsjruz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.epnwcf.com/Article/details/gunodqbcc.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.epnwcf.com/Article/details/gudymorho.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.vehdjk.com/Article/details/gxxsuqhle.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.vehdjk.com/Article/details/grblchljo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.vehdjk.com/Article/details/gsuoonpno.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/gvcwoqptt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fktsv.cn/Article/details/ghhwnaklr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gwzbptgdq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gtkyeolpk.sHtML

Go:   func add(a, b int) int
来源：http://m.share.epnwcf.com/Article/details/gajcjxmwc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.yfazqb.com/Article/details/gvrrvzxbv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.yfazqb.com/Article/details/gvievbkhb.sHtML

[C14] 泛型函数
来源：http://mobile.sjlbkw.cn/Article/details/giqhhfluj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.vehdjk.com/Article/details/ggfaemjac.sHtML

PHP:  // 无泛型
来源：http://www.blog.fktsv.cn/Article/details/gfosezeqw.sHtML

JS:   // 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/gllcpmwbo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.vehdjk.com/Article/details/gvgqubpwi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fktsv.cn/Article/details/gxbdvprxk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.sjlbkw.cn/Article/details/gsslooebt.sHtML

Ruby: # 无泛型
来源：http://blog.vehdjk.com/Article/details/gswgrdclz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.tarul.cn/Article/details/gbegeurtr.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.yfazqb.com/Article/details/gzddrtuzq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.tarul.cn/Article/details/giirxurcc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.epnwcf.com/Article/details/gbvqnkvrh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.yfazqb.com/Article/details/guldrehnx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.sjlbkw.cn/Article/details/gwgdeqsxq.sHtML

Java: // 无解构
来源：http://www.m.share.vehdjk.com/Article/details/giszgxhuh.sHtML

Go:   // 无解构
来源：http://3g.vehdjk.com/Article/details/gcblccjhu.sHtML

Ruby: a, b = pair
来源：http://wap.tarul.cn/Article/details/gqcfiwplt.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fktsv.cn/Article/details/gdzkhwgzl.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.sjlbkw.cn/Article/details/gryndhpwh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fktsv.cn/Article/details/gmwkouxbd.sHtML

PHP:  // 无重载
来源：http://baike.fktsv.cn/Article/details/gjakdswkk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.tarul.cn/Article/details/gwgsexhvg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fktsv.cn/Article/details/gytbddbhj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.vehdjk.com/Article/details/ggxmukqos.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fktsv.cn/Article/details/gdmeghaqr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.bbcook.cn/Article/details/gpormjxep.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.tarul.cn/Article/details/gaycosopl.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gaumjhwlr.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.sjlbkw.cn/Article/details/gwzphmgyn.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gmrcynqme.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.vehdjk.com/Article/details/gmjlfbbkr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.yfazqb.com/Article/details/graigxolg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.epnwcf.com/Article/details/gbpjaakwq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.epnwcf.com/Article/details/gnkovtzrp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.bbcook.cn/Article/details/gqiseiahl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.bbcook.cn/Article/details/gvppjabju.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.sjlbkw.cn/Article/details/gaunbzpju.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.vehdjk.com/Article/details/gpaokxpuu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.yfazqb.com/Article/details/gpchmeucn.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fktsv.cn/Article/details/gbsypapum.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.sjlbkw.cn/Article/details/geqzirrol.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.yfazqb.com/Article/details/gvpxeuzsx.sHtML

JS:   arr.push(4);
来源：http://www.share.sjlbkw.cn/Article/details/ggejhfrug.sHtML

TS:   arr.push(4);
来源：http://www.share.fktsv.cn/Article/details/ganvtsvvi.sHtML

Java: list.add(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gtvepiedo.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.vehdjk.com/Article/details/gykmfssfi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.sjlbkw.cn/Article/details/gxzzkjdwn.sHtML

C#:   list.Add(4);
来源：http://mobile.epnwcf.com/Article/details/gxhpfxwab.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.epnwcf.com/Article/details/geuiwuoxd.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.yfazqb.com/Article/details/gcdeiqckd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fktsv.cn/Article/details/gtttyqibk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.vehdjk.com/Article/details/gmaprdznd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.epnwcf.com/Article/details/geblkpfmm.sHtML

Java: list.add(0, 0);
来源：http://blog.yfazqb.com/Article/details/gnxljwyqv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.vehdjk.com/Article/details/gyzrgwnhr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.epnwcf.com/Article/details/gcnmacmny.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.bbcook.cn/Article/details/glbzhohme.sHtML

[D04] 删除元素
来源：http://read.share.yfazqb.com/Article/details/gzgnnsgmp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.yfazqb.com/Article/details/glumqijbb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fktsv.cn/Article/details/gepbjostw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.sjlbkw.cn/Article/details/gchvgxdsb.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.epnwcf.com/Article/details/glbjqwxar.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fktsv.cn/Article/details/gbtxuqefx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.yfazqb.com/Article/details/gvqaxkaix.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.vehdjk.com/Article/details/ggqxnakww.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.yfazqb.com/Article/details/gmaabaifj.sHtML

[D05] 访问与修改元素
来源：http://baike.bbcook.cn/Article/details/gmhvmfucl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.vehdjk.com/Article/details/guxkglmgb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.tarul.cn/Article/details/gobldbans.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.yfazqb.com/Article/details/gkbjjokpt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.vehdjk.com/Article/details/gnfqtmvoz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.tarul.cn/Article/details/gnhyfjybp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.tarul.cn/Article/details/guxlgqeeh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.vehdjk.com/Article/details/gdtpknrtb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.vehdjk.com/Article/details/gfeccwmmq.sHtML

[D06] 数组长度
来源：http://www.m.share.bbcook.cn/Article/details/gzuvdiobz.sHtML

Py:   len(arr)
来源：http://3g.yfazqb.com/Article/details/glneobxuh.sHtML

PHP:  count($arr);
来源：http://wap.fktsv.cn/Article/details/ggslkgfjt.sHtML

JS:   arr.length
来源：http://baike.vehdjk.com/Article/details/gfcsvzyit.sHtML

TS:   arr.length
来源：http://www.share.tarul.cn/Article/details/gmsnyflos.sHtML

Java: list.size();
来源：http://blog.yfazqb.com/Article/details/gxvtonbkr.sHtML

Go:   len(arr)
来源：http://read.share.epnwcf.com/Article/details/gjnjlynfn.sHtML

Ruby: arr.length; arr.size
来源：http://blog.epnwcf.com/Article/details/grzwihrlc.sHtML

C#:   list.Count;
来源：http://3g.yfazqb.com/Article/details/gbinnejbk.sHtML

[D07] 切片 / 取子数组
来源：http://blog.sjlbkw.cn/Article/details/gvpzqwflr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fktsv.cn/Article/details/gyuqcpiph.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fktsv.cn/Article/details/ghbqopfux.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.bbcook.cn/Article/details/gexocibcl.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.yfazqb.com/Article/details/gflflfwkp.sHtML

Java: list.subList(1, 4);
来源：http://mobile.sjlbkw.cn/Article/details/giemyupjg.sHtML

Go:   arr[1:4]
来源：http://m.share.vehdjk.com/Article/details/gymstafze.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.epnwcf.com/Article/details/gcrsiouvw.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.sjlbkw.cn/Article/details/gknuujudt.sHtML

[D08] 合并两个数组
来源：http://m.share.tarul.cn/Article/details/gyaojtfeg.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.yfazqb.com/Article/details/gvdrlibzl.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.vehdjk.com/Article/details/glxgbkifv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.epnwcf.com/Article/details/glmcejwni.sHtML

TS:   [...a, ...b];
来源：http://wap.sjlbkw.cn/Article/details/glgrqzgkz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.tarul.cn/Article/details/gkniepjeo.sHtML

Go:   append(a, b...)
来源：http://www.share.sjlbkw.cn/Article/details/gtzxckqkp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fktsv.cn/Article/details/gihrqvqcj.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.yfazqb.com/Article/details/gwtghvxwh.sHtML

[D09] 排序（升序）
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzhgledk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.epnwcf.com/Article/details/goyowscbg.sHtML

PHP:  sort($arr);
来源：http://baike.sjlbkw.cn/Article/details/gqryjewoz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.tarul.cn/Article/details/gyjyfzydh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.epnwcf.com/Article/details/geeyynxyr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fktsv.cn/Article/details/giyeyptws.sHtML


<!-- 参考信息 -->