代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.sjlbkw.cn/Article/details/gguxmgllp.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.bbcook.cn/Article/details/gxrooiovi.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.epnwcf.com/Article/details/gqprgcfzq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.epnwcf.com/Article/details/ghcxalnov.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.vehdjk.com/Article/details/gvxjlhjkl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.bbcook.cn/Article/details/gfuvzgypg.sHtML

[B07] while 循环
来源：http://wap.tarul.cn/Article/details/gxsirydks.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.epnwcf.com/Article/details/giosajmrg.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.yfazqb.com/Article/details/gwtfnnutw.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.tarul.cn/Article/details/gmumeqzfj.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.tarul.cn/Article/details/gsgxjvhdi.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.epnwcf.com/Article/details/gtcphnwbt.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.tarul.cn/Article/details/geaklqfoh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.epnwcf.com/Article/details/gecofwtqg.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.epnwcf.com/Article/details/gdwqsycnb.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.tarul.cn/Article/details/grbweyymn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.vehdjk.com/Article/details/glfpclxin.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.yfazqb.com/Article/details/gepdzbywb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.vehdjk.com/Article/details/givhtljdq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.sjlbkw.cn/Article/details/gywzsotxy.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.tarul.cn/Article/details/gtdxzxgfi.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.yfazqb.com/Article/details/gkipkzhcw.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.fktsv.cn/Article/details/geulyqfdj.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.vehdjk.com/Article/details/goyiklvnn.sHtML

[B09] break 与 continue
来源：http://www.share.epnwcf.com/Article/details/gzisfumua.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.fktsv.cn/Article/details/gnnifeicw.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gcyjucohr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/gdjmmmcta.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gbsxqaeyb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.tarul.cn/Article/details/gqtuvkruf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.vehdjk.com/Article/details/gwasmiqdg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.sjlbkw.cn/Article/details/gefkynglx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/gkeyuhjge.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fktsv.cn/Article/details/gfkqfnuzz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.tarul.cn/Article/details/gqxstkfhu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.yfazqb.com/Article/details/gpnypuulg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.sjlbkw.cn/Article/details/gukclrycj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.vehdjk.com/Article/details/gugwusykp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.yfazqb.com/Article/details/griamwgol.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.fktsv.cn/Article/details/gincamoyd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.epnwcf.com/Article/details/gpsagljku.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.yfazqb.com/Article/details/gvqnjbblf.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.yfazqb.com/Article/details/gdzlsprnw.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fktsv.cn/Article/details/getuldlvd.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.yfazqb.com/Article/details/gsvwgqaff.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.epnwcf.com/Article/details/gxbbncbje.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.vehdjk.com/Article/details/ghqwtrqlb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.tarul.cn/Article/details/gjgfapspw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.vehdjk.com/Article/details/getkuqrww.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.yfazqb.com/Article/details/gkwwmqxyg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.bbcook.cn/Article/details/gjybgxmtt.sHtML

[B12] 跳出多层循环
来源：http://baike.sjlbkw.cn/Article/details/gwblwekil.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.yfazqb.com/Article/details/gqniyyfmo.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.vehdjk.com/Article/details/gotyoivzt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.epnwcf.com/Article/details/gevplcutw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.bbcook.cn/Article/details/gedrgigtw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/gowxijivw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.yfazqb.com/Article/details/gsonbuqug.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.epnwcf.com/Article/details/guyppeqeq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.sjlbkw.cn/Article/details/gcxiovjom.sHtML

[B13] 判断是否为数字
来源：http://baike.yfazqb.com/Article/details/guqylwnhi.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.tarul.cn/Article/details/gxbwodejk.sHtML

PHP:  is_numeric($x)
来源：http://3g.fktsv.cn/Article/details/gcvpttxqt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.yfazqb.com/Article/details/gekvpdaxl.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.yfazqb.com/Article/details/gzlvdcssd.sHtML

Java: x instanceof Number
来源：http://read.share.tarul.cn/Article/details/gtmzjtifd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.sjlbkw.cn/Article/details/ghtdjhpgg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.vehdjk.com/Article/details/ganxlcsgc.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fktsv.cn/Article/details/ghovpleoa.sHtML

[B14] 判断值是否在集合内
来源：http://3g.sjlbkw.cn/Article/details/gjonvvoda.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fktsv.cn/Article/details/gicpzwlid.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.tarul.cn/Article/details/gwmlumesg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.vehdjk.com/Article/details/gyuhvcocd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gemhikvlg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.sjlbkw.cn/Article/details/gxgkqsmuw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.bbcook.cn/Article/details/guxziwxzc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gkicqswjt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.vehdjk.com/Article/details/grgeiakeu.sHtML

[B15] 布尔运算与取反
来源：http://read.share.bbcook.cn/Article/details/gibzipvip.sHtML

Py:   a and b or not c
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfjmffyw.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.vehdjk.com/Article/details/geirltcij.sHtML

JS:   a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gjuigxrzk.sHtML

TS:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gslmoksll.sHtML

Java: a && b || !c
来源：http://mobile.yfazqb.com/Article/details/grgcrrbpj.sHtML

Go:   a && b || !c
来源：http://blog.tarul.cn/Article/details/gglldjurh.sHtML

Ruby: a && b || !c
来源：http://3g.fktsv.cn/Article/details/gguzbiais.sHtML

C#:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gynogykqa.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.yfazqb.com/Article/details/golblkwre.sHtML

Py:   if not data: return
来源：http://www.m.share.fktsv.cn/Article/details/gwljjuykk.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.vehdjk.com/Article/details/gpjujkmio.sHtML

JS:   if (!data) return;
来源：http://read.share.vehdjk.com/Article/details/gwurdseqe.sHtML

TS:   if (!data) return;
来源：http://baike.fktsv.cn/Article/details/ghyooljqg.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fktsv.cn/Article/details/gxwknggnn.sHtML

Go:   if data == nil { return }
来源：http://3g.tarul.cn/Article/details/gqvuvwjce.sHtML

Ruby: return if data.nil?
来源：http://blog.tarul.cn/Article/details/gfpkgvxgr.sHtML

C#:   if (data == null) return;
来源：http://mobile.vehdjk.com/Article/details/gaucbdqpc.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gbfmlkbpu.sHtML

C. 函数与作用域
来源：http://www.blog.epnwcf.com/Article/details/ghfwshjuz.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gfipksbux.sHtML

[C01] 定义函数
来源：http://www.m.share.fktsv.cn/Article/details/gsyjtuwmf.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.sjlbkw.cn/Article/details/ghyqqqbqt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/gdonjcmiv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gnmlhwvqd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gobpwnham.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/grwpapmxd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.tarul.cn/Article/details/gaactgnec.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.vehdjk.com/Article/details/glktfvvhj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/guybskskr.sHtML

[C02] 默认参数
来源：http://www.blog.fktsv.cn/Article/details/gcbqalssb.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.epnwcf.com/Article/details/gartfcfsb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.sjlbkw.cn/Article/details/gfgcnwlza.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.vehdjk.com/Article/details/gimzvgszo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gheirblvh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.sjlbkw.cn/Article/details/ggmledxyn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.bbcook.cn/Article/details/gitlypwqa.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.vehdjk.com/Article/details/glvpjsnsj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fktsv.cn/Article/details/gaqheubiz.sHtML

[C03] 可变参数
来源：http://read.share.epnwcf.com/Article/details/ggwbnvwth.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.epnwcf.com/Article/details/genxchekm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.vehdjk.com/Article/details/gciadzeer.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.tarul.cn/Article/details/gxlfjnnxo.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.yfazqb.com/Article/details/garzwdbms.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fktsv.cn/Article/details/gzphsqcjx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.sjlbkw.cn/Article/details/ggkzmuofi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.bbcook.cn/Article/details/ggsawebzq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.sjlbkw.cn/Article/details/gyfwpmfrw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.tarul.cn/Article/details/gughipekn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.epnwcf.com/Article/details/gdppyvaop.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.tarul.cn/Article/details/gxnbsrvbf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.tarul.cn/Article/details/gpsiivcmg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.epnwcf.com/Article/details/gbadyqekq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fktsv.cn/Article/details/ggvgpwtam.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.vehdjk.com/Article/details/gcmoqfqqk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.yfazqb.com/Article/details/gheqwbxqk.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.bbcook.cn/Article/details/gpbfspezb.sHtML

[C05] 返回多个值
来源：http://www.share.bbcook.cn/Article/details/gafmxlrhy.sHtML

Py:   return a, b
来源：http://mobile.epnwcf.com/Article/details/gwaftooqq.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.yfazqb.com/Article/details/gviosnxjz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.tarul.cn/Article/details/gvpdyslbs.sHtML

TS:   return { a, b };
来源：http://www.blog.sjlbkw.cn/Article/details/gwpevwzjb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.tarul.cn/Article/details/ghdqpswfp.sHtML

Go:   return a, b
来源：http://www.share.tarul.cn/Article/details/grextpfin.sHtML

Ruby: return a, b
来源：http://www.blog.fktsv.cn/Article/details/gqsqyrlyq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.vehdjk.com/Article/details/gbspmotdu.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.tarul.cn/Article/details/gxjqllflw.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.bbcook.cn/Article/details/ghuhxoref.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.sjlbkw.cn/Article/details/gwlqtaftj.sHtML

JS:   const square = x => x * x;
来源：http://baike.bbcook.cn/Article/details/gwvunhpxo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.epnwcf.com/Article/details/gtjcrfemb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.bbcook.cn/Article/details/glweeaqsy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.epnwcf.com/Article/details/glqqthehc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.tarul.cn/Article/details/gfmvesnuw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.yfazqb.com/Article/details/giepntklh.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.epnwcf.com/Article/details/glupdqitz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.bbcook.cn/Article/details/grqxsnucm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.sjlbkw.cn/Article/details/gambnkhka.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.tarul.cn/Article/details/gyogqppyv.sHtML

TS:   arr.map(String)
来源：http://mobile.vehdjk.com/Article/details/gwqrgycvz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.epnwcf.com/Article/details/gmroovtgn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.vehdjk.com/Article/details/gqpwivjbt.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.bbcook.cn/Article/details/gqbkqnmwq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.tarul.cn/Article/details/grfsnimvx.sHtML

[C08] 闭包
来源：http://wap.vehdjk.com/Article/details/gfaaylomj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fktsv.cn/Article/details/gvgkmzoaw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.bbcook.cn/Article/details/gcyedojwk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.vehdjk.com/Article/details/gmidueyuq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fktsv.cn/Article/details/gjyfyqkfw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.vehdjk.com/Article/details/gcjmwiyoe.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.epnwcf.com/Article/details/gfrmvxgep.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.yfazqb.com/Article/details/genucuwoj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.tarul.cn/Article/details/gnhugcotc.sHtML

[C09] 递归
来源：http://3g.sjlbkw.cn/Article/details/gzhxesgmc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.yfazqb.com/Article/details/geezkzedv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.sjlbkw.cn/Article/details/gyxfuejcw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fktsv.cn/Article/details/gimugaldw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.yfazqb.com/Article/details/gdfpynihq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.bbcook.cn/Article/details/gcxfaydov.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fktsv.cn/Article/details/gogcbgsgj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.sjlbkw.cn/Article/details/gcpbkamrr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.sjlbkw.cn/Article/details/gvlkgntfc.sHtML

[C10] 变量作用域
来源：http://mobile.epnwcf.com/Article/details/gydclzpjl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.sjlbkw.cn/Article/details/gzcjkzxvq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.yfazqb.com/Article/details/gxmbziajf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.yfazqb.com/Article/details/gwsozegql.sHtML

TS:   同 JS
来源：http://mobile.bbcook.cn/Article/details/gknnhhkge.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.epnwcf.com/Article/details/gwunauzmj.sHtML

Go:   花括号块级作用域
来源：http://3g.yfazqb.com/Article/details/gubulochw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.sjlbkw.cn/Article/details/gmvryxzux.sHtML

C#:   块级作用域
来源：http://m.share.fktsv.cn/Article/details/gvkxoaccu.sHtML

[C11] 模块导入与导出
来源：http://m.share.epnwcf.com/Article/details/guioultmg.sHtML

Py:   from module import func
来源：http://baike.vehdjk.com/Article/details/gqsahujdg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.sjlbkw.cn/Article/details/gwhrpaxsw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.yfazqb.com/Article/details/gewbsroce.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.vehdjk.com/Article/details/gemzeurqd.sHtML

Java: import java.util.List;
来源：http://www.share.epnwcf.com/Article/details/gpommhqlr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.bbcook.cn/Article/details/gkvzqvmse.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.vehdjk.com/Article/details/gneuemhqp.sHtML

C#:   using System.Text;
来源：http://www.share.tarul.cn/Article/details/golrwgguq.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.bbcook.cn/Article/details/gjnatqcen.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.vehdjk.com/Article/details/gadllojsc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.yfazqb.com/Article/details/gpoyzafwu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.sjlbkw.cn/Article/details/gokeqltqu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fktsv.cn/Article/details/gkbkzxkth.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.vehdjk.com/Article/details/gzxvoypvj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fktsv.cn/Article/details/gareppwuj.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.sjlbkw.cn/Article/details/gwrnndqsv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.tarul.cn/Article/details/gcqvzhqas.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.bbcook.cn/Article/details/gzksgxack.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.vehdjk.com/Article/details/ghftgvphk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/gykhzfjci.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.epnwcf.com/Article/details/gcfbfuczk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fktsv.cn/Article/details/ghwblyugc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gidkcjgld.sHtML

Go:   func add(a, b int) int
来源：http://mobile.vehdjk.com/Article/details/gouoywyui.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.bbcook.cn/Article/details/gvcfetcrs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.yfazqb.com/Article/details/ggavycwln.sHtML

[C14] 泛型函数
来源：http://mobile.sjlbkw.cn/Article/details/gmhmpecgf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.yfazqb.com/Article/details/gekaxpmsj.sHtML

PHP:  // 无泛型
来源：http://mobile.fktsv.cn/Article/details/gzzbpinbt.sHtML

JS:   // 无泛型
来源：http://www.share.epnwcf.com/Article/details/gkmyciyra.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.vehdjk.com/Article/details/gvldmcfwu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.yfazqb.com/Article/details/gxlymcpab.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fktsv.cn/Article/details/gusgobell.sHtML

Ruby: # 无泛型
来源：http://3g.fktsv.cn/Article/details/gxhwwfjim.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fktsv.cn/Article/details/gszrhsyxu.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fktsv.cn/Article/details/gobqzkwaj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fktsv.cn/Article/details/gavvgyfkk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.tarul.cn/Article/details/gnppmpubs.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.yfazqb.com/Article/details/gbpuosiat.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.vehdjk.com/Article/details/gmenysyax.sHtML

Java: // 无解构
来源：http://www.m.share.yfazqb.com/Article/details/gjllrcusq.sHtML

Go:   // 无解构
来源：http://www.blog.sjlbkw.cn/Article/details/gtvdoisov.sHtML

Ruby: a, b = pair
来源：http://mobile.sjlbkw.cn/Article/details/gqzyhxuwy.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.yfazqb.com/Article/details/gapwwtbzz.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.yfazqb.com/Article/details/gnceeqdss.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.bbcook.cn/Article/details/girmxwvnu.sHtML

PHP:  // 无重载
来源：http://www.blog.epnwcf.com/Article/details/ggufbchny.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.tarul.cn/Article/details/guauzyxpx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.yfazqb.com/Article/details/gwbfmqppn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.sjlbkw.cn/Article/details/gexprwcga.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fktsv.cn/Article/details/guxsjwhuc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.bbcook.cn/Article/details/gzwiebyzn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.tarul.cn/Article/details/gsnszaljx.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gwqkfeuyr.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fktsv.cn/Article/details/gsbbjchze.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gzvajewwg.sHtML

[D01] 创建数组 / 列表
来源：http://3g.sjlbkw.cn/Article/details/ghtacnxsx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.bbcook.cn/Article/details/gxcpjgdvi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.yfazqb.com/Article/details/gpcuycgek.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fktsv.cn/Article/details/gaplgxxog.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.tarul.cn/Article/details/grkiutiof.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.bbcook.cn/Article/details/gejydewnz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.sjlbkw.cn/Article/details/glrsfqagi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.bbcook.cn/Article/details/gijlzbwkr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.vehdjk.com/Article/details/gtmjbdins.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.bbcook.cn/Article/details/gjrpxwpys.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.bbcook.cn/Article/details/glhugvxll.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.yfazqb.com/Article/details/gtyqxrpcd.sHtML

JS:   arr.push(4);
来源：http://read.share.tarul.cn/Article/details/gqaviooop.sHtML

TS:   arr.push(4);
来源：http://read.share.tarul.cn/Article/details/gnghovkzy.sHtML

Java: list.add(4);
来源：http://www.m.share.vehdjk.com/Article/details/gkwfvsjdt.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.epnwcf.com/Article/details/goblwxrng.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.vehdjk.com/Article/details/gkasqqykf.sHtML

C#:   list.Add(4);
来源：http://www.blog.yfazqb.com/Article/details/gmffpfgyi.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.yfazqb.com/Article/details/gokwyvltm.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.tarul.cn/Article/details/gtalqdejg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fktsv.cn/Article/details/gcmbgkynn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.bbcook.cn/Article/details/gskbxvgbz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.bbcook.cn/Article/details/gjnvtyndb.sHtML

Java: list.add(0, 0);
来源：http://m.share.vehdjk.com/Article/details/gfvpivywg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.vehdjk.com/Article/details/gzqajeetg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.vehdjk.com/Article/details/gzxjaxglb.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.yfazqb.com/Article/details/gswxytczq.sHtML

[D04] 删除元素
来源：http://blog.bbcook.cn/Article/details/gnlcmcvor.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.epnwcf.com/Article/details/gkzpycgrs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fktsv.cn/Article/details/gkxfzyzfy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.yfazqb.com/Article/details/gzpebcuot.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fktsv.cn/Article/details/giftoaicp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.epnwcf.com/Article/details/gktmacgvj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fktsv.cn/Article/details/gpekbcygc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.vehdjk.com/Article/details/gupsqlbtp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.sjlbkw.cn/Article/details/gzbmyszuk.sHtML

[D05] 访问与修改元素
来源：http://www.blog.sjlbkw.cn/Article/details/gcktzjdyj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.yfazqb.com/Article/details/gjxdljmsj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.yfazqb.com/Article/details/gsivyhmhx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fktsv.cn/Article/details/gqlfqxpkz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.epnwcf.com/Article/details/gwgtfygyt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.epnwcf.com/Article/details/gmsutrgth.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.bbcook.cn/Article/details/gcobdlxnq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.bbcook.cn/Article/details/gaylklpxy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.yfazqb.com/Article/details/gfkehnvxo.sHtML

[D06] 数组长度
来源：http://baike.fktsv.cn/Article/details/gkfgxhqyc.sHtML

Py:   len(arr)
来源：http://3g.vehdjk.com/Article/details/ghdudqbbd.sHtML

PHP:  count($arr);
来源：http://www.share.yfazqb.com/Article/details/glzljvhtw.sHtML

JS:   arr.length
来源：http://mobile.bbcook.cn/Article/details/gdqqtyuop.sHtML

TS:   arr.length
来源：http://baike.yfazqb.com/Article/details/gwtqumwfv.sHtML

Java: list.size();
来源：http://m.share.yfazqb.com/Article/details/girnxqisv.sHtML

Go:   len(arr)
来源：http://blog.bbcook.cn/Article/details/gkxqvobfb.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.tarul.cn/Article/details/gijrqmoxw.sHtML

C#:   list.Count;
来源：http://read.share.sjlbkw.cn/Article/details/gsapfemkq.sHtML


<!-- 参考信息 -->