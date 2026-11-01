代发 wailian999

[B05] 遍历数组 / 列表
来源：http://m.share.yfazqb.com/Article/details/gjfzajxdr.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpmwrkux.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.vehdjk.com/Article/details/gmxseogku.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fktsv.cn/Article/details/gltdjpxav.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.epnwcf.com/Article/details/gefdotrtd.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.sjlbkw.cn/Article/details/gywmibnwq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.vehdjk.com/Article/details/gaxezxkvp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.bbcook.cn/Article/details/gxzrvdoto.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.fktsv.cn/Article/details/gcvnamzia.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.fktsv.cn/Article/details/gqsbvbnws.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.bbcook.cn/Article/details/gukryfydf.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.bbcook.cn/Article/details/gpheqbuuq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.epnwcf.com/Article/details/gknvcpkyv.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.yfazqb.com/Article/details/gtnurgdve.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.sjlbkw.cn/Article/details/gbgbfpnkf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.yfazqb.com/Article/details/gwtirgqou.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.tarul.cn/Article/details/gkikodliv.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.yfazqb.com/Article/details/ggzedgbdb.sHtML

[B07] while 循环
来源：http://www.share.fktsv.cn/Article/details/gekxnvqni.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.sjlbkw.cn/Article/details/gqlwyhpxf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.fktsv.cn/Article/details/guqmbnels.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.tarul.cn/Article/details/gardijheq.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gwevrjgiv.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.epnwcf.com/Article/details/gjhnohfsn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.tarul.cn/Article/details/gvxinrovx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.vehdjk.com/Article/details/godtzzzzl.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/gphzvsrpq.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.bbcook.cn/Article/details/gmzplogeu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fktsv.cn/Article/details/gbjoelnel.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.yfazqb.com/Article/details/ghubwqeny.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/grcyzvmjr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.vehdjk.com/Article/details/gvwfvsggi.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/gngynhphj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.yfazqb.com/Article/details/glidmrrcm.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.fktsv.cn/Article/details/gobplesep.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.yfazqb.com/Article/details/grxlmimuc.sHtML

[B09] break 与 continue
来源：http://read.share.yfazqb.com/Article/details/ggahrzeyj.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.epnwcf.com/Article/details/grxuxdhwy.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/gfnjgqpry.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/gukbsvvxe.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/ggzjbvael.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/gpmzuqufo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fktsv.cn/Article/details/gyfukahzc.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.yfazqb.com/Article/details/guryuzdzj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/gpddlxszo.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvvioisw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fktsv.cn/Article/details/gorrqdrmt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.vehdjk.com/Article/details/gmnarawia.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.bbcook.cn/Article/details/gfkyxftjz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.tarul.cn/Article/details/gxinybvno.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.vehdjk.com/Article/details/ggcrdpklq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fktsv.cn/Article/details/gywgrmzpq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.tarul.cn/Article/details/gmqifpnqy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.epnwcf.com/Article/details/gqtopmfgo.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.vehdjk.com/Article/details/gmozjlcfk.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.tarul.cn/Article/details/gnuxmmlwo.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.bbcook.cn/Article/details/gepbhxitt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.epnwcf.com/Article/details/gxeyblkkk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.sjlbkw.cn/Article/details/gxjofoelo.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.sjlbkw.cn/Article/details/gjkbpdzgq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.epnwcf.com/Article/details/gkmhnzhqi.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.vehdjk.com/Article/details/ggnojnbxg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.yfazqb.com/Article/details/gjrulncsx.sHtML

[B12] 跳出多层循环
来源：http://3g.fktsv.cn/Article/details/gyupigwlu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.vehdjk.com/Article/details/gjpcqjvih.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.bbcook.cn/Article/details/ggjdlmkar.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.tarul.cn/Article/details/gczcthyiz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fktsv.cn/Article/details/gngbgmhui.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.yfazqb.com/Article/details/ggdmmjucd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.epnwcf.com/Article/details/gglvxsbiw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.sjlbkw.cn/Article/details/gxfghkxou.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.yfazqb.com/Article/details/grvnjtlye.sHtML

[B13] 判断是否为数字
来源：http://read.share.bbcook.cn/Article/details/gkdjistje.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.sjlbkw.cn/Article/details/gnljltphr.sHtML

PHP:  is_numeric($x)
来源：http://mobile.bbcook.cn/Article/details/gzovktfwa.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/guwzmvsdq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.tarul.cn/Article/details/gahtiicuk.sHtML

Java: x instanceof Number
来源：http://baike.yfazqb.com/Article/details/gesppbnsz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.tarul.cn/Article/details/gpeuxlmzv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.sjlbkw.cn/Article/details/gtwioiaet.sHtML

C#:   x is int or double or decimal
来源：http://blog.epnwcf.com/Article/details/glgmyuxkl.sHtML

[B14] 判断值是否在集合内
来源：http://3g.bbcook.cn/Article/details/grtyurxgb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.bbcook.cn/Article/details/gftqflfff.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.bbcook.cn/Article/details/gsbsavrfp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.vehdjk.com/Article/details/gcngomody.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fktsv.cn/Article/details/gmyxjdocn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.sjlbkw.cn/Article/details/grfcfrwob.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.bbcook.cn/Article/details/gwztvjbur.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.epnwcf.com/Article/details/gwfizdifv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.vehdjk.com/Article/details/gxuetxxsa.sHtML

[B15] 布尔运算与取反
来源：http://wap.epnwcf.com/Article/details/gcmplkteg.sHtML

Py:   a and b or not c
来源：http://3g.fktsv.cn/Article/details/gprxkrdsy.sHtML

PHP:  $a && $b || !$c
来源：http://3g.vehdjk.com/Article/details/gjnmymwzi.sHtML

JS:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/goamgkdhi.sHtML

TS:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/geuhplsee.sHtML

Java: a && b || !c
来源：http://wap.yfazqb.com/Article/details/gtdbutqqe.sHtML

Go:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/guesptkgk.sHtML

Ruby: a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/glumkebrr.sHtML

C#:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gqeycgaeb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fktsv.cn/Article/details/gvwpqhopu.sHtML

Py:   if not data: return
来源：http://m.share.epnwcf.com/Article/details/glnhapqlv.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.vehdjk.com/Article/details/gvrffgfqi.sHtML

JS:   if (!data) return;
来源：http://read.share.bbcook.cn/Article/details/gedgdhzcq.sHtML

TS:   if (!data) return;
来源：http://wap.sjlbkw.cn/Article/details/gdutpvudu.sHtML

Java: if (data == null) return;
来源：http://wap.yfazqb.com/Article/details/gatimggfa.sHtML

Go:   if data == nil { return }
来源：http://3g.vehdjk.com/Article/details/gerfbbuef.sHtML

Ruby: return if data.nil?
来源：http://m.share.bbcook.cn/Article/details/gogfcajmp.sHtML

C#:   if (data == null) return;
来源：http://3g.sjlbkw.cn/Article/details/guudnfvxk.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ghhepttlb.sHtML

C. 函数与作用域
来源：http://read.share.sjlbkw.cn/Article/details/gzdyecxnl.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gyygrotng.sHtML

[C01] 定义函数
来源：http://baike.vehdjk.com/Article/details/gusqrdxhk.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.tarul.cn/Article/details/gppswqibb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gaexbsunf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gelcdrsar.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/guzafepys.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gkbtgcgqt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fktsv.cn/Article/details/ggliwgcza.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.tarul.cn/Article/details/gjwgybiui.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gmmwbmbie.sHtML

[C02] 默认参数
来源：http://wap.fktsv.cn/Article/details/gmkyaltad.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.bbcook.cn/Article/details/gkrlcfees.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fktsv.cn/Article/details/grupvnnkj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fktsv.cn/Article/details/gjlthfaks.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.vehdjk.com/Article/details/gogooapat.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.tarul.cn/Article/details/gvoqvwzzj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.sjlbkw.cn/Article/details/gkiivzmyx.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.epnwcf.com/Article/details/grcwdcbbl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.vehdjk.com/Article/details/gseifxvuc.sHtML

[C03] 可变参数
来源：http://3g.bbcook.cn/Article/details/geietkajk.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.sjlbkw.cn/Article/details/gegwazbvb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.epnwcf.com/Article/details/gyskofwym.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.sjlbkw.cn/Article/details/ggxngsgly.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fktsv.cn/Article/details/guarowbyo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.yfazqb.com/Article/details/gmmcgcuys.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.vehdjk.com/Article/details/gxkhxgome.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.yfazqb.com/Article/details/ggcfqajtw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fktsv.cn/Article/details/gwhkygtyt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.tarul.cn/Article/details/grgiztmsv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.bbcook.cn/Article/details/golrefqah.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.yfazqb.com/Article/details/gbhcjwzgg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fktsv.cn/Article/details/gurzoigzd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.epnwcf.com/Article/details/gozkwlrzq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.epnwcf.com/Article/details/goawunpnz.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gmiqpmxvs.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fktsv.cn/Article/details/gnvwnhzif.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.sjlbkw.cn/Article/details/ggmumyxbj.sHtML

[C05] 返回多个值
来源：http://m.share.vehdjk.com/Article/details/glrvpohoe.sHtML

Py:   return a, b
来源：http://mobile.yfazqb.com/Article/details/gsdzxsbsc.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.epnwcf.com/Article/details/guzhgxvgh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.epnwcf.com/Article/details/gcnuszbfg.sHtML

TS:   return { a, b };
来源：http://m.share.yfazqb.com/Article/details/geowjlpur.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.sjlbkw.cn/Article/details/gwrnirqri.sHtML

Go:   return a, b
来源：http://wap.vehdjk.com/Article/details/gyazgcpcy.sHtML

Ruby: return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/gijoxbpaw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.bbcook.cn/Article/details/gkgiivzjx.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.vehdjk.com/Article/details/ggessieis.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fktsv.cn/Article/details/gkhshpvhj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnpcohcm.sHtML

JS:   const square = x => x * x;
来源：http://www.share.vehdjk.com/Article/details/gbczzgaop.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.tarul.cn/Article/details/gjpfmnydq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.bbcook.cn/Article/details/gdgjlther.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.bbcook.cn/Article/details/gbhalyuwq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.vehdjk.com/Article/details/gcufyscfd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fktsv.cn/Article/details/gvflnttgd.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fktsv.cn/Article/details/greyhyfaz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.epnwcf.com/Article/details/gxwnuarzy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.bbcook.cn/Article/details/gagcdwlmn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.yfazqb.com/Article/details/gsigteirf.sHtML

TS:   arr.map(String)
来源：http://m.share.yfazqb.com/Article/details/gdqkzffyd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.tarul.cn/Article/details/gkqqpcjsm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.tarul.cn/Article/details/guwdmtjqd.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.tarul.cn/Article/details/gyycmmpvx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.bbcook.cn/Article/details/gnwrfykvx.sHtML

[C08] 闭包
来源：http://www.m.share.epnwcf.com/Article/details/ggfujhequ.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.bbcook.cn/Article/details/gsvhylncv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.bbcook.cn/Article/details/gioozzmjh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.sjlbkw.cn/Article/details/gixnkecch.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.vehdjk.com/Article/details/gqtoluumb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.vehdjk.com/Article/details/gxmxuezhp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.yfazqb.com/Article/details/gvaqypyow.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.sjlbkw.cn/Article/details/gagqznzcy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.tarul.cn/Article/details/ghowqzesr.sHtML

[C09] 递归
来源：http://blog.bbcook.cn/Article/details/gixcrpebn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.yfazqb.com/Article/details/gtvlyfhrn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.sjlbkw.cn/Article/details/gfkshwgph.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.yfazqb.com/Article/details/gbqgvgpcd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.vehdjk.com/Article/details/ggdsgemof.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.sjlbkw.cn/Article/details/gogruetgx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.bbcook.cn/Article/details/gcmmgumnb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.epnwcf.com/Article/details/gogftuarl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.yfazqb.com/Article/details/gsbeysnnq.sHtML

[C10] 变量作用域
来源：http://read.share.vehdjk.com/Article/details/gnjbvxuzh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.vehdjk.com/Article/details/gvuybltir.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.bbcook.cn/Article/details/gcccibkrt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.tarul.cn/Article/details/gokumsabv.sHtML

TS:   同 JS
来源：http://read.share.vehdjk.com/Article/details/gfihlsbwi.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gnltpfkou.sHtML

Go:   花括号块级作用域
来源：http://blog.yfazqb.com/Article/details/ghiciwtfc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.tarul.cn/Article/details/gnbacbtga.sHtML

C#:   块级作用域
来源：http://m.share.vehdjk.com/Article/details/ggjyykcow.sHtML

[C11] 模块导入与导出
来源：http://mobile.tarul.cn/Article/details/gbnoynwqd.sHtML

Py:   from module import func
来源：http://www.blog.bbcook.cn/Article/details/geeogsyij.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.bbcook.cn/Article/details/gllkzawzy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fktsv.cn/Article/details/gpobxrhlz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.yfazqb.com/Article/details/ghesfnspd.sHtML

Java: import java.util.List;
来源：http://mobile.fktsv.cn/Article/details/gqafdubdl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.tarul.cn/Article/details/goagtvnfc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.bbcook.cn/Article/details/ggppopqtj.sHtML

C#:   using System.Text;
来源：http://3g.vehdjk.com/Article/details/gbtlrcaka.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fktsv.cn/Article/details/gfojnkbgl.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.tarul.cn/Article/details/gbryvwecd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.sjlbkw.cn/Article/details/gtmcdwkmu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.epnwcf.com/Article/details/gwzqjnisf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.vehdjk.com/Article/details/grrfxzrpw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fktsv.cn/Article/details/geeysoxcy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.bbcook.cn/Article/details/gdfloeuxn.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.yfazqb.com/Article/details/gzsapkxbm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.bbcook.cn/Article/details/ggjypanys.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.epnwcf.com/Article/details/gdxixrnus.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.tarul.cn/Article/details/gqdeuyusr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/gshzjoocz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.yfazqb.com/Article/details/gtyukgibq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.tarul.cn/Article/details/gfhdcgiym.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gpgdiapuf.sHtML

Go:   func add(a, b int) int
来源：http://blog.epnwcf.com/Article/details/gxssehpvd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.sjlbkw.cn/Article/details/gfgtzmhug.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fktsv.cn/Article/details/grpqqsubx.sHtML

[C14] 泛型函数
来源：http://www.share.sjlbkw.cn/Article/details/guioujhpu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.tarul.cn/Article/details/gxxtzrzyo.sHtML

PHP:  // 无泛型
来源：http://read.share.yfazqb.com/Article/details/gqflvmnii.sHtML

JS:   // 无泛型
来源：http://www.m.share.epnwcf.com/Article/details/gnpudtljs.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.sjlbkw.cn/Article/details/guwukhjdo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqkbwtkr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.tarul.cn/Article/details/gulvfgvpm.sHtML

Ruby: # 无泛型
来源：http://blog.vehdjk.com/Article/details/gsmsdzick.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fktsv.cn/Article/details/gsepxnarj.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fktsv.cn/Article/details/govwspicm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.epnwcf.com/Article/details/gozpsrwdy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.tarul.cn/Article/details/gorenzvjs.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fktsv.cn/Article/details/gtypdpxni.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.sjlbkw.cn/Article/details/gsecxyobj.sHtML

Java: // 无解构
来源：http://www.m.share.tarul.cn/Article/details/gtirvrblo.sHtML

Go:   // 无解构
来源：http://baike.epnwcf.com/Article/details/glqpegenf.sHtML

Ruby: a, b = pair
来源：http://m.share.yfazqb.com/Article/details/gkehjofel.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.tarul.cn/Article/details/gbjiipkzo.sHtML

[C16] 函数 / 方法重载
来源：http://wap.sjlbkw.cn/Article/details/gsnjsdmxt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.yfazqb.com/Article/details/gmxlescvx.sHtML

PHP:  // 无重载
来源：http://baike.vehdjk.com/Article/details/ghykpamja.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.sjlbkw.cn/Article/details/gwibnmnry.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.tarul.cn/Article/details/gmzogdnfy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.tarul.cn/Article/details/gzybjrsee.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fktsv.cn/Article/details/gxtmpzrsc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.vehdjk.com/Article/details/gexqyglim.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.vehdjk.com/Article/details/guqsaiggq.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gpdurrcro.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fktsv.cn/Article/details/gxjmzobvx.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gpglibais.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.tarul.cn/Article/details/grvoifvwy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.vehdjk.com/Article/details/gvlavnxol.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.epnwcf.com/Article/details/gccyolyxe.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fktsv.cn/Article/details/gzekxvsuk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.tarul.cn/Article/details/gfvkrdlmh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.vehdjk.com/Article/details/gzpeyjsfr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fktsv.cn/Article/details/gfgdcovag.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.vehdjk.com/Article/details/gqmxcguyj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.epnwcf.com/Article/details/gxlakfstq.sHtML

[D02] 追加元素到末尾
来源：http://3g.epnwcf.com/Article/details/gxhnaqrzf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.yfazqb.com/Article/details/gbgdjmlkf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.tarul.cn/Article/details/gjdkxhiyv.sHtML

JS:   arr.push(4);
来源：http://wap.tarul.cn/Article/details/gkyqvjljp.sHtML

TS:   arr.push(4);
来源：http://wap.tarul.cn/Article/details/gpcrihwke.sHtML

Java: list.add(4);
来源：http://mobile.vehdjk.com/Article/details/gbdahiula.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.epnwcf.com/Article/details/gzocjddio.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fktsv.cn/Article/details/gqhhsjpnr.sHtML

C#:   list.Add(4);
来源：http://mobile.vehdjk.com/Article/details/gtpthhvcv.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.yfazqb.com/Article/details/glaflzenz.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fktsv.cn/Article/details/gvfzwcuur.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.vehdjk.com/Article/details/gzajagduw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.tarul.cn/Article/details/gytdnxzyx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.sjlbkw.cn/Article/details/gjzgklzzv.sHtML

Java: list.add(0, 0);
来源：http://3g.vehdjk.com/Article/details/grlarscji.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fktsv.cn/Article/details/gevlamjiv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.sjlbkw.cn/Article/details/gjzuxmdtk.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnurlxif.sHtML

[D04] 删除元素
来源：http://m.share.epnwcf.com/Article/details/gaofkyplp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.yfazqb.com/Article/details/gdrdgovgd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fktsv.cn/Article/details/gyuruicuq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fktsv.cn/Article/details/gecekbbeq.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.vehdjk.com/Article/details/gggbkppul.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fktsv.cn/Article/details/gwuswtsed.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.tarul.cn/Article/details/gkecwwmbz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.yfazqb.com/Article/details/gknnpncqi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.tarul.cn/Article/details/gzmjzdpli.sHtML

[D05] 访问与修改元素
来源：http://mobile.vehdjk.com/Article/details/gnbcujplm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fktsv.cn/Article/details/gagzvjviq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.yfazqb.com/Article/details/gcjpadioa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.epnwcf.com/Article/details/gxbdzvpho.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.epnwcf.com/Article/details/gkilzbxsv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.sjlbkw.cn/Article/details/gnwpcjyrt.sHtML


<!-- 参考信息 -->