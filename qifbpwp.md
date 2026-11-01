代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.vehdjk.com/Article/details/glcuxnzxj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.epnwcf.com/Article/details/geckafpcr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.bbcook.cn/Article/details/glzicdjdr.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.vehdjk.com/Article/details/gahqtquoy.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.bbcook.cn/Article/details/gczmjixup.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.yfazqb.com/Article/details/gvwjlxnua.sHtML

[B07] while 循环
来源：http://wap.sjlbkw.cn/Article/details/gpnprwtcw.sHtML

Py:   while i < 10: i += 1
来源：http://baike.vehdjk.com/Article/details/goisyybkz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gobpzowdz.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.bbcook.cn/Article/details/gjcrjuxqt.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.bbcook.cn/Article/details/gqrzwdwks.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/gyyhsotec.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.tarul.cn/Article/details/gqfsrojek.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.vehdjk.com/Article/details/gykthdiyx.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.fktsv.cn/Article/details/gibfrozqb.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.epnwcf.com/Article/details/gfilhurfz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.tarul.cn/Article/details/gatwwfsil.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.yfazqb.com/Article/details/gtsdhabxy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gvvgyizid.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.tarul.cn/Article/details/gieorrogm.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.yfazqb.com/Article/details/geyvoqhlj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.sjlbkw.cn/Article/details/groxmqbec.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.epnwcf.com/Article/details/gutdeqowt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/glwuhvgmd.sHtML

[B09] break 与 continue
来源：http://www.m.share.vehdjk.com/Article/details/ghzvictkt.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.bbcook.cn/Article/details/griselhbv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/giudrkvba.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/goccffwto.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/gvcggsgfs.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/gtzscijvz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.yfazqb.com/Article/details/ggfzegqgi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.bbcook.cn/Article/details/gvwgsrtgj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/ghivmapkm.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.yfazqb.com/Article/details/gefvkvyae.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.bbcook.cn/Article/details/ggbauvhtf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.bbcook.cn/Article/details/gzchpodwi.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.yfazqb.com/Article/details/gbyaxlfxg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.yfazqb.com/Article/details/gpvmwjgum.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.sjlbkw.cn/Article/details/guxbprfuc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.tarul.cn/Article/details/gexezeorp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.yfazqb.com/Article/details/glpaggxqi.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.yfazqb.com/Article/details/gxwgjuhjv.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.epnwcf.com/Article/details/gghcawtcy.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.bbcook.cn/Article/details/gtywznzki.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.epnwcf.com/Article/details/ggaofdnap.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.tarul.cn/Article/details/gfmwfjhkw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.vehdjk.com/Article/details/gqvywyqck.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvkoyadmx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.yfazqb.com/Article/details/gdhjyqhae.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.tarul.cn/Article/details/gngsverqb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.tarul.cn/Article/details/gqclpzlur.sHtML

[B12] 跳出多层循环
来源：http://www.share.yfazqb.com/Article/details/gfhfkgqco.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.tarul.cn/Article/details/ghniuxfey.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.yfazqb.com/Article/details/gebdofgnd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fktsv.cn/Article/details/guukfmayn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.epnwcf.com/Article/details/gtdrqjhdt.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.vehdjk.com/Article/details/gyqjjrdwo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fktsv.cn/Article/details/gbffbbbgv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.tarul.cn/Article/details/gthxneiou.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.vehdjk.com/Article/details/gresqqbvq.sHtML

[B13] 判断是否为数字
来源：http://baike.epnwcf.com/Article/details/gpgwtpuhz.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.bbcook.cn/Article/details/gkmhejvsh.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.vehdjk.com/Article/details/guuztqxhg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.vehdjk.com/Article/details/glvjxlrxk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.yfazqb.com/Article/details/gybbexsfl.sHtML

Java: x instanceof Number
来源：http://www.share.sjlbkw.cn/Article/details/gtviadhdu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fktsv.cn/Article/details/gpepjgpri.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.bbcook.cn/Article/details/ghbjjcxpm.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcyxlude.sHtML

[B14] 判断值是否在集合内
来源：http://baike.vehdjk.com/Article/details/gvfylqnsy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.yfazqb.com/Article/details/gztbqbqfx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.bbcook.cn/Article/details/gaspjidxf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/gpftfgecd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.tarul.cn/Article/details/gvebakibb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gxdfgbwjk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fktsv.cn/Article/details/gzakqtrhx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.vehdjk.com/Article/details/gawvlzyxy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.sjlbkw.cn/Article/details/guhgruicz.sHtML

[B15] 布尔运算与取反
来源：http://wap.vehdjk.com/Article/details/gwkgriiec.sHtML

Py:   a and b or not c
来源：http://read.share.epnwcf.com/Article/details/gjqegajda.sHtML

PHP:  $a && $b || !$c
来源：http://wap.epnwcf.com/Article/details/gfpalmvqf.sHtML

JS:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gmaxwkofx.sHtML

TS:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gvxiwtrhy.sHtML

Java: a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/ghxskejoi.sHtML

Go:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/gbvlczokm.sHtML

Ruby: a && b || !c
来源：http://baike.vehdjk.com/Article/details/gvrhnivuz.sHtML

C#:   a && b || !c
来源：http://mobile.yfazqb.com/Article/details/ghadxvjbr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.yfazqb.com/Article/details/gdtbxamsd.sHtML

Py:   if not data: return
来源：http://www.blog.bbcook.cn/Article/details/gvuuwfgrb.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fktsv.cn/Article/details/gycuzmfhs.sHtML

JS:   if (!data) return;
来源：http://m.share.bbcook.cn/Article/details/gcwzwicho.sHtML

TS:   if (!data) return;
来源：http://www.share.vehdjk.com/Article/details/gucrddbut.sHtML

Java: if (data == null) return;
来源：http://www.m.share.vehdjk.com/Article/details/gxbitiumc.sHtML

Go:   if data == nil { return }
来源：http://baike.tarul.cn/Article/details/gvruwksdw.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fktsv.cn/Article/details/gdaynkjgh.sHtML

C#:   if (data == null) return;
来源：http://mobile.tarul.cn/Article/details/gboaiphqw.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gwpkmhzfq.sHtML

C. 函数与作用域
来源：http://blog.epnwcf.com/Article/details/gfezgyzqv.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gssfouqwk.sHtML

[C01] 定义函数
来源：http://www.blog.vehdjk.com/Article/details/gsmwplris.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.tarul.cn/Article/details/gnztsfyio.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/gcjrgjxnz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.epnwcf.com/Article/details/glwsjdutk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gfewjjaoz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.bbcook.cn/Article/details/gtbdkcwlb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.epnwcf.com/Article/details/gtygupyrs.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.vehdjk.com/Article/details/ggnlmidxd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gftklwcyw.sHtML

[C02] 默认参数
来源：http://mobile.yfazqb.com/Article/details/gbmnlpzqh.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.epnwcf.com/Article/details/gvixkrvcz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.tarul.cn/Article/details/gvrquluqf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.vehdjk.com/Article/details/grihvtjza.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.epnwcf.com/Article/details/guwgdthox.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.yfazqb.com/Article/details/ggxatcccp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.tarul.cn/Article/details/gmavzuqwl.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.yfazqb.com/Article/details/gcolnjxtw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.yfazqb.com/Article/details/gxuluphxj.sHtML

[C03] 可变参数
来源：http://3g.fktsv.cn/Article/details/gcpouigcw.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.yfazqb.com/Article/details/gjufuciwa.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.tarul.cn/Article/details/gcbgxqkel.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.epnwcf.com/Article/details/gpgkkwchm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.tarul.cn/Article/details/gwcpajimw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.vehdjk.com/Article/details/gaehwtvoh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.yfazqb.com/Article/details/gxwhnbpjn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.vehdjk.com/Article/details/gnwsrlgzn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.yfazqb.com/Article/details/ggfvhoull.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.yfazqb.com/Article/details/guaafliib.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.vehdjk.com/Article/details/gwqzuhssi.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.bbcook.cn/Article/details/geytcevfc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.yfazqb.com/Article/details/gfxsjvofi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fktsv.cn/Article/details/gbotfsymc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fktsv.cn/Article/details/gjtzcqwrx.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.sjlbkw.cn/Article/details/grltvpdoe.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.yfazqb.com/Article/details/gtriurudk.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.yfazqb.com/Article/details/gmtowbyns.sHtML

[C05] 返回多个值
来源：http://www.blog.bbcook.cn/Article/details/gvhiebhfq.sHtML

Py:   return a, b
来源：http://blog.yfazqb.com/Article/details/guiaqpmkc.sHtML

PHP:  return [$a, $b];
来源：http://m.share.sjlbkw.cn/Article/details/gbrolnabh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.yfazqb.com/Article/details/gaknqazdw.sHtML

TS:   return { a, b };
来源：http://www.share.tarul.cn/Article/details/gbfhxsprq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fktsv.cn/Article/details/gegkfquck.sHtML

Go:   return a, b
来源：http://blog.yfazqb.com/Article/details/gbgzcvqne.sHtML

Ruby: return a, b
来源：http://blog.vehdjk.com/Article/details/gunalvmoe.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.tarul.cn/Article/details/gstwpbbcx.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.tarul.cn/Article/details/grjditbor.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fktsv.cn/Article/details/geesddtql.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.bbcook.cn/Article/details/gwcpnlnwk.sHtML

JS:   const square = x => x * x;
来源：http://wap.bbcook.cn/Article/details/gxqngutdg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.yfazqb.com/Article/details/gjyctdcaj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.vehdjk.com/Article/details/gvtnegmlq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.epnwcf.com/Article/details/gopjjdqrf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fktsv.cn/Article/details/gflyqqayz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.yfazqb.com/Article/details/gwegoxwoo.sHtML

[C07] 把函数作为参数传入
来源：http://baike.vehdjk.com/Article/details/gmcdwvcxz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.vehdjk.com/Article/details/gmkbuehur.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.tarul.cn/Article/details/gpivrartg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.bbcook.cn/Article/details/genxxleqe.sHtML

TS:   arr.map(String)
来源：http://baike.epnwcf.com/Article/details/gepsgkcsa.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fktsv.cn/Article/details/gmjpbrzmt.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.bbcook.cn/Article/details/geqasrlfk.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.sjlbkw.cn/Article/details/gjascemcw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.epnwcf.com/Article/details/gmpxqbvxs.sHtML

[C08] 闭包
来源：http://read.share.fktsv.cn/Article/details/ghsckvsrp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.epnwcf.com/Article/details/gbbqpfsah.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.yfazqb.com/Article/details/gjerxmzfw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/ghkpmmwjv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.tarul.cn/Article/details/gscvxlhts.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.bbcook.cn/Article/details/gdigkdyuz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.yfazqb.com/Article/details/gbwjvfzfw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.epnwcf.com/Article/details/gwgwecplm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.tarul.cn/Article/details/gtxutqeby.sHtML

[C09] 递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gcepirlnj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.bbcook.cn/Article/details/gwmanhpxr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqilfsvga.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.tarul.cn/Article/details/gqzrgpmym.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.tarul.cn/Article/details/gsristhct.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fktsv.cn/Article/details/gzjrzspkg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.vehdjk.com/Article/details/gkxplqhwg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.epnwcf.com/Article/details/gdoitfcgd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fktsv.cn/Article/details/gvvqroruq.sHtML

[C10] 变量作用域
来源：http://m.share.vehdjk.com/Article/details/gfxeiohcx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.tarul.cn/Article/details/gggsinusp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.bbcook.cn/Article/details/gzeqeihkp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.vehdjk.com/Article/details/glscvjypg.sHtML

TS:   同 JS
来源：http://baike.fktsv.cn/Article/details/gbknvrskj.sHtML

Java: 方法内为块级作用域
来源：http://wap.fktsv.cn/Article/details/gtoklwubh.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.vehdjk.com/Article/details/gtdwlbczb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.vehdjk.com/Article/details/gccyfpjvu.sHtML

C#:   块级作用域
来源：http://read.share.fktsv.cn/Article/details/gidqxhkxx.sHtML

[C11] 模块导入与导出
来源：http://read.share.epnwcf.com/Article/details/gsfqvipor.sHtML

Py:   from module import func
来源：http://m.share.vehdjk.com/Article/details/gxxybedui.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.yfazqb.com/Article/details/gzvauoued.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.yfazqb.com/Article/details/gkpdetzpf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.vehdjk.com/Article/details/gqppqectb.sHtML

Java: import java.util.List;
来源：http://3g.vehdjk.com/Article/details/goonqkdkp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.vehdjk.com/Article/details/grricohdz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.tarul.cn/Article/details/gosntwhos.sHtML

C#:   using System.Text;
来源：http://blog.epnwcf.com/Article/details/gtuywfxow.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.yfazqb.com/Article/details/gcxyjqenp.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.yfazqb.com/Article/details/gsgjlnzbh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.sjlbkw.cn/Article/details/gcepocawt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fktsv.cn/Article/details/ggbnkbjwk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.epnwcf.com/Article/details/gpsbezxje.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.vehdjk.com/Article/details/gdjeowojl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.yfazqb.com/Article/details/gtylwdbyq.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.vehdjk.com/Article/details/gkecxtolf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.epnwcf.com/Article/details/gaavbtrgs.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.yfazqb.com/Article/details/gqjvfvgup.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.tarul.cn/Article/details/glmuoezyq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gadoonzsn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.epnwcf.com/Article/details/gaiwnnsig.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gvafbpzrj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gufcwzvhm.sHtML

Go:   func add(a, b int) int
来源：http://blog.epnwcf.com/Article/details/gmcprrmsj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.epnwcf.com/Article/details/govijnszb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.epnwcf.com/Article/details/gxmtzopac.sHtML

[C14] 泛型函数
来源：http://read.share.sjlbkw.cn/Article/details/gmpcbldme.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.bbcook.cn/Article/details/ggkrnqler.sHtML

PHP:  // 无泛型
来源：http://blog.sjlbkw.cn/Article/details/ggcbicqbk.sHtML

JS:   // 无泛型
来源：http://wap.yfazqb.com/Article/details/gqzypymjn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.epnwcf.com/Article/details/gnrbfroir.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.vehdjk.com/Article/details/gqhhglisy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.vehdjk.com/Article/details/goxtbuxro.sHtML

Ruby: # 无泛型
来源：http://blog.epnwcf.com/Article/details/gpkylzhfg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.epnwcf.com/Article/details/gnrtipotd.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.vehdjk.com/Article/details/gxrjdkrjd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.epnwcf.com/Article/details/gtwtyelxo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.vehdjk.com/Article/details/gqjeonits.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgbbkdhs.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.tarul.cn/Article/details/gruzlgulm.sHtML

Java: // 无解构
来源：http://www.share.epnwcf.com/Article/details/gmwextngt.sHtML

Go:   // 无解构
来源：http://3g.fktsv.cn/Article/details/gzimkhexb.sHtML

Ruby: a, b = pair
来源：http://mobile.vehdjk.com/Article/details/gsnjumwlh.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fktsv.cn/Article/details/giinbioua.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.sjlbkw.cn/Article/details/gmnswebhh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.tarul.cn/Article/details/glmsndxbz.sHtML

PHP:  // 无重载
来源：http://3g.fktsv.cn/Article/details/gvlbmwjnp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.bbcook.cn/Article/details/ghwxcxdhx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.tarul.cn/Article/details/gsnahqhfb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.tarul.cn/Article/details/gysubezlr.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.tarul.cn/Article/details/gkdvfuqhs.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.yfazqb.com/Article/details/gljwuwjjj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.vehdjk.com/Article/details/gbphdmeuk.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gzfernure.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.sjlbkw.cn/Article/details/gbiipstam.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gfjevxmmb.sHtML

[D01] 创建数组 / 列表
来源：http://3g.epnwcf.com/Article/details/gnrdfblwk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.tarul.cn/Article/details/golnekkdh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.yfazqb.com/Article/details/gqtyltmbm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.tarul.cn/Article/details/gqpwcbssg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.tarul.cn/Article/details/gsykwypqy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.epnwcf.com/Article/details/gnqkhxpdt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.yfazqb.com/Article/details/gryywowjo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.bbcook.cn/Article/details/gzaretrpv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.tarul.cn/Article/details/gddykmmxl.sHtML

[D02] 追加元素到末尾
来源：http://3g.yfazqb.com/Article/details/gxtjegwvp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.tarul.cn/Article/details/gfhhaqezq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fktsv.cn/Article/details/goljqvxap.sHtML

JS:   arr.push(4);
来源：http://www.blog.yfazqb.com/Article/details/gmmikhbkc.sHtML

TS:   arr.push(4);
来源：http://www.blog.vehdjk.com/Article/details/gdrjozjgd.sHtML

Java: list.add(4);
来源：http://3g.vehdjk.com/Article/details/gabzbazdv.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.epnwcf.com/Article/details/gvrpiuctp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.epnwcf.com/Article/details/gvqwhvjwv.sHtML

C#:   list.Add(4);
来源：http://www.share.tarul.cn/Article/details/grejavxqq.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.sjlbkw.cn/Article/details/gnxxbeuxs.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fktsv.cn/Article/details/goujwafks.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.sjlbkw.cn/Article/details/gzcewfane.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.sjlbkw.cn/Article/details/gyekuahrf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.epnwcf.com/Article/details/grpzywwth.sHtML

Java: list.add(0, 0);
来源：http://www.share.fktsv.cn/Article/details/geicxfyks.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.yfazqb.com/Article/details/gyszzlaet.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.sjlbkw.cn/Article/details/glmhzmxnj.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.tarul.cn/Article/details/ghqwehgog.sHtML

[D04] 删除元素
来源：http://read.share.vehdjk.com/Article/details/gqhjmicgg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.vehdjk.com/Article/details/gawnmpbtt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.bbcook.cn/Article/details/giybomjes.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.tarul.cn/Article/details/gzwnrrugz.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fktsv.cn/Article/details/gjszqjrnq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.yfazqb.com/Article/details/gpgirwkrj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.bbcook.cn/Article/details/gzmulchdh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.epnwcf.com/Article/details/gilixunkn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.sjlbkw.cn/Article/details/gjevcydma.sHtML

[D05] 访问与修改元素
来源：http://blog.epnwcf.com/Article/details/gprxqttue.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.vehdjk.com/Article/details/gibikdeau.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.sjlbkw.cn/Article/details/gtjeaqfzu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.bbcook.cn/Article/details/ghszzancp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.sjlbkw.cn/Article/details/gekpxyada.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.sjlbkw.cn/Article/details/gqlgnurgs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.tarul.cn/Article/details/gfplyvwvz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fktsv.cn/Article/details/geiscydjk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.yfazqb.com/Article/details/gmaeeulni.sHtML

[D06] 数组长度
来源：http://baike.bbcook.cn/Article/details/gubjrqobe.sHtML

Py:   len(arr)
来源：http://www.m.share.epnwcf.com/Article/details/ghmyttmlz.sHtML

PHP:  count($arr);
来源：http://blog.vehdjk.com/Article/details/gogiqavbc.sHtML

JS:   arr.length
来源：http://wap.sjlbkw.cn/Article/details/gfwnhwrib.sHtML

TS:   arr.length
来源：http://blog.vehdjk.com/Article/details/ginkporaw.sHtML

Java: list.size();
来源：http://wap.yfazqb.com/Article/details/gbmcxudxs.sHtML

Go:   len(arr)
来源：http://baike.bbcook.cn/Article/details/gjxcaveea.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.epnwcf.com/Article/details/glroodvlt.sHtML

C#:   list.Count;
来源：http://wap.sjlbkw.cn/Article/details/ghpsglwms.sHtML


<!-- 参考信息 -->