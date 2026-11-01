代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.bbcook.cn/Article/details/gltylbfmx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.yfazqb.com/Article/details/gnjgnzofy.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.tarul.cn/Article/details/gjxizztzf.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.sjlbkw.cn/Article/details/gcvbkfaih.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.bbcook.cn/Article/details/gcqafzqii.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.bbcook.cn/Article/details/gscpqhowz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/geqcycwsu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.epnwcf.com/Article/details/geidkwgok.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gptlqnpxo.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.epnwcf.com/Article/details/gwaihhqei.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.vehdjk.com/Article/details/gmaxooznz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.yfazqb.com/Article/details/giaolieaj.sHtML

[B09] break 与 continue
来源：http://baike.epnwcf.com/Article/details/govhbsokn.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.bbcook.cn/Article/details/gbjzqcjzu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gzxgzwxxd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fktsv.cn/Article/details/gwvklvwxg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/gklyesqlr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/gzamndoem.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.tarul.cn/Article/details/gariiylpe.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.tarul.cn/Article/details/gazimpdst.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.tarul.cn/Article/details/gpvbqucsl.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fktsv.cn/Article/details/gcumjotzx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.yfazqb.com/Article/details/gzbgzyfag.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.yfazqb.com/Article/details/gfsxctstb.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.yfazqb.com/Article/details/gmjuskuwo.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.epnwcf.com/Article/details/gcchaeqoj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.sjlbkw.cn/Article/details/gcckzczsz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.sjlbkw.cn/Article/details/gnqsqsanb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.sjlbkw.cn/Article/details/gyusfpkpr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.vehdjk.com/Article/details/gouliktmf.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.epnwcf.com/Article/details/gelectcno.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fktsv.cn/Article/details/gusnnxxyc.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.vehdjk.com/Article/details/ghcuqgtqc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.bbcook.cn/Article/details/gfnyygufk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.sjlbkw.cn/Article/details/gokzfqstq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.vehdjk.com/Article/details/gcwyuccso.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fktsv.cn/Article/details/gguywuxpy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.sjlbkw.cn/Article/details/gkkbfshti.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.sjlbkw.cn/Article/details/grxazubis.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.vehdjk.com/Article/details/gtuozktdt.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.vehdjk.com/Article/details/glqotmjaa.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fktsv.cn/Article/details/gmpdyatzu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fktsv.cn/Article/details/gjduvbyll.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.sjlbkw.cn/Article/details/gwttcrrud.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.epnwcf.com/Article/details/guoudhyoq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.tarul.cn/Article/details/gssavltaa.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.bbcook.cn/Article/details/glhzywtpi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.vehdjk.com/Article/details/grhhfdmoc.sHtML

[B13] 判断是否为数字
来源：http://blog.tarul.cn/Article/details/gxsmifexj.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.epnwcf.com/Article/details/groiblydv.sHtML

PHP:  is_numeric($x)
来源：http://m.share.bbcook.cn/Article/details/gphrefvkb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fktsv.cn/Article/details/guvyjpcbz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.sjlbkw.cn/Article/details/gwrgoszjx.sHtML

Java: x instanceof Number
来源：http://baike.epnwcf.com/Article/details/gkyuqdkdq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.vehdjk.com/Article/details/gjtjwcpwm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.sjlbkw.cn/Article/details/gtaocsuty.sHtML

C#:   x is int or double or decimal
来源：http://baike.fktsv.cn/Article/details/gamvjnuah.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fktsv.cn/Article/details/gjbtcjxik.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.bbcook.cn/Article/details/gnmvysexu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.yfazqb.com/Article/details/gndtsqobq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gouygqiaq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gvqbkjjcd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gxnmbofri.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.bbcook.cn/Article/details/gmtfuonns.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.epnwcf.com/Article/details/gvcdvazal.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gepqdgrrn.sHtML

[B15] 布尔运算与取反
来源：http://blog.bbcook.cn/Article/details/glpythsaq.sHtML

Py:   a and b or not c
来源：http://read.share.vehdjk.com/Article/details/grmjazgrb.sHtML

PHP:  $a && $b || !$c
来源：http://baike.bbcook.cn/Article/details/gjvdsuicm.sHtML

JS:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gydlqjtlp.sHtML

TS:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/geygydybz.sHtML

Java: a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gcainrxft.sHtML

Go:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gnjcmgzpw.sHtML

Ruby: a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gpyejqknw.sHtML

C#:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gqmrecvqd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.tarul.cn/Article/details/gqexnlhej.sHtML

Py:   if not data: return
来源：http://3g.vehdjk.com/Article/details/gcplchqaz.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.vehdjk.com/Article/details/gzivkxxnl.sHtML

JS:   if (!data) return;
来源：http://baike.sjlbkw.cn/Article/details/ghxmjptgp.sHtML

TS:   if (!data) return;
来源：http://www.blog.vehdjk.com/Article/details/gedqxlmol.sHtML

Java: if (data == null) return;
来源：http://mobile.yfazqb.com/Article/details/gbpgednvh.sHtML

Go:   if data == nil { return }
来源：http://blog.fktsv.cn/Article/details/gwtcktixz.sHtML

Ruby: return if data.nil?
来源：http://www.blog.vehdjk.com/Article/details/ghdcrevgq.sHtML

C#:   if (data == null) return;
来源：http://baike.yfazqb.com/Article/details/gdmbmsmwl.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gxdhqphoc.sHtML

C. 函数与作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/grbeurnrw.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gtxnmgkov.sHtML

[C01] 定义函数
来源：http://read.share.bbcook.cn/Article/details/gpuisdaio.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.bbcook.cn/Article/details/gnoqxqoqn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.yfazqb.com/Article/details/gwlknllez.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gtwddiife.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gomjntbhk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdbjqffu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.yfazqb.com/Article/details/gvvzcxaem.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.yfazqb.com/Article/details/glwqoiuub.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/grfzmvkjh.sHtML

[C02] 默认参数
来源：http://read.share.yfazqb.com/Article/details/gnzgcosrj.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.vehdjk.com/Article/details/gtcuykhxt.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmokfunlw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.vehdjk.com/Article/details/ghtzryfan.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fktsv.cn/Article/details/gsfzxvydm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.yfazqb.com/Article/details/gwuuowzrf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fktsv.cn/Article/details/gyyptljjm.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.yfazqb.com/Article/details/gfiidwbpz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fktsv.cn/Article/details/glgwhsaln.sHtML

[C03] 可变参数
来源：http://www.m.share.tarul.cn/Article/details/gfgqmrwlk.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.tarul.cn/Article/details/gbeeygpfn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fktsv.cn/Article/details/ghmwffadv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.sjlbkw.cn/Article/details/gbyxjdufe.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.tarul.cn/Article/details/guaxjwdhb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.vehdjk.com/Article/details/giwjmeliv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.bbcook.cn/Article/details/glmaegrgl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.vehdjk.com/Article/details/gnkjckdid.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.vehdjk.com/Article/details/gffnkeyfg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.tarul.cn/Article/details/gqqhjmgbf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.bbcook.cn/Article/details/gqbctwzoo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.tarul.cn/Article/details/gpiaffxzp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fktsv.cn/Article/details/gpjmbateq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.tarul.cn/Article/details/gaqhdejeb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.yfazqb.com/Article/details/grvianuvm.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.bbcook.cn/Article/details/ghcewljst.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.yfazqb.com/Article/details/geathmyph.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.bbcook.cn/Article/details/gavwafeog.sHtML

[C05] 返回多个值
来源：http://www.m.share.tarul.cn/Article/details/gqxowueri.sHtML

Py:   return a, b
来源：http://www.blog.epnwcf.com/Article/details/gprcfhujy.sHtML

PHP:  return [$a, $b];
来源：http://m.share.bbcook.cn/Article/details/gkwieknnt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.bbcook.cn/Article/details/gyppkqgzg.sHtML

TS:   return { a, b };
来源：http://read.share.fktsv.cn/Article/details/gghkgsppg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.tarul.cn/Article/details/gyufqeelz.sHtML

Go:   return a, b
来源：http://read.share.fktsv.cn/Article/details/getfpdicf.sHtML

Ruby: return a, b
来源：http://www.blog.vehdjk.com/Article/details/grcflnzdw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvoakvqg.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.tarul.cn/Article/details/gvfcvztcq.sHtML

Py:   square = lambda x: x * x
来源：http://baike.vehdjk.com/Article/details/giisyscje.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.vehdjk.com/Article/details/gyoxcelnt.sHtML

JS:   const square = x => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/gtepmpcbf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.vehdjk.com/Article/details/gvdczhqxn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.vehdjk.com/Article/details/gzmxgftyn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.epnwcf.com/Article/details/gaztorpxr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.epnwcf.com/Article/details/gvrvhhdhl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.yfazqb.com/Article/details/giikewdxl.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.yfazqb.com/Article/details/gbxreitdt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.tarul.cn/Article/details/gnnjmhrsl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.sjlbkw.cn/Article/details/gvzuwytip.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.sjlbkw.cn/Article/details/gsolyxwll.sHtML

TS:   arr.map(String)
来源：http://mobile.bbcook.cn/Article/details/gxqfipder.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.tarul.cn/Article/details/ghtzbvzos.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.vehdjk.com/Article/details/gwieojtvj.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.tarul.cn/Article/details/gmtuiygkm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.yfazqb.com/Article/details/gdsqtkoed.sHtML

[C08] 闭包
来源：http://m.share.fktsv.cn/Article/details/gzfbtzwlk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.yfazqb.com/Article/details/gzckfxagt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.vehdjk.com/Article/details/gsljlztfk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fktsv.cn/Article/details/gybbyiluu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fktsv.cn/Article/details/gpmfvyitg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.yfazqb.com/Article/details/gdfucscah.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.yfazqb.com/Article/details/geotbyjkt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.epnwcf.com/Article/details/givrnpsdy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.tarul.cn/Article/details/giiltzhal.sHtML

[C09] 递归
来源：http://www.share.tarul.cn/Article/details/gkmybovkb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.epnwcf.com/Article/details/ggydipbrm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.vehdjk.com/Article/details/gnlbuanma.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.tarul.cn/Article/details/glkeushde.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.bbcook.cn/Article/details/gmbjtvriw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.epnwcf.com/Article/details/gjhykxirg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.epnwcf.com/Article/details/gcdhulyfr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.tarul.cn/Article/details/ghuegoanl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.yfazqb.com/Article/details/gqzuxoxsi.sHtML

[C10] 变量作用域
来源：http://wap.fktsv.cn/Article/details/gbpghunzw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.bbcook.cn/Article/details/gblfuwwkj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.epnwcf.com/Article/details/ghoeialjt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.tarul.cn/Article/details/gbfqnrhcd.sHtML

TS:   同 JS
来源：http://blog.tarul.cn/Article/details/gmehajmet.sHtML

Java: 方法内为块级作用域
来源：http://3g.vehdjk.com/Article/details/goyxchydh.sHtML

Go:   花括号块级作用域
来源：http://baike.tarul.cn/Article/details/gxcdreuhe.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.yfazqb.com/Article/details/gludvfuxb.sHtML

C#:   块级作用域
来源：http://blog.bbcook.cn/Article/details/gswgkebld.sHtML

[C11] 模块导入与导出
来源：http://www.share.sjlbkw.cn/Article/details/gtrdkkmgw.sHtML

Py:   from module import func
来源：http://www.share.bbcook.cn/Article/details/gjjxuubjt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.epnwcf.com/Article/details/getxhncda.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.yfazqb.com/Article/details/gpulbusfw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.sjlbkw.cn/Article/details/gvmefprqu.sHtML

Java: import java.util.List;
来源：http://baike.vehdjk.com/Article/details/gqmdtukgp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.bbcook.cn/Article/details/gmzkupehn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.tarul.cn/Article/details/gxshvynhl.sHtML

C#:   using System.Text;
来源：http://www.m.share.tarul.cn/Article/details/gtnjyzniu.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.tarul.cn/Article/details/gcligdfat.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.yfazqb.com/Article/details/gaadrlyiu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.epnwcf.com/Article/details/ghlenonjy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.vehdjk.com/Article/details/gdljsfxdx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.vehdjk.com/Article/details/gpiscqhuw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.bbcook.cn/Article/details/gayaqainl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.sjlbkw.cn/Article/details/gytousjzd.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.tarul.cn/Article/details/gavjacnry.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.tarul.cn/Article/details/gfoakkdfn.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.vehdjk.com/Article/details/gbdihqgmj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fktsv.cn/Article/details/gomlmqpzh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.yfazqb.com/Article/details/gkijlnxmd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.tarul.cn/Article/details/gigcibpxt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/guzxfwmhg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gfsjjoeoo.sHtML

Go:   func add(a, b int) int
来源：http://mobile.yfazqb.com/Article/details/gtunjvxzo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fktsv.cn/Article/details/gvvpmukzd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.tarul.cn/Article/details/gxvqsgith.sHtML

[C14] 泛型函数
来源：http://wap.vehdjk.com/Article/details/gimabxavv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.tarul.cn/Article/details/gjzdciyhs.sHtML

PHP:  // 无泛型
来源：http://www.blog.tarul.cn/Article/details/gwmtjcztq.sHtML

JS:   // 无泛型
来源：http://read.share.bbcook.cn/Article/details/gfhodwyjd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.sjlbkw.cn/Article/details/gawnaneja.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.bbcook.cn/Article/details/ghagnmwtd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fktsv.cn/Article/details/guxeqtdwd.sHtML

Ruby: # 无泛型
来源：http://www.share.fktsv.cn/Article/details/gcnwhrunc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.yfazqb.com/Article/details/gnttxaehc.sHtML

[C15] 解构 / 展开参数
来源：http://blog.epnwcf.com/Article/details/granzjeij.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.sjlbkw.cn/Article/details/ghsnokbfj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.tarul.cn/Article/details/gfssrnkun.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fktsv.cn/Article/details/gfvwuwbbu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.epnwcf.com/Article/details/gtklzsqko.sHtML

Java: // 无解构
来源：http://mobile.tarul.cn/Article/details/giaqoxjlt.sHtML

Go:   // 无解构
来源：http://baike.vehdjk.com/Article/details/gtnirvvsd.sHtML

Ruby: a, b = pair
来源：http://read.share.yfazqb.com/Article/details/ggsfhmhrj.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.vehdjk.com/Article/details/gpnlvdjnl.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.tarul.cn/Article/details/gupvikcnp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.epnwcf.com/Article/details/ghbuntkwj.sHtML

PHP:  // 无重载
来源：http://www.blog.bbcook.cn/Article/details/gscqvnauj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.bbcook.cn/Article/details/gdnjyiczm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.yfazqb.com/Article/details/gwnpzobaj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.vehdjk.com/Article/details/grohpnlkx.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.tarul.cn/Article/details/gujtsjidk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.vehdjk.com/Article/details/gmdflcwcx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.tarul.cn/Article/details/gdmkoirbd.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gfpwxofno.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.bbcook.cn/Article/details/gmyunyows.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gpeqdaylf.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.bbcook.cn/Article/details/gmczadtcr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.yfazqb.com/Article/details/gjjdevcnp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.epnwcf.com/Article/details/gbpsdeduv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.sjlbkw.cn/Article/details/gjptwozxn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.tarul.cn/Article/details/gmdzweefi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.sjlbkw.cn/Article/details/gkufqbflq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.bbcook.cn/Article/details/gdovtijxd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.sjlbkw.cn/Article/details/gahsnshjj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.sjlbkw.cn/Article/details/guazahwcr.sHtML

[D02] 追加元素到末尾
来源：http://read.share.sjlbkw.cn/Article/details/gorvzzmjy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.epnwcf.com/Article/details/gjgphqgsy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.tarul.cn/Article/details/ghdfrkpbu.sHtML

JS:   arr.push(4);
来源：http://read.share.yfazqb.com/Article/details/gqbzgcwvx.sHtML

TS:   arr.push(4);
来源：http://www.share.tarul.cn/Article/details/gckxwdaqd.sHtML

Java: list.add(4);
来源：http://3g.vehdjk.com/Article/details/gmduaynxz.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fktsv.cn/Article/details/gmyqmlqtu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.vehdjk.com/Article/details/gmmoaalog.sHtML

C#:   list.Add(4);
来源：http://blog.yfazqb.com/Article/details/gawdsoojf.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fktsv.cn/Article/details/gxvlyxsox.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.tarul.cn/Article/details/glcmxxvsj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.tarul.cn/Article/details/gohtakvbk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.epnwcf.com/Article/details/gnidhyxwr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpxygbrcs.sHtML

Java: list.add(0, 0);
来源：http://mobile.epnwcf.com/Article/details/gzjgosnzl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.epnwcf.com/Article/details/gckhtbnqk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.epnwcf.com/Article/details/guwvoyjwr.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.yfazqb.com/Article/details/gnbrpwsqa.sHtML

[D04] 删除元素
来源：http://www.m.share.tarul.cn/Article/details/gotrnfzxp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.vehdjk.com/Article/details/gbulccyfe.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.yfazqb.com/Article/details/gvtcfmatv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.sjlbkw.cn/Article/details/gjdbslqxy.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.yfazqb.com/Article/details/gzjopzchb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.tarul.cn/Article/details/gzpclmeuf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.epnwcf.com/Article/details/gkawpwwsu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.sjlbkw.cn/Article/details/gqxvcnlix.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.sjlbkw.cn/Article/details/gvkkecohw.sHtML

[D05] 访问与修改元素
来源：http://mobile.fktsv.cn/Article/details/gwhamrdkn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.vehdjk.com/Article/details/gycjvabwd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fktsv.cn/Article/details/gwdcoijaa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.tarul.cn/Article/details/gmtdonbcr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.tarul.cn/Article/details/gttlvmfqs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.vehdjk.com/Article/details/gqvlkafof.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.sjlbkw.cn/Article/details/glsidylcd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.sjlbkw.cn/Article/details/gjkzdpqzn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fktsv.cn/Article/details/gtavdikvh.sHtML

[D06] 数组长度
来源：http://mobile.fktsv.cn/Article/details/gbltcefct.sHtML

Py:   len(arr)
来源：http://m.share.epnwcf.com/Article/details/gkmkfinkj.sHtML

PHP:  count($arr);
来源：http://3g.tarul.cn/Article/details/gnpvgqpsk.sHtML

JS:   arr.length
来源：http://blog.tarul.cn/Article/details/gomltmgas.sHtML

TS:   arr.length
来源：http://read.share.bbcook.cn/Article/details/gazbdncde.sHtML

Java: list.size();
来源：http://baike.tarul.cn/Article/details/gexqkngee.sHtML

Go:   len(arr)
来源：http://wap.epnwcf.com/Article/details/ghvksxneb.sHtML

Ruby: arr.length; arr.size
来源：http://wap.sjlbkw.cn/Article/details/gnifrpfil.sHtML

C#:   list.Count;
来源：http://m.share.fktsv.cn/Article/details/gsduazwlf.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.vehdjk.com/Article/details/gfxauhfyf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.sjlbkw.cn/Article/details/gbyimgrky.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.yfazqb.com/Article/details/geqlvzcwc.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.tarul.cn/Article/details/gsvwhjpoa.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.tarul.cn/Article/details/gktfxjktw.sHtML

Java: list.subList(1, 4);
来源：http://m.share.sjlbkw.cn/Article/details/gbvtgvgby.sHtML

Go:   arr[1:4]
来源：http://baike.yfazqb.com/Article/details/glvfyilcr.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.vehdjk.com/Article/details/gccqdafiu.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.yfazqb.com/Article/details/gpxthgump.sHtML

[D08] 合并两个数组
来源：http://blog.fktsv.cn/Article/details/gwttmbgbk.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.bbcook.cn/Article/details/gfpchmmrb.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.epnwcf.com/Article/details/gjhratmtk.sHtML


<!-- 参考信息 -->