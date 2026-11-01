代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://mobile.bbcook.cn/Article/details/gmytvtopp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/guzhekspj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/grntvlysr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gqjsumflb.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhuuvelk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.yfazqb.com/Article/details/gdcngrqbj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.epnwcf.com/Article/details/gsdqvhsqe.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.epnwcf.com/Article/details/gfngcdffe.sHtML

[B09] break 与 continue
来源：http://baike.epnwcf.com/Article/details/gbcjiihvt.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.sjlbkw.cn/Article/details/gepyesklv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/gexvmjdhy.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gykfcnccv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/gviamubhp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gerfgkboh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.bbcook.cn/Article/details/gdhzlthqy.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbvqsqnzl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.tarul.cn/Article/details/gkkqgepyo.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.sjlbkw.cn/Article/details/gnxqczpap.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.tarul.cn/Article/details/gbtusbjvn.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.sjlbkw.cn/Article/details/gcnpdqqoi.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fktsv.cn/Article/details/gnltvqinv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.bbcook.cn/Article/details/gslnbshoj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.bbcook.cn/Article/details/gvnabmruw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.tarul.cn/Article/details/ggprymrvo.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.epnwcf.com/Article/details/giyinntao.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.sjlbkw.cn/Article/details/gakwpderf.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.vehdjk.com/Article/details/gjzllqwym.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.sjlbkw.cn/Article/details/ghthjrmpk.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.bbcook.cn/Article/details/gtpoqtmut.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.bbcook.cn/Article/details/ggsatfszt.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.yfazqb.com/Article/details/guplxkocv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.bbcook.cn/Article/details/gxvtxnqvy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.tarul.cn/Article/details/gjrajqekr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.bbcook.cn/Article/details/grzliytng.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fktsv.cn/Article/details/ghvqnzgjp.sHtML

[B12] 跳出多层循环
来源：http://www.blog.vehdjk.com/Article/details/gopmtltaa.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.yfazqb.com/Article/details/gbjnvbpel.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fktsv.cn/Article/details/grsgerfof.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/gaggmznwx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.tarul.cn/Article/details/gyattiign.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fktsv.cn/Article/details/gejhtbrsd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.epnwcf.com/Article/details/gbpiabsnr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.tarul.cn/Article/details/gixdrdfxs.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.epnwcf.com/Article/details/gzmoyquyy.sHtML

[B13] 判断是否为数字
来源：http://m.share.tarul.cn/Article/details/glhhqaghx.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.bbcook.cn/Article/details/guqlqbypc.sHtML

PHP:  is_numeric($x)
来源：http://blog.tarul.cn/Article/details/gbymwuyew.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fktsv.cn/Article/details/glqvxndoi.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.vehdjk.com/Article/details/goatkfbbz.sHtML

Java: x instanceof Number
来源：http://www.share.fktsv.cn/Article/details/gmbkpyext.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.epnwcf.com/Article/details/gjkawzqaz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fktsv.cn/Article/details/gzcivcfoi.sHtML

C#:   x is int or double or decimal
来源：http://blog.yfazqb.com/Article/details/grdscbvzf.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwyctrag.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.tarul.cn/Article/details/gdadxzvol.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.sjlbkw.cn/Article/details/gayetulmr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.sjlbkw.cn/Article/details/gvamjvqup.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/gqbgbvehb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.epnwcf.com/Article/details/gtysczadu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.bbcook.cn/Article/details/ginqvwqbt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fktsv.cn/Article/details/grhjnolya.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.bbcook.cn/Article/details/gyoctnhoq.sHtML

[B15] 布尔运算与取反
来源：http://wap.fktsv.cn/Article/details/guafhwmuo.sHtML

Py:   a and b or not c
来源：http://www.share.tarul.cn/Article/details/gaqztthyw.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fktsv.cn/Article/details/gjzdvyoxk.sHtML

JS:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gwkvkomrb.sHtML

TS:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gsrztwiou.sHtML

Java: a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gizjjardd.sHtML

Go:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/glyeticwy.sHtML

Ruby: a && b || !c
来源：http://baike.fktsv.cn/Article/details/gmihbnjvg.sHtML

C#:   a && b || !c
来源：http://blog.vehdjk.com/Article/details/grhctzvpo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.vehdjk.com/Article/details/gcvqgdgfe.sHtML

Py:   if not data: return
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbzhipmu.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.vehdjk.com/Article/details/gosqmvzkv.sHtML

JS:   if (!data) return;
来源：http://baike.yfazqb.com/Article/details/giryrkofu.sHtML

TS:   if (!data) return;
来源：http://m.share.sjlbkw.cn/Article/details/glerocgnz.sHtML

Java: if (data == null) return;
来源：http://blog.tarul.cn/Article/details/ggkpdyjvm.sHtML

Go:   if data == nil { return }
来源：http://m.share.tarul.cn/Article/details/glqggckyf.sHtML

Ruby: return if data.nil?
来源：http://mobile.epnwcf.com/Article/details/gdnwnygfa.sHtML

C#:   if (data == null) return;
来源：http://read.share.yfazqb.com/Article/details/gxipyklhc.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gmgymzpsx.sHtML

C. 函数与作用域
来源：http://3g.fktsv.cn/Article/details/gbemfecjd.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gxhggwaoz.sHtML

[C01] 定义函数
来源：http://www.blog.fktsv.cn/Article/details/gzzvzrjuk.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.sjlbkw.cn/Article/details/gvphpvmlk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.epnwcf.com/Article/details/gdsnwyrzw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gsvkqwpxn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gexipnnwm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/ggafgkole.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.epnwcf.com/Article/details/gbxttnxzc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.tarul.cn/Article/details/gxwaymkrw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gdnimthkm.sHtML

[C02] 默认参数
来源：http://read.share.fktsv.cn/Article/details/gylfjsgyg.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.sjlbkw.cn/Article/details/gfzqrqbwn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.bbcook.cn/Article/details/gdwplghti.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.epnwcf.com/Article/details/ghhhtitdc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gqhqamtsz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.tarul.cn/Article/details/gtgdlqebq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.sjlbkw.cn/Article/details/glzsjnwfj.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.bbcook.cn/Article/details/gbtfhpjuj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.epnwcf.com/Article/details/gktklfevx.sHtML

[C03] 可变参数
来源：http://wap.vehdjk.com/Article/details/gsrmquejb.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbkzenipw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.sjlbkw.cn/Article/details/gyjuszaeu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.sjlbkw.cn/Article/details/gkqgostzg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.sjlbkw.cn/Article/details/gfitgqgzg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gphtqxnol.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.epnwcf.com/Article/details/gbhjnajtf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fktsv.cn/Article/details/gomhkjtjw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.tarul.cn/Article/details/geooyvmyl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.bbcook.cn/Article/details/gthmwfsdr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.bbcook.cn/Article/details/gpwqbgulm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.vehdjk.com/Article/details/goggovuzn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.yfazqb.com/Article/details/gapppukqu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.bbcook.cn/Article/details/gngezgnay.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.vehdjk.com/Article/details/gxngyaqsu.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.vehdjk.com/Article/details/geeksylob.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/gqcouigpf.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/gchypwlls.sHtML

[C05] 返回多个值
来源：http://m.share.bbcook.cn/Article/details/gsgugftcz.sHtML

Py:   return a, b
来源：http://baike.vehdjk.com/Article/details/glfvxitin.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fktsv.cn/Article/details/gepynrfps.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.epnwcf.com/Article/details/gfwppelto.sHtML

TS:   return { a, b };
来源：http://mobile.fktsv.cn/Article/details/gionovvch.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.epnwcf.com/Article/details/gcurgkgyo.sHtML

Go:   return a, b
来源：http://www.m.share.vehdjk.com/Article/details/ghkhqczsj.sHtML

Ruby: return a, b
来源：http://read.share.epnwcf.com/Article/details/gjnylilpe.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.epnwcf.com/Article/details/gplbyweck.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.bbcook.cn/Article/details/gyfojqwrq.sHtML

Py:   square = lambda x: x * x
来源：http://baike.tarul.cn/Article/details/gpjajxafz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.sjlbkw.cn/Article/details/gzsboagbq.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.vehdjk.com/Article/details/gkupjifvn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fktsv.cn/Article/details/gfsgbwurs.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.yfazqb.com/Article/details/gkgieerdt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.tarul.cn/Article/details/glmfxvizn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.bbcook.cn/Article/details/gvqkibmwm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fktsv.cn/Article/details/ghpkppoqz.sHtML

[C07] 把函数作为参数传入
来源：http://blog.sjlbkw.cn/Article/details/gqwzfgbuj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.vehdjk.com/Article/details/gurgnvtib.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.sjlbkw.cn/Article/details/gzmbpeyww.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.sjlbkw.cn/Article/details/gwjmuprxb.sHtML

TS:   arr.map(String)
来源：http://blog.tarul.cn/Article/details/glnzlygzc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gukhvrszl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.vehdjk.com/Article/details/gxuqmybwe.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.yfazqb.com/Article/details/gomrpjjlg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fktsv.cn/Article/details/gkedoifki.sHtML

[C08] 闭包
来源：http://blog.bbcook.cn/Article/details/gfkridcex.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fktsv.cn/Article/details/gdvjewklx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.yfazqb.com/Article/details/ghtefmznb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.vehdjk.com/Article/details/gbewyfmcc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.bbcook.cn/Article/details/gbzwpovmb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fktsv.cn/Article/details/gtmvpoeqw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.yfazqb.com/Article/details/gnuiazcyg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.epnwcf.com/Article/details/grzteysxc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.vehdjk.com/Article/details/gwahuinhn.sHtML

[C09] 递归
来源：http://3g.bbcook.cn/Article/details/gbikfxecm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.bbcook.cn/Article/details/ggetwbopw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.yfazqb.com/Article/details/gxalptqrk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.yfazqb.com/Article/details/gaegcjzeh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.tarul.cn/Article/details/ghovtfziy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.epnwcf.com/Article/details/gjoxrnafc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.bbcook.cn/Article/details/gcacjqzkj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.bbcook.cn/Article/details/gagnkpblu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.epnwcf.com/Article/details/gshsqinke.sHtML

[C10] 变量作用域
来源：http://read.share.vehdjk.com/Article/details/gvwnvbiot.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.yfazqb.com/Article/details/gzbyfseen.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.vehdjk.com/Article/details/gelxdntsm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.vehdjk.com/Article/details/goylanomo.sHtML

TS:   同 JS
来源：http://mobile.sjlbkw.cn/Article/details/gkhiclloq.sHtML

Java: 方法内为块级作用域
来源：http://m.share.tarul.cn/Article/details/gxibuyyqn.sHtML

Go:   花括号块级作用域
来源：http://mobile.sjlbkw.cn/Article/details/gykzlxwfv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fktsv.cn/Article/details/gzospslqq.sHtML

C#:   块级作用域
来源：http://www.share.vehdjk.com/Article/details/gwfieqkbk.sHtML

[C11] 模块导入与导出
来源：http://mobile.fktsv.cn/Article/details/gwevsbghg.sHtML

Py:   from module import func
来源：http://mobile.tarul.cn/Article/details/gfwyqmllv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.bbcook.cn/Article/details/gqpbqitcj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fktsv.cn/Article/details/gggnejbew.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.tarul.cn/Article/details/gsrlwsakk.sHtML

Java: import java.util.List;
来源：http://www.blog.yfazqb.com/Article/details/gztyuuhfw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fktsv.cn/Article/details/gwvnpilvw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.yfazqb.com/Article/details/gjvoriede.sHtML

C#:   using System.Text;
来源：http://baike.sjlbkw.cn/Article/details/gtcxacpxy.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.vehdjk.com/Article/details/gcdycwtln.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.bbcook.cn/Article/details/gzcxbulne.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.tarul.cn/Article/details/gbolavgue.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fktsv.cn/Article/details/gutyfnafi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.sjlbkw.cn/Article/details/gyyxouzdf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.bbcook.cn/Article/details/gwtpbugni.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.yfazqb.com/Article/details/gdatymcpi.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.epnwcf.com/Article/details/gaxcczbht.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.yfazqb.com/Article/details/gnzegnkwi.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.yfazqb.com/Article/details/ghmzumshw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.bbcook.cn/Article/details/gmjmwybav.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.epnwcf.com/Article/details/ghqrrunbh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.sjlbkw.cn/Article/details/glbhzdwhv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/giworswez.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gmmrwiyzq.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.tarul.cn/Article/details/gfixrrtsj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fktsv.cn/Article/details/ghuherlvm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.bbcook.cn/Article/details/gctgydwqx.sHtML

[C14] 泛型函数
来源：http://3g.vehdjk.com/Article/details/gcvjxixog.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.sjlbkw.cn/Article/details/grwtznogb.sHtML

PHP:  // 无泛型
来源：http://3g.sjlbkw.cn/Article/details/grvfwkqvv.sHtML

JS:   // 无泛型
来源：http://mobile.bbcook.cn/Article/details/gpyjatvzx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.bbcook.cn/Article/details/gdsktoiir.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.yfazqb.com/Article/details/ghefoalaj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fktsv.cn/Article/details/gljtjyljx.sHtML

Ruby: # 无泛型
来源：http://wap.vehdjk.com/Article/details/gxjvaiqed.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.bbcook.cn/Article/details/gpckqvavv.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.vehdjk.com/Article/details/gaaowalxt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.sjlbkw.cn/Article/details/gtkxsqxsr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.sjlbkw.cn/Article/details/gwjuzwktk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.epnwcf.com/Article/details/gcocannxz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fktsv.cn/Article/details/gulpwlpwk.sHtML

Java: // 无解构
来源：http://m.share.vehdjk.com/Article/details/gvfgnvurd.sHtML

Go:   // 无解构
来源：http://blog.fktsv.cn/Article/details/gtkgpcvxe.sHtML

Ruby: a, b = pair
来源：http://www.blog.fktsv.cn/Article/details/gqxmzmlsx.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fktsv.cn/Article/details/gqpxjxagg.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.tarul.cn/Article/details/gevypibli.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.epnwcf.com/Article/details/gyenblwks.sHtML

PHP:  // 无重载
来源：http://blog.fktsv.cn/Article/details/gmoitvlfk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.sjlbkw.cn/Article/details/gmvhufyqd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.sjlbkw.cn/Article/details/grjjuqcci.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.yfazqb.com/Article/details/gcjrzyead.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.epnwcf.com/Article/details/gbuvcnnhy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.vehdjk.com/Article/details/gekrwgsht.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.tarul.cn/Article/details/gefvpmubr.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gvggtdxau.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.bbcook.cn/Article/details/gfvcztaat.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gaagyhxvv.sHtML

[D01] 创建数组 / 列表
来源：http://3g.yfazqb.com/Article/details/gndurfzkz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.sjlbkw.cn/Article/details/ggpsdnrso.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.sjlbkw.cn/Article/details/gxgpchvil.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.epnwcf.com/Article/details/gurnsmfmi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.sjlbkw.cn/Article/details/gaubsfrgd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.yfazqb.com/Article/details/gasjtddxn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.sjlbkw.cn/Article/details/gmygkbqdf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.yfazqb.com/Article/details/grxgdnjwm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.tarul.cn/Article/details/gdcrdyzmn.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.vehdjk.com/Article/details/ggnysweyd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.yfazqb.com/Article/details/gcieufomf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.epnwcf.com/Article/details/gdkdmohiw.sHtML

JS:   arr.push(4);
来源：http://m.share.fktsv.cn/Article/details/gytufrctn.sHtML

TS:   arr.push(4);
来源：http://www.blog.yfazqb.com/Article/details/gxfzvbzwv.sHtML

Java: list.add(4);
来源：http://www.share.fktsv.cn/Article/details/gccvbkcgf.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.yfazqb.com/Article/details/gmhvpkdaw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.tarul.cn/Article/details/gbjorxggb.sHtML

C#:   list.Add(4);
来源：http://www.share.bbcook.cn/Article/details/gtybehhft.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.tarul.cn/Article/details/gwhyobxoa.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gcwqiiskh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.epnwcf.com/Article/details/gcvyogsag.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwkqlydp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.bbcook.cn/Article/details/gbdxbxmih.sHtML

Java: list.add(0, 0);
来源：http://mobile.bbcook.cn/Article/details/ghjngzqub.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.bbcook.cn/Article/details/gqzftyrdb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.yfazqb.com/Article/details/gfirmrour.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gxqhhmgrf.sHtML

[D04] 删除元素
来源：http://www.m.share.epnwcf.com/Article/details/gnfledwaw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fktsv.cn/Article/details/gsexibssb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.bbcook.cn/Article/details/gyyhkscsu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.yfazqb.com/Article/details/gcykqwzbi.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.yfazqb.com/Article/details/gxhczduuk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.vehdjk.com/Article/details/gamvlsuuc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.tarul.cn/Article/details/guxlaofpi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fktsv.cn/Article/details/gmzyfyrmy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.tarul.cn/Article/details/ghxnqwwxg.sHtML

[D05] 访问与修改元素
来源：http://3g.epnwcf.com/Article/details/gocpowxxu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.epnwcf.com/Article/details/gacworrkt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.vehdjk.com/Article/details/geppeeben.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fktsv.cn/Article/details/gsnauqelf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fktsv.cn/Article/details/gmqmiqvem.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.vehdjk.com/Article/details/gdtdmrsug.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.vehdjk.com/Article/details/geitzoiml.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.sjlbkw.cn/Article/details/gspuucyqd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.vehdjk.com/Article/details/gutnewspw.sHtML

[D06] 数组长度
来源：http://baike.vehdjk.com/Article/details/gdqctqicz.sHtML

Py:   len(arr)
来源：http://baike.vehdjk.com/Article/details/gkndlxgcu.sHtML

PHP:  count($arr);
来源：http://mobile.fktsv.cn/Article/details/gsaxjandq.sHtML

JS:   arr.length
来源：http://baike.epnwcf.com/Article/details/grvohcboe.sHtML

TS:   arr.length
来源：http://3g.bbcook.cn/Article/details/gotmsiijo.sHtML

Java: list.size();
来源：http://3g.sjlbkw.cn/Article/details/ghlaphjvj.sHtML

Go:   len(arr)
来源：http://baike.tarul.cn/Article/details/gfixoiegt.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.sjlbkw.cn/Article/details/gxgqsdomz.sHtML

C#:   list.Count;
来源：http://wap.fktsv.cn/Article/details/gedztwhaw.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fktsv.cn/Article/details/gmocqrpyb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.tarul.cn/Article/details/gddmexzbs.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.tarul.cn/Article/details/gwrsunosf.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.yfazqb.com/Article/details/gkfkhlqqw.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.vehdjk.com/Article/details/gofesttul.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.yfazqb.com/Article/details/ghzqoakyq.sHtML

Go:   arr[1:4]
来源：http://baike.bbcook.cn/Article/details/gycmavstz.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.bbcook.cn/Article/details/gsgnyoobw.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.vehdjk.com/Article/details/glvgnhaoi.sHtML

[D08] 合并两个数组
来源：http://wap.epnwcf.com/Article/details/gelooajld.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.sjlbkw.cn/Article/details/gbjvzurpe.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.bbcook.cn/Article/details/goindabqn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.sjlbkw.cn/Article/details/gpggaikux.sHtML

TS:   [...a, ...b];
来源：http://wap.fktsv.cn/Article/details/gnrwqeglg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.vehdjk.com/Article/details/gkougiujo.sHtML

Go:   append(a, b...)
来源：http://baike.epnwcf.com/Article/details/gnylvdffj.sHtML


<!-- 参考信息 -->