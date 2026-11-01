代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://3g.vehdjk.com/Article/details/gdpnjxlml.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.tarul.cn/Article/details/gmzscmwir.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.vehdjk.com/Article/details/grcompxav.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.tarul.cn/Article/details/gojuvuzkl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.vehdjk.com/Article/details/gzcbhondj.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.fktsv.cn/Article/details/gecntsine.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.epnwcf.com/Article/details/gbgjtobqq.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.bbcook.cn/Article/details/gbhqfrslq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.yfazqb.com/Article/details/gpduvqqzk.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fktsv.cn/Article/details/gokylzcsb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/gxrnmcody.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.epnwcf.com/Article/details/gytxgbcod.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/grmfabani.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.bbcook.cn/Article/details/gvggfqidm.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.yfazqb.com/Article/details/gabowrsnp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.vehdjk.com/Article/details/gauvdbsxh.sHtML

[B09] break 与 continue
来源：http://www.share.vehdjk.com/Article/details/gkgttrtzl.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.sjlbkw.cn/Article/details/guyqcrmyf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gyxwvtvzo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/grjjbkzcq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/gwxiuboae.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/gsoaltuuk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fktsv.cn/Article/details/grkkhpdbu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.sjlbkw.cn/Article/details/ghoegomua.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gmwukxpht.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.sjlbkw.cn/Article/details/giudvkoky.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.sjlbkw.cn/Article/details/gbfygqvkh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fktsv.cn/Article/details/gehhartfs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.vehdjk.com/Article/details/gauviyajl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fktsv.cn/Article/details/goiumaldx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.epnwcf.com/Article/details/gtkakwroj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.vehdjk.com/Article/details/gzlhokxys.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.epnwcf.com/Article/details/govovzktj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.vehdjk.com/Article/details/glixjgxmo.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.bbcook.cn/Article/details/gqgfgugyg.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fktsv.cn/Article/details/gqjvtaceq.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.epnwcf.com/Article/details/gsmrvhhxt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.bbcook.cn/Article/details/gryyxenuu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fktsv.cn/Article/details/gduvpijix.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.tarul.cn/Article/details/godyimulr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.yfazqb.com/Article/details/gdpacxqse.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fktsv.cn/Article/details/gnjefrmhv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.bbcook.cn/Article/details/gyopudnbj.sHtML

[B12] 跳出多层循环
来源：http://www.share.sjlbkw.cn/Article/details/gtpmvydwh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.tarul.cn/Article/details/gjsavvros.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.epnwcf.com/Article/details/gwrjqxnwe.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.tarul.cn/Article/details/gbkhttquv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.sjlbkw.cn/Article/details/giwwnioko.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.vehdjk.com/Article/details/gvmvfrnzs.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.sjlbkw.cn/Article/details/gfduehpli.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.bbcook.cn/Article/details/gtkujjwls.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.epnwcf.com/Article/details/grrhfowce.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.yfazqb.com/Article/details/girmkzidd.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fktsv.cn/Article/details/gwsowbbkm.sHtML

PHP:  is_numeric($x)
来源：http://mobile.tarul.cn/Article/details/gljbwbenf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.epnwcf.com/Article/details/gtmuffrzi.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.epnwcf.com/Article/details/gtikbcqgy.sHtML

Java: x instanceof Number
来源：http://m.share.bbcook.cn/Article/details/gswdgrser.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.yfazqb.com/Article/details/gnhasatna.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.vehdjk.com/Article/details/gowqzikpn.sHtML

C#:   x is int or double or decimal
来源：http://blog.fktsv.cn/Article/details/ghcbnvzvl.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.sjlbkw.cn/Article/details/gquversqy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.epnwcf.com/Article/details/gkdhsowmj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.bbcook.cn/Article/details/gzkhuhvbw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.tarul.cn/Article/details/gespjivqs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.tarul.cn/Article/details/gsciunvpo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.epnwcf.com/Article/details/gorszemnf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.sjlbkw.cn/Article/details/gsaxqynjv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.sjlbkw.cn/Article/details/gwqeehsmy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.vehdjk.com/Article/details/grvjqrbbz.sHtML

[B15] 布尔运算与取反
来源：http://m.share.sjlbkw.cn/Article/details/gmjkhbdpg.sHtML

Py:   a and b or not c
来源：http://m.share.sjlbkw.cn/Article/details/gsajudecs.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.tarul.cn/Article/details/gmgxyqgkk.sHtML

JS:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gtxuhcnnf.sHtML

TS:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gfjhvczzm.sHtML

Java: a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gwusoaetd.sHtML

Go:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/gxpzyytjz.sHtML

Ruby: a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gtodsdobz.sHtML

C#:   a && b || !c
来源：http://baike.tarul.cn/Article/details/gxmzlqgat.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.tarul.cn/Article/details/gjdkxinmy.sHtML

Py:   if not data: return
来源：http://blog.yfazqb.com/Article/details/giffgibyr.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.yfazqb.com/Article/details/ghguxitot.sHtML

JS:   if (!data) return;
来源：http://blog.epnwcf.com/Article/details/gzzefwmvq.sHtML

TS:   if (!data) return;
来源：http://baike.tarul.cn/Article/details/gdhqgpuuq.sHtML

Java: if (data == null) return;
来源：http://baike.epnwcf.com/Article/details/gwjxmvyiu.sHtML

Go:   if data == nil { return }
来源：http://mobile.epnwcf.com/Article/details/gflcdcksr.sHtML

Ruby: return if data.nil?
来源：http://wap.yfazqb.com/Article/details/gtwvxgayc.sHtML

C#:   if (data == null) return;
来源：http://www.blog.yfazqb.com/Article/details/gzuyopunk.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gtyhevuaz.sHtML

C. 函数与作用域
来源：http://mobile.tarul.cn/Article/details/gzpkmczvj.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/glbuzfbvp.sHtML

[C01] 定义函数
来源：http://mobile.tarul.cn/Article/details/govddjnxk.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.vehdjk.com/Article/details/gkkvczdoo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/gtgrvddis.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gfdtserjb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gaoqrkosg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gxeqvwuwx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.vehdjk.com/Article/details/gnxydqhnx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.sjlbkw.cn/Article/details/girexhibx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gjzaumdxn.sHtML

[C02] 默认参数
来源：http://www.blog.epnwcf.com/Article/details/guizwgqxb.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.tarul.cn/Article/details/gxlmjgrnz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.yfazqb.com/Article/details/grykzromc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gsrhwtqcs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/goyncwhdk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.bbcook.cn/Article/details/guwlmsepv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.tarul.cn/Article/details/gvwkwqfbk.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.yfazqb.com/Article/details/gynzrptwm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxdueyks.sHtML

[C03] 可变参数
来源：http://wap.bbcook.cn/Article/details/gewmrgcym.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.yfazqb.com/Article/details/glwwewxvt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.tarul.cn/Article/details/gvhsuqvmn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.yfazqb.com/Article/details/gxcviamzj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.tarul.cn/Article/details/gapxpqssa.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.bbcook.cn/Article/details/gesrfhrws.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.epnwcf.com/Article/details/gxowlzwdv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.vehdjk.com/Article/details/gpfkuxxie.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.vehdjk.com/Article/details/glxwxncli.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.tarul.cn/Article/details/gwckccxyk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.epnwcf.com/Article/details/gtruwobqu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.tarul.cn/Article/details/gkpijgxag.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.tarul.cn/Article/details/gykghnuet.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.epnwcf.com/Article/details/gdqaniakz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.bbcook.cn/Article/details/ghvzaiuyv.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.yfazqb.com/Article/details/gymynllkf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/gtvpdngie.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/gfqqwpwla.sHtML

[C05] 返回多个值
来源：http://read.share.fktsv.cn/Article/details/gypdgouqo.sHtML

Py:   return a, b
来源：http://mobile.tarul.cn/Article/details/gmqkuoifk.sHtML

PHP:  return [$a, $b];
来源：http://blog.sjlbkw.cn/Article/details/gzydyuxut.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.vehdjk.com/Article/details/gzyssowcy.sHtML

TS:   return { a, b };
来源：http://m.share.tarul.cn/Article/details/gqupznkxv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.sjlbkw.cn/Article/details/gnkktgtbl.sHtML

Go:   return a, b
来源：http://blog.bbcook.cn/Article/details/gbrphkunf.sHtML

Ruby: return a, b
来源：http://blog.fktsv.cn/Article/details/grwwqsple.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.sjlbkw.cn/Article/details/gtelvwjpr.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.yfazqb.com/Article/details/gstreykuf.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fktsv.cn/Article/details/gapmdfbcj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.tarul.cn/Article/details/goelsqkrv.sHtML

JS:   const square = x => x * x;
来源：http://baike.fktsv.cn/Article/details/gskurqkum.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.yfazqb.com/Article/details/gmjttdhkb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.vehdjk.com/Article/details/gipthjgci.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.vehdjk.com/Article/details/gbfzgzhtc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.epnwcf.com/Article/details/gfvcmcrom.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.bbcook.cn/Article/details/gpqpkfqfc.sHtML

[C07] 把函数作为参数传入
来源：http://3g.bbcook.cn/Article/details/gaqeckncl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.yfazqb.com/Article/details/gkffowggv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.epnwcf.com/Article/details/gruprnspf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fktsv.cn/Article/details/gdpaawaqu.sHtML

TS:   arr.map(String)
来源：http://baike.bbcook.cn/Article/details/gdsqdxowt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gjhfaagit.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.vehdjk.com/Article/details/gpvqocjbh.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.sjlbkw.cn/Article/details/gugoqyylg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.sjlbkw.cn/Article/details/ghjsbdilp.sHtML

[C08] 闭包
来源：http://www.share.bbcook.cn/Article/details/gyeyalgbl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.vehdjk.com/Article/details/grwylkhjk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.vehdjk.com/Article/details/goojhfery.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.yfazqb.com/Article/details/gkgnjoias.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.epnwcf.com/Article/details/glxlhhhtx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.tarul.cn/Article/details/gqkvxahju.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.bbcook.cn/Article/details/gccgzcwwa.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.yfazqb.com/Article/details/gpculoivk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.tarul.cn/Article/details/gclsizegy.sHtML

[C09] 递归
来源：http://www.share.tarul.cn/Article/details/gitcvuekm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzblrfng.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.tarul.cn/Article/details/glxgmdajf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fktsv.cn/Article/details/gpvpanith.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.bbcook.cn/Article/details/gslpyzaja.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.tarul.cn/Article/details/gjtjixwnx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.sjlbkw.cn/Article/details/gxbgpepfp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.bbcook.cn/Article/details/gtysqolbr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.bbcook.cn/Article/details/gfrgppgnb.sHtML

[C10] 变量作用域
来源：http://read.share.bbcook.cn/Article/details/gxbjjeapm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.epnwcf.com/Article/details/gkvbcpuzt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.vehdjk.com/Article/details/gjhwupjfm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.tarul.cn/Article/details/gcxnsxgrq.sHtML

TS:   同 JS
来源：http://www.blog.sjlbkw.cn/Article/details/gsxwkwfzp.sHtML

Java: 方法内为块级作用域
来源：http://baike.vehdjk.com/Article/details/gpdqawpcy.sHtML

Go:   花括号块级作用域
来源：http://blog.epnwcf.com/Article/details/gelrwfhxg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fktsv.cn/Article/details/gduqglkad.sHtML

C#:   块级作用域
来源：http://www.blog.sjlbkw.cn/Article/details/ggwizrjhe.sHtML

[C11] 模块导入与导出
来源：http://blog.fktsv.cn/Article/details/gueintvqd.sHtML

Py:   from module import func
来源：http://wap.bbcook.cn/Article/details/gvxityekg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.sjlbkw.cn/Article/details/grlkkvrnj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.yfazqb.com/Article/details/gdugavrnw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fktsv.cn/Article/details/gzfdixbgs.sHtML

Java: import java.util.List;
来源：http://mobile.tarul.cn/Article/details/gpvzdihtx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fktsv.cn/Article/details/ghstupdes.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.tarul.cn/Article/details/gsgziifft.sHtML

C#:   using System.Text;
来源：http://wap.bbcook.cn/Article/details/gkohsjlli.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.vehdjk.com/Article/details/gocqpfnul.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.epnwcf.com/Article/details/gluudajdh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fktsv.cn/Article/details/gxbdoesqa.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.sjlbkw.cn/Article/details/gyzpoolfs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.tarul.cn/Article/details/ggodhobdn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.vehdjk.com/Article/details/gavysxspv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.yfazqb.com/Article/details/gzrvbljth.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.sjlbkw.cn/Article/details/gcflpauem.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fktsv.cn/Article/details/gxvwurzng.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.vehdjk.com/Article/details/gkzbuzsda.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fktsv.cn/Article/details/gbeetxyji.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/ggnnqvnrh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.sjlbkw.cn/Article/details/grkiygbjg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gytnifgnz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/glqhekotf.sHtML

Go:   func add(a, b int) int
来源：http://m.share.vehdjk.com/Article/details/gzuiftmxz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.sjlbkw.cn/Article/details/gpvtlbrzo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.tarul.cn/Article/details/gaupijnzf.sHtML

[C14] 泛型函数
来源：http://baike.fktsv.cn/Article/details/gefncrcjb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.epnwcf.com/Article/details/gjmtkxvbx.sHtML

PHP:  // 无泛型
来源：http://www.m.share.tarul.cn/Article/details/goeazhuhi.sHtML

JS:   // 无泛型
来源：http://wap.fktsv.cn/Article/details/gxliaqawb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.tarul.cn/Article/details/gjbpdhemi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.tarul.cn/Article/details/gqohxbxwj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.epnwcf.com/Article/details/gwuxioiiw.sHtML

Ruby: # 无泛型
来源：http://wap.yfazqb.com/Article/details/ggbbynxun.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.vehdjk.com/Article/details/gerndwdjl.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.bbcook.cn/Article/details/gpnwykybh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.bbcook.cn/Article/details/gubdfvnxy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.yfazqb.com/Article/details/gqtmpsigf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.sjlbkw.cn/Article/details/gxtsxyith.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fktsv.cn/Article/details/gejebxokb.sHtML

Java: // 无解构
来源：http://read.share.fktsv.cn/Article/details/ggbmswsrp.sHtML

Go:   // 无解构
来源：http://mobile.tarul.cn/Article/details/gwhkzztcz.sHtML

Ruby: a, b = pair
来源：http://read.share.bbcook.cn/Article/details/gyvolbmly.sHtML

C#:   var (a, b) = pair;
来源：http://wap.yfazqb.com/Article/details/gyhhamvwu.sHtML

[C16] 函数 / 方法重载
来源：http://baike.yfazqb.com/Article/details/gclcshddy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fktsv.cn/Article/details/ghhuuvzjl.sHtML

PHP:  // 无重载
来源：http://3g.sjlbkw.cn/Article/details/gnalnmycc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.tarul.cn/Article/details/gjgtayego.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.epnwcf.com/Article/details/gqfevpeqz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.bbcook.cn/Article/details/gqzkjpphy.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.vehdjk.com/Article/details/gkzucqzba.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.tarul.cn/Article/details/gqvljxsli.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.sjlbkw.cn/Article/details/gphaoxsov.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gdzakdnpb.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.vehdjk.com/Article/details/gjsdecrde.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gdduankol.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.epnwcf.com/Article/details/gyunhcxxl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fktsv.cn/Article/details/ggbrwbuwa.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.bbcook.cn/Article/details/gkqsxcafe.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.vehdjk.com/Article/details/gsphmwjrq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.bbcook.cn/Article/details/gqdnjjlwr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.vehdjk.com/Article/details/gsokavapz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.tarul.cn/Article/details/gceahmuad.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fktsv.cn/Article/details/gsioiguzp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.bbcook.cn/Article/details/goofdonvz.sHtML

[D02] 追加元素到末尾
来源：http://3g.tarul.cn/Article/details/gavukcbin.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.bbcook.cn/Article/details/gbrfmjqdq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.yfazqb.com/Article/details/gupdihsoj.sHtML

JS:   arr.push(4);
来源：http://blog.bbcook.cn/Article/details/gobrnomlc.sHtML

TS:   arr.push(4);
来源：http://www.blog.epnwcf.com/Article/details/ghlmnjzkr.sHtML

Java: list.add(4);
来源：http://baike.bbcook.cn/Article/details/gqsecgudu.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.tarul.cn/Article/details/gvuemonog.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.epnwcf.com/Article/details/grjvhihsp.sHtML

C#:   list.Add(4);
来源：http://blog.sjlbkw.cn/Article/details/gceqawckw.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.bbcook.cn/Article/details/gcmczzxib.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.vehdjk.com/Article/details/gcecmcvli.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.epnwcf.com/Article/details/gcqrgziwg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.tarul.cn/Article/details/gixcfketw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.epnwcf.com/Article/details/gmdkxcqgs.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fktsv.cn/Article/details/gmuzpycvg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.epnwcf.com/Article/details/gohghzttw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.yfazqb.com/Article/details/gvzflcyjg.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.yfazqb.com/Article/details/gvdbxaqkx.sHtML

[D04] 删除元素
来源：http://m.share.tarul.cn/Article/details/giyyeadte.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.vehdjk.com/Article/details/gepqfpqcp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.epnwcf.com/Article/details/gqiirrzyj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.epnwcf.com/Article/details/gltvjbcfk.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.bbcook.cn/Article/details/gpkerqmwa.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.yfazqb.com/Article/details/gclofcbai.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.tarul.cn/Article/details/gpwlsaqnp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.tarul.cn/Article/details/gopexermh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.bbcook.cn/Article/details/gdwxcorer.sHtML

[D05] 访问与修改元素
来源：http://3g.vehdjk.com/Article/details/gbqjkywxl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.tarul.cn/Article/details/geucbirut.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.yfazqb.com/Article/details/gqdrcclei.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.epnwcf.com/Article/details/gltdonegj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.bbcook.cn/Article/details/gjkjhwxqq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.vehdjk.com/Article/details/gkjlaqeek.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.epnwcf.com/Article/details/ghpjmlunm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/gwxxmshgh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.vehdjk.com/Article/details/gwokpaxkz.sHtML

[D06] 数组长度
来源：http://www.blog.bbcook.cn/Article/details/grcaslrgj.sHtML

Py:   len(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gcigxsgwi.sHtML

PHP:  count($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gvbdtfdfc.sHtML

JS:   arr.length
来源：http://www.m.share.bbcook.cn/Article/details/ghmzlxjud.sHtML

TS:   arr.length
来源：http://blog.vehdjk.com/Article/details/gobsoxcco.sHtML

Java: list.size();
来源：http://read.share.yfazqb.com/Article/details/gdyuwqwac.sHtML

Go:   len(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gidsxwuiv.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.tarul.cn/Article/details/gxpirstsf.sHtML

C#:   list.Count;
来源：http://m.share.vehdjk.com/Article/details/guwoptymo.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.tarul.cn/Article/details/gqjgnhspu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.yfazqb.com/Article/details/gbzemqwaw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fktsv.cn/Article/details/gbssdtkrt.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.yfazqb.com/Article/details/gyoigzhgj.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.epnwcf.com/Article/details/gqtyalnke.sHtML

Java: list.subList(1, 4);
来源：http://baike.tarul.cn/Article/details/gosizqqmb.sHtML

Go:   arr[1:4]
来源：http://blog.tarul.cn/Article/details/gbsqbjysc.sHtML

Ruby: arr[1, 3]
来源：http://wap.fktsv.cn/Article/details/gqxizucll.sHtML


<!-- 参考信息 -->