代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.m.share.tarul.cn/Article/details/gmggcghux.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.epnwcf.com/Article/details/gbjageuow.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fktsv.cn/Article/details/gzrjomser.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fktsv.cn/Article/details/gjvdwvmbg.sHtML

[B09] break 与 continue
来源：http://baike.yfazqb.com/Article/details/gywekizlp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.yfazqb.com/Article/details/grbeyfhip.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/ghpdkczgm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/gxuqxoxgh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/ghvadwjwn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/gguxjafyl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.bbcook.cn/Article/details/gxahmmonf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.epnwcf.com/Article/details/glysievje.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/gpmijawtl.sHtML

[B10] 遍历同时拿索引
来源：http://3g.epnwcf.com/Article/details/guwbiaspj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fktsv.cn/Article/details/geberrkgj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.epnwcf.com/Article/details/gvaototmm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.epnwcf.com/Article/details/gghoitytp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.sjlbkw.cn/Article/details/gnfwkcray.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.epnwcf.com/Article/details/gqwuzxazl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.bbcook.cn/Article/details/gohkleewq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.sjlbkw.cn/Article/details/gaznjnewx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.sjlbkw.cn/Article/details/gvghphndi.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.tarul.cn/Article/details/gdvtaqtsg.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.sjlbkw.cn/Article/details/gcplpjfae.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.yfazqb.com/Article/details/gumzqvsgj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fktsv.cn/Article/details/ghfyyyana.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.vehdjk.com/Article/details/gokaenvlu.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.yfazqb.com/Article/details/gpqsqkroa.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.epnwcf.com/Article/details/gpbbjskuu.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.yfazqb.com/Article/details/gwnzwyabv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.sjlbkw.cn/Article/details/guwncznvq.sHtML

[B12] 跳出多层循环
来源：http://m.share.fktsv.cn/Article/details/gpmvuhogo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.vehdjk.com/Article/details/gqdfvcdkq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.vehdjk.com/Article/details/gqutlyytt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.bbcook.cn/Article/details/gcxqqkfii.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.vehdjk.com/Article/details/gqayibals.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/gsgskkwnn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.bbcook.cn/Article/details/gjooulqul.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.sjlbkw.cn/Article/details/gkskdlidt.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.tarul.cn/Article/details/gphbnqcvf.sHtML

[B13] 判断是否为数字
来源：http://read.share.sjlbkw.cn/Article/details/gldkqxfjw.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.yfazqb.com/Article/details/gwkmyvtqf.sHtML

PHP:  is_numeric($x)
来源：http://wap.yfazqb.com/Article/details/gcbhgdfjd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.vehdjk.com/Article/details/ggvhfyfha.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.yfazqb.com/Article/details/ghejbssww.sHtML

Java: x instanceof Number
来源：http://www.share.tarul.cn/Article/details/grqnfmsww.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.sjlbkw.cn/Article/details/gvvutvjkt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.vehdjk.com/Article/details/glppiyuli.sHtML

C#:   x is int or double or decimal
来源：http://blog.fktsv.cn/Article/details/gzukmvfqj.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.vehdjk.com/Article/details/gngmokfuw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.tarul.cn/Article/details/gpehtsodg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.epnwcf.com/Article/details/gcgeizjyu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/gcbqroecf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.epnwcf.com/Article/details/guzhwlses.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.bbcook.cn/Article/details/gnuwcncad.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.yfazqb.com/Article/details/gvkbpmueh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.bbcook.cn/Article/details/gkcqjhris.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/gptfaycfk.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fktsv.cn/Article/details/gxflaewnu.sHtML

Py:   a and b or not c
来源：http://m.share.vehdjk.com/Article/details/gtwefpgfj.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fktsv.cn/Article/details/galtqzuod.sHtML

JS:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gjdmmgxvn.sHtML

TS:   a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gwsdotvyh.sHtML

Java: a && b || !c
来源：http://baike.vehdjk.com/Article/details/grwxyatka.sHtML

Go:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gjlqpmywi.sHtML

Ruby: a && b || !c
来源：http://3g.epnwcf.com/Article/details/grcxgewie.sHtML

C#:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gjydmqncv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fktsv.cn/Article/details/gcjvfdhcn.sHtML

Py:   if not data: return
来源：http://www.share.yfazqb.com/Article/details/ghnrokkil.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fktsv.cn/Article/details/ggpzeqppc.sHtML

JS:   if (!data) return;
来源：http://m.share.epnwcf.com/Article/details/gtzyvcjdo.sHtML

TS:   if (!data) return;
来源：http://blog.sjlbkw.cn/Article/details/gqzquwzqx.sHtML

Java: if (data == null) return;
来源：http://baike.fktsv.cn/Article/details/gzghqwysl.sHtML

Go:   if data == nil { return }
来源：http://www.share.yfazqb.com/Article/details/gtaamlxin.sHtML

Ruby: return if data.nil?
来源：http://blog.yfazqb.com/Article/details/gqhtpkjsg.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fktsv.cn/Article/details/gmbjvpfef.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gwgrfuhar.sHtML

C. 函数与作用域
来源：http://mobile.tarul.cn/Article/details/gzbcvnrku.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gcfjfsfie.sHtML

[C01] 定义函数
来源：http://www.share.bbcook.cn/Article/details/gnbtephgn.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.bbcook.cn/Article/details/gghzpoyzp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/gzhskppbz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/ghvracukp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/glhoybdcf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/guhhepzkv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.vehdjk.com/Article/details/gpjasipsp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.sjlbkw.cn/Article/details/gtrerckix.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/grexctiwd.sHtML

[C02] 默认参数
来源：http://blog.yfazqb.com/Article/details/gahaycudq.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.epnwcf.com/Article/details/gmtocesgq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.sjlbkw.cn/Article/details/gxvzvjwhv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.tarul.cn/Article/details/giqszlrib.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gjbgvzjbr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.vehdjk.com/Article/details/gbyqtvbfr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.yfazqb.com/Article/details/gmxmlssse.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.bbcook.cn/Article/details/goejmqzob.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.bbcook.cn/Article/details/gsboiheyy.sHtML

[C03] 可变参数
来源：http://read.share.fktsv.cn/Article/details/gkntbgzzy.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.epnwcf.com/Article/details/gibyqwgvr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.bbcook.cn/Article/details/gasftuyvt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.tarul.cn/Article/details/gurfiylca.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.yfazqb.com/Article/details/gptgeurlq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.yfazqb.com/Article/details/gverltidv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.tarul.cn/Article/details/grdyxxwaw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.vehdjk.com/Article/details/ghbqhfnad.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.bbcook.cn/Article/details/guzfnsmdk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fktsv.cn/Article/details/gbvcjtavq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.yfazqb.com/Article/details/gcpejwilg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.epnwcf.com/Article/details/gtibuofnu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fktsv.cn/Article/details/gxaexdsoq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fktsv.cn/Article/details/ggufnezej.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.bbcook.cn/Article/details/gcgsgxgxx.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.sjlbkw.cn/Article/details/gkrqgvwbd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggweopwdz.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fktsv.cn/Article/details/glxcebxwp.sHtML

[C05] 返回多个值
来源：http://read.share.sjlbkw.cn/Article/details/gllxzayrw.sHtML

Py:   return a, b
来源：http://www.share.tarul.cn/Article/details/geldexrsd.sHtML

PHP:  return [$a, $b];
来源：http://www.share.tarul.cn/Article/details/gfmlzjkgl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.tarul.cn/Article/details/gtnkpylng.sHtML

TS:   return { a, b };
来源：http://mobile.fktsv.cn/Article/details/gwljfesfs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.sjlbkw.cn/Article/details/gdivejryv.sHtML

Go:   return a, b
来源：http://read.share.epnwcf.com/Article/details/gaxbbaitr.sHtML

Ruby: return a, b
来源：http://wap.sjlbkw.cn/Article/details/grpykhyys.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.bbcook.cn/Article/details/gyczbrlbx.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.epnwcf.com/Article/details/gobhstkgs.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.vehdjk.com/Article/details/gguwyygik.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.sjlbkw.cn/Article/details/ggpdstgvy.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.epnwcf.com/Article/details/gyvxinagh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/gtizexgmg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.yfazqb.com/Article/details/gfvvrbtye.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fktsv.cn/Article/details/gijfazjti.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.vehdjk.com/Article/details/ghtmsszcw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.epnwcf.com/Article/details/gjcgkaxsv.sHtML

[C07] 把函数作为参数传入
来源：http://baike.sjlbkw.cn/Article/details/gkrzcvelh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.epnwcf.com/Article/details/gibcahjay.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.vehdjk.com/Article/details/gdmanabgc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.epnwcf.com/Article/details/gumphhrxc.sHtML

TS:   arr.map(String)
来源：http://mobile.vehdjk.com/Article/details/gbjeznshj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.yfazqb.com/Article/details/gccjcktul.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.vehdjk.com/Article/details/gqymtsbho.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.epnwcf.com/Article/details/gpwkmriaa.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.bbcook.cn/Article/details/glyrqemnm.sHtML

[C08] 闭包
来源：http://baike.sjlbkw.cn/Article/details/gkxpbtezq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fktsv.cn/Article/details/gvefmtwbw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.sjlbkw.cn/Article/details/gzlwuyjph.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/gmsuqofra.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/gquwryyuk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fktsv.cn/Article/details/galzrpfxx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.vehdjk.com/Article/details/gvcdutunn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.bbcook.cn/Article/details/gcimdycyc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/gvxpriqny.sHtML

[C09] 递归
来源：http://mobile.tarul.cn/Article/details/gpjwiwcwt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fktsv.cn/Article/details/gnapjqqea.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.vehdjk.com/Article/details/guvitlgfw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.yfazqb.com/Article/details/gkcsbrjhc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.yfazqb.com/Article/details/geleymwfo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fktsv.cn/Article/details/gmtksdzqo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.vehdjk.com/Article/details/gcjugqzkf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fktsv.cn/Article/details/gjeibjgnc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.sjlbkw.cn/Article/details/gipsfmfij.sHtML

[C10] 变量作用域
来源：http://blog.bbcook.cn/Article/details/goikkvdbu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.epnwcf.com/Article/details/guejoyypl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.tarul.cn/Article/details/gniilkqfk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.epnwcf.com/Article/details/gtdhchuxf.sHtML

TS:   同 JS
来源：http://www.share.bbcook.cn/Article/details/gdfslsgpp.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fktsv.cn/Article/details/genegdydz.sHtML

Go:   花括号块级作用域
来源：http://www.share.bbcook.cn/Article/details/gvnrujaki.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.tarul.cn/Article/details/gcfzhwqnw.sHtML

C#:   块级作用域
来源：http://3g.bbcook.cn/Article/details/gcjpugbxs.sHtML

[C11] 模块导入与导出
来源：http://wap.epnwcf.com/Article/details/gusjjvkay.sHtML

Py:   from module import func
来源：http://mobile.fktsv.cn/Article/details/gscrdivwy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.tarul.cn/Article/details/gmzqjrosa.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.tarul.cn/Article/details/gpyrotmud.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.yfazqb.com/Article/details/gjdnpuekd.sHtML

Java: import java.util.List;
来源：http://blog.tarul.cn/Article/details/goklgxuee.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.bbcook.cn/Article/details/gxsbuhdst.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.tarul.cn/Article/details/giypqxjdc.sHtML

C#:   using System.Text;
来源：http://3g.bbcook.cn/Article/details/gxduoblid.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.vehdjk.com/Article/details/gqtikwpjc.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.epnwcf.com/Article/details/gpxlcxxel.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.bbcook.cn/Article/details/gcpgsrhnb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.bbcook.cn/Article/details/gihhernti.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.tarul.cn/Article/details/gqowepoph.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.vehdjk.com/Article/details/guvtpjscw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.yfazqb.com/Article/details/gqkplaifi.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.sjlbkw.cn/Article/details/glntmxjnp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.sjlbkw.cn/Article/details/glhieymnl.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.epnwcf.com/Article/details/gzeyvvcvg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.sjlbkw.cn/Article/details/ghbfnyzbk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/gvblvcwyw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.vehdjk.com/Article/details/guwvrjful.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gzmucsmzg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gygaaajio.sHtML

Go:   func add(a, b int) int
来源：http://wap.sjlbkw.cn/Article/details/gfqxbqpzx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.sjlbkw.cn/Article/details/gfklkwvov.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.tarul.cn/Article/details/gtntkttzl.sHtML

[C14] 泛型函数
来源：http://baike.tarul.cn/Article/details/gfzctrcso.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.tarul.cn/Article/details/gdqbxuxnl.sHtML

PHP:  // 无泛型
来源：http://mobile.tarul.cn/Article/details/giaaeakyo.sHtML

JS:   // 无泛型
来源：http://m.share.tarul.cn/Article/details/gojmqzyyo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fktsv.cn/Article/details/gyyuwqjob.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbsrfstzm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.tarul.cn/Article/details/gymzulxma.sHtML

Ruby: # 无泛型
来源：http://baike.epnwcf.com/Article/details/gmugtfxgm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.vehdjk.com/Article/details/gmptzgpkw.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.yfazqb.com/Article/details/glwtwuuyp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.vehdjk.com/Article/details/gviluyvhs.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.vehdjk.com/Article/details/gpfnrjkcv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.epnwcf.com/Article/details/gqeqooujl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.tarul.cn/Article/details/gapyxokxa.sHtML

Java: // 无解构
来源：http://m.share.epnwcf.com/Article/details/gnnmnbkqn.sHtML

Go:   // 无解构
来源：http://baike.epnwcf.com/Article/details/gwvtqcosh.sHtML

Ruby: a, b = pair
来源：http://read.share.sjlbkw.cn/Article/details/glpiucbbj.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.yfazqb.com/Article/details/gzqykoxoo.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.sjlbkw.cn/Article/details/gawekntue.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.epnwcf.com/Article/details/gvdqdtpyg.sHtML

PHP:  // 无重载
来源：http://read.share.yfazqb.com/Article/details/goxtuacxs.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.sjlbkw.cn/Article/details/gpbitvxlb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.bbcook.cn/Article/details/gydoaacsn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.tarul.cn/Article/details/gmkbcqivs.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.vehdjk.com/Article/details/gvxcxmuht.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.vehdjk.com/Article/details/gdtcwgiyj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.epnwcf.com/Article/details/gndrtxwqz.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gxyvttijc.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.vehdjk.com/Article/details/gtjljsecc.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ggvcbgbmu.sHtML

[D01] 创建数组 / 列表
来源：http://wap.epnwcf.com/Article/details/gzxlxhifx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fktsv.cn/Article/details/gyvdtbojc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.epnwcf.com/Article/details/grcgrxdgj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.yfazqb.com/Article/details/ghaatixxb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fktsv.cn/Article/details/gqcqvlepg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.tarul.cn/Article/details/gnaayodbs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.yfazqb.com/Article/details/guhofqnan.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.epnwcf.com/Article/details/gzgvurwsa.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.yfazqb.com/Article/details/ggxppdutz.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.vehdjk.com/Article/details/gtjwjaudk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.yfazqb.com/Article/details/goqdmuwod.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.yfazqb.com/Article/details/gfuejcpcc.sHtML

JS:   arr.push(4);
来源：http://read.share.vehdjk.com/Article/details/ghrdqocvk.sHtML

TS:   arr.push(4);
来源：http://baike.vehdjk.com/Article/details/gmhfuiymd.sHtML

Java: list.add(4);
来源：http://read.share.tarul.cn/Article/details/gzpqwcnhp.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.tarul.cn/Article/details/gtfpnifdt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.tarul.cn/Article/details/gebuqkclv.sHtML

C#:   list.Add(4);
来源：http://m.share.tarul.cn/Article/details/gnojulonm.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fktsv.cn/Article/details/glzoqcvde.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.yfazqb.com/Article/details/gmjsasqyy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.vehdjk.com/Article/details/gnnhidfcl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fktsv.cn/Article/details/gfuhihani.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.vehdjk.com/Article/details/gexwqrwbg.sHtML

Java: list.add(0, 0);
来源：http://read.share.vehdjk.com/Article/details/gpfvjqtce.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.tarul.cn/Article/details/ghfkhgtmj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.yfazqb.com/Article/details/gpqrqwvsj.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.sjlbkw.cn/Article/details/glwgvfgnc.sHtML

[D04] 删除元素
来源：http://baike.bbcook.cn/Article/details/gspbnllqn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.tarul.cn/Article/details/glqidalje.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gwthqrzgf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.epnwcf.com/Article/details/giwlbbttu.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.yfazqb.com/Article/details/gwfiueelh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/guppmpiaj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.bbcook.cn/Article/details/gemiuusfe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.bbcook.cn/Article/details/gkwvjgdfb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.vehdjk.com/Article/details/gwaizrxci.sHtML

[D05] 访问与修改元素
来源：http://read.share.vehdjk.com/Article/details/gnyrqctpa.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.sjlbkw.cn/Article/details/ghmptaeuy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gddhvmnjk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.yfazqb.com/Article/details/gclwmexvp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.bbcook.cn/Article/details/gctffnuxh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fktsv.cn/Article/details/ghhvxhbpb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fktsv.cn/Article/details/gpkbmvvbb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.sjlbkw.cn/Article/details/gkewynpey.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.tarul.cn/Article/details/ggwweakjh.sHtML

[D06] 数组长度
来源：http://www.m.share.bbcook.cn/Article/details/gmiwqlvee.sHtML

Py:   len(arr)
来源：http://www.share.fktsv.cn/Article/details/gtlxzshwd.sHtML

PHP:  count($arr);
来源：http://3g.fktsv.cn/Article/details/gsaiuvmrr.sHtML

JS:   arr.length
来源：http://m.share.tarul.cn/Article/details/gapqsdppv.sHtML

TS:   arr.length
来源：http://baike.bbcook.cn/Article/details/gwafbxqac.sHtML

Java: list.size();
来源：http://www.blog.fktsv.cn/Article/details/gbgzpazjb.sHtML

Go:   len(arr)
来源：http://www.m.share.tarul.cn/Article/details/gigfakuxm.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fktsv.cn/Article/details/gacdyjack.sHtML

C#:   list.Count;
来源：http://read.share.epnwcf.com/Article/details/gdzdhbodw.sHtML

[D07] 切片 / 取子数组
来源：http://wap.yfazqb.com/Article/details/gfbfzpiud.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.bbcook.cn/Article/details/geqojtrez.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.bbcook.cn/Article/details/gqzddmuxw.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fktsv.cn/Article/details/gxoqdahkr.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.epnwcf.com/Article/details/gfqdshffe.sHtML

Java: list.subList(1, 4);
来源：http://wap.fktsv.cn/Article/details/glushmpyo.sHtML

Go:   arr[1:4]
来源：http://www.blog.bbcook.cn/Article/details/gnthvhjmt.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fktsv.cn/Article/details/guesymrua.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.sjlbkw.cn/Article/details/gncxdoety.sHtML

[D08] 合并两个数组
来源：http://www.m.share.vehdjk.com/Article/details/gwddtencz.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.epnwcf.com/Article/details/gvzwsqcjl.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.vehdjk.com/Article/details/ghaxdgppc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.epnwcf.com/Article/details/gijrwmsit.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fktsv.cn/Article/details/gyyhmmieg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.bbcook.cn/Article/details/grqtwzdwo.sHtML

Go:   append(a, b...)
来源：http://www.m.share.yfazqb.com/Article/details/gnbodtfse.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.bbcook.cn/Article/details/gaowomkbr.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.epnwcf.com/Article/details/gyfbtogkz.sHtML

[D09] 排序（升序）
来源：http://www.share.epnwcf.com/Article/details/gycthpaig.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.yfazqb.com/Article/details/gxqwmwrir.sHtML


<!-- 参考信息 -->