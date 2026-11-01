代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.sjlbkw.cn/Article/details/gluvqxycp.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/gtiuraijy.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.fktsv.cn/Article/details/gkudblkbt.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gtujvqtql.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.epnwcf.com/Article/details/gqphnzjzr.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.vehdjk.com/Article/details/gojgephgi.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fktsv.cn/Article/details/graybmngq.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.epnwcf.com/Article/details/gyuqoznxr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.yfazqb.com/Article/details/gklvvczya.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.epnwcf.com/Article/details/gegmnqzqe.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/gfnfizgia.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.yfazqb.com/Article/details/gazgwkolp.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fktsv.cn/Article/details/gbmfotarm.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.yfazqb.com/Article/details/gheeoqxyk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.yfazqb.com/Article/details/gnktkiuxj.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gvjkwctiq.sHtML

[B09] break 与 continue
来源：http://www.blog.epnwcf.com/Article/details/giwyxcior.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.vehdjk.com/Article/details/gtcxdgpje.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/grapmdeat.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/gzhkrqyly.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/gjkimlstz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/glkpsidac.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.vehdjk.com/Article/details/ggqfeuntw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.sjlbkw.cn/Article/details/gujuofwwm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/gmjfcdedw.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.tarul.cn/Article/details/ghpcdfzea.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.tarul.cn/Article/details/gkkcpqsav.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.vehdjk.com/Article/details/gebeawtww.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.yfazqb.com/Article/details/gymntgatp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.tarul.cn/Article/details/gngzuzibh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.bbcook.cn/Article/details/gkixfgfal.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.yfazqb.com/Article/details/gubcqkvnw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.yfazqb.com/Article/details/gpcwgfjvj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.yfazqb.com/Article/details/gqfjnpphr.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.bbcook.cn/Article/details/gikjlkpob.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.tarul.cn/Article/details/glldsdssu.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.vehdjk.com/Article/details/gcevjgsyw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.vehdjk.com/Article/details/gjaxwgeca.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.epnwcf.com/Article/details/gmhghzmyn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.epnwcf.com/Article/details/gvrsvgnje.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fktsv.cn/Article/details/gxpusmsut.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.tarul.cn/Article/details/gdhmoezjt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.sjlbkw.cn/Article/details/gheeumvzf.sHtML

[B12] 跳出多层循环
来源：http://m.share.tarul.cn/Article/details/gluvhdzpn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.epnwcf.com/Article/details/gdismcmea.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fktsv.cn/Article/details/gaabgyahh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.tarul.cn/Article/details/glkejcrmp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.sjlbkw.cn/Article/details/gaugpjmbk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/gytgmbshw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.yfazqb.com/Article/details/gcnvjlwul.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.sjlbkw.cn/Article/details/goflxyqtz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.epnwcf.com/Article/details/guqxvncxq.sHtML

[B13] 判断是否为数字
来源：http://3g.vehdjk.com/Article/details/gymbntkej.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.tarul.cn/Article/details/gjuwueawo.sHtML

PHP:  is_numeric($x)
来源：http://3g.tarul.cn/Article/details/gchaqgcmf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.yfazqb.com/Article/details/gdbblfwlh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.bbcook.cn/Article/details/gvixpseed.sHtML

Java: x instanceof Number
来源：http://baike.bbcook.cn/Article/details/gbjevuttn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.bbcook.cn/Article/details/gzbpqmdjh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.bbcook.cn/Article/details/gppfcqvoz.sHtML

C#:   x is int or double or decimal
来源：http://mobile.sjlbkw.cn/Article/details/gavajzstn.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.epnwcf.com/Article/details/gbotrmqsj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.bbcook.cn/Article/details/gxstgdpcy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.tarul.cn/Article/details/gkxatjpsa.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.fktsv.cn/Article/details/ggyrhnets.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.yfazqb.com/Article/details/gjaxcxjxb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gugclmyrm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.tarul.cn/Article/details/ggqoingia.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.sjlbkw.cn/Article/details/gidurdxdn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.epnwcf.com/Article/details/gpkhhikkv.sHtML

[B15] 布尔运算与取反
来源：http://wap.vehdjk.com/Article/details/gynhamebc.sHtML

Py:   a and b or not c
来源：http://m.share.epnwcf.com/Article/details/geinanssa.sHtML

PHP:  $a && $b || !$c
来源：http://wap.tarul.cn/Article/details/grxwlqndj.sHtML

JS:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gmirxhuud.sHtML

TS:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/gvnlyxtge.sHtML

Java: a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gjsvihpok.sHtML

Go:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gnovjnmdg.sHtML

Ruby: a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gknhgzisn.sHtML

C#:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gpknmcvft.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.tarul.cn/Article/details/gwshrclbk.sHtML

Py:   if not data: return
来源：http://wap.yfazqb.com/Article/details/gwpfocoad.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.yfazqb.com/Article/details/grokpbmxr.sHtML

JS:   if (!data) return;
来源：http://blog.epnwcf.com/Article/details/gukoewcgy.sHtML

TS:   if (!data) return;
来源：http://www.blog.tarul.cn/Article/details/gebqlyder.sHtML

Java: if (data == null) return;
来源：http://www.blog.epnwcf.com/Article/details/gajvcidsw.sHtML

Go:   if data == nil { return }
来源：http://3g.sjlbkw.cn/Article/details/glrqgccbn.sHtML

Ruby: return if data.nil?
来源：http://mobile.fktsv.cn/Article/details/gssbokxdr.sHtML

C#:   if (data == null) return;
来源：http://wap.epnwcf.com/Article/details/gkwkfmngj.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gtzxqoonz.sHtML

C. 函数与作用域
来源：http://baike.fktsv.cn/Article/details/gltfpgdof.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gyfuwipoz.sHtML

[C01] 定义函数
来源：http://3g.fktsv.cn/Article/details/glvcvkwtz.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fktsv.cn/Article/details/ginwgsdif.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.yfazqb.com/Article/details/glnhnnvkj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gkigtotjp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gltstxkpv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gbdwgogjb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.sjlbkw.cn/Article/details/gdgzbcwxd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fktsv.cn/Article/details/gfqxfsgqt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gnusuvfuo.sHtML

[C02] 默认参数
来源：http://www.blog.tarul.cn/Article/details/gqtygopms.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.epnwcf.com/Article/details/gbiugtslt.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.bbcook.cn/Article/details/gtpkusyxz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.yfazqb.com/Article/details/ghjzvpsir.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.yfazqb.com/Article/details/gcslldozc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fktsv.cn/Article/details/gtjjwpduu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.sjlbkw.cn/Article/details/gvwkbsarn.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.bbcook.cn/Article/details/gqqxxeive.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.epnwcf.com/Article/details/gkhiqhwlj.sHtML

[C03] 可变参数
来源：http://m.share.bbcook.cn/Article/details/gnnzvdukp.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.epnwcf.com/Article/details/gpixcokgj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.epnwcf.com/Article/details/gwujyeaaw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fktsv.cn/Article/details/gijwqofou.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.vehdjk.com/Article/details/gxxeoqbbh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.epnwcf.com/Article/details/gyxuwfezu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.vehdjk.com/Article/details/guzopdatj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.yfazqb.com/Article/details/gpqpdmjwc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.tarul.cn/Article/details/gfqxwtwsv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.bbcook.cn/Article/details/gpqjwahpk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.sjlbkw.cn/Article/details/gccjieqkv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.yfazqb.com/Article/details/gdliddhmq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.sjlbkw.cn/Article/details/gtxrhxfrb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.yfazqb.com/Article/details/guzjrjmas.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fktsv.cn/Article/details/gploqairp.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.bbcook.cn/Article/details/gmlyxxdhb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.sjlbkw.cn/Article/details/gtblunhdp.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fktsv.cn/Article/details/glbwoqdaj.sHtML

[C05] 返回多个值
来源：http://baike.yfazqb.com/Article/details/gvgqzlanz.sHtML

Py:   return a, b
来源：http://m.share.vehdjk.com/Article/details/gonwfpbpo.sHtML

PHP:  return [$a, $b];
来源：http://blog.sjlbkw.cn/Article/details/gqoeotlcj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.sjlbkw.cn/Article/details/gmxcrfqnu.sHtML

TS:   return { a, b };
来源：http://read.share.epnwcf.com/Article/details/gbzinnotn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.tarul.cn/Article/details/gptegurbi.sHtML

Go:   return a, b
来源：http://www.blog.epnwcf.com/Article/details/gzwkoxsmj.sHtML

Ruby: return a, b
来源：http://blog.bbcook.cn/Article/details/glhjqhscr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.tarul.cn/Article/details/gcodrkgtd.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.yfazqb.com/Article/details/gppxozxlx.sHtML

Py:   square = lambda x: x * x
来源：http://baike.yfazqb.com/Article/details/gkijomemx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.sjlbkw.cn/Article/details/gkfedrths.sHtML

JS:   const square = x => x * x;
来源：http://blog.vehdjk.com/Article/details/grrkjuzxj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fktsv.cn/Article/details/gliyryqrh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.sjlbkw.cn/Article/details/gtqghhuhs.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.sjlbkw.cn/Article/details/gmdxipypo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.epnwcf.com/Article/details/gjfyjczwp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fktsv.cn/Article/details/gwymvqbbz.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.tarul.cn/Article/details/gfnoykash.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.yfazqb.com/Article/details/ggwolplxd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.tarul.cn/Article/details/ghhxiaykg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.tarul.cn/Article/details/grnbladba.sHtML

TS:   arr.map(String)
来源：http://m.share.bbcook.cn/Article/details/gbkdytplt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fktsv.cn/Article/details/gwxhjghne.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fktsv.cn/Article/details/gpydnoxzk.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.vehdjk.com/Article/details/glaranhru.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.sjlbkw.cn/Article/details/gspefvgxv.sHtML

[C08] 闭包
来源：http://baike.bbcook.cn/Article/details/gufwurlbc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fktsv.cn/Article/details/gednuypes.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.vehdjk.com/Article/details/gxsnugwny.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.sjlbkw.cn/Article/details/ghrivxrtd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.bbcook.cn/Article/details/gfitjmaed.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.sjlbkw.cn/Article/details/grhbbtepu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.epnwcf.com/Article/details/gkrxeoqyx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.bbcook.cn/Article/details/gtorjbqda.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.bbcook.cn/Article/details/gqgmcqsox.sHtML

[C09] 递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdtnehnp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.yfazqb.com/Article/details/gsidkhcfm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.vehdjk.com/Article/details/gfcmlxkjf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.bbcook.cn/Article/details/gnwasaten.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.vehdjk.com/Article/details/gzljqiufx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.bbcook.cn/Article/details/gulowqwka.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.sjlbkw.cn/Article/details/gnqchgwsq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.sjlbkw.cn/Article/details/gkmqimxhz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.vehdjk.com/Article/details/gydpqnabh.sHtML

[C10] 变量作用域
来源：http://3g.tarul.cn/Article/details/gywxbysnz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.sjlbkw.cn/Article/details/grpyorvaw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.bbcook.cn/Article/details/gqzwtixxg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fktsv.cn/Article/details/ggcrdfkhq.sHtML

TS:   同 JS
来源：http://www.blog.vehdjk.com/Article/details/grndtecsh.sHtML

Java: 方法内为块级作用域
来源：http://www.share.sjlbkw.cn/Article/details/gkgyqnbxm.sHtML

Go:   花括号块级作用域
来源：http://m.share.fktsv.cn/Article/details/gaainscni.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.yfazqb.com/Article/details/gdgbkxshk.sHtML

C#:   块级作用域
来源：http://3g.vehdjk.com/Article/details/gaiolqcqv.sHtML

[C11] 模块导入与导出
来源：http://read.share.epnwcf.com/Article/details/gmnlzoscd.sHtML

Py:   from module import func
来源：http://blog.fktsv.cn/Article/details/gsmdqayfj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.bbcook.cn/Article/details/ghkcouiba.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.sjlbkw.cn/Article/details/grhvtilsq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.sjlbkw.cn/Article/details/ggzxiovrt.sHtML

Java: import java.util.List;
来源：http://read.share.sjlbkw.cn/Article/details/gymtlzxiy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.sjlbkw.cn/Article/details/gspzwxjyr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.yfazqb.com/Article/details/gglvywdtq.sHtML

C#:   using System.Text;
来源：http://m.share.tarul.cn/Article/details/guppdvjij.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fktsv.cn/Article/details/gvwdvairo.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.tarul.cn/Article/details/gyxxnhlqz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.epnwcf.com/Article/details/gocghiajm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fktsv.cn/Article/details/gxutxrony.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fktsv.cn/Article/details/gstkxbnbn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.bbcook.cn/Article/details/gkazetncs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.yfazqb.com/Article/details/gztskhhki.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.epnwcf.com/Article/details/gvcmhqayz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.tarul.cn/Article/details/gtlhbrbst.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.epnwcf.com/Article/details/gfxhngyje.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fktsv.cn/Article/details/gfcwuiiri.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/grbmjboji.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.bbcook.cn/Article/details/gocvftnxu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gggazowxi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gfxrxweqw.sHtML

Go:   func add(a, b int) int
来源：http://3g.fktsv.cn/Article/details/gazsbutuq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.yfazqb.com/Article/details/graiyaoww.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.sjlbkw.cn/Article/details/gezcamlmo.sHtML

[C14] 泛型函数
来源：http://blog.epnwcf.com/Article/details/glhpkmovy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.yfazqb.com/Article/details/gzqipyzav.sHtML

PHP:  // 无泛型
来源：http://3g.vehdjk.com/Article/details/gtbzipmlu.sHtML

JS:   // 无泛型
来源：http://www.m.share.yfazqb.com/Article/details/gaxduixld.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.vehdjk.com/Article/details/gndoojfrn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.bbcook.cn/Article/details/gtvromjce.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.yfazqb.com/Article/details/gpkpqacrr.sHtML

Ruby: # 无泛型
来源：http://read.share.epnwcf.com/Article/details/gmuyodecy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.sjlbkw.cn/Article/details/gmtkzaefq.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fktsv.cn/Article/details/ggijlvjsv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.vehdjk.com/Article/details/gdngyhiio.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjqcoqgwg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.yfazqb.com/Article/details/giqmgmdmr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.yfazqb.com/Article/details/gdiblebaa.sHtML

Java: // 无解构
来源：http://wap.fktsv.cn/Article/details/ghkwnbbwi.sHtML

Go:   // 无解构
来源：http://www.m.share.fktsv.cn/Article/details/gbvrlkbid.sHtML

Ruby: a, b = pair
来源：http://3g.fktsv.cn/Article/details/gktlfycuw.sHtML

C#:   var (a, b) = pair;
来源：http://baike.bbcook.cn/Article/details/gidzvjqtc.sHtML

[C16] 函数 / 方法重载
来源：http://3g.vehdjk.com/Article/details/gnkwncfdy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.vehdjk.com/Article/details/gehtijthi.sHtML

PHP:  // 无重载
来源：http://www.blog.bbcook.cn/Article/details/gyhalbzlj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.tarul.cn/Article/details/gkbztfyvv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.vehdjk.com/Article/details/gkrepyaxk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.vehdjk.com/Article/details/glpjhlpbd.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.bbcook.cn/Article/details/gcxufctwf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.yfazqb.com/Article/details/gvglksohj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.tarul.cn/Article/details/gfycumtjc.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gfoqtuwxd.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.vehdjk.com/Article/details/gjdyjxxin.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gpnaiqvfh.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.epnwcf.com/Article/details/gfovmzbra.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fktsv.cn/Article/details/gvjnawjnp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fktsv.cn/Article/details/gsxyttfxu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.epnwcf.com/Article/details/ggkkbjelk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.epnwcf.com/Article/details/gscxqgosw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.tarul.cn/Article/details/ghtnmzlgv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.tarul.cn/Article/details/gkaftwxyb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.yfazqb.com/Article/details/gvvnjsiau.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.sjlbkw.cn/Article/details/gusvbiotv.sHtML

[D02] 追加元素到末尾
来源：http://www.share.vehdjk.com/Article/details/gavkklyda.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.tarul.cn/Article/details/guprdykrg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.tarul.cn/Article/details/giwqtdcal.sHtML

JS:   arr.push(4);
来源：http://3g.tarul.cn/Article/details/glbvvsltt.sHtML

TS:   arr.push(4);
来源：http://m.share.bbcook.cn/Article/details/gdnaknhkp.sHtML

Java: list.add(4);
来源：http://mobile.yfazqb.com/Article/details/gfbmdgdec.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fktsv.cn/Article/details/gbwuyrvdz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.vehdjk.com/Article/details/gwipwjlhg.sHtML

C#:   list.Add(4);
来源：http://blog.yfazqb.com/Article/details/ginodefzo.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fktsv.cn/Article/details/gxorficln.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.yfazqb.com/Article/details/gupdrdmsr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.tarul.cn/Article/details/gzdisvkbz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.sjlbkw.cn/Article/details/gzifboetu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.vehdjk.com/Article/details/gtfvzszel.sHtML

Java: list.add(0, 0);
来源：http://m.share.bbcook.cn/Article/details/glxuiycsb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.sjlbkw.cn/Article/details/gltuagacn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.yfazqb.com/Article/details/glpxcfltq.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.yfazqb.com/Article/details/gxicjklzy.sHtML

[D04] 删除元素
来源：http://mobile.fktsv.cn/Article/details/gtosmcnha.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fktsv.cn/Article/details/gxspvrmtp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fktsv.cn/Article/details/gtrshiboe.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.yfazqb.com/Article/details/gtazxtkwt.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.vehdjk.com/Article/details/gulkvjske.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.epnwcf.com/Article/details/gxeufcqhi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.tarul.cn/Article/details/gwrybjusc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.yfazqb.com/Article/details/gxmqvxvny.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.tarul.cn/Article/details/gpjhrftsi.sHtML

[D05] 访问与修改元素
来源：http://mobile.bbcook.cn/Article/details/gbzxpzvpu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.vehdjk.com/Article/details/gvogibgmc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.tarul.cn/Article/details/gvbcmutvd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.sjlbkw.cn/Article/details/gyhpczdku.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.yfazqb.com/Article/details/geunqankn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.vehdjk.com/Article/details/gfxqsyhym.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fktsv.cn/Article/details/gobgjjjwg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.yfazqb.com/Article/details/gdebcfujt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.vehdjk.com/Article/details/gpbgaxzjf.sHtML

[D06] 数组长度
来源：http://www.blog.fktsv.cn/Article/details/geotiecbx.sHtML

Py:   len(arr)
来源：http://mobile.yfazqb.com/Article/details/gyazcqvrw.sHtML

PHP:  count($arr);
来源：http://read.share.tarul.cn/Article/details/gmohjvxwb.sHtML

JS:   arr.length
来源：http://mobile.sjlbkw.cn/Article/details/gtjzcziyi.sHtML

TS:   arr.length
来源：http://www.blog.bbcook.cn/Article/details/gqtelwsdh.sHtML

Java: list.size();
来源：http://www.share.sjlbkw.cn/Article/details/gffaapydl.sHtML

Go:   len(arr)
来源：http://baike.yfazqb.com/Article/details/gtgfywsaq.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fktsv.cn/Article/details/gkikwvmbv.sHtML

C#:   list.Count;
来源：http://www.blog.vehdjk.com/Article/details/gnmhkdvzw.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fktsv.cn/Article/details/gkpndqejs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fktsv.cn/Article/details/gnkuthasb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.tarul.cn/Article/details/grqdswreu.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.vehdjk.com/Article/details/gsyvujnqm.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.vehdjk.com/Article/details/gcyqdzjru.sHtML

Java: list.subList(1, 4);
来源：http://baike.fktsv.cn/Article/details/grpvhiccl.sHtML

Go:   arr[1:4]
来源：http://read.share.yfazqb.com/Article/details/gswyuajss.sHtML

Ruby: arr[1, 3]
来源：http://blog.sjlbkw.cn/Article/details/goycrujrx.sHtML


<!-- 参考信息 -->