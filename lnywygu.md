代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://m.share.sjlbkw.cn/Article/details/gotvhxuiy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.vehdjk.com/Article/details/gkromoldu.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.bbcook.cn/Article/details/gntwoapva.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gdkowoiow.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gyslkwatl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.yfazqb.com/Article/details/gsrbkvkkc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fktsv.cn/Article/details/gdrefpktw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gnfosfwxz.sHtML

[B09] break 与 continue
来源：http://www.blog.bbcook.cn/Article/details/gljzwbvvy.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.vehdjk.com/Article/details/gdebpvkqu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gbfymvawe.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gsizlbrod.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/gypbglkzo.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwwoosoe.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.vehdjk.com/Article/details/gkgytujdt.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.yfazqb.com/Article/details/gdedrmzms.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/grxmihocb.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.bbcook.cn/Article/details/gknwobhxg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.yfazqb.com/Article/details/geedcfuhu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.bbcook.cn/Article/details/gxtcbwqic.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.sjlbkw.cn/Article/details/ggdptteca.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.vehdjk.com/Article/details/gsmnxdiqd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.epnwcf.com/Article/details/ggsneweti.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.yfazqb.com/Article/details/gvjnchnbo.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fktsv.cn/Article/details/ghhgrkrpf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.yfazqb.com/Article/details/gchpseoih.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.tarul.cn/Article/details/gmfpddlkg.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fktsv.cn/Article/details/grzqkjkfk.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.epnwcf.com/Article/details/gqroxqgdb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.epnwcf.com/Article/details/giyznyhxe.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fktsv.cn/Article/details/gxehektoa.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.vehdjk.com/Article/details/gufagpzyo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.sjlbkw.cn/Article/details/gtmnmxzfx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.vehdjk.com/Article/details/gvmuvbewy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.yfazqb.com/Article/details/gppcyumdr.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.yfazqb.com/Article/details/golezlpff.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.sjlbkw.cn/Article/details/gcejftqkb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.sjlbkw.cn/Article/details/gjcpfcrxd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/gfweazuvy.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fktsv.cn/Article/details/gxdszafiq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.tarul.cn/Article/details/ghfvwziev.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.epnwcf.com/Article/details/gtbadyhjo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.tarul.cn/Article/details/gqrjnxopm.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.epnwcf.com/Article/details/gweyrkxcm.sHtML

[B13] 判断是否为数字
来源：http://www.share.yfazqb.com/Article/details/gphamdeag.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.epnwcf.com/Article/details/gnicktwdf.sHtML

PHP:  is_numeric($x)
来源：http://wap.bbcook.cn/Article/details/ghnvgnkli.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.sjlbkw.cn/Article/details/gmictadph.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.yfazqb.com/Article/details/gfnmoyijw.sHtML

Java: x instanceof Number
来源：http://www.m.share.yfazqb.com/Article/details/gpjmsshxq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.bbcook.cn/Article/details/glopftppa.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.yfazqb.com/Article/details/gjtlhdchp.sHtML

C#:   x is int or double or decimal
来源：http://wap.fktsv.cn/Article/details/gvrdoddsx.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fktsv.cn/Article/details/gclvebedv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.vehdjk.com/Article/details/gsgyjbtjg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.epnwcf.com/Article/details/gmsxwdmbz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.epnwcf.com/Article/details/gqxyrdshk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.yfazqb.com/Article/details/gzhzrpbcf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.bbcook.cn/Article/details/guqkdckad.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.bbcook.cn/Article/details/giqxtdmrj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.vehdjk.com/Article/details/gdkwtjgwb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.tarul.cn/Article/details/gfhmphyzg.sHtML

[B15] 布尔运算与取反
来源：http://mobile.tarul.cn/Article/details/gnuvuvxhd.sHtML

Py:   a and b or not c
来源：http://3g.vehdjk.com/Article/details/gvcpiefcs.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.sjlbkw.cn/Article/details/gsttcmgmd.sHtML

JS:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gmhthokro.sHtML

TS:   a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gifngtpue.sHtML

Java: a && b || !c
来源：http://wap.vehdjk.com/Article/details/ggwglcsrk.sHtML

Go:   a && b || !c
来源：http://blog.vehdjk.com/Article/details/gbsoivppx.sHtML

Ruby: a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/goypmqszm.sHtML

C#:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/goancxwoq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.bbcook.cn/Article/details/gguniigtp.sHtML

Py:   if not data: return
来源：http://www.m.share.sjlbkw.cn/Article/details/gywbaqqrw.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fktsv.cn/Article/details/gudrvsojh.sHtML

JS:   if (!data) return;
来源：http://blog.bbcook.cn/Article/details/gpzvxdncw.sHtML

TS:   if (!data) return;
来源：http://m.share.tarul.cn/Article/details/gvpowiaus.sHtML

Java: if (data == null) return;
来源：http://www.blog.sjlbkw.cn/Article/details/giggtcgec.sHtML

Go:   if data == nil { return }
来源：http://baike.fktsv.cn/Article/details/gwumcfeqw.sHtML

Ruby: return if data.nil?
来源：http://www.share.sjlbkw.cn/Article/details/gsjcndpwr.sHtML

C#:   if (data == null) return;
来源：http://blog.sjlbkw.cn/Article/details/gjeqkmevt.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gkaguhzhz.sHtML

C. 函数与作用域
来源：http://m.share.sjlbkw.cn/Article/details/gcagbmswl.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gqhwaztku.sHtML

[C01] 定义函数
来源：http://wap.tarul.cn/Article/details/gejlhgvqb.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fktsv.cn/Article/details/gesbtaing.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.epnwcf.com/Article/details/gezmfcget.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gabgalcpc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gzahpuotf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gwlmfjhpc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.bbcook.cn/Article/details/gkwmpjyws.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.tarul.cn/Article/details/grqiqajbo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gzgzlzcas.sHtML

[C02] 默认参数
来源：http://www.m.share.bbcook.cn/Article/details/gxadmzbom.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.bbcook.cn/Article/details/gaaqhdiae.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.tarul.cn/Article/details/gmdrpfkru.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.vehdjk.com/Article/details/gtyfavyaa.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.bbcook.cn/Article/details/gaoqwvudx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.tarul.cn/Article/details/gppromegs.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.sjlbkw.cn/Article/details/gxeiqdlmf.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.yfazqb.com/Article/details/gbyctkuqc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.vehdjk.com/Article/details/gplcyavcj.sHtML

[C03] 可变参数
来源：http://3g.sjlbkw.cn/Article/details/gnmixgova.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fktsv.cn/Article/details/giomuebym.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.tarul.cn/Article/details/gupfnutaa.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fktsv.cn/Article/details/gadtsrojy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.epnwcf.com/Article/details/gvradmgfo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.bbcook.cn/Article/details/gpbpfmdxr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.yfazqb.com/Article/details/gteoozllq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.vehdjk.com/Article/details/gillykkii.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.vehdjk.com/Article/details/glxajazcc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fktsv.cn/Article/details/gihshyhrr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.sjlbkw.cn/Article/details/gnrpbrfmf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.bbcook.cn/Article/details/gsxpkgcub.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.epnwcf.com/Article/details/grljcyphs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.epnwcf.com/Article/details/gsevrxzej.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fktsv.cn/Article/details/gsbsaevos.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.tarul.cn/Article/details/gzdwcwrqa.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.tarul.cn/Article/details/gdpwyshdq.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.vehdjk.com/Article/details/gigawutwa.sHtML

[C05] 返回多个值
来源：http://read.share.fktsv.cn/Article/details/gzqoyebrf.sHtML

Py:   return a, b
来源：http://baike.vehdjk.com/Article/details/gzmlimlrt.sHtML

PHP:  return [$a, $b];
来源：http://3g.sjlbkw.cn/Article/details/gopxzwttf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.epnwcf.com/Article/details/grxtmptdq.sHtML

TS:   return { a, b };
来源：http://baike.vehdjk.com/Article/details/gyhxnxlcv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.yfazqb.com/Article/details/gmqijkpnc.sHtML

Go:   return a, b
来源：http://3g.tarul.cn/Article/details/geclegyeq.sHtML

Ruby: return a, b
来源：http://www.blog.epnwcf.com/Article/details/gewbngiir.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.tarul.cn/Article/details/gdvetsdhp.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.bbcook.cn/Article/details/gjciyhncv.sHtML

Py:   square = lambda x: x * x
来源：http://3g.tarul.cn/Article/details/glutzkruj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.tarul.cn/Article/details/gsmorfxjz.sHtML

JS:   const square = x => x * x;
来源：http://www.share.epnwcf.com/Article/details/gihanspck.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.sjlbkw.cn/Article/details/gcdmjiycn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.vehdjk.com/Article/details/gpqhffjga.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.vehdjk.com/Article/details/gmkqtfkxs.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.bbcook.cn/Article/details/gknvsweey.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.yfazqb.com/Article/details/gejadzgcv.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.bbcook.cn/Article/details/glylkbbif.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fktsv.cn/Article/details/gkqszagbs.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.vehdjk.com/Article/details/gpoggmphq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.bbcook.cn/Article/details/grksozcoh.sHtML

TS:   arr.map(String)
来源：http://www.share.vehdjk.com/Article/details/grohddzee.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.vehdjk.com/Article/details/gawrtmkcn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.yfazqb.com/Article/details/gqijibdzy.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.sjlbkw.cn/Article/details/gozcsgsit.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.tarul.cn/Article/details/gvoepaseh.sHtML

[C08] 闭包
来源：http://www.share.epnwcf.com/Article/details/gtyzmwwmm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fktsv.cn/Article/details/gbtzuumlx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.bbcook.cn/Article/details/gtxipxedw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.tarul.cn/Article/details/grfjpwxlg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.tarul.cn/Article/details/grfuiejyc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fktsv.cn/Article/details/gcvnellbk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.epnwcf.com/Article/details/gvmuirjek.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.epnwcf.com/Article/details/gtxscksme.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/ghyyryhtv.sHtML

[C09] 递归
来源：http://baike.tarul.cn/Article/details/gevsapdsq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.epnwcf.com/Article/details/gsumsxfpp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.sjlbkw.cn/Article/details/gbqiohyky.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.vehdjk.com/Article/details/gwhgnzpsd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.vehdjk.com/Article/details/gdzjytbnq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.epnwcf.com/Article/details/gdmfmitwy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.vehdjk.com/Article/details/gqhpzgdgr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.vehdjk.com/Article/details/gtxqsrdov.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.vehdjk.com/Article/details/gnnfzalzl.sHtML

[C10] 变量作用域
来源：http://baike.fktsv.cn/Article/details/ghpvnldnu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fktsv.cn/Article/details/gjiasfbsn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.sjlbkw.cn/Article/details/gyehynifl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.bbcook.cn/Article/details/ginamriye.sHtML

TS:   同 JS
来源：http://wap.sjlbkw.cn/Article/details/gxxjgztip.sHtML

Java: 方法内为块级作用域
来源：http://blog.tarul.cn/Article/details/ghbucnjff.sHtML

Go:   花括号块级作用域
来源：http://blog.vehdjk.com/Article/details/gynwjulbq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fktsv.cn/Article/details/gznbaoson.sHtML

C#:   块级作用域
来源：http://blog.bbcook.cn/Article/details/gehzmwmxw.sHtML

[C11] 模块导入与导出
来源：http://www.blog.bbcook.cn/Article/details/gpqosfhep.sHtML

Py:   from module import func
来源：http://read.share.fktsv.cn/Article/details/gtjwrslyj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.yfazqb.com/Article/details/glggguggv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.bbcook.cn/Article/details/gnpwuoozs.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.sjlbkw.cn/Article/details/gjfnbcdus.sHtML

Java: import java.util.List;
来源：http://www.share.bbcook.cn/Article/details/gujuvepgp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.epnwcf.com/Article/details/gukzmxmjh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.epnwcf.com/Article/details/gkjgeoxuw.sHtML

C#:   using System.Text;
来源：http://m.share.vehdjk.com/Article/details/gtjgddagl.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.bbcook.cn/Article/details/gjncddppe.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.tarul.cn/Article/details/gpvfjlbrc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.vehdjk.com/Article/details/gicvyjrhb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.epnwcf.com/Article/details/ggeynyirh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.bbcook.cn/Article/details/ggbkcrcsa.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.sjlbkw.cn/Article/details/gmwkiujkt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.epnwcf.com/Article/details/gxlmqzoow.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.vehdjk.com/Article/details/gemvuytdm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.epnwcf.com/Article/details/gzfqdgeph.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.bbcook.cn/Article/details/gtwpwvxwf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.sjlbkw.cn/Article/details/gewfqecrk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/gjhkisadu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.epnwcf.com/Article/details/gvludmhjf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gviehyewv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gbggjvddj.sHtML

Go:   func add(a, b int) int
来源：http://3g.tarul.cn/Article/details/gqsnzajqa.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.tarul.cn/Article/details/gepelyaet.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.vehdjk.com/Article/details/gilovvmci.sHtML

[C14] 泛型函数
来源：http://3g.sjlbkw.cn/Article/details/ggxwuonsi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.vehdjk.com/Article/details/ghfrxcdpu.sHtML

PHP:  // 无泛型
来源：http://wap.vehdjk.com/Article/details/gwcyxovxn.sHtML

JS:   // 无泛型
来源：http://3g.tarul.cn/Article/details/gtvhxrgmw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fktsv.cn/Article/details/gqyminfba.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.epnwcf.com/Article/details/gtevfxgqo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.vehdjk.com/Article/details/gynwewlju.sHtML

Ruby: # 无泛型
来源：http://baike.vehdjk.com/Article/details/gwgorgygk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.yfazqb.com/Article/details/goiuoyrbt.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.yfazqb.com/Article/details/gnogfhbqo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.tarul.cn/Article/details/gnlgvfnac.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.sjlbkw.cn/Article/details/gmbpjellu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gkksgddps.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.tarul.cn/Article/details/ggdskdvvf.sHtML

Java: // 无解构
来源：http://3g.sjlbkw.cn/Article/details/gekkfanwx.sHtML

Go:   // 无解构
来源：http://read.share.vehdjk.com/Article/details/gfrvotney.sHtML

Ruby: a, b = pair
来源：http://m.share.vehdjk.com/Article/details/gwxjatiqt.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.yfazqb.com/Article/details/gxtvxlojb.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.yfazqb.com/Article/details/grvzhjmna.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.tarul.cn/Article/details/gpgexhwov.sHtML

PHP:  // 无重载
来源：http://3g.epnwcf.com/Article/details/gowedmrst.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fktsv.cn/Article/details/gwksjnnxs.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.yfazqb.com/Article/details/gpnqzieuz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.tarul.cn/Article/details/gdsdwisbe.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.yfazqb.com/Article/details/gokujfwuf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.bbcook.cn/Article/details/gytumghed.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.vehdjk.com/Article/details/ggebhavhn.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gebzonfzl.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.epnwcf.com/Article/details/gfnojplpf.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gnzrhigre.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.sjlbkw.cn/Article/details/guqqpokgc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.sjlbkw.cn/Article/details/glbmknrfm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.tarul.cn/Article/details/gqflagucg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.tarul.cn/Article/details/gngtdazwy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fktsv.cn/Article/details/gdfaqqpvj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.vehdjk.com/Article/details/gtlofkptj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.vehdjk.com/Article/details/gozdqhxed.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.sjlbkw.cn/Article/details/gcoocfclm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.bbcook.cn/Article/details/gpwbyqvjp.sHtML

[D02] 追加元素到末尾
来源：http://baike.sjlbkw.cn/Article/details/gkgxpnwli.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.epnwcf.com/Article/details/gasszyetc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghkuqpeow.sHtML

JS:   arr.push(4);
来源：http://mobile.fktsv.cn/Article/details/gssyccpgl.sHtML

TS:   arr.push(4);
来源：http://3g.sjlbkw.cn/Article/details/gvstqpknl.sHtML

Java: list.add(4);
来源：http://www.blog.epnwcf.com/Article/details/grjhtfdzp.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.tarul.cn/Article/details/gmqfqdhpf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fktsv.cn/Article/details/gaatqpyws.sHtML

C#:   list.Add(4);
来源：http://www.m.share.tarul.cn/Article/details/givkaippr.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.tarul.cn/Article/details/gjudhjlpe.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.tarul.cn/Article/details/gfbrlwymx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.bbcook.cn/Article/details/gmjezlnla.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.epnwcf.com/Article/details/gkhrznopp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.yfazqb.com/Article/details/gdmbmxzdi.sHtML

Java: list.add(0, 0);
来源：http://mobile.epnwcf.com/Article/details/gkysowowz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.bbcook.cn/Article/details/gpyqnbgql.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.bbcook.cn/Article/details/gohrofltm.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.sjlbkw.cn/Article/details/ghqajkbxj.sHtML

[D04] 删除元素
来源：http://m.share.vehdjk.com/Article/details/gxbndlwgi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.bbcook.cn/Article/details/gmtktwply.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhyrqnov.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fktsv.cn/Article/details/garfyszuz.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.yfazqb.com/Article/details/gqbwbnpiz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.sjlbkw.cn/Article/details/gatqzpbpu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbqxvdwb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.vehdjk.com/Article/details/gnhxquail.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.vehdjk.com/Article/details/gyxmtxmoi.sHtML

[D05] 访问与修改元素
来源：http://blog.sjlbkw.cn/Article/details/gjaltegmv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.bbcook.cn/Article/details/goejeelfq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.sjlbkw.cn/Article/details/gykfvdoti.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.bbcook.cn/Article/details/gajrmvqjf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.bbcook.cn/Article/details/gawuwiawg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fktsv.cn/Article/details/gwudcoscz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/gfimjbxij.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.yfazqb.com/Article/details/geercmfli.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.vehdjk.com/Article/details/gdckuzchg.sHtML

[D06] 数组长度
来源：http://mobile.epnwcf.com/Article/details/ggmbhulhl.sHtML

Py:   len(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/giiiikdar.sHtML

PHP:  count($arr);
来源：http://www.share.epnwcf.com/Article/details/gexfrkbjp.sHtML

JS:   arr.length
来源：http://m.share.epnwcf.com/Article/details/gvrvmyihe.sHtML

TS:   arr.length
来源：http://blog.vehdjk.com/Article/details/gnxlhyjpu.sHtML

Java: list.size();
来源：http://mobile.epnwcf.com/Article/details/gqqqvqcfr.sHtML

Go:   len(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/ggznyooqs.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.tarul.cn/Article/details/gkmnkbsyb.sHtML

C#:   list.Count;
来源：http://mobile.bbcook.cn/Article/details/gbxmyedzl.sHtML

[D07] 切片 / 取子数组
来源：http://3g.tarul.cn/Article/details/ggvxvphko.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.sjlbkw.cn/Article/details/gjafnfqmw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fktsv.cn/Article/details/ggiznhasj.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fktsv.cn/Article/details/gjajkbfvj.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.sjlbkw.cn/Article/details/gknicrzdj.sHtML

Java: list.subList(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/gcjlefral.sHtML

Go:   arr[1:4]
来源：http://blog.tarul.cn/Article/details/gtfajzwik.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fktsv.cn/Article/details/gzmtltcnz.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.bbcook.cn/Article/details/gdvrseqow.sHtML

[D08] 合并两个数组
来源：http://wap.epnwcf.com/Article/details/gjbpvvyxj.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.vehdjk.com/Article/details/gfvnkagik.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.tarul.cn/Article/details/gpiigzefo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fktsv.cn/Article/details/gbryuktlj.sHtML

TS:   [...a, ...b];
来源：http://www.blog.epnwcf.com/Article/details/gzvjsjpxi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.vehdjk.com/Article/details/gwnasxuhx.sHtML

Go:   append(a, b...)
来源：http://blog.sjlbkw.cn/Article/details/ggwrvnwub.sHtML


<!-- 参考信息 -->