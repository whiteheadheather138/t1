代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.epnwcf.com/Article/details/gpjuvqcng.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.vehdjk.com/Article/details/gllnxlkiz.sHtML

[B07] while 循环
来源：http://mobile.sjlbkw.cn/Article/details/gtcqdsdvo.sHtML

Py:   while i < 10: i += 1
来源：http://baike.sjlbkw.cn/Article/details/grqmmqsjb.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.epnwcf.com/Article/details/gejublqce.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.bbcook.cn/Article/details/gwbeqkcss.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.sjlbkw.cn/Article/details/gbzpswcde.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/gervwyeas.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.tarul.cn/Article/details/ghcgmawtq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.sjlbkw.cn/Article/details/ghhgmlcpw.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.epnwcf.com/Article/details/gxtmrxyfv.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.bbcook.cn/Article/details/ghezemhmq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.sjlbkw.cn/Article/details/gwknswwkq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.bbcook.cn/Article/details/ggcquapqt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gunbnwkyc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.sjlbkw.cn/Article/details/gvuoheryp.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.tarul.cn/Article/details/gylcfojmq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.vehdjk.com/Article/details/gghigswuy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.vehdjk.com/Article/details/ghegdkgod.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fktsv.cn/Article/details/gughebgev.sHtML

[B09] break 与 continue
来源：http://www.share.vehdjk.com/Article/details/gunhrrwbf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.epnwcf.com/Article/details/gsvxenzqn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/giqoqeqod.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gdmeclbqp.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gfaokqerc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/genurmfpx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.epnwcf.com/Article/details/gtjrllvvm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fktsv.cn/Article/details/geruhlzpz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gnvjqufqz.sHtML

[B10] 遍历同时拿索引
来源：http://wap.sjlbkw.cn/Article/details/gjdnpgoks.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.yfazqb.com/Article/details/gbadxlusa.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.epnwcf.com/Article/details/gdprzezyf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.sjlbkw.cn/Article/details/gbspybfvj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.sjlbkw.cn/Article/details/gebuhnxbi.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.epnwcf.com/Article/details/gikmniloq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.epnwcf.com/Article/details/gepbrzfpu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.yfazqb.com/Article/details/glyofosua.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.vehdjk.com/Article/details/gqyptdslb.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.yfazqb.com/Article/details/gxemijjfx.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.bbcook.cn/Article/details/grlluccms.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.yfazqb.com/Article/details/gcxirmsop.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.vehdjk.com/Article/details/ghnrcbrxo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.bbcook.cn/Article/details/gtqalhqio.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.yfazqb.com/Article/details/gllxfvgig.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.epnwcf.com/Article/details/gaifuphuz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fktsv.cn/Article/details/gvmzbtggt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.yfazqb.com/Article/details/gmzxtuedu.sHtML

[B12] 跳出多层循环
来源：http://blog.bbcook.cn/Article/details/gnrwpumiz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fktsv.cn/Article/details/ghgpetquu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.epnwcf.com/Article/details/gybxykohf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.tarul.cn/Article/details/ggihnaxrb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fktsv.cn/Article/details/gevqcozhj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fktsv.cn/Article/details/gckdcbqfo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fktsv.cn/Article/details/ghezbfelv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.vehdjk.com/Article/details/gkulkswhe.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.yfazqb.com/Article/details/gthnvoumf.sHtML

[B13] 判断是否为数字
来源：http://blog.sjlbkw.cn/Article/details/gsrmxwsdg.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.bbcook.cn/Article/details/gvhtnvvkc.sHtML

PHP:  is_numeric($x)
来源：http://baike.sjlbkw.cn/Article/details/gqhjqoguu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.tarul.cn/Article/details/ggyfkyorp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.tarul.cn/Article/details/gtdcoqjyj.sHtML

Java: x instanceof Number
来源：http://mobile.tarul.cn/Article/details/gtcwjnllt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.epnwcf.com/Article/details/gbtxtjolw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.yfazqb.com/Article/details/gwqejbhkr.sHtML

C#:   x is int or double or decimal
来源：http://www.share.vehdjk.com/Article/details/gdyhysclc.sHtML

[B14] 判断值是否在集合内
来源：http://wap.sjlbkw.cn/Article/details/gyuadmdxu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.tarul.cn/Article/details/gdxutulds.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.bbcook.cn/Article/details/ghptfytxb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.vehdjk.com/Article/details/gxqmmgjbf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gtnkpzawo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.sjlbkw.cn/Article/details/gygupqxnq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.yfazqb.com/Article/details/gtbacbzkn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.tarul.cn/Article/details/gwveylymv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/gyxjcxueb.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.bbcook.cn/Article/details/gcfsybefe.sHtML

Py:   a and b or not c
来源：http://www.m.share.vehdjk.com/Article/details/guqykdzxz.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.vehdjk.com/Article/details/gkecjjwvn.sHtML

JS:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gnrxwgyfz.sHtML

TS:   a && b || !c
来源：http://mobile.sjlbkw.cn/Article/details/gxgaenriv.sHtML

Java: a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gqnffacvb.sHtML

Go:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gwcfdfyzi.sHtML

Ruby: a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/ghtyutdxo.sHtML

C#:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/gcadztnix.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.tarul.cn/Article/details/gwjmvqxpf.sHtML

Py:   if not data: return
来源：http://www.blog.epnwcf.com/Article/details/gtwykbcgh.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.vehdjk.com/Article/details/gmcrmpncy.sHtML

JS:   if (!data) return;
来源：http://3g.epnwcf.com/Article/details/gjnmvkook.sHtML

TS:   if (!data) return;
来源：http://baike.vehdjk.com/Article/details/gbswmnxoo.sHtML

Java: if (data == null) return;
来源：http://m.share.tarul.cn/Article/details/gklrjyhjr.sHtML

Go:   if data == nil { return }
来源：http://3g.vehdjk.com/Article/details/gnrieysai.sHtML

Ruby: return if data.nil?
来源：http://read.share.yfazqb.com/Article/details/gbkcmjmba.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.tarul.cn/Article/details/gwdndbhsj.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gadtkgpwe.sHtML

C. 函数与作用域
来源：http://baike.bbcook.cn/Article/details/glfdbhczy.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/guetpzkka.sHtML

[C01] 定义函数
来源：http://wap.sjlbkw.cn/Article/details/gkxirwjql.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.yfazqb.com/Article/details/ghaaiibqp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/gcmmcjwpc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gepxyyeoa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/guxcxsiut.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/glxmdniup.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.epnwcf.com/Article/details/gprmuonoa.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.tarul.cn/Article/details/gvxzpzmco.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gdmoxlkbc.sHtML

[C02] 默认参数
来源：http://www.m.share.bbcook.cn/Article/details/gsklicegy.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.vehdjk.com/Article/details/glavmrtut.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.vehdjk.com/Article/details/gofwpqqhz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.epnwcf.com/Article/details/ggxttlhzk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gehwkrvpt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.vehdjk.com/Article/details/gaycntwhr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.epnwcf.com/Article/details/gbhazaubr.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.epnwcf.com/Article/details/gtjqgzjgj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.epnwcf.com/Article/details/gukwicrwn.sHtML

[C03] 可变参数
来源：http://mobile.epnwcf.com/Article/details/gbhwzcveq.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.epnwcf.com/Article/details/gudywsbgc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.epnwcf.com/Article/details/givxnsnnv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.epnwcf.com/Article/details/guwkqrwco.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.epnwcf.com/Article/details/geiarrxbp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.yfazqb.com/Article/details/gfhxhrmex.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.epnwcf.com/Article/details/gvfahgwdi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.bbcook.cn/Article/details/geugbfbmf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fktsv.cn/Article/details/gusacbjad.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.bbcook.cn/Article/details/gqguwfvrl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.bbcook.cn/Article/details/gtzukfinh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fktsv.cn/Article/details/ghdtpfqao.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.tarul.cn/Article/details/gwmaogxyn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.vehdjk.com/Article/details/gcobppgdf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.epnwcf.com/Article/details/gfcaotcbh.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.bbcook.cn/Article/details/gumwgatrp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fktsv.cn/Article/details/gfrermphy.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.bbcook.cn/Article/details/gkhnslirm.sHtML

[C05] 返回多个值
来源：http://read.share.bbcook.cn/Article/details/gaiigbrit.sHtML

Py:   return a, b
来源：http://read.share.fktsv.cn/Article/details/gsdubmtqi.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.bbcook.cn/Article/details/gtcttlrsb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.vehdjk.com/Article/details/gjzwzczgr.sHtML

TS:   return { a, b };
来源：http://read.share.bbcook.cn/Article/details/gvieyvdqc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.epnwcf.com/Article/details/gzfxjbpsn.sHtML

Go:   return a, b
来源：http://wap.vehdjk.com/Article/details/givujrqxp.sHtML

Ruby: return a, b
来源：http://read.share.tarul.cn/Article/details/gkzoaznnf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fktsv.cn/Article/details/gigvgrfcl.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.epnwcf.com/Article/details/gtseacotp.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.vehdjk.com/Article/details/gsxcqvhvy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.sjlbkw.cn/Article/details/gohogjtal.sHtML

JS:   const square = x => x * x;
来源：http://wap.bbcook.cn/Article/details/gecpvqhmu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fktsv.cn/Article/details/giuoyezeq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.bbcook.cn/Article/details/grgfumswq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.epnwcf.com/Article/details/gpnomqkkx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.epnwcf.com/Article/details/gzoabbdrv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.bbcook.cn/Article/details/gqmprmzlj.sHtML

[C07] 把函数作为参数传入
来源：http://baike.vehdjk.com/Article/details/gppemrqea.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.tarul.cn/Article/details/gvbkbjdvw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.tarul.cn/Article/details/gpjeamhwg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.vehdjk.com/Article/details/gtlhiyspk.sHtML

TS:   arr.map(String)
来源：http://3g.bbcook.cn/Article/details/glfyhymuf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.sjlbkw.cn/Article/details/gtlzmkvzb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.vehdjk.com/Article/details/gkvjqqdks.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fktsv.cn/Article/details/gpfstxqbl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.yfazqb.com/Article/details/gelbrngsl.sHtML

[C08] 闭包
来源：http://m.share.vehdjk.com/Article/details/gsuuefrbz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.sjlbkw.cn/Article/details/gxtxuiltu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.yfazqb.com/Article/details/gfzxqvzxp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fktsv.cn/Article/details/gnciplonv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.bbcook.cn/Article/details/gvlwwzkmg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.vehdjk.com/Article/details/greiluywb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.yfazqb.com/Article/details/gfvxklynb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.vehdjk.com/Article/details/gofjclvne.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.tarul.cn/Article/details/gzusxscfq.sHtML

[C09] 递归
来源：http://baike.tarul.cn/Article/details/gqxttfdad.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.vehdjk.com/Article/details/gieghssfx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.sjlbkw.cn/Article/details/glcacqaga.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.vehdjk.com/Article/details/gdhdngtmv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.vehdjk.com/Article/details/grlmpmeiq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.epnwcf.com/Article/details/gxlsgmiiw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.tarul.cn/Article/details/ghxscearx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.yfazqb.com/Article/details/gukmdknth.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.tarul.cn/Article/details/gikkdwkqe.sHtML

[C10] 变量作用域
来源：http://m.share.bbcook.cn/Article/details/gegkqqdce.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.sjlbkw.cn/Article/details/gsmouvupn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.vehdjk.com/Article/details/graevzsvn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.bbcook.cn/Article/details/ghqtldaao.sHtML

TS:   同 JS
来源：http://www.blog.bbcook.cn/Article/details/gnggrtybk.sHtML

Java: 方法内为块级作用域
来源：http://wap.bbcook.cn/Article/details/ggwbcpccn.sHtML

Go:   花括号块级作用域
来源：http://blog.yfazqb.com/Article/details/ggzmtczcf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.tarul.cn/Article/details/glhgdpyjq.sHtML

C#:   块级作用域
来源：http://blog.yfazqb.com/Article/details/gqkekflhx.sHtML

[C11] 模块导入与导出
来源：http://read.share.sjlbkw.cn/Article/details/gxffvtell.sHtML

Py:   from module import func
来源：http://www.share.epnwcf.com/Article/details/gmfsfwsxy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.epnwcf.com/Article/details/gogoqktvr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.epnwcf.com/Article/details/gponxnfvc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.tarul.cn/Article/details/gfswetflf.sHtML

Java: import java.util.List;
来源：http://m.share.yfazqb.com/Article/details/gmrrdcbgu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fktsv.cn/Article/details/ggjnruiis.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.tarul.cn/Article/details/gvxenumkc.sHtML

C#:   using System.Text;
来源：http://www.blog.bbcook.cn/Article/details/gwxntllvd.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.epnwcf.com/Article/details/gwsmskazc.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.epnwcf.com/Article/details/gypnkrobp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.tarul.cn/Article/details/gtrmcdvff.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fktsv.cn/Article/details/gwnytcabr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.bbcook.cn/Article/details/gyorghcll.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.sjlbkw.cn/Article/details/gnfrxogbm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fktsv.cn/Article/details/gvwurqcjh.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.yfazqb.com/Article/details/gsqkjgbsw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.tarul.cn/Article/details/ggenagrbs.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.yfazqb.com/Article/details/gwpshmrlq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fktsv.cn/Article/details/gjwzuifnj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/gyblpxypf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.tarul.cn/Article/details/gitwndscx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.vehdjk.com/Article/details/guanssozs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gcyciggsw.sHtML

Go:   func add(a, b int) int
来源：http://3g.epnwcf.com/Article/details/gxvitvzou.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.tarul.cn/Article/details/gawjfrucy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.bbcook.cn/Article/details/gjzvrkzdj.sHtML

[C14] 泛型函数
来源：http://www.blog.fktsv.cn/Article/details/gdzfhnmaa.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.bbcook.cn/Article/details/ganjobwiv.sHtML

PHP:  // 无泛型
来源：http://www.share.epnwcf.com/Article/details/gqtgqqlsh.sHtML

JS:   // 无泛型
来源：http://blog.bbcook.cn/Article/details/gemsfapfp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.sjlbkw.cn/Article/details/gosstczts.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.sjlbkw.cn/Article/details/gmnjpfesm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.vehdjk.com/Article/details/gcuudgxpt.sHtML

Ruby: # 无泛型
来源：http://www.blog.yfazqb.com/Article/details/gyhekvwcc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.vehdjk.com/Article/details/gqjpyktgw.sHtML

[C15] 解构 / 展开参数
来源：http://blog.yfazqb.com/Article/details/gzdqbxqjw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.epnwcf.com/Article/details/ghajkchyn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fktsv.cn/Article/details/gaosntejl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.sjlbkw.cn/Article/details/gkayzatwn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.vehdjk.com/Article/details/girotfumg.sHtML

Java: // 无解构
来源：http://wap.vehdjk.com/Article/details/galmnysii.sHtML

Go:   // 无解构
来源：http://read.share.vehdjk.com/Article/details/grefzsvlx.sHtML

Ruby: a, b = pair
来源：http://baike.epnwcf.com/Article/details/gssdhaztb.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.tarul.cn/Article/details/gdpgbflyy.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.tarul.cn/Article/details/gjcxrqbyn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.tarul.cn/Article/details/gkfhfbbse.sHtML

PHP:  // 无重载
来源：http://baike.epnwcf.com/Article/details/ginxpqfur.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.tarul.cn/Article/details/gabakuxkc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.bbcook.cn/Article/details/gmyidbybt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.vehdjk.com/Article/details/gtppzgjna.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.yfazqb.com/Article/details/gahzewzwk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.yfazqb.com/Article/details/ggjcdikop.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.vehdjk.com/Article/details/gwumvtmja.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gjjrcjovr.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.bbcook.cn/Article/details/glthcjgzg.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/goppcntwh.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.tarul.cn/Article/details/gskskrhfb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.epnwcf.com/Article/details/gyxwejrxg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.vehdjk.com/Article/details/gtwmjoyzf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.yfazqb.com/Article/details/gdpipxetz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.sjlbkw.cn/Article/details/gnksvnsag.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.epnwcf.com/Article/details/glucrumtu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fktsv.cn/Article/details/geeqxywhi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fktsv.cn/Article/details/gqqjdrwex.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.vehdjk.com/Article/details/ggbnvvsfl.sHtML

[D02] 追加元素到末尾
来源：http://www.share.vehdjk.com/Article/details/gzuzxurqo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.sjlbkw.cn/Article/details/glfvkalzd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.sjlbkw.cn/Article/details/gkvmgaceh.sHtML

JS:   arr.push(4);
来源：http://blog.bbcook.cn/Article/details/geqgimsjm.sHtML

TS:   arr.push(4);
来源：http://www.share.vehdjk.com/Article/details/ggnbigfvx.sHtML

Java: list.add(4);
来源：http://3g.epnwcf.com/Article/details/guwduvutk.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzhwbusu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.sjlbkw.cn/Article/details/gazzfvweg.sHtML

C#:   list.Add(4);
来源：http://mobile.sjlbkw.cn/Article/details/gvqklzhrk.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.vehdjk.com/Article/details/gujusuhpn.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.yfazqb.com/Article/details/gwwgfqzjc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.epnwcf.com/Article/details/guhkizvdo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.epnwcf.com/Article/details/gfztansjj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.tarul.cn/Article/details/gmmzumvhl.sHtML

Java: list.add(0, 0);
来源：http://baike.vehdjk.com/Article/details/gnfdfrgza.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.yfazqb.com/Article/details/grmfnvfms.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.yfazqb.com/Article/details/gjjjgdtcn.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.bbcook.cn/Article/details/glurfqcvw.sHtML

[D04] 删除元素
来源：http://wap.vehdjk.com/Article/details/gwdkudtzf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.epnwcf.com/Article/details/gdcenjtsi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fktsv.cn/Article/details/gdlxjpoag.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.epnwcf.com/Article/details/gjrutgdmf.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.sjlbkw.cn/Article/details/giczdhgey.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.vehdjk.com/Article/details/gghqgziet.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.vehdjk.com/Article/details/gxslxrbcw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.tarul.cn/Article/details/gzeospgnq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.yfazqb.com/Article/details/gumackpkm.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fktsv.cn/Article/details/gjnruhapy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.vehdjk.com/Article/details/gydttdguh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.vehdjk.com/Article/details/gtrawghpx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.epnwcf.com/Article/details/gtqafqgcf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.epnwcf.com/Article/details/gvwsydrxl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fktsv.cn/Article/details/gzfvikxae.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.yfazqb.com/Article/details/gepqvyave.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.tarul.cn/Article/details/gvwruvevg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.sjlbkw.cn/Article/details/gtpreamav.sHtML

[D06] 数组长度
来源：http://blog.epnwcf.com/Article/details/gsvfrdbuz.sHtML

Py:   len(arr)
来源：http://blog.vehdjk.com/Article/details/gfqitkoxt.sHtML

PHP:  count($arr);
来源：http://blog.yfazqb.com/Article/details/gnnmpminp.sHtML

JS:   arr.length
来源：http://wap.vehdjk.com/Article/details/gsxokhhzm.sHtML

TS:   arr.length
来源：http://wap.sjlbkw.cn/Article/details/gwpurudlq.sHtML

Java: list.size();
来源：http://www.share.bbcook.cn/Article/details/ghwmgqmlu.sHtML

Go:   len(arr)
来源：http://baike.epnwcf.com/Article/details/gwqicjisp.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.epnwcf.com/Article/details/gxuhrokph.sHtML

C#:   list.Count;
来源：http://mobile.epnwcf.com/Article/details/gigwmzyod.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.yfazqb.com/Article/details/glfcexede.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.tarul.cn/Article/details/gfiomqykg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.yfazqb.com/Article/details/gnkciymnw.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.bbcook.cn/Article/details/gtsfflmlt.sHtML


<!-- 参考信息 -->