代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://wap.vehdjk.com/Article/details/glrtilvfb.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.yfazqb.com/Article/details/groilbaii.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fktsv.cn/Article/details/gsxrapylm.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/gcbqbkigc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.tarul.cn/Article/details/ghfjjukmj.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.epnwcf.com/Article/details/gmhcidnbc.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.tarul.cn/Article/details/glzostmpc.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.yfazqb.com/Article/details/gdtxsxdkl.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.fktsv.cn/Article/details/gocpwwgib.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.fktsv.cn/Article/details/gzpyfiktq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.fktsv.cn/Article/details/givmheweq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/givvinbac.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gosttpbdb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fktsv.cn/Article/details/gfucehhzn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.sjlbkw.cn/Article/details/goazykffp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.tarul.cn/Article/details/gitkvakwn.sHtML

[B09] break 与 continue
来源：http://read.share.bbcook.cn/Article/details/gogrdgcec.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.yfazqb.com/Article/details/gtzwsdndz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gsbvjizeq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.vehdjk.com/Article/details/glisitksr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/glfaneiiz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.yfazqb.com/Article/details/gyxirnbkz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.bbcook.cn/Article/details/gdldncmrt.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fktsv.cn/Article/details/gbsbqeuvk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/gkulqxnkh.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.sjlbkw.cn/Article/details/geehmhkmd.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.tarul.cn/Article/details/gmkltroqu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.bbcook.cn/Article/details/gkmjhpjfg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.sjlbkw.cn/Article/details/gyarctqds.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.sjlbkw.cn/Article/details/gjkjtwezp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.tarul.cn/Article/details/gubdrrinp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.vehdjk.com/Article/details/gjioblcpf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.bbcook.cn/Article/details/gkxzojxjl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbzxcauko.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fktsv.cn/Article/details/gvayrrhfb.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.tarul.cn/Article/details/gwxazktev.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fktsv.cn/Article/details/ghjhoujge.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.tarul.cn/Article/details/grgjgjith.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.bbcook.cn/Article/details/gmhurtvoa.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.yfazqb.com/Article/details/gxbfwqsse.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.yfazqb.com/Article/details/gjzrfepqc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.epnwcf.com/Article/details/goomgbjnv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.yfazqb.com/Article/details/gphsajobf.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fktsv.cn/Article/details/goyakahla.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.bbcook.cn/Article/details/gazruzeue.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.tarul.cn/Article/details/gxzlmrskt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/gjzexrdcz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.vehdjk.com/Article/details/gqsfajtiw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.bbcook.cn/Article/details/grlgftzjf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.yfazqb.com/Article/details/gaxefcmyf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.sjlbkw.cn/Article/details/geuowxprx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.bbcook.cn/Article/details/ghmlfhuxu.sHtML

[B13] 判断是否为数字
来源：http://mobile.sjlbkw.cn/Article/details/ghtiyhgws.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fktsv.cn/Article/details/groulmbyd.sHtML

PHP:  is_numeric($x)
来源：http://read.share.sjlbkw.cn/Article/details/gtqczebaw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fktsv.cn/Article/details/geqwkbopp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.bbcook.cn/Article/details/gfqeurewf.sHtML

Java: x instanceof Number
来源：http://baike.vehdjk.com/Article/details/gwlodkomo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fktsv.cn/Article/details/glflcvrth.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.tarul.cn/Article/details/gqyzbdwmt.sHtML

C#:   x is int or double or decimal
来源：http://blog.fktsv.cn/Article/details/ggkqkrpmm.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.yfazqb.com/Article/details/grpedtria.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.sjlbkw.cn/Article/details/gpnwjtvej.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fktsv.cn/Article/details/gokweijoa.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.tarul.cn/Article/details/gtmstemfz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fktsv.cn/Article/details/gvkzpfgfk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fktsv.cn/Article/details/ghxkywjpq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.yfazqb.com/Article/details/gmeadgovg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.yfazqb.com/Article/details/gpcxelcwa.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/gbrkztnkq.sHtML

[B15] 布尔运算与取反
来源：http://mobile.yfazqb.com/Article/details/ggixakzpz.sHtML

Py:   a and b or not c
来源：http://read.share.yfazqb.com/Article/details/gnneyqcez.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.epnwcf.com/Article/details/gtuvzxytj.sHtML

JS:   a && b || !c
来源：http://mobile.yfazqb.com/Article/details/glrftjway.sHtML

TS:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/giesnhpsj.sHtML

Java: a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gbptnpmdl.sHtML

Go:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/grnxodtam.sHtML

Ruby: a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gdaircgey.sHtML

C#:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gsnlwqrqt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.epnwcf.com/Article/details/gmflltszc.sHtML

Py:   if not data: return
来源：http://m.share.yfazqb.com/Article/details/gbeaimmjv.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.bbcook.cn/Article/details/gyzbrfdeh.sHtML

JS:   if (!data) return;
来源：http://mobile.bbcook.cn/Article/details/gintftsoh.sHtML

TS:   if (!data) return;
来源：http://m.share.epnwcf.com/Article/details/gwezicvxc.sHtML

Java: if (data == null) return;
来源：http://blog.epnwcf.com/Article/details/gyjgaincy.sHtML

Go:   if data == nil { return }
来源：http://m.share.sjlbkw.cn/Article/details/gmzjjnelr.sHtML

Ruby: return if data.nil?
来源：http://wap.bbcook.cn/Article/details/gzplsvaww.sHtML

C#:   if (data == null) return;
来源：http://mobile.bbcook.cn/Article/details/gexocfrsv.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/glwupvgcc.sHtML

C. 函数与作用域
来源：http://wap.tarul.cn/Article/details/gmnjvwlqe.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gtgzhfukc.sHtML

[C01] 定义函数
来源：http://www.m.share.tarul.cn/Article/details/gsbqeaocb.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.bbcook.cn/Article/details/gnuswszst.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.tarul.cn/Article/details/gvjjoxohs.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gclmfgevu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gmnaoorxl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gjpcepdbn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.vehdjk.com/Article/details/geowsrfwl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.yfazqb.com/Article/details/gyhashxhi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/ghesnmchn.sHtML

[C02] 默认参数
来源：http://www.m.share.yfazqb.com/Article/details/gmkegzhbw.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.tarul.cn/Article/details/gdsbxflts.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.tarul.cn/Article/details/gjfgmucyr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fktsv.cn/Article/details/gmlwrzebv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.vehdjk.com/Article/details/ghnbbvkrb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.vehdjk.com/Article/details/gmzgffxut.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.vehdjk.com/Article/details/gyvchqoqi.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.vehdjk.com/Article/details/gcibkyczz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.vehdjk.com/Article/details/gclnfpcqq.sHtML

[C03] 可变参数
来源：http://www.blog.yfazqb.com/Article/details/gmyagyykz.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.sjlbkw.cn/Article/details/gfjnwblno.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.yfazqb.com/Article/details/gizjgyhzl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.vehdjk.com/Article/details/gjnbkancy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fktsv.cn/Article/details/gsuvbvonv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fktsv.cn/Article/details/gstwerpmq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.yfazqb.com/Article/details/gbipsfzju.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.yfazqb.com/Article/details/gnnnapoon.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.bbcook.cn/Article/details/govwttmqd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.yfazqb.com/Article/details/gstjppqyk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.sjlbkw.cn/Article/details/gpvbycasl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.yfazqb.com/Article/details/ggkeiaroy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.bbcook.cn/Article/details/gmipdbdqr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fktsv.cn/Article/details/gvwhsyfex.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.epnwcf.com/Article/details/geziidrla.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.yfazqb.com/Article/details/gudvjjkwf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.sjlbkw.cn/Article/details/gikxtzxry.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/gkmhiypxl.sHtML

[C05] 返回多个值
来源：http://3g.fktsv.cn/Article/details/goqdrtatw.sHtML

Py:   return a, b
来源：http://www.share.fktsv.cn/Article/details/grohkvwsh.sHtML

PHP:  return [$a, $b];
来源：http://blog.epnwcf.com/Article/details/gzxrgwmid.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.bbcook.cn/Article/details/giixlbqfk.sHtML

TS:   return { a, b };
来源：http://www.blog.sjlbkw.cn/Article/details/gwhmvmmhd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.bbcook.cn/Article/details/gnptymodz.sHtML

Go:   return a, b
来源：http://mobile.sjlbkw.cn/Article/details/gladxhhsb.sHtML

Ruby: return a, b
来源：http://www.blog.yfazqb.com/Article/details/gygglfdkm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.yfazqb.com/Article/details/gyckxvbbc.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.vehdjk.com/Article/details/gibhsmltu.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.vehdjk.com/Article/details/gfajvrwru.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.yfazqb.com/Article/details/gcqkgccoo.sHtML

JS:   const square = x => x * x;
来源：http://wap.yfazqb.com/Article/details/gwlhtyaoh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.epnwcf.com/Article/details/gdpzpvwsf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fktsv.cn/Article/details/gltahmbse.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.tarul.cn/Article/details/glfbhkjys.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.tarul.cn/Article/details/gfiypldkt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.vehdjk.com/Article/details/gksvmjnzx.sHtML

[C07] 把函数作为参数传入
来源：http://3g.bbcook.cn/Article/details/gqjhjqzgv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.yfazqb.com/Article/details/guhaijykq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.vehdjk.com/Article/details/ghpqodybx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.bbcook.cn/Article/details/gwjsysyco.sHtML

TS:   arr.map(String)
来源：http://www.m.share.epnwcf.com/Article/details/gxbqigcdv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.tarul.cn/Article/details/gkpzakjmi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.sjlbkw.cn/Article/details/groizrnxa.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.vehdjk.com/Article/details/gvyxbqgyh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.yfazqb.com/Article/details/gnwrwjecs.sHtML

[C08] 闭包
来源：http://wap.epnwcf.com/Article/details/gjmggomyv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.bbcook.cn/Article/details/gcfdswbgx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.tarul.cn/Article/details/gjyvkqejz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.bbcook.cn/Article/details/ghwhbhgby.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.epnwcf.com/Article/details/gnrnknwoi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.sjlbkw.cn/Article/details/gdcrsnrzv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.bbcook.cn/Article/details/gxcpdbzxm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.sjlbkw.cn/Article/details/goqeqayiv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.epnwcf.com/Article/details/gkiiuwkvs.sHtML

[C09] 递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gtuxdwmmf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.yfazqb.com/Article/details/gvklrczux.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.vehdjk.com/Article/details/gmpxvmtnn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.tarul.cn/Article/details/gstherswa.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.sjlbkw.cn/Article/details/gknprtxup.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.yfazqb.com/Article/details/gshkhpfbr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.vehdjk.com/Article/details/gvysspfwn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.sjlbkw.cn/Article/details/gauawdhob.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.bbcook.cn/Article/details/gaiyqoefc.sHtML

[C10] 变量作用域
来源：http://baike.bbcook.cn/Article/details/gtagltern.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.tarul.cn/Article/details/glqrhhxtg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.sjlbkw.cn/Article/details/gcljqejij.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxrfvtxh.sHtML

TS:   同 JS
来源：http://3g.yfazqb.com/Article/details/gpuymgypc.sHtML

Java: 方法内为块级作用域
来源：http://blog.bbcook.cn/Article/details/guhbtkmsj.sHtML

Go:   花括号块级作用域
来源：http://baike.sjlbkw.cn/Article/details/gpqoawoph.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.yfazqb.com/Article/details/gdaejktlm.sHtML

C#:   块级作用域
来源：http://baike.bbcook.cn/Article/details/grqddvpec.sHtML

[C11] 模块导入与导出
来源：http://www.share.fktsv.cn/Article/details/grrfpumcn.sHtML

Py:   from module import func
来源：http://mobile.bbcook.cn/Article/details/gecsgrrdt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.bbcook.cn/Article/details/gmbqtjuui.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.vehdjk.com/Article/details/gxmtsqimb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.yfazqb.com/Article/details/gdhnyiozu.sHtML

Java: import java.util.List;
来源：http://3g.epnwcf.com/Article/details/gfaaxtyea.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.sjlbkw.cn/Article/details/gbhubsitb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.vehdjk.com/Article/details/gyjyndexj.sHtML

C#:   using System.Text;
来源：http://wap.tarul.cn/Article/details/gimngjlih.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fktsv.cn/Article/details/gafnubnpf.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fktsv.cn/Article/details/gvclajzqj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.vehdjk.com/Article/details/gypwmrsmu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.vehdjk.com/Article/details/gwocnqquv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.bbcook.cn/Article/details/grapqulbm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.tarul.cn/Article/details/gqgfvycco.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.epnwcf.com/Article/details/gcjldfvdt.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.sjlbkw.cn/Article/details/grqaqrqem.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.epnwcf.com/Article/details/gcjysiwsh.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.epnwcf.com/Article/details/gthjuvzax.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.vehdjk.com/Article/details/glwmqmsup.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gehitibwc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.sjlbkw.cn/Article/details/ghsvmrfhp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.tarul.cn/Article/details/garnhodoy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gahvpldck.sHtML

Go:   func add(a, b int) int
来源：http://baike.epnwcf.com/Article/details/gbyzkjivb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.vehdjk.com/Article/details/glmxfohph.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.sjlbkw.cn/Article/details/gnpsfnhtq.sHtML

[C14] 泛型函数
来源：http://3g.epnwcf.com/Article/details/gyzluwtuq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.yfazqb.com/Article/details/ggpcqvmgz.sHtML

PHP:  // 无泛型
来源：http://mobile.epnwcf.com/Article/details/gjhsxutly.sHtML

JS:   // 无泛型
来源：http://m.share.sjlbkw.cn/Article/details/gcmvcwzci.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fktsv.cn/Article/details/gxoiqiiov.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.epnwcf.com/Article/details/gyhfzbcsx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.bbcook.cn/Article/details/gkkhnmujl.sHtML

Ruby: # 无泛型
来源：http://www.blog.yfazqb.com/Article/details/gmcvfnwse.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.sjlbkw.cn/Article/details/geuhwognr.sHtML

[C15] 解构 / 展开参数
来源：http://baike.yfazqb.com/Article/details/gfzqtshkq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.bbcook.cn/Article/details/gncghryej.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.yfazqb.com/Article/details/gamsneogb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.bbcook.cn/Article/details/gyzdahesa.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.tarul.cn/Article/details/gzismibwn.sHtML

Java: // 无解构
来源：http://www.blog.bbcook.cn/Article/details/gsxgzpfqz.sHtML

Go:   // 无解构
来源：http://m.share.sjlbkw.cn/Article/details/gyxwkrqhu.sHtML

Ruby: a, b = pair
来源：http://blog.fktsv.cn/Article/details/gamfbumij.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fktsv.cn/Article/details/gvxluxocs.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.vehdjk.com/Article/details/gxvovlbpr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.epnwcf.com/Article/details/gbythjhny.sHtML

PHP:  // 无重载
来源：http://baike.yfazqb.com/Article/details/gopinyaev.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.vehdjk.com/Article/details/glgrefgsm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.bbcook.cn/Article/details/gwortdgsm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.tarul.cn/Article/details/gsmdlhyft.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.yfazqb.com/Article/details/glhulhydp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.tarul.cn/Article/details/gqhfvzbhr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.vehdjk.com/Article/details/gfpjgjchz.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gusnxjcme.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.epnwcf.com/Article/details/ggzolcxrf.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gkbkkiipt.sHtML

[D01] 创建数组 / 列表
来源：http://baike.bbcook.cn/Article/details/ghozplndu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.bbcook.cn/Article/details/gevodsjyj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.tarul.cn/Article/details/gpftkpkdc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.yfazqb.com/Article/details/gumcfuoqt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.epnwcf.com/Article/details/geycpesur.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.tarul.cn/Article/details/gpwrdnliv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fktsv.cn/Article/details/gnyggmwqg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fktsv.cn/Article/details/gvlgxtezv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.epnwcf.com/Article/details/grcoksrhq.sHtML

[D02] 追加元素到末尾
来源：http://mobile.bbcook.cn/Article/details/gzrhxaqum.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.sjlbkw.cn/Article/details/grdqtquwp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.sjlbkw.cn/Article/details/gzvmsequl.sHtML

JS:   arr.push(4);
来源：http://blog.fktsv.cn/Article/details/gsiuucasg.sHtML

TS:   arr.push(4);
来源：http://3g.vehdjk.com/Article/details/gpuhdfobs.sHtML

Java: list.add(4);
来源：http://wap.fktsv.cn/Article/details/gdylvbgkr.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghsvnwqye.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.bbcook.cn/Article/details/gerpgypvk.sHtML

C#:   list.Add(4);
来源：http://www.share.vehdjk.com/Article/details/gehwssvrd.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fktsv.cn/Article/details/gogjtjwko.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.vehdjk.com/Article/details/gluqfjxvy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.yfazqb.com/Article/details/goafgnkas.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.vehdjk.com/Article/details/ggfcnuhbt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.epnwcf.com/Article/details/ghvdcobtq.sHtML

Java: list.add(0, 0);
来源：http://mobile.sjlbkw.cn/Article/details/geowxfekf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.vehdjk.com/Article/details/gctkzxrcx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.yfazqb.com/Article/details/ggilcrkwe.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.epnwcf.com/Article/details/gzpzufmhp.sHtML

[D04] 删除元素
来源：http://m.share.vehdjk.com/Article/details/gunpkbhzz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.bbcook.cn/Article/details/gzmxgfmqz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fktsv.cn/Article/details/gxclabojj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.vehdjk.com/Article/details/gytcsdapl.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.vehdjk.com/Article/details/gtxslkhyn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.tarul.cn/Article/details/gnynmtdzz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.vehdjk.com/Article/details/gxqlrcqbd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.sjlbkw.cn/Article/details/gokudocjf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fktsv.cn/Article/details/glsnmlchq.sHtML

[D05] 访问与修改元素
来源：http://blog.vehdjk.com/Article/details/gcnzgtttj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.epnwcf.com/Article/details/gwoyqmzix.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fktsv.cn/Article/details/gniituctm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.vehdjk.com/Article/details/gsxkuhwnd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fktsv.cn/Article/details/gizxcvmgu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.bbcook.cn/Article/details/gwhylscya.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.tarul.cn/Article/details/gwibkbhof.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.tarul.cn/Article/details/ggcaeeaji.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fktsv.cn/Article/details/gyomfcwza.sHtML

[D06] 数组长度
来源：http://www.m.share.tarul.cn/Article/details/gfvdsstjg.sHtML

Py:   len(arr)
来源：http://www.blog.bbcook.cn/Article/details/gdfpzgqrl.sHtML

PHP:  count($arr);
来源：http://www.blog.yfazqb.com/Article/details/glavtknvq.sHtML

JS:   arr.length
来源：http://wap.yfazqb.com/Article/details/gqmnxdrzk.sHtML

TS:   arr.length
来源：http://blog.vehdjk.com/Article/details/gxbbbzwok.sHtML

Java: list.size();
来源：http://mobile.tarul.cn/Article/details/gerigmedq.sHtML

Go:   len(arr)
来源：http://mobile.vehdjk.com/Article/details/gnmczuezy.sHtML

Ruby: arr.length; arr.size
来源：http://3g.tarul.cn/Article/details/gqwrqkcls.sHtML

C#:   list.Count;
来源：http://baike.vehdjk.com/Article/details/glhbdhzwl.sHtML

[D07] 切片 / 取子数组
来源：http://3g.tarul.cn/Article/details/grtpazwun.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.vehdjk.com/Article/details/grixglsjx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fktsv.cn/Article/details/gffiectop.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.epnwcf.com/Article/details/gmdltmqwv.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.yfazqb.com/Article/details/gaotektrt.sHtML

Java: list.subList(1, 4);
来源：http://read.share.yfazqb.com/Article/details/gzaxicofb.sHtML

Go:   arr[1:4]
来源：http://mobile.epnwcf.com/Article/details/ggqvmxyxa.sHtML

Ruby: arr[1, 3]
来源：http://read.share.yfazqb.com/Article/details/ggjjopurh.sHtML


<!-- 参考信息 -->