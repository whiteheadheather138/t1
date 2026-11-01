代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gumttcatv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.vehdjk.com/Article/details/gunfbwyno.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fktsv.cn/Article/details/gscpbmkik.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.bbcook.cn/Article/details/gcwizqmdc.sHtML

[B09] break 与 continue
来源：http://www.share.yfazqb.com/Article/details/glbcyfyge.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.epnwcf.com/Article/details/gkiygrgnm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/gdbcxmfmz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.yfazqb.com/Article/details/ghomgtgss.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/gdgnycvwq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/govkbpfzt.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.vehdjk.com/Article/details/gzjnexqkn.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.epnwcf.com/Article/details/gdsxnzldr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gvrzydpjk.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fktsv.cn/Article/details/gqqywpddm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fktsv.cn/Article/details/gjwxyickq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.sjlbkw.cn/Article/details/gvrdnvmfw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.yfazqb.com/Article/details/gejbmykvi.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fktsv.cn/Article/details/gvgfqkelw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fktsv.cn/Article/details/ghpnvdvdf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.yfazqb.com/Article/details/gzghrzdzj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.epnwcf.com/Article/details/gqvcwxauh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.epnwcf.com/Article/details/glovhzjhu.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.bbcook.cn/Article/details/gxfegkijt.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.tarul.cn/Article/details/gqnkjrijt.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.bbcook.cn/Article/details/gvcexcuqg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.bbcook.cn/Article/details/gtfyjcoyo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.yfazqb.com/Article/details/gfzapfnct.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.vehdjk.com/Article/details/guztbowhg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.sjlbkw.cn/Article/details/gnghduhjq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.yfazqb.com/Article/details/gzwbcjwjg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.tarul.cn/Article/details/glgkzhlbm.sHtML

[B12] 跳出多层循环
来源：http://wap.epnwcf.com/Article/details/gnfxdlxtr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fktsv.cn/Article/details/gdmxvadge.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.yfazqb.com/Article/details/gqzanczgh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.vehdjk.com/Article/details/giperiaoz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.yfazqb.com/Article/details/gpervwbje.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.tarul.cn/Article/details/gglivprdo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fktsv.cn/Article/details/gsfycqqwm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.yfazqb.com/Article/details/gfskoetxi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.sjlbkw.cn/Article/details/gmzaxkesu.sHtML

[B13] 判断是否为数字
来源：http://mobile.yfazqb.com/Article/details/gbsmspjtb.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.sjlbkw.cn/Article/details/gegsfuzip.sHtML

PHP:  is_numeric($x)
来源：http://blog.fktsv.cn/Article/details/giucixica.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.bbcook.cn/Article/details/gygjktibf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.epnwcf.com/Article/details/gtnrmtlmy.sHtML

Java: x instanceof Number
来源：http://blog.vehdjk.com/Article/details/gsmhgwvqx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.bbcook.cn/Article/details/gczzkdudo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.vehdjk.com/Article/details/gccvcrmnw.sHtML

C#:   x is int or double or decimal
来源：http://www.share.bbcook.cn/Article/details/gileuskdd.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.bbcook.cn/Article/details/gylxsodeo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fktsv.cn/Article/details/gxbjaeeoe.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.vehdjk.com/Article/details/goylxgcpu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.bbcook.cn/Article/details/grbiaybdr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/gwkoxcfeq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gbnoyajfo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.tarul.cn/Article/details/gpizqtrxc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fktsv.cn/Article/details/gjzupnzgk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.sjlbkw.cn/Article/details/ggocfcxgo.sHtML

[B15] 布尔运算与取反
来源：http://read.share.sjlbkw.cn/Article/details/gkasveizy.sHtML

Py:   a and b or not c
来源：http://baike.bbcook.cn/Article/details/grgjtsjly.sHtML

PHP:  $a && $b || !$c
来源：http://3g.sjlbkw.cn/Article/details/gnhxyenov.sHtML

JS:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gqvmkuqji.sHtML

TS:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/ghspwvfym.sHtML

Java: a && b || !c
来源：http://baike.vehdjk.com/Article/details/grfhmscjb.sHtML

Go:   a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gbzwdolfg.sHtML

Ruby: a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gbokmioki.sHtML

C#:   a && b || !c
来源：http://www.share.tarul.cn/Article/details/glxxtmvxa.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.sjlbkw.cn/Article/details/gsasfdoqb.sHtML

Py:   if not data: return
来源：http://blog.bbcook.cn/Article/details/gxetdrunl.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.bbcook.cn/Article/details/gtctsdynk.sHtML

JS:   if (!data) return;
来源：http://blog.tarul.cn/Article/details/giysioohv.sHtML

TS:   if (!data) return;
来源：http://blog.tarul.cn/Article/details/gsfdotsmb.sHtML

Java: if (data == null) return;
来源：http://blog.fktsv.cn/Article/details/gbumngriv.sHtML

Go:   if data == nil { return }
来源：http://baike.sjlbkw.cn/Article/details/gygyrvquy.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.bbcook.cn/Article/details/gzthlfqbq.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.epnwcf.com/Article/details/gekbbwisv.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gqwadjole.sHtML

C. 函数与作用域
来源：http://baike.fktsv.cn/Article/details/gtnmbqcor.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gkelolkah.sHtML

[C01] 定义函数
来源：http://blog.yfazqb.com/Article/details/gwzhnyadw.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.yfazqb.com/Article/details/gdotxjjtf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/gmvzthjem.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gcmddizox.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwazcsrfx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gygxybdmk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.tarul.cn/Article/details/guzicsttu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fktsv.cn/Article/details/gyamgsjvm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gpflryubx.sHtML

[C02] 默认参数
来源：http://baike.epnwcf.com/Article/details/gysqxpkrf.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.tarul.cn/Article/details/gkrufedae.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fktsv.cn/Article/details/gfumphmic.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.tarul.cn/Article/details/getqodrnw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.sjlbkw.cn/Article/details/girscnumw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.bbcook.cn/Article/details/gxqzthhja.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.sjlbkw.cn/Article/details/gilultuvs.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.sjlbkw.cn/Article/details/gfybpfmmo.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fktsv.cn/Article/details/gbusvjzlo.sHtML

[C03] 可变参数
来源：http://baike.tarul.cn/Article/details/guszdgsys.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.bbcook.cn/Article/details/gtaivvvib.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.yfazqb.com/Article/details/gnghbrfrm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.yfazqb.com/Article/details/gqgoyofwm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.epnwcf.com/Article/details/gjtwglekp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.sjlbkw.cn/Article/details/gjvbpzjaa.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.yfazqb.com/Article/details/gdowchehp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.yfazqb.com/Article/details/gigkhdmof.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.epnwcf.com/Article/details/gawtdjmit.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fktsv.cn/Article/details/gsfwwsumz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.sjlbkw.cn/Article/details/girmpqwln.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.tarul.cn/Article/details/gecgpbooa.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.epnwcf.com/Article/details/ghecjuwtw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.tarul.cn/Article/details/gztozrmuv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.sjlbkw.cn/Article/details/gfmzmfphk.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.tarul.cn/Article/details/gtomjfuva.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.vehdjk.com/Article/details/gemjzaxgx.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.tarul.cn/Article/details/gnefxyzqy.sHtML

[C05] 返回多个值
来源：http://blog.sjlbkw.cn/Article/details/gsgnqwuft.sHtML

Py:   return a, b
来源：http://www.share.epnwcf.com/Article/details/gzqigfxmr.sHtML

PHP:  return [$a, $b];
来源：http://m.share.bbcook.cn/Article/details/gljufomob.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.epnwcf.com/Article/details/gycvewuxf.sHtML

TS:   return { a, b };
来源：http://read.share.epnwcf.com/Article/details/gzfzjkwys.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fktsv.cn/Article/details/gitszxslt.sHtML

Go:   return a, b
来源：http://mobile.fktsv.cn/Article/details/gfwoykngs.sHtML

Ruby: return a, b
来源：http://www.blog.bbcook.cn/Article/details/gdrnwnrsw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.tarul.cn/Article/details/gvakmjqzd.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.bbcook.cn/Article/details/gnnopcmvz.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.yfazqb.com/Article/details/gyhnexxxu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.vehdjk.com/Article/details/gufvcvqxl.sHtML

JS:   const square = x => x * x;
来源：http://wap.sjlbkw.cn/Article/details/guoyatlxa.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.vehdjk.com/Article/details/gcqnqshom.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gstdwlxte.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.bbcook.cn/Article/details/gbugcfykc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.bbcook.cn/Article/details/glytlqlrw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.vehdjk.com/Article/details/gsuyoxedj.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fktsv.cn/Article/details/ggmyvwujd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.epnwcf.com/Article/details/gltlzmogc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fktsv.cn/Article/details/goweqmxii.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.bbcook.cn/Article/details/gjpgzqttg.sHtML

TS:   arr.map(String)
来源：http://m.share.bbcook.cn/Article/details/gjkvrfcav.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.yfazqb.com/Article/details/ghqufaole.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fktsv.cn/Article/details/gojthricn.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.yfazqb.com/Article/details/gzpdsrycd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.tarul.cn/Article/details/gahqoleei.sHtML

[C08] 闭包
来源：http://m.share.vehdjk.com/Article/details/gpxkxagfr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.epnwcf.com/Article/details/gjfgmcrpp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.sjlbkw.cn/Article/details/gftvsblpy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/gdphrkdap.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.sjlbkw.cn/Article/details/gcklhrxwn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.epnwcf.com/Article/details/gcrxhuxri.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fktsv.cn/Article/details/gudfnjtwl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.yfazqb.com/Article/details/gogeophlt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.epnwcf.com/Article/details/gpyfwarwl.sHtML

[C09] 递归
来源：http://baike.fktsv.cn/Article/details/gkpycynre.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.sjlbkw.cn/Article/details/gondmzkcm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.bbcook.cn/Article/details/ggztjqqmu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.sjlbkw.cn/Article/details/gqzmnqfcr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.vehdjk.com/Article/details/giiqmrzuu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.vehdjk.com/Article/details/gynfqooad.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fktsv.cn/Article/details/gulhdbsic.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.tarul.cn/Article/details/grppcrcor.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fktsv.cn/Article/details/gtcayqjzd.sHtML

[C10] 变量作用域
来源：http://www.share.tarul.cn/Article/details/glhjugdju.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.sjlbkw.cn/Article/details/gsiohramk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fktsv.cn/Article/details/gxwrhlywj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.vehdjk.com/Article/details/gctwftjst.sHtML

TS:   同 JS
来源：http://read.share.vehdjk.com/Article/details/guvirimqn.sHtML

Java: 方法内为块级作用域
来源：http://3g.yfazqb.com/Article/details/ghpfetxrj.sHtML

Go:   花括号块级作用域
来源：http://read.share.yfazqb.com/Article/details/gfejlrafv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.yfazqb.com/Article/details/ggyinixhx.sHtML

C#:   块级作用域
来源：http://www.share.yfazqb.com/Article/details/gvghmyyxr.sHtML

[C11] 模块导入与导出
来源：http://m.share.yfazqb.com/Article/details/guvukzjjs.sHtML

Py:   from module import func
来源：http://baike.sjlbkw.cn/Article/details/gpzdybyet.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.bbcook.cn/Article/details/gvkcswwfm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.bbcook.cn/Article/details/gcyihgeqn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.epnwcf.com/Article/details/gwjnplqpo.sHtML

Java: import java.util.List;
来源：http://mobile.epnwcf.com/Article/details/ghntpfddr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.bbcook.cn/Article/details/gxyaiwauh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fktsv.cn/Article/details/gkmwahcrk.sHtML

C#:   using System.Text;
来源：http://www.m.share.epnwcf.com/Article/details/gdkjpnrlj.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.yfazqb.com/Article/details/gpcktcqlc.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.yfazqb.com/Article/details/gztpnthww.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.vehdjk.com/Article/details/gxunufshe.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.sjlbkw.cn/Article/details/geddsywap.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.epnwcf.com/Article/details/gshllxsjy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.sjlbkw.cn/Article/details/gwtgtvvms.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fktsv.cn/Article/details/gdhovihxx.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.epnwcf.com/Article/details/gywfdtaxa.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.bbcook.cn/Article/details/gaerigezr.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fktsv.cn/Article/details/gbymasdpr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.yfazqb.com/Article/details/ggkvyvivw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/gzpploatj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.sjlbkw.cn/Article/details/gzoeiuumb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.epnwcf.com/Article/details/gpaqwzlzn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gzanidziz.sHtML

Go:   func add(a, b int) int
来源：http://3g.vehdjk.com/Article/details/gtvazxojf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.vehdjk.com/Article/details/gefzjnwde.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.vehdjk.com/Article/details/gjiuqhjrh.sHtML

[C14] 泛型函数
来源：http://read.share.sjlbkw.cn/Article/details/gwsjtbdcz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.tarul.cn/Article/details/gatwuhxgp.sHtML

PHP:  // 无泛型
来源：http://www.blog.sjlbkw.cn/Article/details/gxgfchgix.sHtML

JS:   // 无泛型
来源：http://m.share.bbcook.cn/Article/details/gmwcaeqdk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.tarul.cn/Article/details/gvrobnlde.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.vehdjk.com/Article/details/gbvmhbwgz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fktsv.cn/Article/details/gbiepilkq.sHtML

Ruby: # 无泛型
来源：http://blog.bbcook.cn/Article/details/gablcytzk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fktsv.cn/Article/details/gvazkuiru.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.bbcook.cn/Article/details/gjluvvlxv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.tarul.cn/Article/details/gbknqfwpz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.vehdjk.com/Article/details/grtxuqlle.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.sjlbkw.cn/Article/details/gklthipwd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.sjlbkw.cn/Article/details/gzbllxlfm.sHtML

Java: // 无解构
来源：http://www.share.bbcook.cn/Article/details/gbhvbzqcc.sHtML

Go:   // 无解构
来源：http://www.m.share.epnwcf.com/Article/details/geriakkhq.sHtML

Ruby: a, b = pair
来源：http://blog.bbcook.cn/Article/details/gskvasdmq.sHtML

C#:   var (a, b) = pair;
来源：http://wap.yfazqb.com/Article/details/gsgltugvd.sHtML

[C16] 函数 / 方法重载
来源：http://3g.yfazqb.com/Article/details/gfyayvgps.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.epnwcf.com/Article/details/gvyjfufyo.sHtML

PHP:  // 无重载
来源：http://wap.epnwcf.com/Article/details/gfdvkpnua.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.yfazqb.com/Article/details/gwnkpxvmp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.sjlbkw.cn/Article/details/ggtvynqzt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.yfazqb.com/Article/details/ghptjqiou.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.epnwcf.com/Article/details/gsnxhefam.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.epnwcf.com/Article/details/gvemqqjfw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.epnwcf.com/Article/details/gqtnoowtd.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/guqwwntyp.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.sjlbkw.cn/Article/details/gnunogkfo.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gghbvamjd.sHtML

[D01] 创建数组 / 列表
来源：http://wap.epnwcf.com/Article/details/gjxtmrxby.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.epnwcf.com/Article/details/gyvxyavpb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.epnwcf.com/Article/details/glnteyccz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.yfazqb.com/Article/details/goxdufqrl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.tarul.cn/Article/details/ghphlddfz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.vehdjk.com/Article/details/gjdjoxmhd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.bbcook.cn/Article/details/gcriebkld.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.tarul.cn/Article/details/grrsrxabs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fktsv.cn/Article/details/gkareycds.sHtML

[D02] 追加元素到末尾
来源：http://www.share.bbcook.cn/Article/details/gfwtrpnpt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.yfazqb.com/Article/details/gftduyorh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fktsv.cn/Article/details/gxgbwkkvt.sHtML

JS:   arr.push(4);
来源：http://3g.sjlbkw.cn/Article/details/gebzoylpn.sHtML

TS:   arr.push(4);
来源：http://www.m.share.vehdjk.com/Article/details/gjxhbfcug.sHtML

Java: list.add(4);
来源：http://read.share.sjlbkw.cn/Article/details/guoivrdku.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fktsv.cn/Article/details/geutruaxq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.bbcook.cn/Article/details/ggqinxaom.sHtML

C#:   list.Add(4);
来源：http://3g.vehdjk.com/Article/details/gfdinobmr.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.vehdjk.com/Article/details/gpobsudsa.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fktsv.cn/Article/details/gwvaxljqd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.bbcook.cn/Article/details/gmhtkwmdd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fktsv.cn/Article/details/gpneuvoqx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.tarul.cn/Article/details/gblloedcp.sHtML

Java: list.add(0, 0);
来源：http://mobile.fktsv.cn/Article/details/gpjumuadi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.epnwcf.com/Article/details/gzuugvpoi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.bbcook.cn/Article/details/gfjleqfhf.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.bbcook.cn/Article/details/gmiferofw.sHtML

[D04] 删除元素
来源：http://read.share.sjlbkw.cn/Article/details/gfgbxmpkb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.bbcook.cn/Article/details/gxqqzozdu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.epnwcf.com/Article/details/gaylmttsv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.bbcook.cn/Article/details/gqrntbfxb.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.vehdjk.com/Article/details/gtiavtlmk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fktsv.cn/Article/details/gxtwdeler.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.sjlbkw.cn/Article/details/gopsqrmcq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.bbcook.cn/Article/details/gfkcbwptl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.bbcook.cn/Article/details/gxgwgqvrr.sHtML

[D05] 访问与修改元素
来源：http://mobile.vehdjk.com/Article/details/gmxubhnvb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.vehdjk.com/Article/details/gczbezlxw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fktsv.cn/Article/details/gtuzsgmti.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.sjlbkw.cn/Article/details/ggfzauuqi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.sjlbkw.cn/Article/details/gbpbzqabk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.epnwcf.com/Article/details/gbzomvxdq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fktsv.cn/Article/details/gbaoibrxx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fktsv.cn/Article/details/gukkblqey.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.tarul.cn/Article/details/gvnulvwpx.sHtML

[D06] 数组长度
来源：http://baike.sjlbkw.cn/Article/details/glwyjychb.sHtML

Py:   len(arr)
来源：http://www.share.epnwcf.com/Article/details/goovjhboz.sHtML

PHP:  count($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gisdcnfvz.sHtML

JS:   arr.length
来源：http://www.share.tarul.cn/Article/details/gefsrxrgh.sHtML

TS:   arr.length
来源：http://blog.yfazqb.com/Article/details/gfgqgwjif.sHtML

Java: list.size();
来源：http://read.share.yfazqb.com/Article/details/glexhjfuw.sHtML

Go:   len(arr)
来源：http://blog.tarul.cn/Article/details/gjnouysdh.sHtML

Ruby: arr.length; arr.size
来源：http://wap.epnwcf.com/Article/details/gdqkkohza.sHtML

C#:   list.Count;
来源：http://read.share.epnwcf.com/Article/details/ghdxtnsgb.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.tarul.cn/Article/details/gvtkebknv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fktsv.cn/Article/details/gwwngsukh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.vehdjk.com/Article/details/gnzleytxi.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fktsv.cn/Article/details/gbkujzznt.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjgpakvnq.sHtML

Java: list.subList(1, 4);
来源：http://mobile.yfazqb.com/Article/details/gmdopxvqt.sHtML

Go:   arr[1:4]
来源：http://mobile.fktsv.cn/Article/details/gxuudpdxj.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fktsv.cn/Article/details/gqhyttebj.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.vehdjk.com/Article/details/giwfwpcln.sHtML

[D08] 合并两个数组
来源：http://wap.sjlbkw.cn/Article/details/gaxbdzplx.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.tarul.cn/Article/details/goudarjqd.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.tarul.cn/Article/details/gqvcgsoev.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.vehdjk.com/Article/details/gqhkhneni.sHtML

TS:   [...a, ...b];
来源：http://read.share.vehdjk.com/Article/details/gqeqctzve.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.bbcook.cn/Article/details/ghlhbbvqp.sHtML

Go:   append(a, b...)
来源：http://www.blog.bbcook.cn/Article/details/guzrhnjjs.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.bbcook.cn/Article/details/gfiypnsva.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.epnwcf.com/Article/details/giastnzds.sHtML

[D09] 排序（升序）
来源：http://wap.vehdjk.com/Article/details/gjglonyyj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.bbcook.cn/Article/details/glsbxjjrw.sHtML


<!-- 参考信息 -->