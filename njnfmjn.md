代发 wailian999

[B05] 遍历数组 / 列表
来源：http://m.share.tarul.cn/Article/details/gvckldvos.sHtML

Py:   for item in arr: print(item)
来源：http://3g.yfazqb.com/Article/details/goczjgjbt.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.fktsv.cn/Article/details/ganksduqs.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.bbcook.cn/Article/details/gilamgpxq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fktsv.cn/Article/details/gehjfgycf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.bbcook.cn/Article/details/gvpghcuxi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.vehdjk.com/Article/details/gmhbtoorw.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.epnwcf.com/Article/details/gwtoqjdgg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fktsv.cn/Article/details/gtvbghlex.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.yfazqb.com/Article/details/grefwfsxc.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.epnwcf.com/Article/details/gawmijypa.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.bbcook.cn/Article/details/gysyoywtk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.tarul.cn/Article/details/gxrpmwtnp.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.bbcook.cn/Article/details/gobfhmbvu.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.fktsv.cn/Article/details/gkvljctps.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.vehdjk.com/Article/details/gwgcbmcyc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.bbcook.cn/Article/details/gxgjdbxpe.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.tarul.cn/Article/details/gebhkxcnd.sHtML

[B07] while 循环
来源：http://mobile.vehdjk.com/Article/details/gqksfdffx.sHtML

Py:   while i < 10: i += 1
来源：http://blog.yfazqb.com/Article/details/gexinpvhi.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.sjlbkw.cn/Article/details/grbmfkpib.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.sjlbkw.cn/Article/details/glcngawrb.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.fktsv.cn/Article/details/gzeucyqrw.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/gjrppdjym.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.vehdjk.com/Article/details/gkflavjda.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.sjlbkw.cn/Article/details/gwmmgbnms.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.fktsv.cn/Article/details/glejyyhhc.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.epnwcf.com/Article/details/gypxovakt.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.vehdjk.com/Article/details/gemvhntqs.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.vehdjk.com/Article/details/goyauhoem.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.vehdjk.com/Article/details/gzmcqjeqz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.fktsv.cn/Article/details/gxophtytx.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.yfazqb.com/Article/details/gaeuznaoh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fktsv.cn/Article/details/geugefmea.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.bbcook.cn/Article/details/gsorxoact.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gmqfxedqi.sHtML

[B09] break 与 continue
来源：http://read.share.vehdjk.com/Article/details/gvqbsdeso.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fktsv.cn/Article/details/giwmwxgkq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/gmmgcqspc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gahvrxjxg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/gilycsgwo.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/gzqbjphhe.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.tarul.cn/Article/details/glzyjreqm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.tarul.cn/Article/details/gfsywisru.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/gmxfokgtq.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.tarul.cn/Article/details/glyojcawe.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.yfazqb.com/Article/details/gjbfduclw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.tarul.cn/Article/details/gqbbxmxrn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.epnwcf.com/Article/details/gugzcicce.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.sjlbkw.cn/Article/details/ghxvujnkc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fktsv.cn/Article/details/gooeyhsia.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.yfazqb.com/Article/details/gnwrrgymu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fktsv.cn/Article/details/gzbiuyuiu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.sjlbkw.cn/Article/details/gdqkoqqtg.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.yfazqb.com/Article/details/gkarvdqoc.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.vehdjk.com/Article/details/gaqwmvwbu.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.bbcook.cn/Article/details/gnahtvszq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.bbcook.cn/Article/details/gyvdndvyx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.bbcook.cn/Article/details/gslukvkes.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.vehdjk.com/Article/details/gtilngudd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.epnwcf.com/Article/details/gciebbwjo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.bbcook.cn/Article/details/gvchgauwi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gyfjmuave.sHtML

[B12] 跳出多层循环
来源：http://mobile.epnwcf.com/Article/details/gvjppvjuc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.bbcook.cn/Article/details/gteebtrwp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.yfazqb.com/Article/details/gsssmuund.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.sjlbkw.cn/Article/details/gcasuaike.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.epnwcf.com/Article/details/gqyvhczsr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.sjlbkw.cn/Article/details/gsnxdhvdh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.tarul.cn/Article/details/gbipkjlyv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.tarul.cn/Article/details/grnojvwfn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.bbcook.cn/Article/details/govwxeqfd.sHtML

[B13] 判断是否为数字
来源：http://3g.sjlbkw.cn/Article/details/glsxqdgev.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fktsv.cn/Article/details/gpuxwfvpr.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.bbcook.cn/Article/details/gviaxdpqf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.epnwcf.com/Article/details/gutvhfdsp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.vehdjk.com/Article/details/gtjydmuat.sHtML

Java: x instanceof Number
来源：http://mobile.vehdjk.com/Article/details/gsjpmauqd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.vehdjk.com/Article/details/gwrgcxxrb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.vehdjk.com/Article/details/gxxglqmvo.sHtML

C#:   x is int or double or decimal
来源：http://read.share.sjlbkw.cn/Article/details/gifeofuuo.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.bbcook.cn/Article/details/gqkxunqpd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.epnwcf.com/Article/details/gwletmxui.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.sjlbkw.cn/Article/details/gjzmgbsaj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.bbcook.cn/Article/details/gesswcvxt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/glswalbdm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fktsv.cn/Article/details/glcclferh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.sjlbkw.cn/Article/details/gkvkpabpx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.epnwcf.com/Article/details/ggookzlji.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.vehdjk.com/Article/details/gtmtkqkhz.sHtML

[B15] 布尔运算与取反
来源：http://www.share.sjlbkw.cn/Article/details/ghttoeecc.sHtML

Py:   a and b or not c
来源：http://www.m.share.bbcook.cn/Article/details/ggjdtgqjs.sHtML

PHP:  $a && $b || !$c
来源：http://wap.bbcook.cn/Article/details/gweklgfmu.sHtML

JS:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/ghnyefxsd.sHtML

TS:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gakcwelts.sHtML

Java: a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gmgvpawwq.sHtML

Go:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gmhkxjavy.sHtML

Ruby: a && b || !c
来源：http://wap.yfazqb.com/Article/details/gsknrzfav.sHtML

C#:   a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gdthnaxyk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fktsv.cn/Article/details/gykajsnwx.sHtML

Py:   if not data: return
来源：http://blog.bbcook.cn/Article/details/glhkkjnqd.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.vehdjk.com/Article/details/gwrvwulca.sHtML

JS:   if (!data) return;
来源：http://3g.epnwcf.com/Article/details/ghesgqlup.sHtML

TS:   if (!data) return;
来源：http://baike.tarul.cn/Article/details/gofpejpdq.sHtML

Java: if (data == null) return;
来源：http://read.share.bbcook.cn/Article/details/gqjfslmkh.sHtML

Go:   if data == nil { return }
来源：http://mobile.sjlbkw.cn/Article/details/gujvhuqrb.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.epnwcf.com/Article/details/ghnvspdij.sHtML

C#:   if (data == null) return;
来源：http://blog.tarul.cn/Article/details/gcqgytjbx.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gqdrdjzro.sHtML

C. 函数与作用域
来源：http://www.blog.bbcook.cn/Article/details/gmbzyqisw.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gzlernizt.sHtML

[C01] 定义函数
来源：http://wap.fktsv.cn/Article/details/gdddlshdo.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.tarul.cn/Article/details/ggvfuddes.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.tarul.cn/Article/details/gcumhgztm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gmdcermkc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gxhjzfeph.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gdtydofts.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fktsv.cn/Article/details/gnkgvcpqw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fktsv.cn/Article/details/gngktglsd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gpatikdlf.sHtML

[C02] 默认参数
来源：http://mobile.vehdjk.com/Article/details/goqkztpdt.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.tarul.cn/Article/details/gxsjvbjrl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjgqdivwq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.yfazqb.com/Article/details/gwpeyrnth.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.epnwcf.com/Article/details/gsugkqgqm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.epnwcf.com/Article/details/ghbqxuhmt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.yfazqb.com/Article/details/gyxmsazbh.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.yfazqb.com/Article/details/gcdcnouii.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.vehdjk.com/Article/details/glfgtxdhw.sHtML

[C03] 可变参数
来源：http://www.m.share.vehdjk.com/Article/details/geomzkkey.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.vehdjk.com/Article/details/ghtcjvgtc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.sjlbkw.cn/Article/details/gzaejtutt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fktsv.cn/Article/details/gtygsndfn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.epnwcf.com/Article/details/ghrxjklan.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.vehdjk.com/Article/details/gvnzjzttf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.sjlbkw.cn/Article/details/gxknkohca.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fktsv.cn/Article/details/gnqgfjxyu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.bbcook.cn/Article/details/gorkpjmie.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fktsv.cn/Article/details/givjismct.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.sjlbkw.cn/Article/details/gbxrvgpjt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.epnwcf.com/Article/details/gejijngqk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.tarul.cn/Article/details/gbvpuemap.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.sjlbkw.cn/Article/details/gbrcfhwid.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.bbcook.cn/Article/details/ghyytlppn.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fktsv.cn/Article/details/glejebqvr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.tarul.cn/Article/details/gamogdytv.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.bbcook.cn/Article/details/gjqhtzhwk.sHtML

[C05] 返回多个值
来源：http://baike.bbcook.cn/Article/details/giavmgzdf.sHtML

Py:   return a, b
来源：http://wap.fktsv.cn/Article/details/ghchrzolf.sHtML

PHP:  return [$a, $b];
来源：http://www.share.tarul.cn/Article/details/gackumauh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.vehdjk.com/Article/details/gvcgbetpg.sHtML

TS:   return { a, b };
来源：http://read.share.yfazqb.com/Article/details/gxlemvsqq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.bbcook.cn/Article/details/gzlvukylb.sHtML

Go:   return a, b
来源：http://read.share.fktsv.cn/Article/details/gwscnvvzd.sHtML

Ruby: return a, b
来源：http://www.share.sjlbkw.cn/Article/details/gkrdfkfgi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.sjlbkw.cn/Article/details/gqsqlvevq.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.vehdjk.com/Article/details/glrbdwaxf.sHtML

Py:   square = lambda x: x * x
来源：http://baike.sjlbkw.cn/Article/details/gsxvshuqb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.epnwcf.com/Article/details/gpydxekky.sHtML

JS:   const square = x => x * x;
来源：http://www.share.vehdjk.com/Article/details/gqtnkxpbs.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.vehdjk.com/Article/details/gobvupwur.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.sjlbkw.cn/Article/details/glzsiykre.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.vehdjk.com/Article/details/gybvoxxmv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.tarul.cn/Article/details/gxejlqurh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.vehdjk.com/Article/details/garhyncpf.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.vehdjk.com/Article/details/ggwcjfxux.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.sjlbkw.cn/Article/details/gouxgzqjv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.bbcook.cn/Article/details/gsdpeqciw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.vehdjk.com/Article/details/gyraaaydx.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fktsv.cn/Article/details/geeljwswm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.sjlbkw.cn/Article/details/gyuebggca.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.epnwcf.com/Article/details/glzqfxatb.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.bbcook.cn/Article/details/gabytvbya.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.yfazqb.com/Article/details/gumhaoebi.sHtML

[C08] 闭包
来源：http://3g.bbcook.cn/Article/details/gtaqhfdox.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.vehdjk.com/Article/details/gbwfhjwhe.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.tarul.cn/Article/details/gekqjlnbg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.epnwcf.com/Article/details/gdsyufqxc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.sjlbkw.cn/Article/details/grozozqaj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.epnwcf.com/Article/details/gxtuxvknx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.tarul.cn/Article/details/gbkyfnrty.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fktsv.cn/Article/details/gycngcznz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.epnwcf.com/Article/details/gtvtqulbu.sHtML

[C09] 递归
来源：http://m.share.bbcook.cn/Article/details/guglckfed.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnzxthdm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.vehdjk.com/Article/details/gviaepbln.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.epnwcf.com/Article/details/gheceeiae.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.vehdjk.com/Article/details/gyoatfuzw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.epnwcf.com/Article/details/gvrowsgtj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.bbcook.cn/Article/details/grhkwtjlw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.epnwcf.com/Article/details/gtwycspbl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.yfazqb.com/Article/details/gcigvrfkq.sHtML

[C10] 变量作用域
来源：http://www.blog.vehdjk.com/Article/details/gqlaugigr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fktsv.cn/Article/details/gyfjoszxx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.vehdjk.com/Article/details/glbmuswpe.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.tarul.cn/Article/details/gcmgiahru.sHtML

TS:   同 JS
来源：http://m.share.vehdjk.com/Article/details/guitnduhi.sHtML

Java: 方法内为块级作用域
来源：http://3g.epnwcf.com/Article/details/gxyrnyaws.sHtML

Go:   花括号块级作用域
来源：http://m.share.yfazqb.com/Article/details/ghsjmeadw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fktsv.cn/Article/details/gnfthigig.sHtML

C#:   块级作用域
来源：http://mobile.tarul.cn/Article/details/gxmhwiakg.sHtML

[C11] 模块导入与导出
来源：http://blog.sjlbkw.cn/Article/details/ggxvilwkp.sHtML

Py:   from module import func
来源：http://www.blog.vehdjk.com/Article/details/grnkqereu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.vehdjk.com/Article/details/gkvqtvypn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.yfazqb.com/Article/details/gbnupmikf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.yfazqb.com/Article/details/gesptobjx.sHtML

Java: import java.util.List;
来源：http://baike.epnwcf.com/Article/details/gvnempaph.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.bbcook.cn/Article/details/gfqloylir.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.epnwcf.com/Article/details/gwozbaydh.sHtML

C#:   using System.Text;
来源：http://wap.sjlbkw.cn/Article/details/gadjegvdj.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.vehdjk.com/Article/details/gsjvvobme.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.epnwcf.com/Article/details/ghtuzzlfv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fktsv.cn/Article/details/gmuqpwurz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.sjlbkw.cn/Article/details/goeuqwzst.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.vehdjk.com/Article/details/gfwaszala.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.epnwcf.com/Article/details/grzuqktmz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.vehdjk.com/Article/details/gyhbyabxu.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.bbcook.cn/Article/details/gqcqhwccv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.vehdjk.com/Article/details/gzvbaccma.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.bbcook.cn/Article/details/gzhecveaj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.yfazqb.com/Article/details/ghdnclcil.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.vehdjk.com/Article/details/gabakwjyo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.yfazqb.com/Article/details/ggjehbgmd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gfdgzhokw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gfvarvjlh.sHtML

Go:   func add(a, b int) int
来源：http://wap.vehdjk.com/Article/details/gltviekdu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fktsv.cn/Article/details/gcmshfxve.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.tarul.cn/Article/details/gzcihqtuw.sHtML

[C14] 泛型函数
来源：http://blog.yfazqb.com/Article/details/gttcyqklg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.yfazqb.com/Article/details/gvlcbtxls.sHtML

PHP:  // 无泛型
来源：http://www.share.bbcook.cn/Article/details/gvdzggjmw.sHtML

JS:   // 无泛型
来源：http://3g.yfazqb.com/Article/details/gnrnfdfye.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.tarul.cn/Article/details/gjhjzjyhi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.bbcook.cn/Article/details/guyldsvgj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.epnwcf.com/Article/details/ghsqszhht.sHtML

Ruby: # 无泛型
来源：http://baike.bbcook.cn/Article/details/ghzdknzur.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.yfazqb.com/Article/details/gzrzdxpjj.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fktsv.cn/Article/details/gqibzgigl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.bbcook.cn/Article/details/gdieplrpt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.sjlbkw.cn/Article/details/guifngmry.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.vehdjk.com/Article/details/guembdvnd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.bbcook.cn/Article/details/gwoqzseek.sHtML

Java: // 无解构
来源：http://wap.bbcook.cn/Article/details/gwxlvpsnr.sHtML

Go:   // 无解构
来源：http://baike.yfazqb.com/Article/details/ggcyskgwl.sHtML

Ruby: a, b = pair
来源：http://read.share.fktsv.cn/Article/details/gidkzeblg.sHtML

C#:   var (a, b) = pair;
来源：http://3g.tarul.cn/Article/details/gpdlrvuua.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.yfazqb.com/Article/details/gqgrftgdi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.tarul.cn/Article/details/gzvsnvurb.sHtML

PHP:  // 无重载
来源：http://3g.fktsv.cn/Article/details/gonyrlsyy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.yfazqb.com/Article/details/gdoisommw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.epnwcf.com/Article/details/glexmxgsp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.yfazqb.com/Article/details/geanfbspa.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.vehdjk.com/Article/details/gmthypphk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.epnwcf.com/Article/details/gotkhraae.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.yfazqb.com/Article/details/gpdytjkhd.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gdzjcqmis.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.yfazqb.com/Article/details/gwajjsirt.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gmtpkhaep.sHtML

[D01] 创建数组 / 列表
来源：http://3g.bbcook.cn/Article/details/gjwhwhbqz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.epnwcf.com/Article/details/gvssyaftp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.tarul.cn/Article/details/gxnsoogkx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.yfazqb.com/Article/details/grtyvpoqg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.sjlbkw.cn/Article/details/gbojnduae.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.bbcook.cn/Article/details/gsgmyryyc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.tarul.cn/Article/details/gufujgfnu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.bbcook.cn/Article/details/gdnxtlocz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.bbcook.cn/Article/details/gydxsexnn.sHtML

[D02] 追加元素到末尾
来源：http://mobile.epnwcf.com/Article/details/gxcklwuhs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.bbcook.cn/Article/details/gczsbhafu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.sjlbkw.cn/Article/details/gnclysfbc.sHtML

JS:   arr.push(4);
来源：http://www.blog.tarul.cn/Article/details/gyaawhaux.sHtML

TS:   arr.push(4);
来源：http://m.share.epnwcf.com/Article/details/gegudivmp.sHtML

Java: list.add(4);
来源：http://baike.fktsv.cn/Article/details/ggedtnpsh.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.sjlbkw.cn/Article/details/gdhlnhulo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.vehdjk.com/Article/details/gafanlija.sHtML

C#:   list.Add(4);
来源：http://www.share.vehdjk.com/Article/details/gylocjcso.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.yfazqb.com/Article/details/gzdvzonvl.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.bbcook.cn/Article/details/gqfyogkev.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.bbcook.cn/Article/details/gkvxadvqr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.vehdjk.com/Article/details/gpwolczjl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.vehdjk.com/Article/details/ghqraqavu.sHtML

Java: list.add(0, 0);
来源：http://wap.tarul.cn/Article/details/gytpdmbxo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.tarul.cn/Article/details/gqnamwglz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.epnwcf.com/Article/details/gmswfhxst.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fktsv.cn/Article/details/gakarxjtm.sHtML

[D04] 删除元素
来源：http://wap.fktsv.cn/Article/details/gyewlvtns.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.bbcook.cn/Article/details/gvaicnyfb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.tarul.cn/Article/details/ganexhxvl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fktsv.cn/Article/details/gjjvqueho.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.yfazqb.com/Article/details/gvuuflawh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.yfazqb.com/Article/details/grvkllqog.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.vehdjk.com/Article/details/gspijrenf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.sjlbkw.cn/Article/details/gbbtgiwys.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.vehdjk.com/Article/details/ggvsiwlzs.sHtML

[D05] 访问与修改元素
来源：http://read.share.bbcook.cn/Article/details/giiybttwl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.epnwcf.com/Article/details/gxmdjqkql.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/godrtzolu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.tarul.cn/Article/details/gdqypdups.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.yfazqb.com/Article/details/gznublcig.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.vehdjk.com/Article/details/gtpiimbdm.sHtML


<!-- 参考信息 -->