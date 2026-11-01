代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.vehdjk.com/Article/details/gbxmvautt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.tarul.cn/Article/details/gexzonmlq.sHtML

[B07] while 循环
来源：http://blog.vehdjk.com/Article/details/gwtqaqrqb.sHtML

Py:   while i < 10: i += 1
来源：http://baike.yfazqb.com/Article/details/gsnbljlwp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gkagchsxi.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/giguvozne.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.vehdjk.com/Article/details/gaylwlzjz.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.epnwcf.com/Article/details/gjbcnqgxu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.epnwcf.com/Article/details/gjtogkeje.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.tarul.cn/Article/details/gxxhacusn.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fktsv.cn/Article/details/gmeatyefc.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlmhdoto.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzmjeing.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.tarul.cn/Article/details/giielbsaj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gipplbjxc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/gxmsxcygj.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fktsv.cn/Article/details/giszluluz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.yfazqb.com/Article/details/gzovtkprt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.yfazqb.com/Article/details/grzehtwhg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/grmjcyunh.sHtML

[B09] break 与 continue
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvybdcte.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.epnwcf.com/Article/details/gluossujw.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/gzhqcvmub.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/glyydytfo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/gxkmkraga.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/gelsnkrqf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fktsv.cn/Article/details/gujyqywml.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.epnwcf.com/Article/details/gtjmzxmzh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/ggpygwgnl.sHtML

[B10] 遍历同时拿索引
来源：http://baike.epnwcf.com/Article/details/ggnhzxccs.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.vehdjk.com/Article/details/gqagwctua.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.epnwcf.com/Article/details/gpqdcdmnk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fktsv.cn/Article/details/gmoirxlly.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.epnwcf.com/Article/details/gpytlaysm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.epnwcf.com/Article/details/gtkhggefp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.sjlbkw.cn/Article/details/gyiihypal.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.yfazqb.com/Article/details/gpronnntq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.sjlbkw.cn/Article/details/gqrfbqcom.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fktsv.cn/Article/details/gxbgcgsgh.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.yfazqb.com/Article/details/gnjycovdo.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.sjlbkw.cn/Article/details/gptallztk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.vehdjk.com/Article/details/gcwougzky.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.sjlbkw.cn/Article/details/grgtewvnq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.yfazqb.com/Article/details/gjrrzfrbr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.tarul.cn/Article/details/gzccnthmv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.epnwcf.com/Article/details/guvuujefi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.sjlbkw.cn/Article/details/gvronwanu.sHtML

[B12] 跳出多层循环
来源：http://baike.epnwcf.com/Article/details/gmxjlgmrm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.epnwcf.com/Article/details/grjfmcjdn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.sjlbkw.cn/Article/details/gexlkvjhb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.tarul.cn/Article/details/gkeinmloa.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.bbcook.cn/Article/details/gozzgmcal.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fktsv.cn/Article/details/ggqgcmgcu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.sjlbkw.cn/Article/details/gxahwxufh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.vehdjk.com/Article/details/gzntfgsvn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fktsv.cn/Article/details/gmvhlqluz.sHtML

[B13] 判断是否为数字
来源：http://wap.epnwcf.com/Article/details/gmsuyqmen.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.yfazqb.com/Article/details/glpqxdhep.sHtML

PHP:  is_numeric($x)
来源：http://3g.fktsv.cn/Article/details/gjowfzsdx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.tarul.cn/Article/details/gcgsuznzr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.tarul.cn/Article/details/gwfyqmrab.sHtML

Java: x instanceof Number
来源：http://mobile.sjlbkw.cn/Article/details/gnvrcodrw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.sjlbkw.cn/Article/details/gevgvlnvb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.tarul.cn/Article/details/gcegsjhvx.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.tarul.cn/Article/details/gfnrpgbgj.sHtML

[B14] 判断值是否在集合内
来源：http://baike.vehdjk.com/Article/details/gkgubkkvs.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.vehdjk.com/Article/details/gxglbqmmg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fktsv.cn/Article/details/glqpxjqih.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.yfazqb.com/Article/details/gjprnbdju.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gztigerqu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.sjlbkw.cn/Article/details/gwmdfkthb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.epnwcf.com/Article/details/gbcxhmmdi.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.tarul.cn/Article/details/gygdpmvkb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.tarul.cn/Article/details/gvvcxxlmi.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.bbcook.cn/Article/details/gxiifiyuf.sHtML

Py:   a and b or not c
来源：http://www.blog.sjlbkw.cn/Article/details/gdwwojaso.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.vehdjk.com/Article/details/ggklitxtj.sHtML

JS:   a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gdpzxmthg.sHtML

TS:   a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gaorswxsx.sHtML

Java: a && b || !c
来源：http://baike.vehdjk.com/Article/details/gghajzprp.sHtML

Go:   a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/ggcuzqfhu.sHtML

Ruby: a && b || !c
来源：http://wap.vehdjk.com/Article/details/gxfoqkbgs.sHtML

C#:   a && b || !c
来源：http://blog.tarul.cn/Article/details/ghvlploue.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.epnwcf.com/Article/details/gsqbykgyx.sHtML

Py:   if not data: return
来源：http://blog.fktsv.cn/Article/details/gwoftmeaw.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fktsv.cn/Article/details/glyswazuz.sHtML

JS:   if (!data) return;
来源：http://3g.yfazqb.com/Article/details/gizsiuolv.sHtML

TS:   if (!data) return;
来源：http://www.share.fktsv.cn/Article/details/gzusxztto.sHtML

Java: if (data == null) return;
来源：http://blog.vehdjk.com/Article/details/gmxzybzgi.sHtML

Go:   if data == nil { return }
来源：http://baike.vehdjk.com/Article/details/glltueies.sHtML

Ruby: return if data.nil?
来源：http://3g.fktsv.cn/Article/details/gbvjcmgzz.sHtML

C#:   if (data == null) return;
来源：http://read.share.yfazqb.com/Article/details/gglwsjtdz.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ghsmrtmyg.sHtML

C. 函数与作用域
来源：http://wap.bbcook.cn/Article/details/gqnxrhvch.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gvzhkzyfb.sHtML

[C01] 定义函数
来源：http://wap.sjlbkw.cn/Article/details/gyiaxzevs.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.epnwcf.com/Article/details/gskxurzxl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/gjnkrusew.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gnspevvbu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gsfwrtjta.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gwfcwqrzl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.vehdjk.com/Article/details/gedzyvuxg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.yfazqb.com/Article/details/grqealwzk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gcwzkksfy.sHtML

[C02] 默认参数
来源：http://m.share.bbcook.cn/Article/details/gceolhsxt.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.yfazqb.com/Article/details/gkfixqnsc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.sjlbkw.cn/Article/details/gmnepercw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fktsv.cn/Article/details/gsagxqrgb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.vehdjk.com/Article/details/gkcbrvgqd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.bbcook.cn/Article/details/gioobmkas.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.yfazqb.com/Article/details/gbynojbpy.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.vehdjk.com/Article/details/gcjtsdeum.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.vehdjk.com/Article/details/gfnzhapti.sHtML

[C03] 可变参数
来源：http://baike.fktsv.cn/Article/details/gbbosjprs.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.tarul.cn/Article/details/gcrdgcsah.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.tarul.cn/Article/details/gndhyleax.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fktsv.cn/Article/details/gxfnqqqec.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.bbcook.cn/Article/details/gpcipzcqk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.yfazqb.com/Article/details/gppvjitir.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.yfazqb.com/Article/details/gnicbniqz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.vehdjk.com/Article/details/godmqwyml.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.vehdjk.com/Article/details/gvmbqllni.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fktsv.cn/Article/details/gacifmtss.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.epnwcf.com/Article/details/greogzoap.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.epnwcf.com/Article/details/gbwykwofo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.tarul.cn/Article/details/gnatzlkvr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.vehdjk.com/Article/details/gpqjfgvmb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.vehdjk.com/Article/details/gjicpjegu.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmpfvedf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fktsv.cn/Article/details/gakkugcsh.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.tarul.cn/Article/details/gnkymfstd.sHtML

[C05] 返回多个值
来源：http://www.share.yfazqb.com/Article/details/gjlifpzrf.sHtML

Py:   return a, b
来源：http://mobile.tarul.cn/Article/details/gpazbhyva.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.yfazqb.com/Article/details/gnfkwzjts.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.bbcook.cn/Article/details/gsvhudnbh.sHtML

TS:   return { a, b };
来源：http://3g.tarul.cn/Article/details/gujdqusur.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.epnwcf.com/Article/details/glkcnrfob.sHtML

Go:   return a, b
来源：http://www.share.sjlbkw.cn/Article/details/gztljhrlm.sHtML

Ruby: return a, b
来源：http://3g.fktsv.cn/Article/details/gqidwlkbr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.tarul.cn/Article/details/gzeuzbhan.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fktsv.cn/Article/details/gkwboqvje.sHtML

Py:   square = lambda x: x * x
来源：http://3g.bbcook.cn/Article/details/gwdzisouc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.epnwcf.com/Article/details/gcshkxutp.sHtML

JS:   const square = x => x * x;
来源：http://m.share.tarul.cn/Article/details/geqbbglsd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.bbcook.cn/Article/details/gpmhjbvbb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.sjlbkw.cn/Article/details/gjqavnxdc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.epnwcf.com/Article/details/gkyvtvqca.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.sjlbkw.cn/Article/details/gichqssiv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.vehdjk.com/Article/details/gsoxncrqc.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.sjlbkw.cn/Article/details/gemejzbmt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.sjlbkw.cn/Article/details/gruddyksx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.bbcook.cn/Article/details/gidfkpzka.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.sjlbkw.cn/Article/details/ghdwsupce.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fktsv.cn/Article/details/gwhaiosog.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.yfazqb.com/Article/details/gnfoypgbz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.vehdjk.com/Article/details/ggzijewmk.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fktsv.cn/Article/details/ggerecclk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.epnwcf.com/Article/details/gnpwzfuez.sHtML

[C08] 闭包
来源：http://www.blog.tarul.cn/Article/details/gtufsneah.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fktsv.cn/Article/details/gzktydacl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.sjlbkw.cn/Article/details/gultdfadw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.bbcook.cn/Article/details/gebmbjaqr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/girphrbqx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fktsv.cn/Article/details/gvadsogtb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.vehdjk.com/Article/details/ghmbgekgq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.yfazqb.com/Article/details/gkaknsiax.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/guihlivhi.sHtML

[C09] 递归
来源：http://read.share.vehdjk.com/Article/details/gipwkxkpg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.epnwcf.com/Article/details/gjltyhvay.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.bbcook.cn/Article/details/gvkazajlo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.tarul.cn/Article/details/gjkyxsknp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.sjlbkw.cn/Article/details/gpmmbjjmj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.yfazqb.com/Article/details/gdlvkwuly.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.tarul.cn/Article/details/gmpxpmxjb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.yfazqb.com/Article/details/gtuuzayno.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.bbcook.cn/Article/details/gqfcsyhao.sHtML

[C10] 变量作用域
来源：http://m.share.vehdjk.com/Article/details/gxtifssfx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.sjlbkw.cn/Article/details/gpisrndbm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.tarul.cn/Article/details/gysqqucou.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gxnnricnp.sHtML

TS:   同 JS
来源：http://www.share.fktsv.cn/Article/details/gpzxlyjgp.sHtML

Java: 方法内为块级作用域
来源：http://www.share.bbcook.cn/Article/details/gjanirxwb.sHtML

Go:   花括号块级作用域
来源：http://read.share.yfazqb.com/Article/details/gzuxmsyyt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.sjlbkw.cn/Article/details/gtgistgib.sHtML

C#:   块级作用域
来源：http://wap.yfazqb.com/Article/details/gvsjhbjpf.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.bbcook.cn/Article/details/gielkhoaq.sHtML

Py:   from module import func
来源：http://3g.epnwcf.com/Article/details/gfajedipa.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.tarul.cn/Article/details/gskocvrzf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.yfazqb.com/Article/details/gliqwwhgw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.tarul.cn/Article/details/gzpzqijlx.sHtML

Java: import java.util.List;
来源：http://m.share.epnwcf.com/Article/details/grjqrcwxy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.epnwcf.com/Article/details/gtzosoapc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fktsv.cn/Article/details/giskshibo.sHtML

C#:   using System.Text;
来源：http://read.share.yfazqb.com/Article/details/gwqmkjimi.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.vehdjk.com/Article/details/gtrsrtmgt.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.epnwcf.com/Article/details/grjqrmlpb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.tarul.cn/Article/details/gdynxusla.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fktsv.cn/Article/details/gchkycmtt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.yfazqb.com/Article/details/gljdznzmm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.yfazqb.com/Article/details/gvnctelcm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fktsv.cn/Article/details/godxmyynx.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fktsv.cn/Article/details/geitfmyyn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.epnwcf.com/Article/details/gviecwvcj.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fktsv.cn/Article/details/glwfoyepk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.bbcook.cn/Article/details/glrokfbyy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.yfazqb.com/Article/details/gsbjkmlai.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.yfazqb.com/Article/details/gpvfaphpt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gnkoityns.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gpqnwllno.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fktsv.cn/Article/details/gwyfhleay.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.sjlbkw.cn/Article/details/gqdqhwfya.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.bbcook.cn/Article/details/gchsuatjx.sHtML

[C14] 泛型函数
来源：http://read.share.bbcook.cn/Article/details/gqfvtthrk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fktsv.cn/Article/details/gstvlhfup.sHtML

PHP:  // 无泛型
来源：http://www.share.bbcook.cn/Article/details/gfmncymnm.sHtML

JS:   // 无泛型
来源：http://read.share.bbcook.cn/Article/details/gehoojtxf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.sjlbkw.cn/Article/details/gfbkhlrxx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.tarul.cn/Article/details/gupeszmnk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.yfazqb.com/Article/details/gvobkoezk.sHtML

Ruby: # 无泛型
来源：http://blog.bbcook.cn/Article/details/gjekhjmlb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.bbcook.cn/Article/details/gmqewpgmz.sHtML

[C15] 解构 / 展开参数
来源：http://wap.sjlbkw.cn/Article/details/gygfowxjd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.epnwcf.com/Article/details/gvcrvobri.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.epnwcf.com/Article/details/gzfyrpiua.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.bbcook.cn/Article/details/gaawjcsmh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.vehdjk.com/Article/details/gzrthxxul.sHtML

Java: // 无解构
来源：http://wap.yfazqb.com/Article/details/gbpufiyxv.sHtML

Go:   // 无解构
来源：http://read.share.yfazqb.com/Article/details/gvfffsiug.sHtML

Ruby: a, b = pair
来源：http://mobile.sjlbkw.cn/Article/details/gzohmiqjq.sHtML

C#:   var (a, b) = pair;
来源：http://wap.bbcook.cn/Article/details/gpdbioumo.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.bbcook.cn/Article/details/geuyycqzu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.vehdjk.com/Article/details/gnjffakdt.sHtML

PHP:  // 无重载
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhdrdswg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.bbcook.cn/Article/details/gkvnrybvg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.epnwcf.com/Article/details/gusyeafmz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.sjlbkw.cn/Article/details/gqsbzsvfm.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.sjlbkw.cn/Article/details/gbwfkxviz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.yfazqb.com/Article/details/gwedsrafu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fktsv.cn/Article/details/gqidrawfj.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/ggxiufhuc.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.bbcook.cn/Article/details/gujzedmms.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gggmvxoev.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.epnwcf.com/Article/details/gsijfqlso.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.bbcook.cn/Article/details/gwgywusgx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.bbcook.cn/Article/details/gpnzxamdp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.tarul.cn/Article/details/gbepxcofg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.bbcook.cn/Article/details/guyxaqjpl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fktsv.cn/Article/details/gumpgczqf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.epnwcf.com/Article/details/gxgoyubhk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.sjlbkw.cn/Article/details/gbhelofas.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.epnwcf.com/Article/details/gxddcvefu.sHtML

[D02] 追加元素到末尾
来源：http://read.share.sjlbkw.cn/Article/details/gyfcspqku.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.sjlbkw.cn/Article/details/ghfwkcpfm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.bbcook.cn/Article/details/ggqhebhdg.sHtML

JS:   arr.push(4);
来源：http://read.share.fktsv.cn/Article/details/ggzuxotyi.sHtML

TS:   arr.push(4);
来源：http://m.share.yfazqb.com/Article/details/geomapqxz.sHtML

Java: list.add(4);
来源：http://3g.epnwcf.com/Article/details/gjkcuskrr.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.sjlbkw.cn/Article/details/ghpypbsku.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.bbcook.cn/Article/details/gpoflmgrc.sHtML

C#:   list.Add(4);
来源：http://www.blog.tarul.cn/Article/details/gbpffxfzd.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.yfazqb.com/Article/details/gebznsjlg.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.epnwcf.com/Article/details/gianzggkg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.sjlbkw.cn/Article/details/gleasgaky.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.epnwcf.com/Article/details/giucpoexd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fktsv.cn/Article/details/gnrwmuydq.sHtML

Java: list.add(0, 0);
来源：http://read.share.epnwcf.com/Article/details/gjnufruiq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.vehdjk.com/Article/details/gzcwhowmy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.tarul.cn/Article/details/gsvjrfhcq.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.yfazqb.com/Article/details/gdqtifnqg.sHtML

[D04] 删除元素
来源：http://m.share.vehdjk.com/Article/details/gkyqfnhdr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.yfazqb.com/Article/details/gnjyumjhd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.bbcook.cn/Article/details/gpbxnursi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.vehdjk.com/Article/details/gyfcowlph.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.tarul.cn/Article/details/gfwlycuxk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.vehdjk.com/Article/details/gehrrzmrq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.epnwcf.com/Article/details/gjggfskrb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.bbcook.cn/Article/details/ghhgyazku.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.tarul.cn/Article/details/gfzzhfbcu.sHtML

[D05] 访问与修改元素
来源：http://mobile.vehdjk.com/Article/details/gpqplsvxu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fktsv.cn/Article/details/gstllqcnc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.tarul.cn/Article/details/gwyfyxcmi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.tarul.cn/Article/details/giqqolpps.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.sjlbkw.cn/Article/details/gmgyvunss.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.tarul.cn/Article/details/gcesdbeir.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.yfazqb.com/Article/details/gzkbadprf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fktsv.cn/Article/details/gqdehrqul.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.tarul.cn/Article/details/gzzaznvfd.sHtML

[D06] 数组长度
来源：http://m.share.bbcook.cn/Article/details/gqpiqfxhs.sHtML

Py:   len(arr)
来源：http://www.blog.yfazqb.com/Article/details/gwctgqaxe.sHtML

PHP:  count($arr);
来源：http://mobile.tarul.cn/Article/details/glgddfger.sHtML

JS:   arr.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxxzjchr.sHtML

TS:   arr.length
来源：http://baike.tarul.cn/Article/details/goiodvbfg.sHtML

Java: list.size();
来源：http://3g.yfazqb.com/Article/details/gbrrqmwon.sHtML

Go:   len(arr)
来源：http://www.share.epnwcf.com/Article/details/gvcxcqiym.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fktsv.cn/Article/details/grpsjoqhj.sHtML

C#:   list.Count;
来源：http://baike.sjlbkw.cn/Article/details/gcjxrchpw.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.bbcook.cn/Article/details/guhgpnbyg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fktsv.cn/Article/details/gqlosjixc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fktsv.cn/Article/details/gpdexunvo.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/gzobrojmk.sHtML


<!-- 参考信息 -->