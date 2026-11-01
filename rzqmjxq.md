代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.vehdjk.com/Article/details/gddofgbbm.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.tarul.cn/Article/details/gppjezeus.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.vehdjk.com/Article/details/grimuuwcp.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.epnwcf.com/Article/details/gayccnevm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fktsv.cn/Article/details/glkwxrzbb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.epnwcf.com/Article/details/gdhqqbpqa.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.tarul.cn/Article/details/gmywywgrw.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.vehdjk.com/Article/details/gixrvabgz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.sjlbkw.cn/Article/details/gtyteyrrl.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.yfazqb.com/Article/details/gygndtnkd.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/gygolncbj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.vehdjk.com/Article/details/gvrvfonhi.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.sjlbkw.cn/Article/details/gzidziivc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.sjlbkw.cn/Article/details/gywjaqhbm.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.tarul.cn/Article/details/gsjrjbtkw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.epnwcf.com/Article/details/gfvzehzsr.sHtML

[B09] break 与 continue
来源：http://3g.bbcook.cn/Article/details/geoqffnwx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.epnwcf.com/Article/details/ghpgzzvvo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/gfyqkydas.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gmjyrmfby.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/geogmbxxs.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/gtoqwrsax.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.bbcook.cn/Article/details/gqezbjvmu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.vehdjk.com/Article/details/gduullths.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gbnkyiphy.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.yfazqb.com/Article/details/gbiwcmmmo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.tarul.cn/Article/details/gyqpqsvek.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.epnwcf.com/Article/details/gbyolfutu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.sjlbkw.cn/Article/details/gryvqnapn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fktsv.cn/Article/details/gxfarwrrn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.tarul.cn/Article/details/gzbfucckt.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fktsv.cn/Article/details/gkttosvsd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.yfazqb.com/Article/details/gssgjswdy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.tarul.cn/Article/details/ggwlidfen.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.sjlbkw.cn/Article/details/gjisdrwlk.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.bbcook.cn/Article/details/glhdoclvs.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fktsv.cn/Article/details/gawywiewf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.epnwcf.com/Article/details/gqnqavaoc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.vehdjk.com/Article/details/gcgpgopiu.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fktsv.cn/Article/details/gqhnpylrm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.yfazqb.com/Article/details/gdasustmq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.yfazqb.com/Article/details/gvxtfcuog.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.tarul.cn/Article/details/gpacvxheu.sHtML

[B12] 跳出多层循环
来源：http://mobile.vehdjk.com/Article/details/gpghegfpv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.sjlbkw.cn/Article/details/gdpcdyzxl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fktsv.cn/Article/details/gfkgluhgp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.sjlbkw.cn/Article/details/gdpaxvpua.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.tarul.cn/Article/details/gmiladarc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.epnwcf.com/Article/details/gnxbnvpfw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.epnwcf.com/Article/details/gfyzaxhmz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.yfazqb.com/Article/details/gtvpqjxof.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.epnwcf.com/Article/details/gbmharzir.sHtML

[B13] 判断是否为数字
来源：http://www.blog.yfazqb.com/Article/details/glnilbads.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fktsv.cn/Article/details/gxnizuysp.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.sjlbkw.cn/Article/details/gqkhkfqkh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.sjlbkw.cn/Article/details/guyzvpkwh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.epnwcf.com/Article/details/gbtdycdby.sHtML

Java: x instanceof Number
来源：http://wap.bbcook.cn/Article/details/gozfzwolr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.tarul.cn/Article/details/galblpyjr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.bbcook.cn/Article/details/gkuwhljct.sHtML

C#:   x is int or double or decimal
来源：http://m.share.sjlbkw.cn/Article/details/gmlgemufb.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.bbcook.cn/Article/details/ggtlazevo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.bbcook.cn/Article/details/gxmotdeky.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.yfazqb.com/Article/details/gphcsukyj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.tarul.cn/Article/details/gajlbpupa.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.epnwcf.com/Article/details/gmuqemlhp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.yfazqb.com/Article/details/gobwxqzeq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.vehdjk.com/Article/details/grxyxcrwj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.epnwcf.com/Article/details/gzrggsmnr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gehfwafki.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.epnwcf.com/Article/details/gbywanizl.sHtML

Py:   a and b or not c
来源：http://mobile.fktsv.cn/Article/details/gdjdhtmvu.sHtML

PHP:  $a && $b || !$c
来源：http://3g.vehdjk.com/Article/details/gqcsxgyfk.sHtML

JS:   a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gqzwtztxp.sHtML

TS:   a && b || !c
来源：http://3g.epnwcf.com/Article/details/gsbyryodw.sHtML

Java: a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/glpisfudx.sHtML

Go:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/ggyppyeua.sHtML

Ruby: a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/gpruyoqhh.sHtML

C#:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/glrjdexnd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.yfazqb.com/Article/details/gdbtoozug.sHtML

Py:   if not data: return
来源：http://m.share.tarul.cn/Article/details/gozurkcwn.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.bbcook.cn/Article/details/gayfwwhfe.sHtML

JS:   if (!data) return;
来源：http://m.share.vehdjk.com/Article/details/gdtbkcsmr.sHtML

TS:   if (!data) return;
来源：http://blog.bbcook.cn/Article/details/gkraanfjg.sHtML

Java: if (data == null) return;
来源：http://www.m.share.yfazqb.com/Article/details/gefkhvzpw.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.vehdjk.com/Article/details/gvxmbajxd.sHtML

Ruby: return if data.nil?
来源：http://3g.epnwcf.com/Article/details/gzhffsjxx.sHtML

C#:   if (data == null) return;
来源：http://baike.tarul.cn/Article/details/gzolyxvwp.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gpljrtjsb.sHtML

C. 函数与作用域
来源：http://mobile.sjlbkw.cn/Article/details/gxltgdmea.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gnvbxlowy.sHtML

[C01] 定义函数
来源：http://read.share.yfazqb.com/Article/details/gkwcfxhby.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fktsv.cn/Article/details/gbadjkotj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/gxfjihnoo.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gimfsqenc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gvtqksrrv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/grkqhuwhp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.vehdjk.com/Article/details/gnybaffub.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fktsv.cn/Article/details/gpthnwjlz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gbvxulsyo.sHtML

[C02] 默认参数
来源：http://www.m.share.vehdjk.com/Article/details/gelbhdfdl.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fktsv.cn/Article/details/gtqgmkzal.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.tarul.cn/Article/details/ghuglksbc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.epnwcf.com/Article/details/gqegccaps.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fktsv.cn/Article/details/glvzxghvf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fktsv.cn/Article/details/gsnbpgvfz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.epnwcf.com/Article/details/gwuphkdet.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.sjlbkw.cn/Article/details/gfmcsakyq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.bbcook.cn/Article/details/gpdvysbao.sHtML

[C03] 可变参数
来源：http://read.share.vehdjk.com/Article/details/gdhvcllox.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.bbcook.cn/Article/details/ghpicyaie.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fktsv.cn/Article/details/ggryilxem.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.yfazqb.com/Article/details/gqevglsyv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.tarul.cn/Article/details/ggyxeyffy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.epnwcf.com/Article/details/ghjdducqo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.epnwcf.com/Article/details/ggyfznliy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fktsv.cn/Article/details/gdvkqhpox.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fktsv.cn/Article/details/gqbuuxukk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.bbcook.cn/Article/details/gdjhizuai.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.sjlbkw.cn/Article/details/gnbjcipbk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.vehdjk.com/Article/details/golnyqwgv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.tarul.cn/Article/details/gphekxlga.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.tarul.cn/Article/details/gatndboxl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fktsv.cn/Article/details/gwrisuyxa.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fktsv.cn/Article/details/godgcfxqc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.tarul.cn/Article/details/gogmdtzye.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.epnwcf.com/Article/details/gwdgavrot.sHtML

[C05] 返回多个值
来源：http://www.blog.yfazqb.com/Article/details/gtzbvqhge.sHtML

Py:   return a, b
来源：http://www.blog.epnwcf.com/Article/details/gxtontwtx.sHtML

PHP:  return [$a, $b];
来源：http://m.share.bbcook.cn/Article/details/gounvkabd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.sjlbkw.cn/Article/details/gaozehpyp.sHtML

TS:   return { a, b };
来源：http://www.share.epnwcf.com/Article/details/gzejjihus.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.tarul.cn/Article/details/gdfkuqgyj.sHtML

Go:   return a, b
来源：http://m.share.bbcook.cn/Article/details/gaawzszyx.sHtML

Ruby: return a, b
来源：http://3g.yfazqb.com/Article/details/grpjavjdv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.yfazqb.com/Article/details/gzqeoxkdu.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.yfazqb.com/Article/details/gikqzlzel.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.tarul.cn/Article/details/gmpguiabh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fktsv.cn/Article/details/geybyerel.sHtML

JS:   const square = x => x * x;
来源：http://m.share.bbcook.cn/Article/details/gxsxooiiq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.yfazqb.com/Article/details/gvnkwzvxm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.bbcook.cn/Article/details/gfwcdgcah.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.epnwcf.com/Article/details/gxgfzdqhz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.yfazqb.com/Article/details/gozdsiwlk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gnzbssozy.sHtML

[C07] 把函数作为参数传入
来源：http://blog.yfazqb.com/Article/details/gctznqvxh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.tarul.cn/Article/details/gqtxcvyuu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.epnwcf.com/Article/details/gqdoekfye.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.yfazqb.com/Article/details/gxgqfveir.sHtML

TS:   arr.map(String)
来源：http://blog.vehdjk.com/Article/details/gimemdngh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.tarul.cn/Article/details/gcwivkspo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fktsv.cn/Article/details/gbmirztuw.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.bbcook.cn/Article/details/gmwfpfyqn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.vehdjk.com/Article/details/gcxvlwrcr.sHtML

[C08] 闭包
来源：http://www.share.bbcook.cn/Article/details/gtxbrqoyg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.vehdjk.com/Article/details/gqiroqzna.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.sjlbkw.cn/Article/details/gotqydwqo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/gszjxxkgw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.vehdjk.com/Article/details/gmynbsdnc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.yfazqb.com/Article/details/gurtiroei.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.epnwcf.com/Article/details/gvlwdtwgb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.epnwcf.com/Article/details/gdxqsnile.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.epnwcf.com/Article/details/gjhmdvcsc.sHtML

[C09] 递归
来源：http://3g.sjlbkw.cn/Article/details/gyozypuha.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.tarul.cn/Article/details/gbsdkdsnl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.tarul.cn/Article/details/ggaqqhrjf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.tarul.cn/Article/details/gsnarvebi.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fktsv.cn/Article/details/giuokpuwp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.vehdjk.com/Article/details/gvjkgqfjh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.yfazqb.com/Article/details/gyvqanlrw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.bbcook.cn/Article/details/gqtydcmbu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.sjlbkw.cn/Article/details/guulblgjf.sHtML

[C10] 变量作用域
来源：http://read.share.sjlbkw.cn/Article/details/ggxpgkcwe.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.sjlbkw.cn/Article/details/gfbedquip.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.sjlbkw.cn/Article/details/gxlkmwupn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.yfazqb.com/Article/details/gbvmnybpz.sHtML

TS:   同 JS
来源：http://m.share.bbcook.cn/Article/details/gqdwmmlle.sHtML

Java: 方法内为块级作用域
来源：http://mobile.yfazqb.com/Article/details/gmxdhhpqc.sHtML

Go:   花括号块级作用域
来源：http://wap.bbcook.cn/Article/details/glokobbdn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fktsv.cn/Article/details/gwnxynvyu.sHtML

C#:   块级作用域
来源：http://www.blog.vehdjk.com/Article/details/gpckqluso.sHtML

[C11] 模块导入与导出
来源：http://3g.epnwcf.com/Article/details/gusmymhoi.sHtML

Py:   from module import func
来源：http://blog.yfazqb.com/Article/details/gkktstcux.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.bbcook.cn/Article/details/gfsfdmmxa.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.sjlbkw.cn/Article/details/gjibzpamx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.vehdjk.com/Article/details/gjsxpzfuc.sHtML

Java: import java.util.List;
来源：http://read.share.tarul.cn/Article/details/gwsaxgqhb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.epnwcf.com/Article/details/gnszmpcgp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.bbcook.cn/Article/details/gntosjpgz.sHtML

C#:   using System.Text;
来源：http://m.share.tarul.cn/Article/details/gispfznqo.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.vehdjk.com/Article/details/gviajauxt.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.bbcook.cn/Article/details/grmgosekb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.sjlbkw.cn/Article/details/gxslmsxmx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.tarul.cn/Article/details/glhsvgtby.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.vehdjk.com/Article/details/gnkyozvvd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.tarul.cn/Article/details/gvtowabdo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.tarul.cn/Article/details/gweivumnj.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.sjlbkw.cn/Article/details/gfcnkegli.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.sjlbkw.cn/Article/details/gmcnvheux.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.tarul.cn/Article/details/gscrtlsqc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.yfazqb.com/Article/details/gfvusyimn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.epnwcf.com/Article/details/gkwykqnwv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.yfazqb.com/Article/details/glbhzyils.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/gchleldpf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gbdhjpwys.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.yfazqb.com/Article/details/gfziucaye.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.epnwcf.com/Article/details/gboxcmpyn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.vehdjk.com/Article/details/gyqlgqfcv.sHtML

[C14] 泛型函数
来源：http://mobile.bbcook.cn/Article/details/gmyirjkcl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.sjlbkw.cn/Article/details/goedmcdjq.sHtML

PHP:  // 无泛型
来源：http://3g.epnwcf.com/Article/details/gwyjdgthg.sHtML

JS:   // 无泛型
来源：http://www.blog.fktsv.cn/Article/details/gtsstchgz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.yfazqb.com/Article/details/golpbvqyk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.yfazqb.com/Article/details/gukurtgnb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fktsv.cn/Article/details/gjndbwatg.sHtML

Ruby: # 无泛型
来源：http://read.share.epnwcf.com/Article/details/ggvarxiwm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.bbcook.cn/Article/details/gawpvywzp.sHtML

[C15] 解构 / 展开参数
来源：http://3g.bbcook.cn/Article/details/gtyexgker.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.tarul.cn/Article/details/gyembpoxf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fktsv.cn/Article/details/gowatafgj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.yfazqb.com/Article/details/gtjvjubux.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.sjlbkw.cn/Article/details/gepgczmro.sHtML

Java: // 无解构
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrqmsbro.sHtML

Go:   // 无解构
来源：http://wap.fktsv.cn/Article/details/gjkzahbdd.sHtML

Ruby: a, b = pair
来源：http://www.share.vehdjk.com/Article/details/gpzqcwrby.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.bbcook.cn/Article/details/gibqdudew.sHtML

[C16] 函数 / 方法重载
来源：http://blog.vehdjk.com/Article/details/grphprtow.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.yfazqb.com/Article/details/gmdyfahzj.sHtML

PHP:  // 无重载
来源：http://mobile.tarul.cn/Article/details/gsnjqfvxj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.yfazqb.com/Article/details/getavuhef.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fktsv.cn/Article/details/gugqobofz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fktsv.cn/Article/details/gqxhzjoaf.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fktsv.cn/Article/details/gqnuvmaxv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.yfazqb.com/Article/details/grqgnwmbq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fktsv.cn/Article/details/ggnjvqbjq.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gzrlmrcdc.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.epnwcf.com/Article/details/gbxkmgoxo.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gseeupywn.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.bbcook.cn/Article/details/gdvfrxbcr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.epnwcf.com/Article/details/gupohrlvh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.tarul.cn/Article/details/gyfrbwgdb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.tarul.cn/Article/details/ghvjkzyou.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.vehdjk.com/Article/details/gzyyrrzcn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.bbcook.cn/Article/details/gwhcdonrt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.vehdjk.com/Article/details/gqcxomrpt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.sjlbkw.cn/Article/details/gjglozrll.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.bbcook.cn/Article/details/gfiovwtiu.sHtML

[D02] 追加元素到末尾
来源：http://baike.vehdjk.com/Article/details/gfxhilumd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.sjlbkw.cn/Article/details/guwdqlkqp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.sjlbkw.cn/Article/details/gcrbgtvam.sHtML

JS:   arr.push(4);
来源：http://wap.tarul.cn/Article/details/giixsleey.sHtML

TS:   arr.push(4);
来源：http://www.m.share.epnwcf.com/Article/details/gkloazyyc.sHtML

Java: list.add(4);
来源：http://3g.vehdjk.com/Article/details/gzazssdgr.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gaimravdr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.bbcook.cn/Article/details/gjooaymvx.sHtML

C#:   list.Add(4);
来源：http://m.share.fktsv.cn/Article/details/gqcjvqcxi.sHtML

[D03] 在指定位置插入元素
来源：http://3g.bbcook.cn/Article/details/gppuldbom.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.epnwcf.com/Article/details/gxhkepbud.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.sjlbkw.cn/Article/details/gbjvsmnfp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.vehdjk.com/Article/details/gqipflepl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.tarul.cn/Article/details/guvmahrtk.sHtML

Java: list.add(0, 0);
来源：http://3g.yfazqb.com/Article/details/gwpabkzmu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fktsv.cn/Article/details/gzyfjjcdj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.tarul.cn/Article/details/grgfoxode.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.vehdjk.com/Article/details/gvujjmgvr.sHtML

[D04] 删除元素
来源：http://m.share.vehdjk.com/Article/details/gejqclxma.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.tarul.cn/Article/details/gzvsrwetb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.vehdjk.com/Article/details/gkdnanexf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.tarul.cn/Article/details/gmyvwbrlk.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.bbcook.cn/Article/details/gcakhapgy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.epnwcf.com/Article/details/gecszmssq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.sjlbkw.cn/Article/details/gjfwygnpe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.bbcook.cn/Article/details/gkyuaqaol.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.vehdjk.com/Article/details/gypnjxrnh.sHtML

[D05] 访问与修改元素
来源：http://3g.fktsv.cn/Article/details/guqdmmdjt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.tarul.cn/Article/details/giumwnqmf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.vehdjk.com/Article/details/grmecedty.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.bbcook.cn/Article/details/gqwxdqvyo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fktsv.cn/Article/details/gbpaxhxds.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.bbcook.cn/Article/details/gmhnwkzoq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fktsv.cn/Article/details/gpsxrorbg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.bbcook.cn/Article/details/gyxjcxvbc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.sjlbkw.cn/Article/details/govivddfq.sHtML

[D06] 数组长度
来源：http://read.share.fktsv.cn/Article/details/glymdddan.sHtML

Py:   len(arr)
来源：http://blog.sjlbkw.cn/Article/details/ghzkzauyt.sHtML

PHP:  count($arr);
来源：http://www.share.bbcook.cn/Article/details/glhrurvkt.sHtML

JS:   arr.length
来源：http://m.share.vehdjk.com/Article/details/gdmjqffxx.sHtML

TS:   arr.length
来源：http://www.m.share.vehdjk.com/Article/details/ggssotvyv.sHtML

Java: list.size();
来源：http://wap.vehdjk.com/Article/details/gksrauini.sHtML

Go:   len(arr)
来源：http://www.share.fktsv.cn/Article/details/gumyfsqlk.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fktsv.cn/Article/details/gckuiiopy.sHtML

C#:   list.Count;
来源：http://read.share.fktsv.cn/Article/details/goqmxvwtu.sHtML

[D07] 切片 / 取子数组
来源：http://blog.sjlbkw.cn/Article/details/gcwuczxhy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.vehdjk.com/Article/details/gcjqrlacp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkncehum.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.epnwcf.com/Article/details/gqtvrivaa.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.epnwcf.com/Article/details/ggkdalitg.sHtML

Java: list.subList(1, 4);
来源：http://baike.fktsv.cn/Article/details/gudhkomsb.sHtML

Go:   arr[1:4]
来源：http://read.share.bbcook.cn/Article/details/grplldtgp.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.tarul.cn/Article/details/gstlypydf.sHtML


<!-- 参考信息 -->