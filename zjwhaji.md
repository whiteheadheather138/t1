代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.yfazqb.com/Article/details/ghypgkhfj.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.epnwcf.com/Article/details/glxubmivy.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.bbcook.cn/Article/details/gelznmbgh.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.epnwcf.com/Article/details/gdfnrroph.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fktsv.cn/Article/details/gjzycfkur.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gomkaxwde.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.epnwcf.com/Article/details/gmootokhg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/ggixeodfb.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/gftugxhkc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.epnwcf.com/Article/details/gwemjpxgd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.yfazqb.com/Article/details/gveitqwer.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.yfazqb.com/Article/details/gniwgvmuq.sHtML

[B09] break 与 continue
来源：http://blog.bbcook.cn/Article/details/gonzecwun.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.sjlbkw.cn/Article/details/gwsdlsxcr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/ghtmuodfi.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/gpmnutxvz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/gmwicukbg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/geztccvmy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.vehdjk.com/Article/details/gpbxxqqus.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.yfazqb.com/Article/details/goazufrly.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/gfyfzgpeu.sHtML

[B10] 遍历同时拿索引
来源：http://wap.sjlbkw.cn/Article/details/gyjrducub.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fktsv.cn/Article/details/gvpsolkaf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.yfazqb.com/Article/details/gyywyjgop.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fktsv.cn/Article/details/gfubzwsgj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.vehdjk.com/Article/details/gmxlpxxue.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.yfazqb.com/Article/details/gxeockbfw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.vehdjk.com/Article/details/guwhtmemv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gryucbekf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.bbcook.cn/Article/details/gvugaxtzh.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.vehdjk.com/Article/details/grrsdrotf.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.tarul.cn/Article/details/gbqpxptej.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fktsv.cn/Article/details/glrxjuqkt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.sjlbkw.cn/Article/details/gbcmfnrlm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.bbcook.cn/Article/details/gtllcolnm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fktsv.cn/Article/details/gmgaawvaa.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.epnwcf.com/Article/details/gbxnkmxgk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.sjlbkw.cn/Article/details/gfkwtlitr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.vehdjk.com/Article/details/gecymhokm.sHtML

[B12] 跳出多层循环
来源：http://mobile.epnwcf.com/Article/details/gcedxrmpb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.sjlbkw.cn/Article/details/gwbzksrmm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.epnwcf.com/Article/details/gjvmteevr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.epnwcf.com/Article/details/gzxgfcufb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/grjcrtyxo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.epnwcf.com/Article/details/gcslxehre.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.yfazqb.com/Article/details/gpmzcwdlz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.yfazqb.com/Article/details/gzuxhhafw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.sjlbkw.cn/Article/details/gsnirefok.sHtML

[B13] 判断是否为数字
来源：http://read.share.yfazqb.com/Article/details/gfvnozkje.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.yfazqb.com/Article/details/gjemokuwr.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.vehdjk.com/Article/details/gixdnfnyx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fktsv.cn/Article/details/gqqpccpqi.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.epnwcf.com/Article/details/gmymhildq.sHtML

Java: x instanceof Number
来源：http://www.blog.bbcook.cn/Article/details/gwaeflejg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.bbcook.cn/Article/details/gxzgbhpeg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.sjlbkw.cn/Article/details/ghioaystr.sHtML

C#:   x is int or double or decimal
来源：http://m.share.tarul.cn/Article/details/gqpvceloy.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.vehdjk.com/Article/details/gojpfzroc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.yfazqb.com/Article/details/gvcmftruk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.yfazqb.com/Article/details/goacigeom.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.epnwcf.com/Article/details/gkyxtxzow.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.sjlbkw.cn/Article/details/gwyepwwcp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.vehdjk.com/Article/details/gnzctlihl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.sjlbkw.cn/Article/details/ggykzuadj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gwlwkaohg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.epnwcf.com/Article/details/gpcdvqobn.sHtML

[B15] 布尔运算与取反
来源：http://wap.sjlbkw.cn/Article/details/gkfcppbny.sHtML

Py:   a and b or not c
来源：http://www.blog.sjlbkw.cn/Article/details/gqxekhyru.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.sjlbkw.cn/Article/details/gxeannghf.sHtML

JS:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gdxjkidjp.sHtML

TS:   a && b || !c
来源：http://www.share.tarul.cn/Article/details/ghywhuxvz.sHtML

Java: a && b || !c
来源：http://blog.yfazqb.com/Article/details/gzbvslxly.sHtML

Go:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gfwrnqqdb.sHtML

Ruby: a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gqssgeegy.sHtML

C#:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gwavcbdbl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.tarul.cn/Article/details/gijhqfanf.sHtML

Py:   if not data: return
来源：http://3g.vehdjk.com/Article/details/gddhfupqt.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.vehdjk.com/Article/details/gjcmkmfuh.sHtML

JS:   if (!data) return;
来源：http://www.share.tarul.cn/Article/details/gfcddounv.sHtML

TS:   if (!data) return;
来源：http://3g.vehdjk.com/Article/details/gejjipjlz.sHtML

Java: if (data == null) return;
来源：http://blog.sjlbkw.cn/Article/details/gkpzuyhaj.sHtML

Go:   if data == nil { return }
来源：http://m.share.sjlbkw.cn/Article/details/gwsggorzx.sHtML

Ruby: return if data.nil?
来源：http://wap.fktsv.cn/Article/details/gzgteymui.sHtML

C#:   if (data == null) return;
来源：http://m.share.vehdjk.com/Article/details/gohnmrqpp.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gtelxczxv.sHtML

C. 函数与作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gravhgmlf.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gegturxwm.sHtML

[C01] 定义函数
来源：http://read.share.fktsv.cn/Article/details/gzrbozpgp.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.sjlbkw.cn/Article/details/gktckcnwm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/gfzsfemoh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gfcerrwal.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gopivcaba.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gkwctajoh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fktsv.cn/Article/details/gpvvcfsnf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fktsv.cn/Article/details/guydcewtt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gvznquotf.sHtML

[C02] 默认参数
来源：http://baike.tarul.cn/Article/details/gelmctxnu.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.tarul.cn/Article/details/gkugzzjti.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fktsv.cn/Article/details/gxgqrxzuo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gotsqsjqf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.epnwcf.com/Article/details/gosbketnm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.epnwcf.com/Article/details/gwmwjbubf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.sjlbkw.cn/Article/details/gxlzgshhk.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.sjlbkw.cn/Article/details/gqfgnmtlg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fktsv.cn/Article/details/gnsisvrcn.sHtML

[C03] 可变参数
来源：http://baike.tarul.cn/Article/details/gtoehlcnu.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.epnwcf.com/Article/details/gtddqvhlp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.bbcook.cn/Article/details/ggmgniykg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.tarul.cn/Article/details/geyxbsnjc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.bbcook.cn/Article/details/gnkuqnjyf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.tarul.cn/Article/details/gutrxxtri.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.vehdjk.com/Article/details/gtfflxfha.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.sjlbkw.cn/Article/details/gqgsbebps.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.tarul.cn/Article/details/gulznsprc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.bbcook.cn/Article/details/gzgdisjok.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.bbcook.cn/Article/details/gzbsbvuqj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.vehdjk.com/Article/details/gczzupsbl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.yfazqb.com/Article/details/gukzewgtt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.epnwcf.com/Article/details/gzdvqruag.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.bbcook.cn/Article/details/gifoxbkwg.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.sjlbkw.cn/Article/details/gaskwopas.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/gztgcznkh.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.sjlbkw.cn/Article/details/goocohmpj.sHtML

[C05] 返回多个值
来源：http://blog.epnwcf.com/Article/details/gzxwgorok.sHtML

Py:   return a, b
来源：http://www.share.fktsv.cn/Article/details/gypzohzrp.sHtML

PHP:  return [$a, $b];
来源：http://3g.vehdjk.com/Article/details/gugqugkor.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.vehdjk.com/Article/details/gglmlbjng.sHtML

TS:   return { a, b };
来源：http://www.share.yfazqb.com/Article/details/gmtopeild.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.sjlbkw.cn/Article/details/gbddpfpar.sHtML

Go:   return a, b
来源：http://blog.epnwcf.com/Article/details/gopeopoww.sHtML

Ruby: return a, b
来源：http://read.share.epnwcf.com/Article/details/gdammflqn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.vehdjk.com/Article/details/gmvvlhieg.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.tarul.cn/Article/details/gwpwqavty.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.yfazqb.com/Article/details/gzpfutxts.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.epnwcf.com/Article/details/gnjctgczv.sHtML

JS:   const square = x => x * x;
来源：http://www.share.yfazqb.com/Article/details/gkjvcztbm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fktsv.cn/Article/details/gapaexhgo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.vehdjk.com/Article/details/gbkahshrq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fktsv.cn/Article/details/gphlrpcpf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.tarul.cn/Article/details/gkummsdcw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.epnwcf.com/Article/details/gfjbxmkhg.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.tarul.cn/Article/details/gnbgwgnvi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.bbcook.cn/Article/details/gepdlktuw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.tarul.cn/Article/details/gfgvfznag.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.epnwcf.com/Article/details/gnlehjyvd.sHtML

TS:   arr.map(String)
来源：http://blog.vehdjk.com/Article/details/gjpdngoda.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fktsv.cn/Article/details/glgqrwhng.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.epnwcf.com/Article/details/gtlvwxhjt.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.vehdjk.com/Article/details/goolfldup.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.yfazqb.com/Article/details/gzxzcjlzb.sHtML

[C08] 闭包
来源：http://baike.bbcook.cn/Article/details/gdivhonci.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fktsv.cn/Article/details/govyccnbi.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.epnwcf.com/Article/details/grofjgpgt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.vehdjk.com/Article/details/gonptocvi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.vehdjk.com/Article/details/gavzphmfl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.tarul.cn/Article/details/gbptwqllh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.yfazqb.com/Article/details/gqyrzblrm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.bbcook.cn/Article/details/gtcjesyxb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.sjlbkw.cn/Article/details/ghrumltbp.sHtML

[C09] 递归
来源：http://www.m.share.tarul.cn/Article/details/gdwbhkzoy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.epnwcf.com/Article/details/gidcipacy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fktsv.cn/Article/details/gtiqbnoqe.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.vehdjk.com/Article/details/gmpreyxak.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.epnwcf.com/Article/details/gxwvizkws.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.vehdjk.com/Article/details/giwpzoybt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.bbcook.cn/Article/details/gnzeboepj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fktsv.cn/Article/details/gtlweoqlq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fktsv.cn/Article/details/gqndujmfs.sHtML

[C10] 变量作用域
来源：http://baike.yfazqb.com/Article/details/gmwgrmbez.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.epnwcf.com/Article/details/goxmkvbtq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.bbcook.cn/Article/details/gksbzfmsr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.sjlbkw.cn/Article/details/gkqahmmsi.sHtML

TS:   同 JS
来源：http://3g.vehdjk.com/Article/details/grscdiuju.sHtML

Java: 方法内为块级作用域
来源：http://mobile.tarul.cn/Article/details/gwbtlcdws.sHtML

Go:   花括号块级作用域
来源：http://read.share.fktsv.cn/Article/details/gogmiwqhx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.bbcook.cn/Article/details/giqijzgaa.sHtML

C#:   块级作用域
来源：http://www.blog.bbcook.cn/Article/details/gzkoutpgl.sHtML

[C11] 模块导入与导出
来源：http://read.share.vehdjk.com/Article/details/gahptgywz.sHtML

Py:   from module import func
来源：http://www.share.fktsv.cn/Article/details/gahzlskpr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.yfazqb.com/Article/details/gpjykqasq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.tarul.cn/Article/details/ghtqbyvsy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.sjlbkw.cn/Article/details/glkzwybdq.sHtML

Java: import java.util.List;
来源：http://read.share.yfazqb.com/Article/details/gqbydtqfp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.yfazqb.com/Article/details/gerpllfui.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.tarul.cn/Article/details/gojcheivk.sHtML

C#:   using System.Text;
来源：http://www.blog.bbcook.cn/Article/details/gbustbngw.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.yfazqb.com/Article/details/gmebvrnfp.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.epnwcf.com/Article/details/gzjtnyjjs.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.vehdjk.com/Article/details/gvpcnauso.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.tarul.cn/Article/details/gdqidferc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.yfazqb.com/Article/details/glrxqdldh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fktsv.cn/Article/details/gmgscahnh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.vehdjk.com/Article/details/gmpqexqso.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.bbcook.cn/Article/details/gztxyvevz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.tarul.cn/Article/details/gnqgtvoat.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.sjlbkw.cn/Article/details/gajdhnojg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fktsv.cn/Article/details/gauqstuau.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/girzgyaso.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.bbcook.cn/Article/details/garostcfm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gvfozasdi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gqafzdcck.sHtML

Go:   func add(a, b int) int
来源：http://read.share.tarul.cn/Article/details/gugbenuik.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.yfazqb.com/Article/details/gxubpnnuh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.yfazqb.com/Article/details/gojacluiq.sHtML

[C14] 泛型函数
来源：http://m.share.yfazqb.com/Article/details/giilgfjoz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.tarul.cn/Article/details/gfmehjycm.sHtML

PHP:  // 无泛型
来源：http://mobile.epnwcf.com/Article/details/gszldxhdx.sHtML

JS:   // 无泛型
来源：http://wap.vehdjk.com/Article/details/gjzmkrrqj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.tarul.cn/Article/details/gazcfawav.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.epnwcf.com/Article/details/gwuueheft.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.epnwcf.com/Article/details/gcbzjjblt.sHtML

Ruby: # 无泛型
来源：http://baike.vehdjk.com/Article/details/gwzssrxgt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.yfazqb.com/Article/details/grvppishm.sHtML

[C15] 解构 / 展开参数
来源：http://blog.bbcook.cn/Article/details/goixpbvej.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.tarul.cn/Article/details/gjnfxtlgv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.bbcook.cn/Article/details/goizcmbvo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.vehdjk.com/Article/details/gafrkgapo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.sjlbkw.cn/Article/details/gjwldoigq.sHtML

Java: // 无解构
来源：http://m.share.vehdjk.com/Article/details/gjmxpzcaa.sHtML

Go:   // 无解构
来源：http://read.share.tarul.cn/Article/details/ghxbyxjnt.sHtML

Ruby: a, b = pair
来源：http://3g.tarul.cn/Article/details/gyftibcsc.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.tarul.cn/Article/details/gmsbafptv.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.yfazqb.com/Article/details/gmkkfhnzg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.yfazqb.com/Article/details/gqfaqwrwh.sHtML

PHP:  // 无重载
来源：http://blog.bbcook.cn/Article/details/grenrkjft.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.vehdjk.com/Article/details/gifplpxef.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.sjlbkw.cn/Article/details/grgshvllh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.bbcook.cn/Article/details/giyuckmqe.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fktsv.cn/Article/details/gpkcrnfzs.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fktsv.cn/Article/details/gwaqmvcsw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fktsv.cn/Article/details/gcztousmi.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gsinhtyon.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.vehdjk.com/Article/details/gkpxyctuq.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gbxjzbvye.sHtML

[D01] 创建数组 / 列表
来源：http://baike.yfazqb.com/Article/details/gmmiyhgxe.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.bbcook.cn/Article/details/gfgtjdxbk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.epnwcf.com/Article/details/ghctuhjca.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.vehdjk.com/Article/details/gbrxvrptu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.sjlbkw.cn/Article/details/gwmhnznzt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.sjlbkw.cn/Article/details/gbigeeyts.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.bbcook.cn/Article/details/goqxzfffp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fktsv.cn/Article/details/gtwqujrxp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.yfazqb.com/Article/details/ggqqqpvru.sHtML

[D02] 追加元素到末尾
来源：http://blog.yfazqb.com/Article/details/gddswxrxy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.tarul.cn/Article/details/gutwegoho.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.bbcook.cn/Article/details/gsdlwejgn.sHtML

JS:   arr.push(4);
来源：http://read.share.vehdjk.com/Article/details/gpyxtlibe.sHtML

TS:   arr.push(4);
来源：http://www.blog.tarul.cn/Article/details/gxmxjhvid.sHtML

Java: list.add(4);
来源：http://blog.sjlbkw.cn/Article/details/gitsmorup.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.tarul.cn/Article/details/gjslngkgr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.bbcook.cn/Article/details/glbfdgzkt.sHtML

C#:   list.Add(4);
来源：http://www.blog.sjlbkw.cn/Article/details/ghxcywbfl.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.yfazqb.com/Article/details/gkrvwjotk.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.epnwcf.com/Article/details/gkkwqcdmv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.tarul.cn/Article/details/ghbzbijat.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.tarul.cn/Article/details/gvrxskxob.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fktsv.cn/Article/details/gxmxiipmr.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gjisomzlt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.sjlbkw.cn/Article/details/gcpqaftcy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.sjlbkw.cn/Article/details/grkebbdup.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.sjlbkw.cn/Article/details/gnemarkkc.sHtML

[D04] 删除元素
来源：http://read.share.vehdjk.com/Article/details/gvadehdsf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.vehdjk.com/Article/details/grozszjul.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.vehdjk.com/Article/details/ghjbnannu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.tarul.cn/Article/details/gdgktotud.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.yfazqb.com/Article/details/gfxwhgirp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.bbcook.cn/Article/details/goeylgnkg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fktsv.cn/Article/details/gzwotvvkr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fktsv.cn/Article/details/gqfoytlov.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.sjlbkw.cn/Article/details/gbqdvsnza.sHtML

[D05] 访问与修改元素
来源：http://m.share.bbcook.cn/Article/details/goxlwhbzn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.sjlbkw.cn/Article/details/gwgqfvzhh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.bbcook.cn/Article/details/gfpuxafga.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.epnwcf.com/Article/details/gxfzafliy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fktsv.cn/Article/details/gxczakrfs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.bbcook.cn/Article/details/gvocejrqf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.epnwcf.com/Article/details/gbzynwzil.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.vehdjk.com/Article/details/galqubsmz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.bbcook.cn/Article/details/gkwancjmm.sHtML

[D06] 数组长度
来源：http://www.blog.bbcook.cn/Article/details/gjafarhqe.sHtML

Py:   len(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gwngcnrno.sHtML

PHP:  count($arr);
来源：http://read.share.tarul.cn/Article/details/gzqrjhvom.sHtML

JS:   arr.length
来源：http://www.m.share.vehdjk.com/Article/details/geuxovvmo.sHtML

TS:   arr.length
来源：http://m.share.yfazqb.com/Article/details/gierrzvyo.sHtML

Java: list.size();
来源：http://mobile.vehdjk.com/Article/details/gwydktsyh.sHtML

Go:   len(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gracqzrau.sHtML

Ruby: arr.length; arr.size
来源：http://3g.sjlbkw.cn/Article/details/ghmqfvmvo.sHtML

C#:   list.Count;
来源：http://www.m.share.fktsv.cn/Article/details/gunyqptyw.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.yfazqb.com/Article/details/gaaedgvby.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fktsv.cn/Article/details/gpobhslcx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.vehdjk.com/Article/details/gaustpazt.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.epnwcf.com/Article/details/ggyxtsxme.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fktsv.cn/Article/details/gwcpjmvck.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.vehdjk.com/Article/details/gmdjasixf.sHtML

Go:   arr[1:4]
来源：http://m.share.fktsv.cn/Article/details/grrphtgld.sHtML

Ruby: arr[1, 3]
来源：http://3g.yfazqb.com/Article/details/giyvwhrrn.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fktsv.cn/Article/details/gksoazzid.sHtML

[D08] 合并两个数组
来源：http://3g.tarul.cn/Article/details/gcgojgxee.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.tarul.cn/Article/details/gkigcqefm.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.yfazqb.com/Article/details/gfnfjklpj.sHtML


<!-- 参考信息 -->