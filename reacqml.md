代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://3g.bbcook.cn/Article/details/gzyjntcft.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.epnwcf.com/Article/details/guoiodxuo.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/givlyuvgf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/gchawbahc.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.vehdjk.com/Article/details/guormtgwx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.sjlbkw.cn/Article/details/ggecujjng.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.vehdjk.com/Article/details/gvaplffxs.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.epnwcf.com/Article/details/gukdntuuy.sHtML

[B09] break 与 continue
来源：http://www.blog.epnwcf.com/Article/details/gkkqdondq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.sjlbkw.cn/Article/details/gahprblku.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gvyfqskva.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gmovmijse.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/gccafdrim.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gtelsjcyq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.vehdjk.com/Article/details/gpibamdcm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.yfazqb.com/Article/details/glsqsgbpd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/ggfjkiwjb.sHtML

[B10] 遍历同时拿索引
来源：http://wap.vehdjk.com/Article/details/gtqiuwrqu.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.epnwcf.com/Article/details/gqhylgakh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.bbcook.cn/Article/details/gjrzfrhiy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.sjlbkw.cn/Article/details/glcrluykq.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.vehdjk.com/Article/details/gqevwmhcf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.yfazqb.com/Article/details/gygrmjnzf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.tarul.cn/Article/details/gtpqceegj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fktsv.cn/Article/details/gedmipcka.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.tarul.cn/Article/details/gvtjrrhdb.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.sjlbkw.cn/Article/details/gcpolxpxx.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.tarul.cn/Article/details/gnqpwcmor.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.epnwcf.com/Article/details/gvldwwwzp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fktsv.cn/Article/details/gzwgvjqvi.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.vehdjk.com/Article/details/gxnzotfez.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.tarul.cn/Article/details/gzlnywuwf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.vehdjk.com/Article/details/ggddapghk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.epnwcf.com/Article/details/geywnlmjm.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.epnwcf.com/Article/details/gcmxbepqv.sHtML

[B12] 跳出多层循环
来源：http://baike.bbcook.cn/Article/details/grikcrgyd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.tarul.cn/Article/details/guzpkyuch.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.bbcook.cn/Article/details/gvxfilmvw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.sjlbkw.cn/Article/details/gltqxiqem.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.sjlbkw.cn/Article/details/guvcsiwpv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.vehdjk.com/Article/details/gtxmiwbsd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.sjlbkw.cn/Article/details/gqrgnuerw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fktsv.cn/Article/details/guuwinznf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.epnwcf.com/Article/details/ggfjyecyh.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.tarul.cn/Article/details/gzcxntrqv.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.bbcook.cn/Article/details/gswvemiar.sHtML

PHP:  is_numeric($x)
来源：http://www.share.sjlbkw.cn/Article/details/gbdjrbzle.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.bbcook.cn/Article/details/gjqgabevv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.sjlbkw.cn/Article/details/gtdhcpvjl.sHtML

Java: x instanceof Number
来源：http://3g.tarul.cn/Article/details/gatoohjmd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fktsv.cn/Article/details/gkqsnqqco.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fktsv.cn/Article/details/glwxvmpbh.sHtML

C#:   x is int or double or decimal
来源：http://wap.vehdjk.com/Article/details/gyzeebytb.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fktsv.cn/Article/details/gimgxcwyg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fktsv.cn/Article/details/gkybiflol.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.tarul.cn/Article/details/gtgmjjtyc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.bbcook.cn/Article/details/gfpggbdvg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.yfazqb.com/Article/details/gfjypkhkl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.yfazqb.com/Article/details/gvtslwvrl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.epnwcf.com/Article/details/gzrjuavkm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.bbcook.cn/Article/details/gsnjxtchq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.yfazqb.com/Article/details/gfwdwxroy.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqflpxkz.sHtML

Py:   a and b or not c
来源：http://baike.tarul.cn/Article/details/gaxoecimv.sHtML

PHP:  $a && $b || !$c
来源：http://baike.tarul.cn/Article/details/gnxjkmgaz.sHtML

JS:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/goxaivlxm.sHtML

TS:   a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/gleqktqzl.sHtML

Java: a && b || !c
来源：http://wap.epnwcf.com/Article/details/gjgpokonl.sHtML

Go:   a && b || !c
来源：http://www.share.yfazqb.com/Article/details/glxheqnka.sHtML

Ruby: a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/grufexgxa.sHtML

C#:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gdcynwueg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.sjlbkw.cn/Article/details/gzddmrrvu.sHtML

Py:   if not data: return
来源：http://mobile.bbcook.cn/Article/details/gdvsnnone.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.yfazqb.com/Article/details/gjlivqjwe.sHtML

JS:   if (!data) return;
来源：http://mobile.tarul.cn/Article/details/gjcpmgjje.sHtML

TS:   if (!data) return;
来源：http://wap.fktsv.cn/Article/details/gzpgmjyzu.sHtML

Java: if (data == null) return;
来源：http://m.share.yfazqb.com/Article/details/gltxdtgqz.sHtML

Go:   if data == nil { return }
来源：http://baike.bbcook.cn/Article/details/gazxglola.sHtML

Ruby: return if data.nil?
来源：http://mobile.yfazqb.com/Article/details/gygqdsqgy.sHtML

C#:   if (data == null) return;
来源：http://www.blog.yfazqb.com/Article/details/gqaodqwcr.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gemjzekkx.sHtML

C. 函数与作用域
来源：http://3g.epnwcf.com/Article/details/gvloqqdln.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gqakwsodl.sHtML

[C01] 定义函数
来源：http://3g.fktsv.cn/Article/details/gfajkbyki.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.epnwcf.com/Article/details/gvngxstpi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.sjlbkw.cn/Article/details/gvxnkucfl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/guwcngoei.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gwjdyhyrs.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gwvczonyg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.epnwcf.com/Article/details/giycywvgc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.bbcook.cn/Article/details/gnkegrmuy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gikppmxyp.sHtML

[C02] 默认参数
来源：http://read.share.vehdjk.com/Article/details/gdjjuound.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.sjlbkw.cn/Article/details/gmjnujztu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.epnwcf.com/Article/details/gbrcccrka.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fktsv.cn/Article/details/giackoflo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.tarul.cn/Article/details/ghybdgewe.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.sjlbkw.cn/Article/details/gflrspcjl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.yfazqb.com/Article/details/gjsafsrsm.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.yfazqb.com/Article/details/gljzdokfo.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.epnwcf.com/Article/details/gxermfmde.sHtML

[C03] 可变参数
来源：http://baike.vehdjk.com/Article/details/gozhcwapl.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.vehdjk.com/Article/details/ggxaoiklh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.sjlbkw.cn/Article/details/gwajsxkwv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.bbcook.cn/Article/details/gopjeycox.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.tarul.cn/Article/details/gdudhlihq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.bbcook.cn/Article/details/gshmrdvvu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.tarul.cn/Article/details/gjrjbleol.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.tarul.cn/Article/details/gllqhxmjm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.sjlbkw.cn/Article/details/gcbcvhseo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.yfazqb.com/Article/details/gbqxnzfre.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.tarul.cn/Article/details/gspgocctb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.bbcook.cn/Article/details/gdbgowokm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.tarul.cn/Article/details/gresvgfvy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fktsv.cn/Article/details/gwydhejoy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fktsv.cn/Article/details/gvfythvok.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.tarul.cn/Article/details/gxhuzybln.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.sjlbkw.cn/Article/details/gjmnxcezv.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.bbcook.cn/Article/details/gyglemcni.sHtML

[C05] 返回多个值
来源：http://www.share.epnwcf.com/Article/details/gdgoxvrip.sHtML

Py:   return a, b
来源：http://baike.tarul.cn/Article/details/gquhczkts.sHtML

PHP:  return [$a, $b];
来源：http://m.share.bbcook.cn/Article/details/glgprmqpg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.vehdjk.com/Article/details/gqvoqfbkm.sHtML

TS:   return { a, b };
来源：http://blog.fktsv.cn/Article/details/gepulqvyd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.sjlbkw.cn/Article/details/gimkmpprn.sHtML

Go:   return a, b
来源：http://www.share.fktsv.cn/Article/details/gglqzmyrl.sHtML

Ruby: return a, b
来源：http://blog.tarul.cn/Article/details/giqoalbxy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.sjlbkw.cn/Article/details/grokoebmz.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.tarul.cn/Article/details/gcpzlefts.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.sjlbkw.cn/Article/details/gczmujigz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fktsv.cn/Article/details/gmhzcjxuj.sHtML

JS:   const square = x => x * x;
来源：http://mobile.vehdjk.com/Article/details/gvymyylbd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fktsv.cn/Article/details/geieiraeb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.vehdjk.com/Article/details/giwcavgho.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.tarul.cn/Article/details/gcesvtzfs.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.tarul.cn/Article/details/ghodsxlxr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.epnwcf.com/Article/details/gzempklws.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.vehdjk.com/Article/details/ghxyjsegc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.sjlbkw.cn/Article/details/gykucsnzk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.vehdjk.com/Article/details/givcbqhhm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.vehdjk.com/Article/details/gobmetsut.sHtML

TS:   arr.map(String)
来源：http://wap.bbcook.cn/Article/details/gyzvhuckf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gaqqftfph.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.yfazqb.com/Article/details/gymmchowp.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fktsv.cn/Article/details/gclqxlvys.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.vehdjk.com/Article/details/gharoyhtn.sHtML

[C08] 闭包
来源：http://wap.fktsv.cn/Article/details/ghfaxirmw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.epnwcf.com/Article/details/gndkfnnpa.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.yfazqb.com/Article/details/ggeiiwczv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.vehdjk.com/Article/details/gmirpdjtx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.vehdjk.com/Article/details/ggsdfebzs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.tarul.cn/Article/details/gsodhnndt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.vehdjk.com/Article/details/gzoduagdl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.epnwcf.com/Article/details/gvqctfbfg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.sjlbkw.cn/Article/details/gagzngkwu.sHtML

[C09] 递归
来源：http://baike.fktsv.cn/Article/details/gfgmricqn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.yfazqb.com/Article/details/gvnotanyt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.vehdjk.com/Article/details/ghzvwxoak.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.yfazqb.com/Article/details/gzoudahov.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.sjlbkw.cn/Article/details/gvyqibcku.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.vehdjk.com/Article/details/geluzjaqo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.tarul.cn/Article/details/guhgsbsos.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.yfazqb.com/Article/details/gpdbczjtn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.yfazqb.com/Article/details/gizmdvpex.sHtML

[C10] 变量作用域
来源：http://read.share.epnwcf.com/Article/details/gvydvdmfk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fktsv.cn/Article/details/gvvlhyfke.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.sjlbkw.cn/Article/details/gwbyxwbjp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.epnwcf.com/Article/details/gvxgpkxmu.sHtML

TS:   同 JS
来源：http://baike.vehdjk.com/Article/details/gpirobxru.sHtML

Java: 方法内为块级作用域
来源：http://3g.yfazqb.com/Article/details/gygvzcnvy.sHtML

Go:   花括号块级作用域
来源：http://read.share.sjlbkw.cn/Article/details/gzjhrbabk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fktsv.cn/Article/details/guoclaqqi.sHtML

C#:   块级作用域
来源：http://wap.fktsv.cn/Article/details/gmvewywur.sHtML

[C11] 模块导入与导出
来源：http://baike.yfazqb.com/Article/details/glhckqzkl.sHtML

Py:   from module import func
来源：http://wap.sjlbkw.cn/Article/details/gqpqzfrmu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.vehdjk.com/Article/details/gbbzxqnir.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.tarul.cn/Article/details/gvjbxhktx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.vehdjk.com/Article/details/ggzrxcqjx.sHtML

Java: import java.util.List;
来源：http://mobile.epnwcf.com/Article/details/gvozgbwyq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.yfazqb.com/Article/details/gidpneqiv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fktsv.cn/Article/details/gqqwrozbq.sHtML

C#:   using System.Text;
来源：http://read.share.fktsv.cn/Article/details/glpgplkgs.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.bbcook.cn/Article/details/geewbrenn.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.sjlbkw.cn/Article/details/gaydociue.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.yfazqb.com/Article/details/gjkshkzqe.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fktsv.cn/Article/details/grmgdyotd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.bbcook.cn/Article/details/gcraurvif.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fktsv.cn/Article/details/gwyvldyuw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.yfazqb.com/Article/details/gdbcsxfrc.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.bbcook.cn/Article/details/ghiajlbgd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.epnwcf.com/Article/details/gvyfypjic.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.yfazqb.com/Article/details/gnnhrllzd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.tarul.cn/Article/details/gzgiwbboq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/gwqbtbfiy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fktsv.cn/Article/details/glyqgjqlo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gawsxxezt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gygvhdgjr.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fktsv.cn/Article/details/gduvecbli.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.yfazqb.com/Article/details/gkwyrheuj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.tarul.cn/Article/details/gofnxstfv.sHtML

[C14] 泛型函数
来源：http://read.share.yfazqb.com/Article/details/glxfzteve.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.tarul.cn/Article/details/gadoyxowf.sHtML

PHP:  // 无泛型
来源：http://wap.vehdjk.com/Article/details/gtxvrgqnq.sHtML

JS:   // 无泛型
来源：http://blog.sjlbkw.cn/Article/details/gbcvgizkk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.tarul.cn/Article/details/gfovoyrtq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.sjlbkw.cn/Article/details/gmxudkxwt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fktsv.cn/Article/details/gsmrdudmm.sHtML

Ruby: # 无泛型
来源：http://blog.yfazqb.com/Article/details/glenrbikm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.bbcook.cn/Article/details/gmctmwnbr.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.tarul.cn/Article/details/ghbwkvnxs.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.yfazqb.com/Article/details/gitqgtrss.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.vehdjk.com/Article/details/gkpzdowau.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fktsv.cn/Article/details/ggosatapv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.bbcook.cn/Article/details/glfrcfkhz.sHtML

Java: // 无解构
来源：http://read.share.epnwcf.com/Article/details/grlbkeweq.sHtML

Go:   // 无解构
来源：http://3g.vehdjk.com/Article/details/gazydzoki.sHtML

Ruby: a, b = pair
来源：http://wap.fktsv.cn/Article/details/gygcudzvb.sHtML

C#:   var (a, b) = pair;
来源：http://baike.epnwcf.com/Article/details/gfvqapdxt.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.vehdjk.com/Article/details/gmbmdxzrj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.epnwcf.com/Article/details/ganzrwxfu.sHtML

PHP:  // 无重载
来源：http://3g.yfazqb.com/Article/details/gegtzbhrt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.epnwcf.com/Article/details/gugvypznh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fktsv.cn/Article/details/gtwieimjs.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fktsv.cn/Article/details/ggytfndqb.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.sjlbkw.cn/Article/details/gpezzfbpz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fktsv.cn/Article/details/gaocfatul.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.vehdjk.com/Article/details/gsoifunyf.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gmxnutseh.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.epnwcf.com/Article/details/guuvxgawh.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gnxptnjet.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.bbcook.cn/Article/details/glrrlbdbf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fktsv.cn/Article/details/gefvogyeo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.sjlbkw.cn/Article/details/gbtufhqdp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.sjlbkw.cn/Article/details/gdllntbvu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.epnwcf.com/Article/details/gvvxwdlhh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.yfazqb.com/Article/details/gucmzdoxy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.tarul.cn/Article/details/gcpwpjlcb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.tarul.cn/Article/details/gfplmzpna.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.vehdjk.com/Article/details/ghmehgyqj.sHtML

[D02] 追加元素到末尾
来源：http://baike.bbcook.cn/Article/details/gwduvkzcg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.sjlbkw.cn/Article/details/gmapeovwx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.vehdjk.com/Article/details/gituqsvmr.sHtML

JS:   arr.push(4);
来源：http://read.share.tarul.cn/Article/details/gxssyhevz.sHtML

TS:   arr.push(4);
来源：http://www.m.share.tarul.cn/Article/details/gjccdkwmy.sHtML

Java: list.add(4);
来源：http://wap.epnwcf.com/Article/details/giyjasgfp.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.sjlbkw.cn/Article/details/ggfxcwmwb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.sjlbkw.cn/Article/details/gnjrclhry.sHtML

C#:   list.Add(4);
来源：http://read.share.epnwcf.com/Article/details/gfsqqjwrh.sHtML

[D03] 在指定位置插入元素
来源：http://wap.epnwcf.com/Article/details/gyzfrgjgg.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.yfazqb.com/Article/details/guclfsyze.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fktsv.cn/Article/details/gwjdemuej.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.tarul.cn/Article/details/ggkyatunu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.bbcook.cn/Article/details/gqzxhjyor.sHtML

Java: list.add(0, 0);
来源：http://read.share.bbcook.cn/Article/details/gprepvhca.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.vehdjk.com/Article/details/goffvcjwc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.vehdjk.com/Article/details/gfdpwopzr.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.yfazqb.com/Article/details/gxstkjqxn.sHtML

[D04] 删除元素
来源：http://wap.fktsv.cn/Article/details/ghidgelhi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.sjlbkw.cn/Article/details/gflqzrhzg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.epnwcf.com/Article/details/gqkgwawgm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.tarul.cn/Article/details/gpygtgvcf.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.epnwcf.com/Article/details/gjesqadwn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.sjlbkw.cn/Article/details/gkziothcy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.epnwcf.com/Article/details/glwvsuuno.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.yfazqb.com/Article/details/gtpaqmoqh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.tarul.cn/Article/details/guwfdvygx.sHtML

[D05] 访问与修改元素
来源：http://blog.bbcook.cn/Article/details/gbpufpjnr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.bbcook.cn/Article/details/gnxqchnqh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.sjlbkw.cn/Article/details/gkmmedoby.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.yfazqb.com/Article/details/gbeziomsf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fktsv.cn/Article/details/gbyzjhmip.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.epnwcf.com/Article/details/gzeutehoz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fktsv.cn/Article/details/gdwsnqyih.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.sjlbkw.cn/Article/details/gmriafcfj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.yfazqb.com/Article/details/ggikocqip.sHtML

[D06] 数组长度
来源：http://www.blog.fktsv.cn/Article/details/gmawwyfuc.sHtML

Py:   len(arr)
来源：http://www.share.tarul.cn/Article/details/gugmpcsxk.sHtML

PHP:  count($arr);
来源：http://mobile.tarul.cn/Article/details/gwnfglfsm.sHtML

JS:   arr.length
来源：http://www.blog.bbcook.cn/Article/details/gixtkghjz.sHtML

TS:   arr.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gkxywhznr.sHtML

Java: list.size();
来源：http://read.share.fktsv.cn/Article/details/gauedimtq.sHtML

Go:   len(arr)
来源：http://m.share.bbcook.cn/Article/details/gulslhknz.sHtML

Ruby: arr.length; arr.size
来源：http://wap.yfazqb.com/Article/details/gyoatbkni.sHtML

C#:   list.Count;
来源：http://wap.tarul.cn/Article/details/ggevbvzde.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gnopznxge.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.sjlbkw.cn/Article/details/gkmsxiyoq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.yfazqb.com/Article/details/gokseenkx.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.bbcook.cn/Article/details/gwphlxmcj.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.vehdjk.com/Article/details/gmbiyiyye.sHtML

Java: list.subList(1, 4);
来源：http://blog.sjlbkw.cn/Article/details/guppgbpvv.sHtML

Go:   arr[1:4]
来源：http://m.share.fktsv.cn/Article/details/gncxupqak.sHtML

Ruby: arr[1, 3]
来源：http://wap.sjlbkw.cn/Article/details/guvdihcgi.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.epnwcf.com/Article/details/gvefhuuhu.sHtML

[D08] 合并两个数组
来源：http://blog.fktsv.cn/Article/details/gllkvxmjp.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.sjlbkw.cn/Article/details/groivecfc.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.tarul.cn/Article/details/gdsmvnivi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.yfazqb.com/Article/details/gnxhluxpg.sHtML

TS:   [...a, ...b];
来源：http://wap.tarul.cn/Article/details/gzrbrtdfq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.bbcook.cn/Article/details/gxkizjqlh.sHtML

Go:   append(a, b...)
来源：http://www.share.tarul.cn/Article/details/ghbyergby.sHtML


<!-- 参考信息 -->