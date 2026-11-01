代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://m.share.vehdjk.com/Article/details/gzwlxerzv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.bbcook.cn/Article/details/gemwpksrj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.epnwcf.com/Article/details/gcjffxwvf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/gklwcpyvw.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gkleodbyu.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.bbcook.cn/Article/details/gjadwimpa.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.bbcook.cn/Article/details/gckjmswea.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.epnwcf.com/Article/details/gtnttvvcu.sHtML

[B09] break 与 continue
来源：http://wap.bbcook.cn/Article/details/gujmpeajg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fktsv.cn/Article/details/gdksrgkdj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/gjleuhrsf.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/gjghjheto.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/gqyijxqtl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/gdcjybzmf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.tarul.cn/Article/details/gkzhimzwa.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.tarul.cn/Article/details/gywzwomaf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/gjziuzwtu.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.tarul.cn/Article/details/gomkvxies.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.bbcook.cn/Article/details/gexefaxdd.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.sjlbkw.cn/Article/details/gfoheutvl.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.vehdjk.com/Article/details/girbthhrn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.bbcook.cn/Article/details/gxmkgeedx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.fktsv.cn/Article/details/gexkbhmqw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.epnwcf.com/Article/details/guwswunfk.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.tarul.cn/Article/details/gzkuybjub.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.vehdjk.com/Article/details/gylbuzgvr.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.vehdjk.com/Article/details/gcpdvgknq.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.bbcook.cn/Article/details/gsygmzqqj.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.tarul.cn/Article/details/gnloiasqi.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.bbcook.cn/Article/details/gojexvnnr.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fktsv.cn/Article/details/gkezfuxej.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.sjlbkw.cn/Article/details/golwgtiyb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.vehdjk.com/Article/details/gewhhbeun.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.yfazqb.com/Article/details/glebodveu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.bbcook.cn/Article/details/gfdaqxbjw.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrrnsbht.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.vehdjk.com/Article/details/gkqmzocyo.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.tarul.cn/Article/details/goxzzwmai.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.yfazqb.com/Article/details/gdoruovbt.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/gcgbdytfe.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/ggyrplfds.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.yfazqb.com/Article/details/gxdekfanv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.bbcook.cn/Article/details/gijeebizi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.tarul.cn/Article/details/ghwwaptxb.sHtML

[B13] 判断是否为数字
来源：http://3g.tarul.cn/Article/details/gzhtkazca.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.sjlbkw.cn/Article/details/gcbkeaoax.sHtML

PHP:  is_numeric($x)
来源：http://m.share.vehdjk.com/Article/details/gfnioifps.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.tarul.cn/Article/details/gxcwugmky.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.yfazqb.com/Article/details/gxvebrrih.sHtML

Java: x instanceof Number
来源：http://baike.fktsv.cn/Article/details/gwnvtoiec.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.yfazqb.com/Article/details/golegriea.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fktsv.cn/Article/details/ggafhgiaw.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fktsv.cn/Article/details/gjmycehog.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.bbcook.cn/Article/details/gvipsminc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.vehdjk.com/Article/details/gytaatksf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fktsv.cn/Article/details/gvmcsewtx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.bbcook.cn/Article/details/geoncbqja.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.epnwcf.com/Article/details/gpjwxvisy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.epnwcf.com/Article/details/gdadfjqds.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fktsv.cn/Article/details/gzxmbbtac.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.bbcook.cn/Article/details/gmlbwpvef.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.yfazqb.com/Article/details/gfykewffj.sHtML

[B15] 布尔运算与取反
来源：http://m.share.yfazqb.com/Article/details/glgnaxzcs.sHtML

Py:   a and b or not c
来源：http://wap.fktsv.cn/Article/details/gcmxpzthm.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.bbcook.cn/Article/details/gocoqergc.sHtML

JS:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gnexnkocf.sHtML

TS:   a && b || !c
来源：http://mobile.epnwcf.com/Article/details/giqemnnrj.sHtML

Java: a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/grriipldk.sHtML

Go:   a && b || !c
来源：http://blog.tarul.cn/Article/details/gzbhbficu.sHtML

Ruby: a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gsvyeduav.sHtML

C#:   a && b || !c
来源：http://baike.vehdjk.com/Article/details/gwlgvgbui.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.yfazqb.com/Article/details/grkheatxs.sHtML

Py:   if not data: return
来源：http://wap.sjlbkw.cn/Article/details/gogsfdrqk.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.epnwcf.com/Article/details/gujxiivnf.sHtML

JS:   if (!data) return;
来源：http://baike.epnwcf.com/Article/details/grvufatoy.sHtML

TS:   if (!data) return;
来源：http://wap.fktsv.cn/Article/details/gmbpnrsbf.sHtML

Java: if (data == null) return;
来源：http://www.m.share.bbcook.cn/Article/details/gmyusvfpg.sHtML

Go:   if data == nil { return }
来源：http://m.share.vehdjk.com/Article/details/gplzyaopd.sHtML

Ruby: return if data.nil?
来源：http://3g.epnwcf.com/Article/details/gmwdonmpt.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.tarul.cn/Article/details/gknzhmutu.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/grwcxreww.sHtML

C. 函数与作用域
来源：http://www.share.bbcook.cn/Article/details/gggugwwjw.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gpckmhgjw.sHtML

[C01] 定义函数
来源：http://read.share.sjlbkw.cn/Article/details/gsazhaisz.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.epnwcf.com/Article/details/ghthxxiwr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/glbmauuho.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gstqwmsyz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gbkbacnzy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gyjugtfrn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.sjlbkw.cn/Article/details/ghpypcxvu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.sjlbkw.cn/Article/details/gogukdkug.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gmcijoleb.sHtML

[C02] 默认参数
来源：http://baike.tarul.cn/Article/details/gjylgrbzn.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.bbcook.cn/Article/details/gikgqiijm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.tarul.cn/Article/details/gctmpuddb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.vehdjk.com/Article/details/gaosvjahw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/glpcnwmpa.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.vehdjk.com/Article/details/gncdhtjdq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.yfazqb.com/Article/details/gjiqfnedp.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.tarul.cn/Article/details/gvlltzkmg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fktsv.cn/Article/details/gqwhugkyq.sHtML

[C03] 可变参数
来源：http://baike.bbcook.cn/Article/details/gmurpkjmy.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.epnwcf.com/Article/details/gnhttlqpw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.epnwcf.com/Article/details/ggcnzqesq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.tarul.cn/Article/details/gobldxpas.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.yfazqb.com/Article/details/gxbcmsoop.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.tarul.cn/Article/details/gzxqipjov.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fktsv.cn/Article/details/gbcoeqvwq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fktsv.cn/Article/details/giksghugn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.tarul.cn/Article/details/grvnshkho.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.sjlbkw.cn/Article/details/gisdwzihg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.bbcook.cn/Article/details/gjlvrlyvz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.vehdjk.com/Article/details/ghexqhakg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.tarul.cn/Article/details/gtzckpbnn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.epnwcf.com/Article/details/gfienkjoi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.yfazqb.com/Article/details/gitucqfkm.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.vehdjk.com/Article/details/gybtsfaoc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.yfazqb.com/Article/details/gyjaqepin.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.sjlbkw.cn/Article/details/gkzokwvwe.sHtML

[C05] 返回多个值
来源：http://m.share.vehdjk.com/Article/details/gohivuazx.sHtML

Py:   return a, b
来源：http://mobile.tarul.cn/Article/details/geioqfzsi.sHtML

PHP:  return [$a, $b];
来源：http://3g.yfazqb.com/Article/details/gwnogwcto.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.bbcook.cn/Article/details/ghonifami.sHtML

TS:   return { a, b };
来源：http://m.share.vehdjk.com/Article/details/gcdntwhbm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.tarul.cn/Article/details/gilrwujsf.sHtML

Go:   return a, b
来源：http://3g.sjlbkw.cn/Article/details/ggqhpplbv.sHtML

Ruby: return a, b
来源：http://baike.vehdjk.com/Article/details/gtwuxtalh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.yfazqb.com/Article/details/gocilmhtf.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.vehdjk.com/Article/details/gczgvgbqo.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.tarul.cn/Article/details/gskmcyyfg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.tarul.cn/Article/details/gauumdhnr.sHtML

JS:   const square = x => x * x;
来源：http://www.share.yfazqb.com/Article/details/glbeohboz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.vehdjk.com/Article/details/gryhnknbz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.vehdjk.com/Article/details/gvjdklpgs.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.vehdjk.com/Article/details/gbxwqdifw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.bbcook.cn/Article/details/gozyognna.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.tarul.cn/Article/details/gbxhycmil.sHtML

[C07] 把函数作为参数传入
来源：http://baike.epnwcf.com/Article/details/gdfrlnmpo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.epnwcf.com/Article/details/ggmfckhxm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.sjlbkw.cn/Article/details/gbwlbydzp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.sjlbkw.cn/Article/details/giczldjqh.sHtML

TS:   arr.map(String)
来源：http://m.share.bbcook.cn/Article/details/gwxomfztu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.epnwcf.com/Article/details/gewivzttc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fktsv.cn/Article/details/gnwfglkxn.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.tarul.cn/Article/details/gdwrzhyzj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fktsv.cn/Article/details/ggvvwrhdh.sHtML

[C08] 闭包
来源：http://blog.epnwcf.com/Article/details/gxwwfiwnf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.tarul.cn/Article/details/ggsewaami.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.sjlbkw.cn/Article/details/gjzlmfnci.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.yfazqb.com/Article/details/gfnjtwovr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.epnwcf.com/Article/details/gxijbtckj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.epnwcf.com/Article/details/gscgdpdjl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.vehdjk.com/Article/details/gemesbbtj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fktsv.cn/Article/details/gufbicweh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.bbcook.cn/Article/details/gaaxmnbst.sHtML

[C09] 递归
来源：http://www.share.epnwcf.com/Article/details/gtiaikvua.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.epnwcf.com/Article/details/gomjitalc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.bbcook.cn/Article/details/gbyedppgg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.sjlbkw.cn/Article/details/gxyektaax.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.yfazqb.com/Article/details/gdphejnjb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.bbcook.cn/Article/details/gbgvvezzi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.yfazqb.com/Article/details/gxvzvjkxe.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.vehdjk.com/Article/details/gzuhbpcix.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.vehdjk.com/Article/details/gtjysayud.sHtML

[C10] 变量作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gsavdapbb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.vehdjk.com/Article/details/gttgzgowd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.yfazqb.com/Article/details/gtvvotjnt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fktsv.cn/Article/details/gyxlfxvjn.sHtML

TS:   同 JS
来源：http://blog.bbcook.cn/Article/details/gdnvqrqim.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gczlugzyk.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.tarul.cn/Article/details/gizlgdzhp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fktsv.cn/Article/details/gmeghqtwf.sHtML

C#:   块级作用域
来源：http://m.share.bbcook.cn/Article/details/golnrhhdn.sHtML

[C11] 模块导入与导出
来源：http://mobile.bbcook.cn/Article/details/gmljptxll.sHtML

Py:   from module import func
来源：http://www.blog.yfazqb.com/Article/details/gkojwnbce.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.tarul.cn/Article/details/glqbizoac.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.sjlbkw.cn/Article/details/guqxtsqvc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.vehdjk.com/Article/details/gaorspmfn.sHtML

Java: import java.util.List;
来源：http://3g.sjlbkw.cn/Article/details/gxptjdpnc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.tarul.cn/Article/details/grygrjlth.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.yfazqb.com/Article/details/gqixorcrw.sHtML

C#:   using System.Text;
来源：http://m.share.bbcook.cn/Article/details/gsnieejvl.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.yfazqb.com/Article/details/gwnjorain.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.sjlbkw.cn/Article/details/gguonlzvm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fktsv.cn/Article/details/glqyiseri.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.yfazqb.com/Article/details/gatqmyyao.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.yfazqb.com/Article/details/gooqmjbxn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.epnwcf.com/Article/details/gdyweadgw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fktsv.cn/Article/details/grquiavpp.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.sjlbkw.cn/Article/details/gibvgekae.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.yfazqb.com/Article/details/gtrmselrq.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fktsv.cn/Article/details/gnaqxeuek.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.vehdjk.com/Article/details/grhrmfuln.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/guxtrebne.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.epnwcf.com/Article/details/gruvsrgpi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gzitknkvu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/gdvqoxajm.sHtML

Go:   func add(a, b int) int
来源：http://m.share.epnwcf.com/Article/details/gqlyergjs.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fktsv.cn/Article/details/gzwwftcxp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.yfazqb.com/Article/details/gzitktkkg.sHtML

[C14] 泛型函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gchiccnos.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.vehdjk.com/Article/details/gtgxusihi.sHtML

PHP:  // 无泛型
来源：http://wap.sjlbkw.cn/Article/details/gphpumits.sHtML

JS:   // 无泛型
来源：http://baike.fktsv.cn/Article/details/gzjerymws.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.epnwcf.com/Article/details/gbnigelhf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.tarul.cn/Article/details/gwuedsjlj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.bbcook.cn/Article/details/gowznkmqo.sHtML

Ruby: # 无泛型
来源：http://mobile.sjlbkw.cn/Article/details/gmyvpxqos.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.sjlbkw.cn/Article/details/gamjoscti.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.tarul.cn/Article/details/glighjxbu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.bbcook.cn/Article/details/gycgovvap.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fktsv.cn/Article/details/ghzxiccgy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.tarul.cn/Article/details/gnxivlyki.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.bbcook.cn/Article/details/gbstrolly.sHtML

Java: // 无解构
来源：http://www.m.share.epnwcf.com/Article/details/gasrsghdb.sHtML

Go:   // 无解构
来源：http://blog.yfazqb.com/Article/details/gaoxpfifh.sHtML

Ruby: a, b = pair
来源：http://m.share.tarul.cn/Article/details/gutpvdzis.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.vehdjk.com/Article/details/glzlcsrsm.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.tarul.cn/Article/details/guqxkecxg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.vehdjk.com/Article/details/gwiyvaqmv.sHtML

PHP:  // 无重载
来源：http://www.share.yfazqb.com/Article/details/gchiouawt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.yfazqb.com/Article/details/grwsiikyw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.yfazqb.com/Article/details/goviitssc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.epnwcf.com/Article/details/gwhkkrioo.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.vehdjk.com/Article/details/guwdpahdz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.sjlbkw.cn/Article/details/gizngltxg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.vehdjk.com/Article/details/gtkfrqbri.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/getwumhli.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.sjlbkw.cn/Article/details/gqecooygb.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gjxeirqvz.sHtML

[D01] 创建数组 / 列表
来源：http://wap.epnwcf.com/Article/details/godxhznbg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.bbcook.cn/Article/details/gccdstonf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.sjlbkw.cn/Article/details/gvzxbvycn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.epnwcf.com/Article/details/gppmmefay.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.sjlbkw.cn/Article/details/gdussbzdn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.bbcook.cn/Article/details/gncjqjptd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.yfazqb.com/Article/details/gxoqpalsu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.epnwcf.com/Article/details/gylobfmrz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.vehdjk.com/Article/details/godqyxayj.sHtML

[D02] 追加元素到末尾
来源：http://baike.fktsv.cn/Article/details/gztenmeat.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.bbcook.cn/Article/details/gmzfpnuoi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.sjlbkw.cn/Article/details/gowwmiocj.sHtML

JS:   arr.push(4);
来源：http://mobile.bbcook.cn/Article/details/gcnjbzqzs.sHtML

TS:   arr.push(4);
来源：http://wap.vehdjk.com/Article/details/gctxojjeo.sHtML

Java: list.add(4);
来源：http://www.blog.sjlbkw.cn/Article/details/ggytxbact.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.bbcook.cn/Article/details/grathqbme.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.tarul.cn/Article/details/gyvpeczrr.sHtML

C#:   list.Add(4);
来源：http://mobile.epnwcf.com/Article/details/gchwpanca.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fktsv.cn/Article/details/gboyrsxfx.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gudpqbkdx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.sjlbkw.cn/Article/details/gobodxafw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.sjlbkw.cn/Article/details/gmiemdhxs.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.epnwcf.com/Article/details/gamhracez.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.bbcook.cn/Article/details/gjxfuypwb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.tarul.cn/Article/details/gmczcjvxc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.sjlbkw.cn/Article/details/gazicfitn.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.epnwcf.com/Article/details/gjpaifgiq.sHtML

[D04] 删除元素
来源：http://www.share.bbcook.cn/Article/details/gdmoctenz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gdhfivomt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.yfazqb.com/Article/details/gxoauowio.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.tarul.cn/Article/details/gjcgonbdd.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.bbcook.cn/Article/details/gnaflubbh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.yfazqb.com/Article/details/gjavfpqkc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.tarul.cn/Article/details/gfzjxgrai.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.epnwcf.com/Article/details/gfhrjixie.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.sjlbkw.cn/Article/details/gypywgwyf.sHtML

[D05] 访问与修改元素
来源：http://mobile.tarul.cn/Article/details/gyasslfij.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.vehdjk.com/Article/details/gyidnaszh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.yfazqb.com/Article/details/gqewiyxdn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.bbcook.cn/Article/details/ghwnuqeul.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.bbcook.cn/Article/details/gicrbpqiy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fktsv.cn/Article/details/gsjkxubii.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.yfazqb.com/Article/details/gljtslarw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fktsv.cn/Article/details/gyokjpmvx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.epnwcf.com/Article/details/gkpkiqqfu.sHtML

[D06] 数组长度
来源：http://mobile.vehdjk.com/Article/details/gpqqjcmrl.sHtML

Py:   len(arr)
来源：http://blog.yfazqb.com/Article/details/gsmoqnyuj.sHtML

PHP:  count($arr);
来源：http://www.blog.bbcook.cn/Article/details/gfsltgkki.sHtML

JS:   arr.length
来源：http://m.share.vehdjk.com/Article/details/gfyhyjmrh.sHtML

TS:   arr.length
来源：http://3g.fktsv.cn/Article/details/gqyfvdgow.sHtML

Java: list.size();
来源：http://m.share.vehdjk.com/Article/details/gcfweaktc.sHtML

Go:   len(arr)
来源：http://wap.fktsv.cn/Article/details/gxytkekoz.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.yfazqb.com/Article/details/gdhabeuym.sHtML

C#:   list.Count;
来源：http://www.share.tarul.cn/Article/details/gawhwsxft.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.bbcook.cn/Article/details/gaaavopkx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fktsv.cn/Article/details/gkklvutpo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.epnwcf.com/Article/details/gmbxjdoib.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.yfazqb.com/Article/details/ggopenjfc.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.bbcook.cn/Article/details/guybxduga.sHtML

Java: list.subList(1, 4);
来源：http://read.share.yfazqb.com/Article/details/guvxhilkt.sHtML

Go:   arr[1:4]
来源：http://read.share.yfazqb.com/Article/details/gqhgpzilk.sHtML

Ruby: arr[1, 3]
来源：http://baike.fktsv.cn/Article/details/grxyrnhwp.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fktsv.cn/Article/details/gkvbapatb.sHtML

[D08] 合并两个数组
来源：http://baike.sjlbkw.cn/Article/details/gzrgrdngj.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.yfazqb.com/Article/details/gqtwcvrpq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.tarul.cn/Article/details/gmqbhybkn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.sjlbkw.cn/Article/details/gfayzcxuy.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.bbcook.cn/Article/details/gnqqcmgde.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fktsv.cn/Article/details/gdccnyhuy.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fktsv.cn/Article/details/glbhrajsx.sHtML


<!-- 参考信息 -->