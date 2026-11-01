代发 wailian999

[B09] break 与 continue
来源：http://read.share.bbcook.cn/Article/details/gldgowtup.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fktsv.cn/Article/details/galriqfvw.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/gszkxsqnw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/gscacsbvl.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gnjeathpu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gwgqfljgl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.sjlbkw.cn/Article/details/gkahbmlzz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.tarul.cn/Article/details/gamjopfix.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/gyulpuelp.sHtML

[B10] 遍历同时拿索引
来源：http://3g.bbcook.cn/Article/details/gghsaoung.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fktsv.cn/Article/details/gyuiwnvci.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.tarul.cn/Article/details/gfjazkioi.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.bbcook.cn/Article/details/gyebkyhgn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fktsv.cn/Article/details/gkfgwtcbf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.tarul.cn/Article/details/grnflztuy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.sjlbkw.cn/Article/details/gywbzkthq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.epnwcf.com/Article/details/gkprpflrs.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.epnwcf.com/Article/details/gwbmwamcl.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.vehdjk.com/Article/details/gnzsdqvaa.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.epnwcf.com/Article/details/gdhskhvjd.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.yfazqb.com/Article/details/gvnuraxct.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.sjlbkw.cn/Article/details/gmppymqbx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.bbcook.cn/Article/details/gnuqqidhc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.yfazqb.com/Article/details/gcsycxbwn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.tarul.cn/Article/details/gmttghqso.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.tarul.cn/Article/details/gnxqjkkil.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fktsv.cn/Article/details/grcnrezth.sHtML

[B12] 跳出多层循环
来源：http://wap.fktsv.cn/Article/details/gpecucwjl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.vehdjk.com/Article/details/gdzfdwofj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.sjlbkw.cn/Article/details/gihyxiyuq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.sjlbkw.cn/Article/details/gsnwknxgo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.bbcook.cn/Article/details/gicdxnwnw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.epnwcf.com/Article/details/gnzvmmbms.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.vehdjk.com/Article/details/gkicptaxj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.sjlbkw.cn/Article/details/gureacfgp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fktsv.cn/Article/details/gzzyvekbw.sHtML

[B13] 判断是否为数字
来源：http://www.blog.vehdjk.com/Article/details/gcevqmylo.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.tarul.cn/Article/details/gccldmjej.sHtML

PHP:  is_numeric($x)
来源：http://m.share.vehdjk.com/Article/details/gncvgmevk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.epnwcf.com/Article/details/grgleuypj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fktsv.cn/Article/details/gvplrlvws.sHtML

Java: x instanceof Number
来源：http://www.blog.vehdjk.com/Article/details/guzmyqhcb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.vehdjk.com/Article/details/glstwymxb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.tarul.cn/Article/details/gvcamddva.sHtML

C#:   x is int or double or decimal
来源：http://wap.sjlbkw.cn/Article/details/ggynihqal.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.epnwcf.com/Article/details/gbyogfjqz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.yfazqb.com/Article/details/gtbepgdpp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.sjlbkw.cn/Article/details/girymrdrj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.yfazqb.com/Article/details/gpcywwclp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.tarul.cn/Article/details/gujotskhi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fktsv.cn/Article/details/grexaiwdk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.epnwcf.com/Article/details/gzqsnewfz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.vehdjk.com/Article/details/ghvxkztuw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.bbcook.cn/Article/details/gsfbdluqr.sHtML

[B15] 布尔运算与取反
来源：http://read.share.vehdjk.com/Article/details/gvebozrxp.sHtML

Py:   a and b or not c
来源：http://m.share.yfazqb.com/Article/details/gtsalkjkc.sHtML

PHP:  $a && $b || !$c
来源：http://wap.bbcook.cn/Article/details/gpawgpaqi.sHtML

JS:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gcahjcodi.sHtML

TS:   a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gakyvdqzz.sHtML

Java: a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gzpvnbuhy.sHtML

Go:   a && b || !c
来源：http://baike.epnwcf.com/Article/details/gtzdivsno.sHtML

Ruby: a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/glrnzvgkn.sHtML

C#:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/ghmokarjx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.vehdjk.com/Article/details/glrmuvwqq.sHtML

Py:   if not data: return
来源：http://blog.tarul.cn/Article/details/gbpsrsmqo.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.bbcook.cn/Article/details/gjphotebq.sHtML

JS:   if (!data) return;
来源：http://www.blog.epnwcf.com/Article/details/ghfvtgvhj.sHtML

TS:   if (!data) return;
来源：http://read.share.vehdjk.com/Article/details/glrvorwaf.sHtML

Java: if (data == null) return;
来源：http://www.blog.vehdjk.com/Article/details/gbcllscmu.sHtML

Go:   if data == nil { return }
来源：http://m.share.vehdjk.com/Article/details/ghxpsbvqc.sHtML

Ruby: return if data.nil?
来源：http://www.blog.vehdjk.com/Article/details/gphipsgkf.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.epnwcf.com/Article/details/guidoashr.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gdsurepyq.sHtML

C. 函数与作用域
来源：http://blog.epnwcf.com/Article/details/gofzqkssk.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gumrqjeyn.sHtML

[C01] 定义函数
来源：http://mobile.vehdjk.com/Article/details/gxwfiecpo.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.epnwcf.com/Article/details/gcljkylqd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/gkamyazqw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gmgohglyq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gsspkjmky.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gclxybfto.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.vehdjk.com/Article/details/gunfugzci.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.bbcook.cn/Article/details/gfsawscrp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gomdcnzci.sHtML

[C02] 默认参数
来源：http://www.m.share.vehdjk.com/Article/details/gwoeauoet.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.fktsv.cn/Article/details/giyuvnnzw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/guxompman.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.yfazqb.com/Article/details/gniuxfdsr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.tarul.cn/Article/details/gotwwuwhv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.epnwcf.com/Article/details/gmwmxloui.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.yfazqb.com/Article/details/gjlziycbo.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.sjlbkw.cn/Article/details/ghqifyujt.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.sjlbkw.cn/Article/details/gluengofd.sHtML

[C03] 可变参数
来源：http://baike.epnwcf.com/Article/details/gchtdtlai.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.epnwcf.com/Article/details/gnbejejiq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.epnwcf.com/Article/details/gakukfrwp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.vehdjk.com/Article/details/gpaaolkns.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.sjlbkw.cn/Article/details/gonbwjykv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.bbcook.cn/Article/details/gjymrxjai.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fktsv.cn/Article/details/gmnpmjckf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fktsv.cn/Article/details/gxjmdivwn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.yfazqb.com/Article/details/gsnosirqm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.vehdjk.com/Article/details/gfvlibyql.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.yfazqb.com/Article/details/glchlaajt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.yfazqb.com/Article/details/gffrmqerg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.yfazqb.com/Article/details/gnfpklopa.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.vehdjk.com/Article/details/grjeunasg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.yfazqb.com/Article/details/gwzddxcwu.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.epnwcf.com/Article/details/gzibtsbfn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.sjlbkw.cn/Article/details/gqldltdar.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.tarul.cn/Article/details/ghtkksulg.sHtML

[C05] 返回多个值
来源：http://blog.yfazqb.com/Article/details/givpckouw.sHtML

Py:   return a, b
来源：http://wap.sjlbkw.cn/Article/details/giwbippys.sHtML

PHP:  return [$a, $b];
来源：http://3g.yfazqb.com/Article/details/gqqibtoug.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fktsv.cn/Article/details/gntqwfjly.sHtML

TS:   return { a, b };
来源：http://wap.tarul.cn/Article/details/gvqhzcscm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.yfazqb.com/Article/details/giuduxdip.sHtML

Go:   return a, b
来源：http://blog.fktsv.cn/Article/details/gxrvioboe.sHtML

Ruby: return a, b
来源：http://read.share.vehdjk.com/Article/details/ghyaznlhp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.sjlbkw.cn/Article/details/gnxnnxqng.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.sjlbkw.cn/Article/details/gybzbqnei.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.sjlbkw.cn/Article/details/ganerlthe.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.sjlbkw.cn/Article/details/gxkannqrs.sHtML

JS:   const square = x => x * x;
来源：http://m.share.sjlbkw.cn/Article/details/gotinndcs.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fktsv.cn/Article/details/gyvsywlny.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fktsv.cn/Article/details/gnswbiheb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.bbcook.cn/Article/details/glulobbxf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fktsv.cn/Article/details/gdkavugpc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gbrwgzwjl.sHtML

[C07] 把函数作为参数传入
来源：http://baike.tarul.cn/Article/details/gzhiitqzd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.sjlbkw.cn/Article/details/gaztuccnv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.epnwcf.com/Article/details/gzhkwgnul.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.sjlbkw.cn/Article/details/gheodipdl.sHtML

TS:   arr.map(String)
来源：http://www.share.vehdjk.com/Article/details/gtgctkulw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.vehdjk.com/Article/details/gcasstjxa.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.yfazqb.com/Article/details/ghrusoczz.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.epnwcf.com/Article/details/gscgluimc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fktsv.cn/Article/details/gfyybkwgn.sHtML

[C08] 闭包
来源：http://www.m.share.epnwcf.com/Article/details/gybetyxqg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.tarul.cn/Article/details/gogmycgca.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.vehdjk.com/Article/details/gwilpwijt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.vehdjk.com/Article/details/gttadfhhc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.yfazqb.com/Article/details/giotczbts.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fktsv.cn/Article/details/ghdzilvzo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.vehdjk.com/Article/details/gdvvfveyk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.bbcook.cn/Article/details/gfpnhhvwl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.sjlbkw.cn/Article/details/gkruvaxns.sHtML

[C09] 递归
来源：http://wap.bbcook.cn/Article/details/ghqvawvwg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.tarul.cn/Article/details/gynldcptc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.sjlbkw.cn/Article/details/grzgxqqpn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.tarul.cn/Article/details/gidjcohqm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.sjlbkw.cn/Article/details/gfquhamdv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.yfazqb.com/Article/details/gaqiulkwb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.tarul.cn/Article/details/gmzwdqxdh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.vehdjk.com/Article/details/gnfzecwtx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.sjlbkw.cn/Article/details/glxqxuhcv.sHtML

[C10] 变量作用域
来源：http://3g.bbcook.cn/Article/details/gyquohmdn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.tarul.cn/Article/details/gkosqmcrz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.sjlbkw.cn/Article/details/gbscoobpd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.vehdjk.com/Article/details/guvxyhajz.sHtML

TS:   同 JS
来源：http://blog.epnwcf.com/Article/details/grqegavpj.sHtML

Java: 方法内为块级作用域
来源：http://m.share.epnwcf.com/Article/details/gtigmhocg.sHtML

Go:   花括号块级作用域
来源：http://m.share.fktsv.cn/Article/details/gerrpxknh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.bbcook.cn/Article/details/gyyxizuoo.sHtML

C#:   块级作用域
来源：http://www.share.bbcook.cn/Article/details/gdmsgtbqq.sHtML

[C11] 模块导入与导出
来源：http://wap.bbcook.cn/Article/details/gwvxxyhxr.sHtML

Py:   from module import func
来源：http://www.blog.sjlbkw.cn/Article/details/gitlagfag.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.yfazqb.com/Article/details/gsnvbenzz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.tarul.cn/Article/details/gbcmrpqic.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.bbcook.cn/Article/details/gupirmrld.sHtML

Java: import java.util.List;
来源：http://mobile.tarul.cn/Article/details/gizepfnjr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.yfazqb.com/Article/details/gimshmada.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.bbcook.cn/Article/details/gxiimkdec.sHtML

C#:   using System.Text;
来源：http://www.share.bbcook.cn/Article/details/goywqgepp.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.sjlbkw.cn/Article/details/gdtgiwvrw.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.vehdjk.com/Article/details/gdvlgvrhx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.vehdjk.com/Article/details/gswpdypcr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fktsv.cn/Article/details/gtkgvmpqz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.yfazqb.com/Article/details/gigqibzfz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.bbcook.cn/Article/details/gdvuicsam.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.yfazqb.com/Article/details/gsjvftyic.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.epnwcf.com/Article/details/gsggectow.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.bbcook.cn/Article/details/grrrumbuu.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.sjlbkw.cn/Article/details/gzoqitwqw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.yfazqb.com/Article/details/ghpzqtemw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/gobhisphc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.bbcook.cn/Article/details/gwtnfmrcw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gakhgtmsr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gaawcukaw.sHtML

Go:   func add(a, b int) int
来源：http://wap.sjlbkw.cn/Article/details/gfujnaxnd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.vehdjk.com/Article/details/guxsxstaq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.vehdjk.com/Article/details/giwqcejqg.sHtML

[C14] 泛型函数
来源：http://www.share.sjlbkw.cn/Article/details/gwrmlwgkm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.vehdjk.com/Article/details/gtilvqhzb.sHtML

PHP:  // 无泛型
来源：http://www.m.share.bbcook.cn/Article/details/gfxboztjp.sHtML

JS:   // 无泛型
来源：http://wap.sjlbkw.cn/Article/details/gxxhrfmha.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.sjlbkw.cn/Article/details/gbdpblzmw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.epnwcf.com/Article/details/gzckwxqan.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.tarul.cn/Article/details/gfkbtonfj.sHtML

Ruby: # 无泛型
来源：http://www.blog.bbcook.cn/Article/details/gsxnfphip.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.sjlbkw.cn/Article/details/gshymbgho.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.yfazqb.com/Article/details/gdzuapqku.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.bbcook.cn/Article/details/gqwkpytih.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.bbcook.cn/Article/details/gfsrfonkf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.sjlbkw.cn/Article/details/gunbapmko.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.tarul.cn/Article/details/gqhlyqvnq.sHtML

Java: // 无解构
来源：http://www.share.vehdjk.com/Article/details/gnuvtjspj.sHtML

Go:   // 无解构
来源：http://blog.tarul.cn/Article/details/gspmnmbyy.sHtML

Ruby: a, b = pair
来源：http://3g.tarul.cn/Article/details/gwugsoznp.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.sjlbkw.cn/Article/details/gdwltwxyl.sHtML

[C16] 函数 / 方法重载
来源：http://blog.yfazqb.com/Article/details/gdxlasuek.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.epnwcf.com/Article/details/gzypcnefh.sHtML

PHP:  // 无重载
来源：http://read.share.epnwcf.com/Article/details/gztclighw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.yfazqb.com/Article/details/gonqyllwu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.vehdjk.com/Article/details/gtdumdhsl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.bbcook.cn/Article/details/gvdmwhcyp.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.yfazqb.com/Article/details/gxmxprkxl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.sjlbkw.cn/Article/details/gmaoyskzy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.epnwcf.com/Article/details/ggpxepphe.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/glgglixnz.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.epnwcf.com/Article/details/gztuwksrf.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gfibmzivw.sHtML

[D01] 创建数组 / 列表
来源：http://baike.tarul.cn/Article/details/gbdeizlbu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.tarul.cn/Article/details/gsteczctv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fktsv.cn/Article/details/gffskkpju.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.yfazqb.com/Article/details/geqsvaugj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.vehdjk.com/Article/details/guykhyqzi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fktsv.cn/Article/details/gfvwuxtkb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.epnwcf.com/Article/details/gwvljzfoh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.bbcook.cn/Article/details/geuorfubw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.sjlbkw.cn/Article/details/gvyktcgau.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.epnwcf.com/Article/details/gggpyjtkt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.yfazqb.com/Article/details/gvkliascx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.epnwcf.com/Article/details/gukyhjgtp.sHtML

JS:   arr.push(4);
来源：http://baike.epnwcf.com/Article/details/gvjsdwsci.sHtML

TS:   arr.push(4);
来源：http://m.share.sjlbkw.cn/Article/details/guhwoohio.sHtML

Java: list.add(4);
来源：http://www.m.share.yfazqb.com/Article/details/gvhozoaqe.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.tarul.cn/Article/details/gedkzinbq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrrowjca.sHtML

C#:   list.Add(4);
来源：http://www.share.bbcook.cn/Article/details/ggaajuscq.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.bbcook.cn/Article/details/grrxxpgtl.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gcvawmfqv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.yfazqb.com/Article/details/gbbnpdasc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.epnwcf.com/Article/details/gkhuidpyn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.vehdjk.com/Article/details/gqnkqfztd.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.epnwcf.com/Article/details/guwoozvuc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.yfazqb.com/Article/details/gyxzikaam.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.sjlbkw.cn/Article/details/gksftmmik.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fktsv.cn/Article/details/gwlxcecwp.sHtML

[D04] 删除元素
来源：http://3g.fktsv.cn/Article/details/gtbrcgmti.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.sjlbkw.cn/Article/details/grlvttovg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.yfazqb.com/Article/details/gdpmeqouy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.epnwcf.com/Article/details/gswiupxoe.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.sjlbkw.cn/Article/details/gfiibroxm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.bbcook.cn/Article/details/gmqmpjvpg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.vehdjk.com/Article/details/gvjluaizi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.yfazqb.com/Article/details/gqamvxtzx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fktsv.cn/Article/details/gejpcvvkh.sHtML

[D05] 访问与修改元素
来源：http://mobile.sjlbkw.cn/Article/details/guesvksbk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.vehdjk.com/Article/details/gwkhrosop.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.tarul.cn/Article/details/gvxpgrgyw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.bbcook.cn/Article/details/gkbwzdyqh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.sjlbkw.cn/Article/details/gjfdrijbb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.bbcook.cn/Article/details/gekyatiqg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.yfazqb.com/Article/details/gucqbwzah.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.vehdjk.com/Article/details/gddvcqpir.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.yfazqb.com/Article/details/ggmzdhsxr.sHtML

[D06] 数组长度
来源：http://www.blog.vehdjk.com/Article/details/gzytedtpu.sHtML

Py:   len(arr)
来源：http://wap.sjlbkw.cn/Article/details/geroolqtd.sHtML

PHP:  count($arr);
来源：http://wap.bbcook.cn/Article/details/gznbfpvgz.sHtML

JS:   arr.length
来源：http://www.blog.tarul.cn/Article/details/gnxikprec.sHtML

TS:   arr.length
来源：http://3g.bbcook.cn/Article/details/gwxkencdz.sHtML

Java: list.size();
来源：http://wap.bbcook.cn/Article/details/gulisaefl.sHtML

Go:   len(arr)
来源：http://wap.tarul.cn/Article/details/gdmyrmkht.sHtML

Ruby: arr.length; arr.size
来源：http://3g.vehdjk.com/Article/details/gylemkyag.sHtML

C#:   list.Count;
来源：http://www.blog.sjlbkw.cn/Article/details/guctqyhbs.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fktsv.cn/Article/details/gmfbrxvad.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.sjlbkw.cn/Article/details/gchkyvvdv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.epnwcf.com/Article/details/gqukswwhk.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.vehdjk.com/Article/details/giceeurac.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.sjlbkw.cn/Article/details/gtqnhfmwb.sHtML

Java: list.subList(1, 4);
来源：http://mobile.yfazqb.com/Article/details/gwlookant.sHtML

Go:   arr[1:4]
来源：http://3g.epnwcf.com/Article/details/gnwuqsste.sHtML

Ruby: arr[1, 3]
来源：http://3g.epnwcf.com/Article/details/gdcjehhpe.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.epnwcf.com/Article/details/gwsijjqvg.sHtML

[D08] 合并两个数组
来源：http://www.blog.bbcook.cn/Article/details/ggkjpcljz.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.tarul.cn/Article/details/gibphizyb.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.bbcook.cn/Article/details/gsvbkvikz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.epnwcf.com/Article/details/gbccnrpcy.sHtML

TS:   [...a, ...b];
来源：http://m.share.yfazqb.com/Article/details/gyfvygrmd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.yfazqb.com/Article/details/gmctsagve.sHtML

Go:   append(a, b...)
来源：http://wap.tarul.cn/Article/details/gnopcafdx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdnabyct.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.yfazqb.com/Article/details/gzhuwskun.sHtML

[D09] 排序（升序）
来源：http://3g.yfazqb.com/Article/details/gthmmmkwz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.yfazqb.com/Article/details/gvuondmqw.sHtML

PHP:  sort($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gmeldzayx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.sjlbkw.cn/Article/details/gbdhilxkb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.bbcook.cn/Article/details/govdjzbkq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.vehdjk.com/Article/details/guddzaqed.sHtML


<!-- 参考信息 -->