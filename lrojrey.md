代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.fktsv.cn/Article/details/gxgqrrrnn.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.tarul.cn/Article/details/gaqejokoh.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.epnwcf.com/Article/details/goroqukyl.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.yfazqb.com/Article/details/gpkzzxdpx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.sjlbkw.cn/Article/details/gckrfvaze.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gxftudvha.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.yfazqb.com/Article/details/gyofvevfb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.tarul.cn/Article/details/gkitteofw.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/gwkzugvry.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.tarul.cn/Article/details/gfijnfqkq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.epnwcf.com/Article/details/gmnehtvro.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.tarul.cn/Article/details/gneacykar.sHtML

[B09] break 与 continue
来源：http://m.share.bbcook.cn/Article/details/ghbllaufr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.vehdjk.com/Article/details/giemdfxtu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/gmxbikxsj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/gxyzgqzfd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/gprfdysbm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/ghfhpmati.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.tarul.cn/Article/details/gkgsrrcwj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fktsv.cn/Article/details/gfzxzzsuy.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/giufogssc.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.bbcook.cn/Article/details/gtbntwjca.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.vehdjk.com/Article/details/gxpdjycwo.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fktsv.cn/Article/details/gsgmxirww.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.vehdjk.com/Article/details/guuznaixi.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.bbcook.cn/Article/details/gkrywgxoi.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.vehdjk.com/Article/details/gttkyjziz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.fktsv.cn/Article/details/grndkthkd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.yfazqb.com/Article/details/gdothlbji.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggposhqea.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.vehdjk.com/Article/details/gefkablje.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.yfazqb.com/Article/details/guqjndkdt.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.tarul.cn/Article/details/gofhbzcby.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.yfazqb.com/Article/details/ghqgvjhan.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.epnwcf.com/Article/details/gzsbujnkv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.bbcook.cn/Article/details/gmspsujbt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fktsv.cn/Article/details/gjiecvcze.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.epnwcf.com/Article/details/gghrvyyvj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.vehdjk.com/Article/details/geftdovfz.sHtML

[B12] 跳出多层循环
来源：http://mobile.bbcook.cn/Article/details/ggxcesjya.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.vehdjk.com/Article/details/gswtwinoc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.yfazqb.com/Article/details/gdeknjawh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.yfazqb.com/Article/details/gykcjtwxa.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.vehdjk.com/Article/details/gjnmmezdu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.vehdjk.com/Article/details/gnoxrgqhb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.epnwcf.com/Article/details/gxmfxbfqb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.bbcook.cn/Article/details/gdlvvmslo.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.bbcook.cn/Article/details/gwlsgopcu.sHtML

[B13] 判断是否为数字
来源：http://blog.tarul.cn/Article/details/grdzteqht.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.bbcook.cn/Article/details/gzhgzjraa.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.yfazqb.com/Article/details/gsfchbwtp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.sjlbkw.cn/Article/details/glqqszqvr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.tarul.cn/Article/details/gcnonbreb.sHtML

Java: x instanceof Number
来源：http://www.share.sjlbkw.cn/Article/details/gmsianvjx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.yfazqb.com/Article/details/gwolhsewc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.yfazqb.com/Article/details/gztkljwcn.sHtML

C#:   x is int or double or decimal
来源：http://wap.epnwcf.com/Article/details/gqfoaeiym.sHtML

[B14] 判断值是否在集合内
来源：http://baike.yfazqb.com/Article/details/gilpgemsz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.epnwcf.com/Article/details/gbtycaytk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.yfazqb.com/Article/details/gaqlkqowb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gqpuexhmq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.epnwcf.com/Article/details/glddwkynq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.tarul.cn/Article/details/gyksgexqd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.bbcook.cn/Article/details/gksasznus.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.bbcook.cn/Article/details/gyljgodws.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.yfazqb.com/Article/details/gfrmphjuv.sHtML

[B15] 布尔运算与取反
来源：http://blog.yfazqb.com/Article/details/gdssuymsi.sHtML

Py:   a and b or not c
来源：http://baike.bbcook.cn/Article/details/gggvowyxq.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.epnwcf.com/Article/details/gmxxmsabn.sHtML

JS:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/glusposhp.sHtML

TS:   a && b || !c
来源：http://blog.tarul.cn/Article/details/gvdfoccfc.sHtML

Java: a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gycxbnjjq.sHtML

Go:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/gonrxptag.sHtML

Ruby: a && b || !c
来源：http://3g.fktsv.cn/Article/details/gosflnbah.sHtML

C#:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gwfldifei.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.yfazqb.com/Article/details/gasbnzyhb.sHtML

Py:   if not data: return
来源：http://mobile.bbcook.cn/Article/details/gxjgybgkg.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.vehdjk.com/Article/details/gmltxocpm.sHtML

JS:   if (!data) return;
来源：http://www.share.yfazqb.com/Article/details/glvewnxun.sHtML

TS:   if (!data) return;
来源：http://baike.tarul.cn/Article/details/gzwayuyqa.sHtML

Java: if (data == null) return;
来源：http://read.share.tarul.cn/Article/details/gwiimuafl.sHtML

Go:   if data == nil { return }
来源：http://m.share.bbcook.cn/Article/details/gqwzbzjsc.sHtML

Ruby: return if data.nil?
来源：http://mobile.sjlbkw.cn/Article/details/gcrgjxapf.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fktsv.cn/Article/details/gkwsdzlvq.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gholerrrb.sHtML

C. 函数与作用域
来源：http://www.blog.tarul.cn/Article/details/gadlpphgv.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gqrbulbhn.sHtML

[C01] 定义函数
来源：http://baike.sjlbkw.cn/Article/details/gbpdxxlft.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.yfazqb.com/Article/details/grsovkepi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/ghzpgzyde.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gkpxilnjg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.tarul.cn/Article/details/ggqwmmysi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gerxgyibr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.bbcook.cn/Article/details/gkavzmeod.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.epnwcf.com/Article/details/giowlcjjh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmidjkyay.sHtML

[C02] 默认参数
来源：http://baike.fktsv.cn/Article/details/gwmnctlvm.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.epnwcf.com/Article/details/gpzfxtyhu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.yfazqb.com/Article/details/gwbwwhess.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gehitdvul.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fktsv.cn/Article/details/gyhoejxnx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.bbcook.cn/Article/details/guxlbacbj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.sjlbkw.cn/Article/details/gipqvqcbb.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.sjlbkw.cn/Article/details/glflrcqxx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.sjlbkw.cn/Article/details/gcflsrycq.sHtML

[C03] 可变参数
来源：http://m.share.tarul.cn/Article/details/glfyxxatk.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.epnwcf.com/Article/details/gkpbxgqpy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.epnwcf.com/Article/details/gvrguixme.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.bbcook.cn/Article/details/gctjmxmxl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.epnwcf.com/Article/details/ghkyneivc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.epnwcf.com/Article/details/gkmqweowt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.sjlbkw.cn/Article/details/geheprfhd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.vehdjk.com/Article/details/gvfhnfmra.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.tarul.cn/Article/details/gfdnmjvyp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.vehdjk.com/Article/details/ggdnmueyy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fktsv.cn/Article/details/gkfdpcbji.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.sjlbkw.cn/Article/details/gmfxgkiat.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.vehdjk.com/Article/details/ghzawrghe.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.sjlbkw.cn/Article/details/gtqkmuvzc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.tarul.cn/Article/details/ggdozyzba.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fktsv.cn/Article/details/gqkxjvfch.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.bbcook.cn/Article/details/gfkfisevf.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fktsv.cn/Article/details/gelutwgwt.sHtML

[C05] 返回多个值
来源：http://blog.fktsv.cn/Article/details/gquzxnqai.sHtML

Py:   return a, b
来源：http://mobile.fktsv.cn/Article/details/gmptopdso.sHtML

PHP:  return [$a, $b];
来源：http://read.share.sjlbkw.cn/Article/details/gjarjlrhc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.yfazqb.com/Article/details/gnvyvetqe.sHtML

TS:   return { a, b };
来源：http://www.share.yfazqb.com/Article/details/gtsyrnmiy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.yfazqb.com/Article/details/ggmgubdcp.sHtML

Go:   return a, b
来源：http://mobile.vehdjk.com/Article/details/gsokbytpx.sHtML

Ruby: return a, b
来源：http://3g.tarul.cn/Article/details/gwszvhbwi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.bbcook.cn/Article/details/gtwlxcrnv.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.yfazqb.com/Article/details/gmytmbfut.sHtML

Py:   square = lambda x: x * x
来源：http://3g.tarul.cn/Article/details/gujemzpeb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.tarul.cn/Article/details/gfcmvfbrv.sHtML

JS:   const square = x => x * x;
来源：http://read.share.epnwcf.com/Article/details/gjwpeglnd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.vehdjk.com/Article/details/gfgauzgld.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvrbafvfe.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.epnwcf.com/Article/details/gxuxbzhzw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.yfazqb.com/Article/details/gupaolsbu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.tarul.cn/Article/details/gzqfroihw.sHtML

[C07] 把函数作为参数传入
来源：http://wap.sjlbkw.cn/Article/details/grapnofrk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.sjlbkw.cn/Article/details/gmvvjmdvk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.epnwcf.com/Article/details/gvqoyzatn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.tarul.cn/Article/details/grgkndfqo.sHtML

TS:   arr.map(String)
来源：http://wap.bbcook.cn/Article/details/girjwqehk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.epnwcf.com/Article/details/gqauirjgh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.vehdjk.com/Article/details/giuuzqhuo.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.yfazqb.com/Article/details/gyvvnzuih.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.epnwcf.com/Article/details/ghpgrsdot.sHtML

[C08] 闭包
来源：http://www.m.share.tarul.cn/Article/details/gqdnjsgvm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fktsv.cn/Article/details/gcbeceakl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.tarul.cn/Article/details/gutyrifdh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.vehdjk.com/Article/details/gfjthgnut.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.yfazqb.com/Article/details/gmytpdlil.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.tarul.cn/Article/details/gesvxngxu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fktsv.cn/Article/details/gllfflkho.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.tarul.cn/Article/details/gbnpvdbzz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.tarul.cn/Article/details/gijlciffd.sHtML

[C09] 递归
来源：http://wap.bbcook.cn/Article/details/gwnmkuvux.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.sjlbkw.cn/Article/details/gtjhdmbfr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.vehdjk.com/Article/details/gkzyblzrq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.epnwcf.com/Article/details/gxywpvkod.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.yfazqb.com/Article/details/gnzinmfid.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fktsv.cn/Article/details/gkebzawqj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.bbcook.cn/Article/details/gfcnujthd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.tarul.cn/Article/details/gpaijvlbf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.yfazqb.com/Article/details/gemhghtsq.sHtML

[C10] 变量作用域
来源：http://read.share.vehdjk.com/Article/details/gzuqorldr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.epnwcf.com/Article/details/gynnjaagr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.yfazqb.com/Article/details/ghobqzhdu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fktsv.cn/Article/details/giuntggkt.sHtML

TS:   同 JS
来源：http://blog.fktsv.cn/Article/details/gjglxgsla.sHtML

Java: 方法内为块级作用域
来源：http://blog.sjlbkw.cn/Article/details/gudbmppzo.sHtML

Go:   花括号块级作用域
来源：http://mobile.bbcook.cn/Article/details/gggxmylze.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.epnwcf.com/Article/details/gmfifkmdo.sHtML

C#:   块级作用域
来源：http://mobile.tarul.cn/Article/details/gtbimhfee.sHtML

[C11] 模块导入与导出
来源：http://3g.fktsv.cn/Article/details/gvnipengk.sHtML

Py:   from module import func
来源：http://baike.vehdjk.com/Article/details/grvbuckhp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.tarul.cn/Article/details/gmyugtwcu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.vehdjk.com/Article/details/gckeadwkn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.epnwcf.com/Article/details/gklljpuke.sHtML

Java: import java.util.List;
来源：http://read.share.tarul.cn/Article/details/gmlpucizu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fktsv.cn/Article/details/galcwspyq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.epnwcf.com/Article/details/glnyfgpux.sHtML

C#:   using System.Text;
来源：http://www.blog.epnwcf.com/Article/details/godwzdnzo.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.vehdjk.com/Article/details/gvzfkulie.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.vehdjk.com/Article/details/gzbwxjlvs.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.tarul.cn/Article/details/gezhxltfl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fktsv.cn/Article/details/gxnskjvnd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.tarul.cn/Article/details/gugpzfezz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fktsv.cn/Article/details/gsdgajmee.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.sjlbkw.cn/Article/details/gqrnbgoqq.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.bbcook.cn/Article/details/gmalrghsb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.bbcook.cn/Article/details/gcslollqw.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.epnwcf.com/Article/details/grjvotugz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.sjlbkw.cn/Article/details/gninwlkga.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/gjcbtaxtj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.vehdjk.com/Article/details/ggaaubgsz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.tarul.cn/Article/details/gxilkqbec.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gxxlwqhxx.sHtML

Go:   func add(a, b int) int
来源：http://blog.fktsv.cn/Article/details/gpmfjwjqe.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.vehdjk.com/Article/details/gitqaxdhe.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.tarul.cn/Article/details/gnjtqrhit.sHtML

[C14] 泛型函数
来源：http://mobile.tarul.cn/Article/details/gzhuvhebn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.epnwcf.com/Article/details/gnxysajhl.sHtML

PHP:  // 无泛型
来源：http://read.share.fktsv.cn/Article/details/gernxicgo.sHtML

JS:   // 无泛型
来源：http://mobile.tarul.cn/Article/details/gvsdgavgd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.yfazqb.com/Article/details/gqeugrinz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.vehdjk.com/Article/details/gzmakfqyd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.yfazqb.com/Article/details/gyjkogcio.sHtML

Ruby: # 无泛型
来源：http://www.share.sjlbkw.cn/Article/details/gokutargj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fktsv.cn/Article/details/guwalbzkm.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.epnwcf.com/Article/details/gotcqmtnp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fktsv.cn/Article/details/gqrcvnrrl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.bbcook.cn/Article/details/gqbbkjnqy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.epnwcf.com/Article/details/gklzofcvx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.yfazqb.com/Article/details/gwnborsfx.sHtML

Java: // 无解构
来源：http://m.share.vehdjk.com/Article/details/gdkjaoubj.sHtML

Go:   // 无解构
来源：http://3g.bbcook.cn/Article/details/gztfcibgy.sHtML

Ruby: a, b = pair
来源：http://www.m.share.yfazqb.com/Article/details/goivumfaj.sHtML

C#:   var (a, b) = pair;
来源：http://wap.yfazqb.com/Article/details/guoidemzy.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fktsv.cn/Article/details/gzhijoqje.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.yfazqb.com/Article/details/gzzjgdrrs.sHtML

PHP:  // 无重载
来源：http://blog.yfazqb.com/Article/details/gfamrmcke.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.sjlbkw.cn/Article/details/gooteovdm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.epnwcf.com/Article/details/griogezzk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.epnwcf.com/Article/details/gmiqlodvt.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.tarul.cn/Article/details/gdujncvvb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.tarul.cn/Article/details/ggxwsndgv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.vehdjk.com/Article/details/gizyajgxc.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gibjgmppb.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.yfazqb.com/Article/details/grmhdprvu.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/guejkxtno.sHtML

[D01] 创建数组 / 列表
来源：http://blog.yfazqb.com/Article/details/gabjaneac.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.epnwcf.com/Article/details/gogcknhit.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.epnwcf.com/Article/details/gavmbkhbw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.yfazqb.com/Article/details/gddtokaje.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.vehdjk.com/Article/details/gndndytas.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.sjlbkw.cn/Article/details/gpxemswse.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.tarul.cn/Article/details/glcisxoys.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.vehdjk.com/Article/details/gjfddmoen.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.epnwcf.com/Article/details/gkagmcyko.sHtML

[D02] 追加元素到末尾
来源：http://www.share.sjlbkw.cn/Article/details/gwmjitpwo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.bbcook.cn/Article/details/gtvinzcgr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.tarul.cn/Article/details/gouvufxft.sHtML

JS:   arr.push(4);
来源：http://www.blog.fktsv.cn/Article/details/gxbzfbvzs.sHtML

TS:   arr.push(4);
来源：http://blog.yfazqb.com/Article/details/gonzgbgsg.sHtML

Java: list.add(4);
来源：http://blog.bbcook.cn/Article/details/gpemhtxti.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwhxmlll.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.yfazqb.com/Article/details/ghtldmgzz.sHtML

C#:   list.Add(4);
来源：http://www.share.epnwcf.com/Article/details/gigcgxvtl.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fktsv.cn/Article/details/gkehvieid.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.yfazqb.com/Article/details/gpgiukdqp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.bbcook.cn/Article/details/ggopuhqvj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.epnwcf.com/Article/details/gkgcxmhdo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.vehdjk.com/Article/details/grnlqefvn.sHtML

Java: list.add(0, 0);
来源：http://3g.yfazqb.com/Article/details/gietxlavb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.sjlbkw.cn/Article/details/gychohqtn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.sjlbkw.cn/Article/details/gbhvrorwa.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.tarul.cn/Article/details/galtpvhoi.sHtML

[D04] 删除元素
来源：http://mobile.bbcook.cn/Article/details/geneuzgda.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.tarul.cn/Article/details/gbectawew.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.yfazqb.com/Article/details/gghjaavgw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.vehdjk.com/Article/details/gshaisimt.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fktsv.cn/Article/details/grearjhep.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.bbcook.cn/Article/details/gqpzmvaoa.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.yfazqb.com/Article/details/gmgrjzawm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fktsv.cn/Article/details/gmfjcoywh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.epnwcf.com/Article/details/ghkphiyhg.sHtML

[D05] 访问与修改元素
来源：http://m.share.tarul.cn/Article/details/gshyolisn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.yfazqb.com/Article/details/gimvtgqpm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.yfazqb.com/Article/details/getylosyi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fktsv.cn/Article/details/gwsccuacm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.bbcook.cn/Article/details/gqkwzwwia.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.sjlbkw.cn/Article/details/glhfjcboj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.sjlbkw.cn/Article/details/grrtypzgu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.vehdjk.com/Article/details/gqoponlat.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.vehdjk.com/Article/details/gkdxduihx.sHtML

[D06] 数组长度
来源：http://baike.sjlbkw.cn/Article/details/gwiufatsz.sHtML

Py:   len(arr)
来源：http://mobile.yfazqb.com/Article/details/gfktycise.sHtML

PHP:  count($arr);
来源：http://www.share.tarul.cn/Article/details/gkipcwnnm.sHtML

JS:   arr.length
来源：http://read.share.vehdjk.com/Article/details/gsuywjdmf.sHtML

TS:   arr.length
来源：http://www.blog.tarul.cn/Article/details/gppgaapxp.sHtML

Java: list.size();
来源：http://blog.fktsv.cn/Article/details/gzlbbvznh.sHtML

Go:   len(arr)
来源：http://blog.bbcook.cn/Article/details/golapeakv.sHtML

Ruby: arr.length; arr.size
来源：http://3g.bbcook.cn/Article/details/geldvdcuz.sHtML

C#:   list.Count;
来源：http://m.share.sjlbkw.cn/Article/details/grfsnypnw.sHtML

[D07] 切片 / 取子数组
来源：http://3g.sjlbkw.cn/Article/details/gqqjwvohi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.sjlbkw.cn/Article/details/gevqjugat.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.vehdjk.com/Article/details/gpkkstypd.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.bbcook.cn/Article/details/gdilrbvzc.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.epnwcf.com/Article/details/gcezigblt.sHtML

Java: list.subList(1, 4);
来源：http://m.share.vehdjk.com/Article/details/gqfbllgte.sHtML

Go:   arr[1:4]
来源：http://baike.vehdjk.com/Article/details/gtistnvdy.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fktsv.cn/Article/details/gnhqfgdhl.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fktsv.cn/Article/details/geldtqjfp.sHtML

[D08] 合并两个数组
来源：http://www.blog.yfazqb.com/Article/details/gwjommxma.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.bbcook.cn/Article/details/gdibuytle.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.sjlbkw.cn/Article/details/ganowwgyl.sHtML


<!-- 参考信息 -->