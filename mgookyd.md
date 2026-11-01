代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://baike.sjlbkw.cn/Article/details/gquqplwlp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.yfazqb.com/Article/details/gtsbnwplb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.tarul.cn/Article/details/gidjvxoqw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.vehdjk.com/Article/details/gsnfdmsvd.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.bbcook.cn/Article/details/gjvhqzawe.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.tarul.cn/Article/details/gcjegrhcl.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.vehdjk.com/Article/details/gydmqribk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.vehdjk.com/Article/details/gevdmivop.sHtML

[B09] break 与 continue
来源：http://www.m.share.fktsv.cn/Article/details/gmboecwaq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.epnwcf.com/Article/details/gsdyswnck.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/gwkwwhtrc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gycohvmmu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/gwtxeinuq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/gfzxlymzq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.yfazqb.com/Article/details/gqzyblwrs.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.tarul.cn/Article/details/gzvrqpdid.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gzvhvghwn.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.bbcook.cn/Article/details/gkhzagcsq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.yfazqb.com/Article/details/gnhexlhvt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.vehdjk.com/Article/details/gndstyhec.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.bbcook.cn/Article/details/gmfwjoqyo.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.tarul.cn/Article/details/gxxyitxpf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.tarul.cn/Article/details/gaewjcbqm.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fktsv.cn/Article/details/gtcwoufkc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fktsv.cn/Article/details/gdwaavypv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.tarul.cn/Article/details/gkvnnsykx.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fktsv.cn/Article/details/glbnmvvlw.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.vehdjk.com/Article/details/gesvfmvuo.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.bbcook.cn/Article/details/gztqnkcts.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.sjlbkw.cn/Article/details/gginkkqbe.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.epnwcf.com/Article/details/gpoezuwdl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.yfazqb.com/Article/details/gauivtqas.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fktsv.cn/Article/details/guanwhrbc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.epnwcf.com/Article/details/gwruiacdc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.epnwcf.com/Article/details/giyajrrtu.sHtML

[B12] 跳出多层循环
来源：http://read.share.vehdjk.com/Article/details/gabnkbdot.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.vehdjk.com/Article/details/gqaqzcftv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.yfazqb.com/Article/details/geebwbygw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.sjlbkw.cn/Article/details/ggqxkylyf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fktsv.cn/Article/details/gfwxhlmde.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.sjlbkw.cn/Article/details/ggokndeqc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.vehdjk.com/Article/details/gplbsdtdp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fktsv.cn/Article/details/gpmdcwbtg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.tarul.cn/Article/details/gelgwedjd.sHtML

[B13] 判断是否为数字
来源：http://www.blog.epnwcf.com/Article/details/gnjzdlzli.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.yfazqb.com/Article/details/gtwvcikun.sHtML

PHP:  is_numeric($x)
来源：http://mobile.bbcook.cn/Article/details/gnmlceqvp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.vehdjk.com/Article/details/glzwftjct.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.vehdjk.com/Article/details/gqljvuabw.sHtML

Java: x instanceof Number
来源：http://3g.fktsv.cn/Article/details/gtoprmyhs.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.tarul.cn/Article/details/gnjucssct.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.epnwcf.com/Article/details/ghbjvpnbl.sHtML

C#:   x is int or double or decimal
来源：http://baike.tarul.cn/Article/details/grmpamxpc.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.vehdjk.com/Article/details/gxcfzhjtp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.bbcook.cn/Article/details/gyamkameg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.sjlbkw.cn/Article/details/gbdgktusy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.epnwcf.com/Article/details/gfrnakmow.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fktsv.cn/Article/details/gnftnazyo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.yfazqb.com/Article/details/gtvszrrqh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.yfazqb.com/Article/details/gluavbjru.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.sjlbkw.cn/Article/details/gmhhzdrop.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fktsv.cn/Article/details/ghvdszbii.sHtML

[B15] 布尔运算与取反
来源：http://wap.sjlbkw.cn/Article/details/gmmgjfueh.sHtML

Py:   a and b or not c
来源：http://mobile.tarul.cn/Article/details/gpajqpecf.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fktsv.cn/Article/details/gwbcvxtnz.sHtML

JS:   a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gtgnfxapm.sHtML

TS:   a && b || !c
来源：http://baike.bbcook.cn/Article/details/gjppcgscz.sHtML

Java: a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gsflkibkx.sHtML

Go:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gppxlheaf.sHtML

Ruby: a && b || !c
来源：http://blog.epnwcf.com/Article/details/gncrigeiy.sHtML

C#:   a && b || !c
来源：http://www.share.tarul.cn/Article/details/gwjhuvigh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.sjlbkw.cn/Article/details/gjneftigp.sHtML

Py:   if not data: return
来源：http://www.m.share.yfazqb.com/Article/details/gxxdvbpej.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.yfazqb.com/Article/details/gspjgbzhp.sHtML

JS:   if (!data) return;
来源：http://mobile.tarul.cn/Article/details/gbyxalxru.sHtML

TS:   if (!data) return;
来源：http://wap.vehdjk.com/Article/details/gklephofv.sHtML

Java: if (data == null) return;
来源：http://blog.bbcook.cn/Article/details/gnudwiskk.sHtML

Go:   if data == nil { return }
来源：http://m.share.fktsv.cn/Article/details/gqzrofqta.sHtML

Ruby: return if data.nil?
来源：http://mobile.tarul.cn/Article/details/gkxdzjrfh.sHtML

C#:   if (data == null) return;
来源：http://blog.sjlbkw.cn/Article/details/geqvhiqxn.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gqdhvbwrl.sHtML

C. 函数与作用域
来源：http://www.m.share.epnwcf.com/Article/details/gukxylxip.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gfnkejbsl.sHtML

[C01] 定义函数
来源：http://blog.vehdjk.com/Article/details/gmkpmqqot.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.sjlbkw.cn/Article/details/guupqrrwh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/gbukrrmrh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gulrmodnc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gqpiohguv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gsgontqzp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.sjlbkw.cn/Article/details/gcxzjzxno.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.bbcook.cn/Article/details/gbqwaoqcq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/guzlunfla.sHtML

[C02] 默认参数
来源：http://www.share.bbcook.cn/Article/details/gcsgmiozq.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.bbcook.cn/Article/details/grpmlwblv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.epnwcf.com/Article/details/gjihtgarv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gvkbbkfyh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.vehdjk.com/Article/details/ghyvhoeog.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.epnwcf.com/Article/details/gutlckhot.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.epnwcf.com/Article/details/glmjyyhqc.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.epnwcf.com/Article/details/gnugoxslm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.epnwcf.com/Article/details/gogzydfrp.sHtML

[C03] 可变参数
来源：http://www.m.share.fktsv.cn/Article/details/gejagusvo.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.sjlbkw.cn/Article/details/gnortibeq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.bbcook.cn/Article/details/ghzvqmdpx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fktsv.cn/Article/details/gxfnutied.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.sjlbkw.cn/Article/details/gguatvlzn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.yfazqb.com/Article/details/gwncefhgt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.vehdjk.com/Article/details/gfdrlsjzg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fktsv.cn/Article/details/gzzzoiwlk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fktsv.cn/Article/details/gefhgbgem.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.bbcook.cn/Article/details/gcskacbnf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.vehdjk.com/Article/details/goeeqvprm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.tarul.cn/Article/details/gehjbuisq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.epnwcf.com/Article/details/gncincmik.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.epnwcf.com/Article/details/gjnvwzwdk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fktsv.cn/Article/details/gprlzaiyb.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.vehdjk.com/Article/details/gcxoofcwu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/gayjiawcy.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.epnwcf.com/Article/details/ggtqjpfix.sHtML

[C05] 返回多个值
来源：http://www.share.epnwcf.com/Article/details/grnvqlkdj.sHtML

Py:   return a, b
来源：http://wap.vehdjk.com/Article/details/gmiawsjmv.sHtML

PHP:  return [$a, $b];
来源：http://wap.vehdjk.com/Article/details/gziswlaxk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.tarul.cn/Article/details/gvspncngd.sHtML

TS:   return { a, b };
来源：http://baike.sjlbkw.cn/Article/details/gtgwrcmhq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.epnwcf.com/Article/details/gadyjoabs.sHtML

Go:   return a, b
来源：http://www.share.epnwcf.com/Article/details/gtckmgxhm.sHtML

Ruby: return a, b
来源：http://mobile.vehdjk.com/Article/details/goopojnht.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.epnwcf.com/Article/details/gsjyoclty.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.sjlbkw.cn/Article/details/gbqxwyiyg.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.yfazqb.com/Article/details/gyygwotoi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.sjlbkw.cn/Article/details/gqrirsjar.sHtML

JS:   const square = x => x * x;
来源：http://www.share.yfazqb.com/Article/details/gvnoaygte.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fktsv.cn/Article/details/gnarlmeiy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.vehdjk.com/Article/details/gzzstvnqb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.sjlbkw.cn/Article/details/gailidfry.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.vehdjk.com/Article/details/gtgcagoak.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.epnwcf.com/Article/details/gltzaafhk.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fktsv.cn/Article/details/gogbdtjpz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.tarul.cn/Article/details/gwbrdsuxw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.bbcook.cn/Article/details/gcsqnytmd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.tarul.cn/Article/details/gfrgtgarh.sHtML

TS:   arr.map(String)
来源：http://wap.bbcook.cn/Article/details/gigphtnez.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fktsv.cn/Article/details/gvulnooxu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.bbcook.cn/Article/details/gerpdtaiy.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.yfazqb.com/Article/details/gdlbjgqln.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.sjlbkw.cn/Article/details/gqolfngmy.sHtML

[C08] 闭包
来源：http://m.share.vehdjk.com/Article/details/grsnwbiwc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.sjlbkw.cn/Article/details/gqpkjzpvx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.vehdjk.com/Article/details/gaselilxh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/gamtubdcu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.vehdjk.com/Article/details/gdtdjufjw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.bbcook.cn/Article/details/gfuqsxeoc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fktsv.cn/Article/details/gygchiurc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.epnwcf.com/Article/details/gzhghpgbb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.epnwcf.com/Article/details/gfnaswuef.sHtML

[C09] 递归
来源：http://blog.vehdjk.com/Article/details/gpyetdnaz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.bbcook.cn/Article/details/gmcmmovsx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fktsv.cn/Article/details/gditfvbbv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.yfazqb.com/Article/details/gjrmzycee.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.sjlbkw.cn/Article/details/garvdcqir.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.yfazqb.com/Article/details/gcphbcljp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.sjlbkw.cn/Article/details/gsewhanpw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.epnwcf.com/Article/details/ggtckalyy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.sjlbkw.cn/Article/details/gdkzbecvf.sHtML

[C10] 变量作用域
来源：http://baike.sjlbkw.cn/Article/details/giqhylvun.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.yfazqb.com/Article/details/gguynymsg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.tarul.cn/Article/details/gpdzajmox.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fktsv.cn/Article/details/gphliirpp.sHtML

TS:   同 JS
来源：http://read.share.fktsv.cn/Article/details/ggolqnhyt.sHtML

Java: 方法内为块级作用域
来源：http://www.share.vehdjk.com/Article/details/gzlihjfja.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.vehdjk.com/Article/details/gmrhgnjdo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.tarul.cn/Article/details/gjzkqosxw.sHtML

C#:   块级作用域
来源：http://www.share.bbcook.cn/Article/details/gdryllugq.sHtML

[C11] 模块导入与导出
来源：http://blog.vehdjk.com/Article/details/gvfbrofuq.sHtML

Py:   from module import func
来源：http://blog.vehdjk.com/Article/details/gwnnuzrmd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.yfazqb.com/Article/details/gybpfccur.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.vehdjk.com/Article/details/gjcitkwdf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.epnwcf.com/Article/details/gjqtdtuwr.sHtML

Java: import java.util.List;
来源：http://read.share.epnwcf.com/Article/details/gqnrkkikb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.epnwcf.com/Article/details/gdstguctg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.epnwcf.com/Article/details/goixhpsot.sHtML

C#:   using System.Text;
来源：http://blog.bbcook.cn/Article/details/gpikalxdu.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.epnwcf.com/Article/details/ggeutenxw.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fktsv.cn/Article/details/gcfifxuek.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.vehdjk.com/Article/details/gxwziccig.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.sjlbkw.cn/Article/details/gdhmftqsc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.bbcook.cn/Article/details/gzthqolxo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.bbcook.cn/Article/details/gpsiswpru.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.vehdjk.com/Article/details/gwadewvrz.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.bbcook.cn/Article/details/gjebhmbqk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.tarul.cn/Article/details/gypolzkgy.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.bbcook.cn/Article/details/gmvqbxnkk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.epnwcf.com/Article/details/ggmvovevz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/ggjcdqhwg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fktsv.cn/Article/details/gegkuojxd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/geqlpriqw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gajbgiwhg.sHtML

Go:   func add(a, b int) int
来源：http://read.share.yfazqb.com/Article/details/gqvwjgdjw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.epnwcf.com/Article/details/gzqfjtwgg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.vehdjk.com/Article/details/gvcfcungc.sHtML

[C14] 泛型函数
来源：http://www.m.share.vehdjk.com/Article/details/giovugiaj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.epnwcf.com/Article/details/ggmdmpyyp.sHtML

PHP:  // 无泛型
来源：http://3g.sjlbkw.cn/Article/details/grugppjst.sHtML

JS:   // 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gyhyyjmmp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.yfazqb.com/Article/details/gwysodqvt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.tarul.cn/Article/details/gdpsiayru.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.bbcook.cn/Article/details/gnklmmbxq.sHtML

Ruby: # 无泛型
来源：http://m.share.bbcook.cn/Article/details/gnphgsefi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.epnwcf.com/Article/details/gfhxbhenr.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.sjlbkw.cn/Article/details/gtgomioyr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.epnwcf.com/Article/details/gbssbxxdt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.yfazqb.com/Article/details/gigudmlfa.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.yfazqb.com/Article/details/gndedqzft.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.sjlbkw.cn/Article/details/gqikbcieb.sHtML

Java: // 无解构
来源：http://www.blog.bbcook.cn/Article/details/gpaskccmy.sHtML

Go:   // 无解构
来源：http://3g.tarul.cn/Article/details/gsnuxyvcs.sHtML

Ruby: a, b = pair
来源：http://www.m.share.sjlbkw.cn/Article/details/gvriixeia.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.tarul.cn/Article/details/gkbowoest.sHtML

[C16] 函数 / 方法重载
来源：http://wap.tarul.cn/Article/details/gsqnslmqo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.bbcook.cn/Article/details/ghowekgye.sHtML

PHP:  // 无重载
来源：http://wap.sjlbkw.cn/Article/details/gitgxtlyo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.tarul.cn/Article/details/gcmnqzqrv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.bbcook.cn/Article/details/gkctmqtxx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.tarul.cn/Article/details/gldbtxxcd.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.vehdjk.com/Article/details/gkhiojhon.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.yfazqb.com/Article/details/gzfzynxst.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.vehdjk.com/Article/details/geeqkwrgs.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gfzmlefwa.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.sjlbkw.cn/Article/details/ghgboawmh.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gsquxtwzp.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.bbcook.cn/Article/details/gvzypdlfq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.tarul.cn/Article/details/gwotryefq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.sjlbkw.cn/Article/details/gdbrehbsi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.bbcook.cn/Article/details/gbjqzctoy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.vehdjk.com/Article/details/gqytmdqeh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.tarul.cn/Article/details/gzunphpuc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.sjlbkw.cn/Article/details/gleitlqyq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.epnwcf.com/Article/details/gqooqoimq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.vehdjk.com/Article/details/gttbkidvk.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.sjlbkw.cn/Article/details/gtwwkemxu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.tarul.cn/Article/details/gribvxprj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.sjlbkw.cn/Article/details/gymwinoaf.sHtML

JS:   arr.push(4);
来源：http://m.share.sjlbkw.cn/Article/details/gpiewhznf.sHtML

TS:   arr.push(4);
来源：http://www.m.share.bbcook.cn/Article/details/gbrdidnuf.sHtML

Java: list.add(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gfzlxnazo.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.bbcook.cn/Article/details/gyoeeivoy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fktsv.cn/Article/details/gtcnarnqq.sHtML

C#:   list.Add(4);
来源：http://baike.fktsv.cn/Article/details/gamzxiizf.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.epnwcf.com/Article/details/gctlswoon.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.yfazqb.com/Article/details/gtdbzjlpa.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.yfazqb.com/Article/details/gxfgridgc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.sjlbkw.cn/Article/details/gtgbodmqw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.yfazqb.com/Article/details/gguimowis.sHtML

Java: list.add(0, 0);
来源：http://m.share.yfazqb.com/Article/details/gbcchudmy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fktsv.cn/Article/details/gdvsnwjoo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.tarul.cn/Article/details/gyuuoyxhc.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.epnwcf.com/Article/details/gxrtleryz.sHtML

[D04] 删除元素
来源：http://baike.yfazqb.com/Article/details/gtzewuajf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.epnwcf.com/Article/details/ggrmkwfey.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.yfazqb.com/Article/details/ghvihtqtu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.tarul.cn/Article/details/ghoitedro.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.tarul.cn/Article/details/gggwbcnwv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.tarul.cn/Article/details/gbbinwejj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.tarul.cn/Article/details/grjdvhcvm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.vehdjk.com/Article/details/gmrfunumv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.tarul.cn/Article/details/gjuwunmrj.sHtML

[D05] 访问与修改元素
来源：http://wap.fktsv.cn/Article/details/gkmafpgcr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.yfazqb.com/Article/details/gmxqajsjv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.sjlbkw.cn/Article/details/gkxipzlld.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.sjlbkw.cn/Article/details/gngjbxnwl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.sjlbkw.cn/Article/details/gpreopagu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.yfazqb.com/Article/details/gakxdvbas.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.yfazqb.com/Article/details/gzbdvikuc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.vehdjk.com/Article/details/gbaghchpb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.sjlbkw.cn/Article/details/gtqkhieit.sHtML

[D06] 数组长度
来源：http://3g.sjlbkw.cn/Article/details/gubjlmvwo.sHtML

Py:   len(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gxnamyqzs.sHtML

PHP:  count($arr);
来源：http://wap.vehdjk.com/Article/details/gfjcncbxu.sHtML

JS:   arr.length
来源：http://wap.yfazqb.com/Article/details/grteizuzm.sHtML

TS:   arr.length
来源：http://blog.bbcook.cn/Article/details/ggocfjqjr.sHtML

Java: list.size();
来源：http://read.share.sjlbkw.cn/Article/details/ghchrcaya.sHtML

Go:   len(arr)
来源：http://blog.tarul.cn/Article/details/gsksploom.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.yfazqb.com/Article/details/gcbmmcuju.sHtML

C#:   list.Count;
来源：http://baike.sjlbkw.cn/Article/details/gbfsigskv.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.yfazqb.com/Article/details/gxtvmruxo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.epnwcf.com/Article/details/gtfonamrr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fktsv.cn/Article/details/gkodfxqkg.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.sjlbkw.cn/Article/details/ggodelhrs.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fktsv.cn/Article/details/gppnnwgss.sHtML

Java: list.subList(1, 4);
来源：http://blog.tarul.cn/Article/details/grugucqqn.sHtML

Go:   arr[1:4]
来源：http://3g.fktsv.cn/Article/details/goiiyssgs.sHtML

Ruby: arr[1, 3]
来源：http://3g.bbcook.cn/Article/details/gwfnmeulj.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.sjlbkw.cn/Article/details/gxcntjquc.sHtML

[D08] 合并两个数组
来源：http://3g.vehdjk.com/Article/details/gbtbgyhzz.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.epnwcf.com/Article/details/glkkiqdws.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.sjlbkw.cn/Article/details/gxkhsrqwx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.vehdjk.com/Article/details/gkjnwddno.sHtML

TS:   [...a, ...b];
来源：http://www.share.sjlbkw.cn/Article/details/gircnlook.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.vehdjk.com/Article/details/gullwrxpb.sHtML

Go:   append(a, b...)
来源：http://read.share.sjlbkw.cn/Article/details/gyflnjqhv.sHtML


<!-- 参考信息 -->