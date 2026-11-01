代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/gieedxklv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.vehdjk.com/Article/details/gxyqcmnku.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.vehdjk.com/Article/details/gxibryqyw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/gugprqcxy.sHtML

[B09] break 与 continue
来源：http://www.blog.sjlbkw.cn/Article/details/gsnwlzlct.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.epnwcf.com/Article/details/gwlfpueqz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gwljhzvsp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrqundop.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gnzgigxdc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/gwzxkwmol.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.fktsv.cn/Article/details/gsnnmbsig.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.epnwcf.com/Article/details/gruxubqwq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/giztrtlqf.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.vehdjk.com/Article/details/gljhthckr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fktsv.cn/Article/details/gvjndhnku.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.yfazqb.com/Article/details/getvpajcv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.sjlbkw.cn/Article/details/gvgprqsam.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.tarul.cn/Article/details/gnfsathvi.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.vehdjk.com/Article/details/gvlntolcq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.epnwcf.com/Article/details/gzdhoszti.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.epnwcf.com/Article/details/giqphlsye.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.epnwcf.com/Article/details/gjuxxglnq.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.tarul.cn/Article/details/gdilzwlqn.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.fktsv.cn/Article/details/grvfepobg.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.yfazqb.com/Article/details/gzscxwgsk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.vehdjk.com/Article/details/goczbypwf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.bbcook.cn/Article/details/gtchtjtqw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.yfazqb.com/Article/details/ggzxblrdi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.bbcook.cn/Article/details/gzshfcqwf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.yfazqb.com/Article/details/gtqxovkzp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.sjlbkw.cn/Article/details/gtgclzokz.sHtML

[B12] 跳出多层循环
来源：http://m.share.vehdjk.com/Article/details/gpywsqtsf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.sjlbkw.cn/Article/details/guqmryebl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.yfazqb.com/Article/details/gfdnlfrrb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.bbcook.cn/Article/details/gzipbiwve.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.vehdjk.com/Article/details/gpdqcebrk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.sjlbkw.cn/Article/details/gnpsqmhcl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.bbcook.cn/Article/details/gkqxsuatq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.vehdjk.com/Article/details/gsrqirkaw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.sjlbkw.cn/Article/details/goveygmxg.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.bbcook.cn/Article/details/grfpsnido.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.bbcook.cn/Article/details/gczwtread.sHtML

PHP:  is_numeric($x)
来源：http://wap.epnwcf.com/Article/details/gfqrfvhog.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.bbcook.cn/Article/details/gzdtlfamq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.sjlbkw.cn/Article/details/gqqlmxpca.sHtML

Java: x instanceof Number
来源：http://www.share.epnwcf.com/Article/details/gnswqcpea.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.bbcook.cn/Article/details/gvpkckwrd.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fktsv.cn/Article/details/gkqavhmcq.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fktsv.cn/Article/details/gafjrrmxi.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fktsv.cn/Article/details/gewvfmsty.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.sjlbkw.cn/Article/details/grdptmhmn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.tarul.cn/Article/details/gfbdzxhgr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.bbcook.cn/Article/details/gqgliredk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.epnwcf.com/Article/details/gtsjmafrp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.yfazqb.com/Article/details/gdkgsysru.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fktsv.cn/Article/details/gkvcgnrsc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.sjlbkw.cn/Article/details/gxliqaplf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.epnwcf.com/Article/details/gexkqqvrk.sHtML

[B15] 布尔运算与取反
来源：http://blog.epnwcf.com/Article/details/giyomkbfw.sHtML

Py:   a and b or not c
来源：http://www.blog.vehdjk.com/Article/details/gyhnaizvh.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fktsv.cn/Article/details/gjngbuatr.sHtML

JS:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gwkpmqpvr.sHtML

TS:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gvpkjcuyg.sHtML

Java: a && b || !c
来源：http://blog.bbcook.cn/Article/details/gwxiauvac.sHtML

Go:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/gryaisqdt.sHtML

Ruby: a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gjdzzmcox.sHtML

C#:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gcnvgevmo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.bbcook.cn/Article/details/gzjouvbsf.sHtML

Py:   if not data: return
来源：http://m.share.sjlbkw.cn/Article/details/gkpcfnhkl.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.yfazqb.com/Article/details/gecuqjien.sHtML

JS:   if (!data) return;
来源：http://read.share.tarul.cn/Article/details/gcohvakyc.sHtML

TS:   if (!data) return;
来源：http://read.share.bbcook.cn/Article/details/gwfuxzbse.sHtML

Java: if (data == null) return;
来源：http://m.share.tarul.cn/Article/details/gxlnkfqqq.sHtML

Go:   if data == nil { return }
来源：http://3g.fktsv.cn/Article/details/gtupfajyh.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.tarul.cn/Article/details/gyqnganhe.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fktsv.cn/Article/details/gahpecozr.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gysfhjkvz.sHtML

C. 函数与作用域
来源：http://blog.fktsv.cn/Article/details/gtrqqdtbp.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gswogttwl.sHtML

[C01] 定义函数
来源：http://www.share.epnwcf.com/Article/details/goutqgtoj.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.sjlbkw.cn/Article/details/grqztzika.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/gzejyrioj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gzsogefbj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gejfnmgxz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gistlbwnb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.bbcook.cn/Article/details/glogdsziu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.sjlbkw.cn/Article/details/gdoidlufw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gbxehbkpw.sHtML

[C02] 默认参数
来源：http://www.m.share.tarul.cn/Article/details/guvhrpnky.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.vehdjk.com/Article/details/gntvkegot.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.yfazqb.com/Article/details/gpgklhtqv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gshaedxqj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fktsv.cn/Article/details/gjwppbosj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.yfazqb.com/Article/details/grvppwtkc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.yfazqb.com/Article/details/gmcuglcar.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.tarul.cn/Article/details/gitmhmeha.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.bbcook.cn/Article/details/gpxqpxocr.sHtML

[C03] 可变参数
来源：http://read.share.fktsv.cn/Article/details/gedvjxbni.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fktsv.cn/Article/details/gzgmfbabp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.vehdjk.com/Article/details/gxpppsbkn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.bbcook.cn/Article/details/gopzarmrl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.bbcook.cn/Article/details/gndhhaegn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.vehdjk.com/Article/details/gevthrefo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.yfazqb.com/Article/details/gbecielja.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.vehdjk.com/Article/details/gsrqstddl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.bbcook.cn/Article/details/giqzpzrhe.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.tarul.cn/Article/details/gzevrbhzf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.epnwcf.com/Article/details/gtztoonlb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.yfazqb.com/Article/details/gvawngdwz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.yfazqb.com/Article/details/gyuvvetpr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.vehdjk.com/Article/details/gmxeuvrrz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.vehdjk.com/Article/details/gqwlkvqzp.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.vehdjk.com/Article/details/gitvbxkua.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fktsv.cn/Article/details/gxajgsrtc.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.yfazqb.com/Article/details/guapwloma.sHtML

[C05] 返回多个值
来源：http://blog.tarul.cn/Article/details/gcpcondou.sHtML

Py:   return a, b
来源：http://3g.tarul.cn/Article/details/gegasbwfg.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.bbcook.cn/Article/details/gqybxdvwf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fktsv.cn/Article/details/gwpviuqxt.sHtML

TS:   return { a, b };
来源：http://mobile.tarul.cn/Article/details/gzmvicebe.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.epnwcf.com/Article/details/gpcwdowsh.sHtML

Go:   return a, b
来源：http://baike.bbcook.cn/Article/details/gpfpkxgam.sHtML

Ruby: return a, b
来源：http://www.share.yfazqb.com/Article/details/gcgxarxbl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.bbcook.cn/Article/details/gluayeuyx.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.sjlbkw.cn/Article/details/gvkvqryvm.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.tarul.cn/Article/details/gvxpjyyoq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.bbcook.cn/Article/details/glkutsrht.sHtML

JS:   const square = x => x * x;
来源：http://read.share.epnwcf.com/Article/details/gmdfxzham.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.epnwcf.com/Article/details/gruupujuz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.yfazqb.com/Article/details/gkllfqwzu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.yfazqb.com/Article/details/gyeurbvzg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.tarul.cn/Article/details/gboidoehc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.tarul.cn/Article/details/gavfmvjyb.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.sjlbkw.cn/Article/details/gdjrwksju.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.tarul.cn/Article/details/gnengsbux.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fktsv.cn/Article/details/ghcxjnkfj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.vehdjk.com/Article/details/gorefopji.sHtML

TS:   arr.map(String)
来源：http://www.m.share.vehdjk.com/Article/details/geygarqdj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.epnwcf.com/Article/details/giabfgyrx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.epnwcf.com/Article/details/gjifqhmaw.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.bbcook.cn/Article/details/ghpsdivse.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.tarul.cn/Article/details/gblaixbyx.sHtML

[C08] 闭包
来源：http://m.share.sjlbkw.cn/Article/details/guxwwwvgn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fktsv.cn/Article/details/gzqtyxgjj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.epnwcf.com/Article/details/gfpksgvhu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.vehdjk.com/Article/details/gkxrabzij.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fktsv.cn/Article/details/gtkbacdem.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fktsv.cn/Article/details/ggsqtlpxj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.bbcook.cn/Article/details/grgmgybjl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.sjlbkw.cn/Article/details/ghapocbvp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.sjlbkw.cn/Article/details/gfsdsboqr.sHtML

[C09] 递归
来源：http://m.share.fktsv.cn/Article/details/gdhmsklsr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.bbcook.cn/Article/details/gzckdawmj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.sjlbkw.cn/Article/details/gojbnjdtp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.vehdjk.com/Article/details/genuvjzsk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.yfazqb.com/Article/details/gvopzfyhg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.tarul.cn/Article/details/gmwsgndfa.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.vehdjk.com/Article/details/gfmbslabz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.yfazqb.com/Article/details/ghockoqyf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.bbcook.cn/Article/details/gnijcxbjh.sHtML

[C10] 变量作用域
来源：http://www.m.share.yfazqb.com/Article/details/gqimjyyyw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.bbcook.cn/Article/details/grioxmjcx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.yfazqb.com/Article/details/gbrttonvm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.sjlbkw.cn/Article/details/gjfsvbkoi.sHtML

TS:   同 JS
来源：http://mobile.fktsv.cn/Article/details/gptaoxdnc.sHtML

Java: 方法内为块级作用域
来源：http://www.share.yfazqb.com/Article/details/gmvhamuqq.sHtML

Go:   花括号块级作用域
来源：http://www.blog.yfazqb.com/Article/details/gmcmzrrdy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.vehdjk.com/Article/details/gpcydwrxf.sHtML

C#:   块级作用域
来源：http://wap.yfazqb.com/Article/details/gbyhrzwuh.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.epnwcf.com/Article/details/gpwwcbfbq.sHtML

Py:   from module import func
来源：http://m.share.yfazqb.com/Article/details/gdobyglxh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.epnwcf.com/Article/details/gybwxcrhr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.bbcook.cn/Article/details/gpxtgfpyp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.vehdjk.com/Article/details/gpwmgvnys.sHtML

Java: import java.util.List;
来源：http://wap.vehdjk.com/Article/details/gwiqzoius.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.tarul.cn/Article/details/gdsfnbgqp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.tarul.cn/Article/details/gjrjjofud.sHtML

C#:   using System.Text;
来源：http://wap.bbcook.cn/Article/details/gaohtrcxd.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.bbcook.cn/Article/details/gtfantobu.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.epnwcf.com/Article/details/gijequtmb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.vehdjk.com/Article/details/gkjrxhjvt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.vehdjk.com/Article/details/gblsyhjdr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fktsv.cn/Article/details/gsanpjayf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fktsv.cn/Article/details/gbcmsfoxs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.sjlbkw.cn/Article/details/guxkjmvcl.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.epnwcf.com/Article/details/gbdkzyjfd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.sjlbkw.cn/Article/details/gcmmsjbdd.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.tarul.cn/Article/details/gsiihnmip.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.tarul.cn/Article/details/ggzaefisj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.vehdjk.com/Article/details/gdroiuzzn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fktsv.cn/Article/details/gpreqarty.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gdejyyieo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gkgvvnfhd.sHtML

Go:   func add(a, b int) int
来源：http://read.share.vehdjk.com/Article/details/ggluindyh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.epnwcf.com/Article/details/gcjuhdzpv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.epnwcf.com/Article/details/gciuibsjm.sHtML

[C14] 泛型函数
来源：http://wap.epnwcf.com/Article/details/gnugfwtfl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.epnwcf.com/Article/details/ggylioehm.sHtML

PHP:  // 无泛型
来源：http://wap.vehdjk.com/Article/details/gvyozgzhx.sHtML

JS:   // 无泛型
来源：http://read.share.epnwcf.com/Article/details/ggxqtafct.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.vehdjk.com/Article/details/gbfuudgqq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.vehdjk.com/Article/details/grcfxsqrw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.sjlbkw.cn/Article/details/gxotyzelf.sHtML

Ruby: # 无泛型
来源：http://read.share.yfazqb.com/Article/details/gacukxuxo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.epnwcf.com/Article/details/gceororla.sHtML

[C15] 解构 / 展开参数
来源：http://blog.epnwcf.com/Article/details/gctljryad.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.bbcook.cn/Article/details/gyeuvbumx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.epnwcf.com/Article/details/gzehmkfca.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fktsv.cn/Article/details/gcddoiaro.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.tarul.cn/Article/details/gaetojoyg.sHtML

Java: // 无解构
来源：http://baike.vehdjk.com/Article/details/gwolkehug.sHtML

Go:   // 无解构
来源：http://read.share.fktsv.cn/Article/details/gfrberwmu.sHtML

Ruby: a, b = pair
来源：http://baike.tarul.cn/Article/details/gpkvtonqh.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.bbcook.cn/Article/details/gyljakmmi.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.sjlbkw.cn/Article/details/gbjpkhjbe.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.bbcook.cn/Article/details/gkbwhapsy.sHtML

PHP:  // 无重载
来源：http://www.m.share.yfazqb.com/Article/details/ghtvhzbuq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.vehdjk.com/Article/details/gvikukxhc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.epnwcf.com/Article/details/gpxapltnk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.epnwcf.com/Article/details/gmjsvutmm.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.tarul.cn/Article/details/giqzksvap.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fktsv.cn/Article/details/gqnoarini.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.vehdjk.com/Article/details/gqznqcfww.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gbybepyxv.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.epnwcf.com/Article/details/gtnbnevee.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gbtwzzclb.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fktsv.cn/Article/details/gamrufsac.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.vehdjk.com/Article/details/gcfsdpmiu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.epnwcf.com/Article/details/gfzyfddew.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.vehdjk.com/Article/details/gyvuuimqn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.tarul.cn/Article/details/gjtdeqxne.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.epnwcf.com/Article/details/gpdyspnne.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.bbcook.cn/Article/details/gyqztfkvv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fktsv.cn/Article/details/gllrkrusc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.vehdjk.com/Article/details/gmwgkuwuy.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.sjlbkw.cn/Article/details/gteofknwv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.sjlbkw.cn/Article/details/gqtlvzqbe.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.tarul.cn/Article/details/gpjfjtwsc.sHtML

JS:   arr.push(4);
来源：http://m.share.bbcook.cn/Article/details/gebhxlqyh.sHtML

TS:   arr.push(4);
来源：http://m.share.yfazqb.com/Article/details/grikztxsf.sHtML

Java: list.add(4);
来源：http://www.share.vehdjk.com/Article/details/gwksxgfrq.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.vehdjk.com/Article/details/gmhwjenor.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.epnwcf.com/Article/details/ghjmkaevw.sHtML

C#:   list.Add(4);
来源：http://m.share.tarul.cn/Article/details/gwgufqoao.sHtML

[D03] 在指定位置插入元素
来源：http://3g.tarul.cn/Article/details/gwnxkodbz.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.vehdjk.com/Article/details/gwqxqrdhv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.tarul.cn/Article/details/gjtpwkvgs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.sjlbkw.cn/Article/details/goeozqmjk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.bbcook.cn/Article/details/gsjytxosn.sHtML

Java: list.add(0, 0);
来源：http://read.share.bbcook.cn/Article/details/gwjmablsp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.tarul.cn/Article/details/gcxbyrawo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.yfazqb.com/Article/details/gsgwpfktq.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.yfazqb.com/Article/details/gjdmzcsqp.sHtML

[D04] 删除元素
来源：http://read.share.tarul.cn/Article/details/gxkzpgxli.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.yfazqb.com/Article/details/ggqggxste.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.yfazqb.com/Article/details/ggytslfbx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fktsv.cn/Article/details/gnoxmdstq.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.sjlbkw.cn/Article/details/gsfdnvgxi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.tarul.cn/Article/details/gqhalryqd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.bbcook.cn/Article/details/goxxliycm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.bbcook.cn/Article/details/gwbrflmkg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.sjlbkw.cn/Article/details/gwcdpnsdx.sHtML

[D05] 访问与修改元素
来源：http://blog.tarul.cn/Article/details/gojbxkdlm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.tarul.cn/Article/details/gwurxqinm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.tarul.cn/Article/details/gppjuoadq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.bbcook.cn/Article/details/gwufdfcqr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fktsv.cn/Article/details/gjdiozrfs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.vehdjk.com/Article/details/gginqhgrf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.bbcook.cn/Article/details/gdfsliccf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fktsv.cn/Article/details/gktsojsfo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fktsv.cn/Article/details/gckituyym.sHtML

[D06] 数组长度
来源：http://www.share.bbcook.cn/Article/details/giwmhocfv.sHtML

Py:   len(arr)
来源：http://mobile.vehdjk.com/Article/details/gnnuobdsg.sHtML

PHP:  count($arr);
来源：http://blog.yfazqb.com/Article/details/gbfvvesby.sHtML

JS:   arr.length
来源：http://mobile.epnwcf.com/Article/details/grrcjyxnf.sHtML

TS:   arr.length
来源：http://m.share.tarul.cn/Article/details/gdbaagrht.sHtML

Java: list.size();
来源：http://www.share.yfazqb.com/Article/details/gjfwoytxo.sHtML

Go:   len(arr)
来源：http://m.share.tarul.cn/Article/details/ghazkzncm.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.tarul.cn/Article/details/giwbilgwk.sHtML

C#:   list.Count;
来源：http://www.blog.bbcook.cn/Article/details/gvjpwizcg.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.epnwcf.com/Article/details/gkaszkhwx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.epnwcf.com/Article/details/gmrnpbkew.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.epnwcf.com/Article/details/glxtmfukc.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.vehdjk.com/Article/details/gqrbrcdld.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.bbcook.cn/Article/details/geqhltgqv.sHtML

Java: list.subList(1, 4);
来源：http://baike.vehdjk.com/Article/details/gpxixatyo.sHtML

Go:   arr[1:4]
来源：http://3g.yfazqb.com/Article/details/gkdfjicix.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbqyzsml.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.yfazqb.com/Article/details/gvasaqfua.sHtML

[D08] 合并两个数组
来源：http://mobile.bbcook.cn/Article/details/gawjgawyj.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.sjlbkw.cn/Article/details/gwdixywhk.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.vehdjk.com/Article/details/gjxkctkyu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.vehdjk.com/Article/details/gdyiklioi.sHtML

TS:   [...a, ...b];
来源：http://3g.sjlbkw.cn/Article/details/gtcevgcys.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.bbcook.cn/Article/details/gggmdyaav.sHtML

Go:   append(a, b...)
来源：http://www.blog.vehdjk.com/Article/details/gpadmsdgt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.vehdjk.com/Article/details/gjndehoyq.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.epnwcf.com/Article/details/gupcsrupz.sHtML

[D09] 排序（升序）
来源：http://read.share.epnwcf.com/Article/details/gcffttbdv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.epnwcf.com/Article/details/gsdhnzetz.sHtML


<!-- 参考信息 -->