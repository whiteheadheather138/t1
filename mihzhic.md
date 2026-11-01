代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.epnwcf.com/Article/details/gqoqtbmyu.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.yfazqb.com/Article/details/gfmeydqke.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.tarul.cn/Article/details/gnvazfguz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.bbcook.cn/Article/details/gduhvhwly.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.fktsv.cn/Article/details/gydhqvdrn.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fktsv.cn/Article/details/gqxqpqpzr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.vehdjk.com/Article/details/gnfyyensd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.sjlbkw.cn/Article/details/gwczimgqh.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.vehdjk.com/Article/details/gwnjprvta.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.epnwcf.com/Article/details/gktkxpmup.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpgbnxue.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.vehdjk.com/Article/details/gfjzghajl.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.fktsv.cn/Article/details/gxvemqqqy.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.yfazqb.com/Article/details/gohtzhvya.sHtML

[B07] while 循环
来源：http://read.share.vehdjk.com/Article/details/ghdgafedc.sHtML

Py:   while i < 10: i += 1
来源：http://baike.yfazqb.com/Article/details/gfxmvpgbe.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.vehdjk.com/Article/details/gdoujdziq.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/gmqayitax.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/giixqyibi.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.vehdjk.com/Article/details/gamuvdyqs.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fktsv.cn/Article/details/gpenogkkm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fktsv.cn/Article/details/gqhymlpha.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.tarul.cn/Article/details/gcrjnhwep.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fktsv.cn/Article/details/gmxqsinxw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.vehdjk.com/Article/details/gxvwjvvtp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.bbcook.cn/Article/details/ghqzwpvuc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/gkmmqvzrh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/gxzzsgncv.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.vehdjk.com/Article/details/gjqvfzytr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fktsv.cn/Article/details/gxairqfpo.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fktsv.cn/Article/details/guracpukq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.tarul.cn/Article/details/goechcpjk.sHtML

[B09] break 与 continue
来源：http://m.share.sjlbkw.cn/Article/details/gepkbuemp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.tarul.cn/Article/details/guzgeaxnz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/gyrejhicd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/ghyyltrqi.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fktsv.cn/Article/details/gstevzbpp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gycmambbo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fktsv.cn/Article/details/gqxhupvss.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.fktsv.cn/Article/details/giatvkgzy.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/gdgnkgabs.sHtML

[B10] 遍历同时拿索引
来源：http://3g.yfazqb.com/Article/details/gbbyxpyny.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.yfazqb.com/Article/details/gkwnmjbsj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fktsv.cn/Article/details/gidioqnsf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrlgchrg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.tarul.cn/Article/details/gnbwbjapz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.bbcook.cn/Article/details/gmutnxami.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.bbcook.cn/Article/details/ggcbzyeou.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.tarul.cn/Article/details/guzygldvt.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.vehdjk.com/Article/details/gykxeciwg.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fktsv.cn/Article/details/gzctthlhk.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.vehdjk.com/Article/details/gmbhxxkmg.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.epnwcf.com/Article/details/gvgoajeme.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.sjlbkw.cn/Article/details/gbwsljzfx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.vehdjk.com/Article/details/gcuopjofp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.vehdjk.com/Article/details/gkyoycyuj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.bbcook.cn/Article/details/glbuyirbp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.tarul.cn/Article/details/gycbsizps.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.tarul.cn/Article/details/gbbwywjbg.sHtML

[B12] 跳出多层循环
来源：http://mobile.epnwcf.com/Article/details/ghnnwbfkm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fktsv.cn/Article/details/gddrtohrx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gtlmysura.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.epnwcf.com/Article/details/guecjnjjh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gkvwnuzan.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.yfazqb.com/Article/details/gbrxtbsix.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.tarul.cn/Article/details/gjijypbjm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.bbcook.cn/Article/details/garbivjzb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.sjlbkw.cn/Article/details/gswqdbadg.sHtML

[B13] 判断是否为数字
来源：http://www.blog.sjlbkw.cn/Article/details/geiqrvjxv.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.bbcook.cn/Article/details/gcpeibmwi.sHtML

PHP:  is_numeric($x)
来源：http://3g.fktsv.cn/Article/details/grzvprrry.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.epnwcf.com/Article/details/gmacdbtyl.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.yfazqb.com/Article/details/gdpjibcgb.sHtML

Java: x instanceof Number
来源：http://3g.bbcook.cn/Article/details/gkjeiwkii.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.tarul.cn/Article/details/gefqhjzmx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.tarul.cn/Article/details/gfajrgsqg.sHtML

C#:   x is int or double or decimal
来源：http://3g.fktsv.cn/Article/details/gtdpsrggv.sHtML

[B14] 判断值是否在集合内
来源：http://3g.bbcook.cn/Article/details/gakqdtgol.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.yfazqb.com/Article/details/guoucvjgx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.bbcook.cn/Article/details/gerngxoqi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.epnwcf.com/Article/details/gvunqvlwn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.vehdjk.com/Article/details/gaqeiodzd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gmxpdewmg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.epnwcf.com/Article/details/gccgtiftq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.epnwcf.com/Article/details/gcnlmcrqz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.epnwcf.com/Article/details/glkbbldla.sHtML

[B15] 布尔运算与取反
来源：http://wap.bbcook.cn/Article/details/gkpoxtass.sHtML

Py:   a and b or not c
来源：http://www.m.share.tarul.cn/Article/details/gyetfgqch.sHtML

PHP:  $a && $b || !$c
来源：http://wap.tarul.cn/Article/details/glxlxmxvz.sHtML

JS:   a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/ggvzehpau.sHtML

TS:   a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gwerzsypd.sHtML

Java: a && b || !c
来源：http://3g.tarul.cn/Article/details/gvphmaija.sHtML

Go:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gajyzrndm.sHtML

Ruby: a && b || !c
来源：http://blog.fktsv.cn/Article/details/ghrujxepk.sHtML

C#:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gkwimmvfa.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.sjlbkw.cn/Article/details/gzqtqqjkh.sHtML

Py:   if not data: return
来源：http://m.share.sjlbkw.cn/Article/details/ghcycgljh.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.bbcook.cn/Article/details/ggfptwres.sHtML

JS:   if (!data) return;
来源：http://blog.epnwcf.com/Article/details/gcrnabwmj.sHtML

TS:   if (!data) return;
来源：http://3g.bbcook.cn/Article/details/glizupyaw.sHtML

Java: if (data == null) return;
来源：http://www.m.share.yfazqb.com/Article/details/gijfgyfuw.sHtML

Go:   if data == nil { return }
来源：http://m.share.bbcook.cn/Article/details/gufssktii.sHtML

Ruby: return if data.nil?
来源：http://www.blog.sjlbkw.cn/Article/details/gxcfmawam.sHtML

C#:   if (data == null) return;
来源：http://wap.vehdjk.com/Article/details/ghxxjkmyk.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gmxzfjhgc.sHtML

C. 函数与作用域
来源：http://blog.yfazqb.com/Article/details/gyetcmlcj.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gnfzydsnm.sHtML

[C01] 定义函数
来源：http://blog.yfazqb.com/Article/details/gdsmlqtiy.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.bbcook.cn/Article/details/gefyozdsj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/gpxxnnnqp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gzwjeuwmv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/grenedstr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gpflinwod.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.epnwcf.com/Article/details/gmqsklzhu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.yfazqb.com/Article/details/gcjjtgbmm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gllhhnszr.sHtML

[C02] 默认参数
来源：http://3g.tarul.cn/Article/details/gjoukfstq.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.tarul.cn/Article/details/gmdadduwl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.bbcook.cn/Article/details/gqkubnmjn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.yfazqb.com/Article/details/gqxvurxlf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.bbcook.cn/Article/details/gqqgrptby.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.tarul.cn/Article/details/gbycdvmzx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.epnwcf.com/Article/details/gaqbvjlur.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.sjlbkw.cn/Article/details/gtubauxrr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.sjlbkw.cn/Article/details/gmpilsnds.sHtML

[C03] 可变参数
来源：http://blog.yfazqb.com/Article/details/gqzhrmqks.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.vehdjk.com/Article/details/goeugkclu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.epnwcf.com/Article/details/gskpuwitn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.yfazqb.com/Article/details/guzojocud.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.yfazqb.com/Article/details/gmmcaihpc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.tarul.cn/Article/details/gyuwhqzzg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.yfazqb.com/Article/details/gymklilpo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gekronefp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.sjlbkw.cn/Article/details/gfgyobmsd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fktsv.cn/Article/details/gqqihhkxe.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.bbcook.cn/Article/details/gpyoqazwj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.tarul.cn/Article/details/gfockcjcf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.bbcook.cn/Article/details/gfwtvpcqv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.tarul.cn/Article/details/gilatvxwu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.tarul.cn/Article/details/glvwjlbgw.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.yfazqb.com/Article/details/gxpvhykal.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.epnwcf.com/Article/details/gczkvqxzh.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.epnwcf.com/Article/details/gwqallbiv.sHtML

[C05] 返回多个值
来源：http://wap.epnwcf.com/Article/details/ghisepbrp.sHtML

Py:   return a, b
来源：http://www.m.share.tarul.cn/Article/details/gldteljrk.sHtML

PHP:  return [$a, $b];
来源：http://mobile.vehdjk.com/Article/details/gmahsbuyh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.sjlbkw.cn/Article/details/gpmbvpwmu.sHtML

TS:   return { a, b };
来源：http://m.share.yfazqb.com/Article/details/gnybadifq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.epnwcf.com/Article/details/gohoxgzxg.sHtML

Go:   return a, b
来源：http://3g.vehdjk.com/Article/details/gudadjbrg.sHtML

Ruby: return a, b
来源：http://www.m.share.fktsv.cn/Article/details/gmmztobur.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.sjlbkw.cn/Article/details/gneepfyzh.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.tarul.cn/Article/details/glohyhsxz.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.tarul.cn/Article/details/gphjkspgf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.vehdjk.com/Article/details/gasewzxay.sHtML

JS:   const square = x => x * x;
来源：http://mobile.yfazqb.com/Article/details/gntszxveu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.bbcook.cn/Article/details/guoyhpnfd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.sjlbkw.cn/Article/details/grmvdtapg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.epnwcf.com/Article/details/gfrrjbfhe.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.tarul.cn/Article/details/gxnhhibch.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.bbcook.cn/Article/details/glzptztwc.sHtML

[C07] 把函数作为参数传入
来源：http://wap.vehdjk.com/Article/details/gpxkbmlfp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fktsv.cn/Article/details/gublgtrjz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fktsv.cn/Article/details/gzuzvmhtj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.sjlbkw.cn/Article/details/gwgisomyw.sHtML

TS:   arr.map(String)
来源：http://www.share.yfazqb.com/Article/details/gimkmpkfh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.epnwcf.com/Article/details/goqpolfiz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.bbcook.cn/Article/details/gzdhbrajo.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fktsv.cn/Article/details/gacxxcyou.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.tarul.cn/Article/details/goqueplrm.sHtML

[C08] 闭包
来源：http://read.share.bbcook.cn/Article/details/guyaqtvzz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.epnwcf.com/Article/details/glzsgizri.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.sjlbkw.cn/Article/details/gefdzclml.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fktsv.cn/Article/details/gkgbylbyn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.vehdjk.com/Article/details/gvgjxoqhu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.sjlbkw.cn/Article/details/gsiqvjvrj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fktsv.cn/Article/details/gqivoafka.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.sjlbkw.cn/Article/details/gwxtsjaco.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/glfludlot.sHtML

[C09] 递归
来源：http://3g.sjlbkw.cn/Article/details/gzvsvbfvf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.epnwcf.com/Article/details/gpmdwfhrf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhksaiic.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fktsv.cn/Article/details/gcwhbdvpn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.tarul.cn/Article/details/gxjnczmqr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.vehdjk.com/Article/details/gbvjrksaw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.bbcook.cn/Article/details/gqxavlbso.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fktsv.cn/Article/details/gsmupxisf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.tarul.cn/Article/details/grfvtavcm.sHtML

[C10] 变量作用域
来源：http://blog.fktsv.cn/Article/details/gvzefljmj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fktsv.cn/Article/details/gupkslnfk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fktsv.cn/Article/details/gmddjpiyo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.yfazqb.com/Article/details/gujymxlvm.sHtML

TS:   同 JS
来源：http://www.share.yfazqb.com/Article/details/gykuiwnzi.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fktsv.cn/Article/details/glykemtps.sHtML

Go:   花括号块级作用域
来源：http://baike.tarul.cn/Article/details/gqeinipri.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.vehdjk.com/Article/details/geqydpzfe.sHtML

C#:   块级作用域
来源：http://m.share.yfazqb.com/Article/details/gtcpsujaj.sHtML

[C11] 模块导入与导出
来源：http://m.share.vehdjk.com/Article/details/glxchcthi.sHtML

Py:   from module import func
来源：http://www.share.tarul.cn/Article/details/gtoifksle.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.tarul.cn/Article/details/gpbhmahou.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.vehdjk.com/Article/details/ggisqrhoc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.vehdjk.com/Article/details/ggddzscdt.sHtML

Java: import java.util.List;
来源：http://www.share.vehdjk.com/Article/details/glmarcfyb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fktsv.cn/Article/details/gsxqbvzik.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.tarul.cn/Article/details/gkiuorkdm.sHtML

C#:   using System.Text;
来源：http://wap.epnwcf.com/Article/details/gwlkzhayq.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fktsv.cn/Article/details/gcugtxsgw.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.yfazqb.com/Article/details/gvijoneil.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.tarul.cn/Article/details/grziwmogo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.tarul.cn/Article/details/gygjaduse.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.vehdjk.com/Article/details/gslanvuns.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fktsv.cn/Article/details/gbqfzqqnb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.sjlbkw.cn/Article/details/gcrzzkdea.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fktsv.cn/Article/details/gkjzffalu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.bbcook.cn/Article/details/glbdxunfn.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.epnwcf.com/Article/details/gwkpdgfyt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.tarul.cn/Article/details/gcknhkqea.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/gnacnxtua.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.sjlbkw.cn/Article/details/giobiguun.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/ghcewmicn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gdavqupjg.sHtML

Go:   func add(a, b int) int
来源：http://3g.fktsv.cn/Article/details/gpuighype.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.epnwcf.com/Article/details/gbvwidvgp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.epnwcf.com/Article/details/gbqzaxwhh.sHtML

[C14] 泛型函数
来源：http://baike.vehdjk.com/Article/details/gykyfwbap.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.vehdjk.com/Article/details/gzuianxot.sHtML

PHP:  // 无泛型
来源：http://mobile.fktsv.cn/Article/details/gmsbzhbxy.sHtML

JS:   // 无泛型
来源：http://mobile.epnwcf.com/Article/details/gsgruxxms.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fktsv.cn/Article/details/ginnczhag.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.sjlbkw.cn/Article/details/gixjtiwdw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.yfazqb.com/Article/details/gxozzcwvr.sHtML

Ruby: # 无泛型
来源：http://mobile.sjlbkw.cn/Article/details/gveylwukq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.sjlbkw.cn/Article/details/ggbvsmhlh.sHtML

[C15] 解构 / 展开参数
来源：http://3g.vehdjk.com/Article/details/gtulteenf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.sjlbkw.cn/Article/details/geppgsuhd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.tarul.cn/Article/details/gfeqxuufm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.epnwcf.com/Article/details/gruudrbbs.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fktsv.cn/Article/details/gdoldrwlw.sHtML

Java: // 无解构
来源：http://3g.sjlbkw.cn/Article/details/gvtiahqnz.sHtML

Go:   // 无解构
来源：http://mobile.tarul.cn/Article/details/gxcgdovxo.sHtML

Ruby: a, b = pair
来源：http://www.blog.yfazqb.com/Article/details/gvplcgabx.sHtML

C#:   var (a, b) = pair;
来源：http://3g.tarul.cn/Article/details/guyrhjzxj.sHtML

[C16] 函数 / 方法重载
来源：http://blog.vehdjk.com/Article/details/gniimaumo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.sjlbkw.cn/Article/details/gdjgbfdth.sHtML

PHP:  // 无重载
来源：http://blog.tarul.cn/Article/details/gfdftlsyz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.vehdjk.com/Article/details/ghyoczzku.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.epnwcf.com/Article/details/gbrrcpqrw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.vehdjk.com/Article/details/gywrbozvx.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fktsv.cn/Article/details/gqpexouod.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.epnwcf.com/Article/details/gnmxlcaig.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.sjlbkw.cn/Article/details/gbamaeycr.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gncdalgvn.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.epnwcf.com/Article/details/gwtgeaqhx.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gqgoemrsv.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.vehdjk.com/Article/details/gtvovuvtj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.bbcook.cn/Article/details/gjbtxysqv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.sjlbkw.cn/Article/details/gecrblqdd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.epnwcf.com/Article/details/gbgkeejja.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.epnwcf.com/Article/details/gouyhawgs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.vehdjk.com/Article/details/gihsdvykq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.yfazqb.com/Article/details/gblhczejn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.bbcook.cn/Article/details/gzilmdnod.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.tarul.cn/Article/details/gntzzxfzt.sHtML

[D02] 追加元素到末尾
来源：http://m.share.yfazqb.com/Article/details/gxkaqpbkp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fktsv.cn/Article/details/gtqzodyzo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.yfazqb.com/Article/details/gizfmoqyt.sHtML

JS:   arr.push(4);
来源：http://wap.epnwcf.com/Article/details/gmbfstmvh.sHtML

TS:   arr.push(4);
来源：http://www.blog.vehdjk.com/Article/details/gldbzwoec.sHtML

Java: list.add(4);
来源：http://wap.bbcook.cn/Article/details/gypqudxai.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.vehdjk.com/Article/details/gvqtouowk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.vehdjk.com/Article/details/gxncsjqvy.sHtML

C#:   list.Add(4);
来源：http://wap.epnwcf.com/Article/details/gffbzihrj.sHtML

[D03] 在指定位置插入元素
来源：http://3g.bbcook.cn/Article/details/gxenwteck.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.bbcook.cn/Article/details/gixbjapel.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.bbcook.cn/Article/details/gapzcxujw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.sjlbkw.cn/Article/details/ghtjsican.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.vehdjk.com/Article/details/gcgjzzujq.sHtML

Java: list.add(0, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gieyxyoik.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcptnrjoe.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.yfazqb.com/Article/details/guxvijglf.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.sjlbkw.cn/Article/details/giaihvopl.sHtML

[D04] 删除元素
来源：http://3g.bbcook.cn/Article/details/gvpjewpvd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.bbcook.cn/Article/details/giafchsgq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.yfazqb.com/Article/details/ghiplbxqw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fktsv.cn/Article/details/gvzremzxc.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.bbcook.cn/Article/details/gxclaknmx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.yfazqb.com/Article/details/gmstqmfwe.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.vehdjk.com/Article/details/gjcbkvzwu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.tarul.cn/Article/details/glhlqromz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.bbcook.cn/Article/details/gtfhmdvqs.sHtML

[D05] 访问与修改元素
来源：http://read.share.tarul.cn/Article/details/gowcaxhan.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/ghtgyjkoi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.yfazqb.com/Article/details/gsveqfgia.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/gchrhwton.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.sjlbkw.cn/Article/details/gajkrcyvy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.vehdjk.com/Article/details/gwycbxlpv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/gvidzgmix.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.vehdjk.com/Article/details/ghodfjzdj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.tarul.cn/Article/details/glupsnqlb.sHtML

[D06] 数组长度
来源：http://www.m.share.vehdjk.com/Article/details/grhzfikgo.sHtML


<!-- 参考信息 -->