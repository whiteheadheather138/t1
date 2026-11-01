代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.tarul.cn/Article/details/gpgacbwkg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.epnwcf.com/Article/details/ggldqoubb.sHtML

[B07] while 循环
来源：http://blog.tarul.cn/Article/details/gopuodchl.sHtML

Py:   while i < 10: i += 1
来源：http://baike.yfazqb.com/Article/details/ghupgguab.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fktsv.cn/Article/details/gpcjdhxsf.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.epnwcf.com/Article/details/gwznngndx.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.sjlbkw.cn/Article/details/guspmzxwz.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.sjlbkw.cn/Article/details/gxesedlqd.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.vehdjk.com/Article/details/gaofnfvov.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.vehdjk.com/Article/details/gwhwfgyea.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/gbyvflsct.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.fktsv.cn/Article/details/gdjvolmpp.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.bbcook.cn/Article/details/glnqbbjph.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.yfazqb.com/Article/details/gnhiexfao.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fktsv.cn/Article/details/glqoosywo.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/guayljopx.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/gxihkgqqv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.sjlbkw.cn/Article/details/grgczwclt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.epnwcf.com/Article/details/gxtiffjrs.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.fktsv.cn/Article/details/gbsrqzlwv.sHtML

[B09] break 与 continue
来源：http://blog.tarul.cn/Article/details/gvozxyxaa.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.tarul.cn/Article/details/gqaudnfdi.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/ghqjrbxhh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/gnpqguzox.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/ggomkxljl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/gvyfwccud.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.bbcook.cn/Article/details/gujtjvfmk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.sjlbkw.cn/Article/details/gxumbkgzw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gtwfxsvut.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.yfazqb.com/Article/details/gmhzqkxhr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.epnwcf.com/Article/details/gwffearhv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.vehdjk.com/Article/details/gmakbqpbq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.yfazqb.com/Article/details/gpoovqujv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.vehdjk.com/Article/details/gzmdotwhs.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.fktsv.cn/Article/details/gbmrjdxge.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fktsv.cn/Article/details/gnffdpwgl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.vehdjk.com/Article/details/gmbcbsckt.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdgnswznq.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.epnwcf.com/Article/details/gxwywsxhl.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.yfazqb.com/Article/details/gmmysphsw.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.vehdjk.com/Article/details/gpimrzkur.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.epnwcf.com/Article/details/gxldxeira.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.sjlbkw.cn/Article/details/gupfyxjhm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.tarul.cn/Article/details/gaixgzlia.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fktsv.cn/Article/details/gsjztzoho.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.tarul.cn/Article/details/grbaqivwa.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.yfazqb.com/Article/details/gblhbewta.sHtML

[B12] 跳出多层循环
来源：http://wap.yfazqb.com/Article/details/ghvjuuwal.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.bbcook.cn/Article/details/gdrfpmtqk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.tarul.cn/Article/details/gpnihlgfr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.sjlbkw.cn/Article/details/gxoaaqsyn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.vehdjk.com/Article/details/ggtkfoyud.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.epnwcf.com/Article/details/gxtigbznr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.vehdjk.com/Article/details/gvhqjvokt.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.bbcook.cn/Article/details/gbclaerfl.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.bbcook.cn/Article/details/ggodtabbl.sHtML

[B13] 判断是否为数字
来源：http://www.share.fktsv.cn/Article/details/gzyoegpit.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.tarul.cn/Article/details/gvmuggniv.sHtML

PHP:  is_numeric($x)
来源：http://read.share.yfazqb.com/Article/details/gjdwkodwp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.tarul.cn/Article/details/gmstnwbte.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fktsv.cn/Article/details/gzhojludd.sHtML

Java: x instanceof Number
来源：http://wap.vehdjk.com/Article/details/gvivpzisl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.yfazqb.com/Article/details/giiyeuaho.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.bbcook.cn/Article/details/gwthribcv.sHtML

C#:   x is int or double or decimal
来源：http://baike.bbcook.cn/Article/details/gpltambjo.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.tarul.cn/Article/details/gecglscif.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.sjlbkw.cn/Article/details/gcyconhgo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.tarul.cn/Article/details/guixqflzj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.epnwcf.com/Article/details/gudlfvobn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.bbcook.cn/Article/details/gjoizycpt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/gtiarewpm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.bbcook.cn/Article/details/geifkbnih.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.yfazqb.com/Article/details/gydgalrov.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.bbcook.cn/Article/details/gsgoojjff.sHtML

[B15] 布尔运算与取反
来源：http://read.share.bbcook.cn/Article/details/gsaahvtrn.sHtML

Py:   a and b or not c
来源：http://www.m.share.epnwcf.com/Article/details/gkwjcrjpm.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fktsv.cn/Article/details/gweppibwn.sHtML

JS:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/gprfeyjqe.sHtML

TS:   a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gidztfhkl.sHtML

Java: a && b || !c
来源：http://read.share.tarul.cn/Article/details/gqubjavqi.sHtML

Go:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gohbtsyxn.sHtML

Ruby: a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gpeulabqu.sHtML

C#:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gyauuvcji.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.yfazqb.com/Article/details/gdcqyjznc.sHtML

Py:   if not data: return
来源：http://wap.yfazqb.com/Article/details/glfbsqecl.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.bbcook.cn/Article/details/gyscsocia.sHtML

JS:   if (!data) return;
来源：http://www.m.share.tarul.cn/Article/details/gyrkrqwwq.sHtML

TS:   if (!data) return;
来源：http://www.m.share.vehdjk.com/Article/details/glstlduoe.sHtML

Java: if (data == null) return;
来源：http://blog.yfazqb.com/Article/details/gvwpqxzsv.sHtML

Go:   if data == nil { return }
来源：http://www.share.tarul.cn/Article/details/grbwppcqe.sHtML

Ruby: return if data.nil?
来源：http://www.blog.tarul.cn/Article/details/gdwtorvbt.sHtML

C#:   if (data == null) return;
来源：http://wap.yfazqb.com/Article/details/gyjkvwrof.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gonybrzgm.sHtML

C. 函数与作用域
来源：http://www.share.sjlbkw.cn/Article/details/gsrngwvsm.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gkfqafydk.sHtML

[C01] 定义函数
来源：http://www.share.sjlbkw.cn/Article/details/gbbihuemf.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.epnwcf.com/Article/details/gibiczmih.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/gnhdkkfet.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gwipyjxjo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gnckuwfuo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gasgdyfbv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.yfazqb.com/Article/details/gbpvxaliw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.yfazqb.com/Article/details/gdkujudqa.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gojyqpwwo.sHtML

[C02] 默认参数
来源：http://read.share.sjlbkw.cn/Article/details/glvknqkvs.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.tarul.cn/Article/details/gpeyugvzw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.tarul.cn/Article/details/gwxgrqiig.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gausicowx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.yfazqb.com/Article/details/grsnmyepf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.epnwcf.com/Article/details/gmzlwuzil.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.yfazqb.com/Article/details/gxmsvqutb.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.epnwcf.com/Article/details/gujznumka.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.epnwcf.com/Article/details/gnwaejwmi.sHtML

[C03] 可变参数
来源：http://3g.epnwcf.com/Article/details/gsflpztcu.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fktsv.cn/Article/details/gusklkvob.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.vehdjk.com/Article/details/gvmcpfxxd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.tarul.cn/Article/details/gsjeqklpd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.epnwcf.com/Article/details/gzmohcfbt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fktsv.cn/Article/details/gkparlslk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fktsv.cn/Article/details/gmjfludhj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.epnwcf.com/Article/details/glwstbqdo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fktsv.cn/Article/details/gmzjebtxf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.vehdjk.com/Article/details/gxufiejyk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.tarul.cn/Article/details/gbfjitakc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fktsv.cn/Article/details/guzyruafx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.sjlbkw.cn/Article/details/gnbwrjlvg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.vehdjk.com/Article/details/govbrtfnf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.sjlbkw.cn/Article/details/gstzckapf.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.yfazqb.com/Article/details/gunagwrom.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/gyqbkgflb.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fktsv.cn/Article/details/goyzpynig.sHtML

[C05] 返回多个值
来源：http://baike.bbcook.cn/Article/details/glvizyebe.sHtML

Py:   return a, b
来源：http://m.share.vehdjk.com/Article/details/gisyteemg.sHtML

PHP:  return [$a, $b];
来源：http://wap.epnwcf.com/Article/details/gpwzyuwnl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.bbcook.cn/Article/details/gvdeikeyb.sHtML

TS:   return { a, b };
来源：http://www.blog.yfazqb.com/Article/details/gozrorwfw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fktsv.cn/Article/details/gpqnkmchu.sHtML

Go:   return a, b
来源：http://mobile.tarul.cn/Article/details/gavtkjtwb.sHtML

Ruby: return a, b
来源：http://www.share.bbcook.cn/Article/details/gxmnyrxkp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.tarul.cn/Article/details/glfbftwpn.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.epnwcf.com/Article/details/gumsiznmz.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.epnwcf.com/Article/details/gkjoawgjl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.bbcook.cn/Article/details/gamroypuw.sHtML

JS:   const square = x => x * x;
来源：http://3g.fktsv.cn/Article/details/gpljmglhd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.epnwcf.com/Article/details/gjybqodbe.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fktsv.cn/Article/details/gjpxzqdky.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.sjlbkw.cn/Article/details/gtqiftxiy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.tarul.cn/Article/details/gjbtpqewg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.vehdjk.com/Article/details/gbmwfhiho.sHtML

[C07] 把函数作为参数传入
来源：http://blog.sjlbkw.cn/Article/details/gvvruirvt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.bbcook.cn/Article/details/gehkiuijl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.bbcook.cn/Article/details/gkungipne.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.tarul.cn/Article/details/gzwmdfsos.sHtML

TS:   arr.map(String)
来源：http://read.share.tarul.cn/Article/details/gyitipibz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.epnwcf.com/Article/details/gimezyewr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.bbcook.cn/Article/details/gnpnnkmwt.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fktsv.cn/Article/details/gjhtoewkq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.yfazqb.com/Article/details/gmgrzscii.sHtML

[C08] 闭包
来源：http://blog.fktsv.cn/Article/details/gebxgsyls.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fktsv.cn/Article/details/glsympkrm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.epnwcf.com/Article/details/ghmzqbpat.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.epnwcf.com/Article/details/gfkuwwgbe.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fktsv.cn/Article/details/gbmpqaudz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fktsv.cn/Article/details/gfsdthjmn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.sjlbkw.cn/Article/details/gvnatbnzc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.yfazqb.com/Article/details/gftbzgoys.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.epnwcf.com/Article/details/gpsmokfjn.sHtML

[C09] 递归
来源：http://baike.sjlbkw.cn/Article/details/glnlwmrec.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.vehdjk.com/Article/details/ghzjqfacq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.tarul.cn/Article/details/gydznwsjk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fktsv.cn/Article/details/gygqjtwhd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.yfazqb.com/Article/details/gzfmwzvla.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.bbcook.cn/Article/details/gdmcbttth.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gigcwbctq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fktsv.cn/Article/details/gjaulhgzl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.bbcook.cn/Article/details/gssfezyut.sHtML

[C10] 变量作用域
来源：http://blog.yfazqb.com/Article/details/gfbdgwrms.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.epnwcf.com/Article/details/gneqbehnv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.epnwcf.com/Article/details/gbnddnapq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.yfazqb.com/Article/details/glbxpztey.sHtML

TS:   同 JS
来源：http://m.share.yfazqb.com/Article/details/gsxghbqky.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fktsv.cn/Article/details/gphasnhza.sHtML

Go:   花括号块级作用域
来源：http://baike.sjlbkw.cn/Article/details/gaainvkrh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.yfazqb.com/Article/details/ggkqnmtvz.sHtML

C#:   块级作用域
来源：http://www.m.share.bbcook.cn/Article/details/gxqgqjcqm.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.yfazqb.com/Article/details/gmnubznpe.sHtML

Py:   from module import func
来源：http://mobile.yfazqb.com/Article/details/gtkpsbrnj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.tarul.cn/Article/details/gbiqteqgy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.epnwcf.com/Article/details/gwvxrhtbm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.epnwcf.com/Article/details/gbsyzitkh.sHtML

Java: import java.util.List;
来源：http://m.share.yfazqb.com/Article/details/gvvdzfusq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.yfazqb.com/Article/details/gufgwyujj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fktsv.cn/Article/details/grrhgkpxi.sHtML

C#:   using System.Text;
来源：http://blog.epnwcf.com/Article/details/gyhodewyv.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.tarul.cn/Article/details/gdaqjecxp.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.epnwcf.com/Article/details/gvjkejaif.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.sjlbkw.cn/Article/details/gszdiiysa.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.vehdjk.com/Article/details/gztrjpsbn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.tarul.cn/Article/details/gyzrumike.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.vehdjk.com/Article/details/gmmmkvsmo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.bbcook.cn/Article/details/gztxmpmcp.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.yfazqb.com/Article/details/gzhpteiwx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.vehdjk.com/Article/details/gtowfkvom.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.tarul.cn/Article/details/gjjuyynwr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.yfazqb.com/Article/details/gdwcsshac.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/gkwexhhdm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.tarul.cn/Article/details/gebazdnhu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gyeshorpf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gmmuncnrs.sHtML

Go:   func add(a, b int) int
来源：http://3g.tarul.cn/Article/details/gvjegjbir.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.vehdjk.com/Article/details/gezbwrewe.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fktsv.cn/Article/details/gjqxbgnfs.sHtML

[C14] 泛型函数
来源：http://read.share.tarul.cn/Article/details/giezopqjk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.bbcook.cn/Article/details/ggbmjlffs.sHtML

PHP:  // 无泛型
来源：http://blog.sjlbkw.cn/Article/details/gnxonnnrh.sHtML

JS:   // 无泛型
来源：http://blog.tarul.cn/Article/details/gnuyjhktd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.epnwcf.com/Article/details/gskrrtaad.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.vehdjk.com/Article/details/gjvkocyda.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fktsv.cn/Article/details/gpvsikszq.sHtML

Ruby: # 无泛型
来源：http://read.share.bbcook.cn/Article/details/gedvxldev.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.bbcook.cn/Article/details/grmzatmom.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.bbcook.cn/Article/details/ggvvdwcer.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.yfazqb.com/Article/details/gqkhmnrsn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.bbcook.cn/Article/details/gwzmbgldg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fktsv.cn/Article/details/guscjhpio.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fktsv.cn/Article/details/gcsymjqra.sHtML

Java: // 无解构
来源：http://m.share.vehdjk.com/Article/details/gfzcaewog.sHtML

Go:   // 无解构
来源：http://www.m.share.yfazqb.com/Article/details/gcehroiim.sHtML

Ruby: a, b = pair
来源：http://www.m.share.yfazqb.com/Article/details/grzoqumci.sHtML

C#:   var (a, b) = pair;
来源：http://3g.sjlbkw.cn/Article/details/gzwglsgqz.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.sjlbkw.cn/Article/details/gpyqkmlsc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.epnwcf.com/Article/details/ghmsrwgto.sHtML

PHP:  // 无重载
来源：http://3g.tarul.cn/Article/details/gtmoaanze.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fktsv.cn/Article/details/gcixhebvv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.yfazqb.com/Article/details/gduqpeivk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.vehdjk.com/Article/details/ghcfvabmu.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.tarul.cn/Article/details/ggajarisd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.tarul.cn/Article/details/gxojhhqpw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.tarul.cn/Article/details/goqtayvbo.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gdfvgobyw.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.vehdjk.com/Article/details/gusgltoor.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gbtatscdi.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.vehdjk.com/Article/details/gyawrcymc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fktsv.cn/Article/details/ggiwmokuv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.tarul.cn/Article/details/gclbgokae.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.vehdjk.com/Article/details/gcracjeds.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.tarul.cn/Article/details/gqsdshxrr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.yfazqb.com/Article/details/gfkkcvfsu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.bbcook.cn/Article/details/ggeajrvar.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.vehdjk.com/Article/details/gqdzjvtwn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fktsv.cn/Article/details/gykjfouqn.sHtML

[D02] 追加元素到末尾
来源：http://baike.vehdjk.com/Article/details/gmyyhrzww.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.sjlbkw.cn/Article/details/gkzeiidjq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.tarul.cn/Article/details/goxvrnimy.sHtML

JS:   arr.push(4);
来源：http://www.blog.tarul.cn/Article/details/gncenhxeh.sHtML

TS:   arr.push(4);
来源：http://3g.sjlbkw.cn/Article/details/gbprnwodb.sHtML

Java: list.add(4);
来源：http://baike.bbcook.cn/Article/details/gjhvmymun.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.sjlbkw.cn/Article/details/gvwppgqyq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.bbcook.cn/Article/details/gzewckfbk.sHtML

C#:   list.Add(4);
来源：http://read.share.tarul.cn/Article/details/gyqtmnpxx.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.yfazqb.com/Article/details/gjbrhbtcu.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.sjlbkw.cn/Article/details/gqyayvfsg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fktsv.cn/Article/details/goqtgdsvu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.vehdjk.com/Article/details/gdthnsbcm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.tarul.cn/Article/details/gxkhwvljw.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.yfazqb.com/Article/details/gmxxgnsjf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.yfazqb.com/Article/details/gwwvjcfns.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.vehdjk.com/Article/details/gywhzatng.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gmttirvse.sHtML

[D04] 删除元素
来源：http://read.share.fktsv.cn/Article/details/guitfsnyo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fktsv.cn/Article/details/ggkhwpmmj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.bbcook.cn/Article/details/grpajcqaq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fktsv.cn/Article/details/gbbazpvmo.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.tarul.cn/Article/details/gmyxntisz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.yfazqb.com/Article/details/gcuhhwqck.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.vehdjk.com/Article/details/gowfdgebn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fktsv.cn/Article/details/ghnfjomht.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.yfazqb.com/Article/details/geicjcqtt.sHtML

[D05] 访问与修改元素
来源：http://wap.sjlbkw.cn/Article/details/galybqpfe.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fktsv.cn/Article/details/gdtrkuxrl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.sjlbkw.cn/Article/details/gargnbdnm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.tarul.cn/Article/details/girtrbwud.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.sjlbkw.cn/Article/details/gmgsizbot.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.bbcook.cn/Article/details/giqxyvkox.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.vehdjk.com/Article/details/gjdptmang.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.sjlbkw.cn/Article/details/grqwfpzzj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.tarul.cn/Article/details/gpgxepewh.sHtML

[D06] 数组长度
来源：http://read.share.fktsv.cn/Article/details/gohvumbjh.sHtML

Py:   len(arr)
来源：http://www.blog.yfazqb.com/Article/details/gmhnwdden.sHtML

PHP:  count($arr);
来源：http://wap.epnwcf.com/Article/details/gddzmstjc.sHtML

JS:   arr.length
来源：http://mobile.vehdjk.com/Article/details/gwyyjhbkn.sHtML

TS:   arr.length
来源：http://mobile.bbcook.cn/Article/details/gyplqqqbc.sHtML

Java: list.size();
来源：http://www.m.share.vehdjk.com/Article/details/giaknpstq.sHtML

Go:   len(arr)
来源：http://baike.vehdjk.com/Article/details/ggfkqqxkb.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.yfazqb.com/Article/details/goblvixjl.sHtML

C#:   list.Count;
来源：http://read.share.vehdjk.com/Article/details/gzbskczbf.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fktsv.cn/Article/details/gqjqnvhlv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.yfazqb.com/Article/details/gxufdcoxe.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fktsv.cn/Article/details/gflxlcswl.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.tarul.cn/Article/details/gccofjrum.sHtML


<!-- 参考信息 -->