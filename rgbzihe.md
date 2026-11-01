代发 wailian999

[B05] 遍历数组 / 列表
来源：http://read.share.sjlbkw.cn/Article/details/gjiwapkzf.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.yfazqb.com/Article/details/gjerpdsbs.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fktsv.cn/Article/details/gmxznqgjw.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.sjlbkw.cn/Article/details/gnizwudab.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.fktsv.cn/Article/details/gkdfosgsk.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.epnwcf.com/Article/details/giouhycyw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fktsv.cn/Article/details/gwkzcxmwg.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.epnwcf.com/Article/details/ggjgerqbb.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.bbcook.cn/Article/details/glcaexckf.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.fktsv.cn/Article/details/gpkfdrlqw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.yfazqb.com/Article/details/gshkohhfh.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.vehdjk.com/Article/details/gkzegarlz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.yfazqb.com/Article/details/gcmxegprp.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.vehdjk.com/Article/details/gzevkntvh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.yfazqb.com/Article/details/gahchprkp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.fktsv.cn/Article/details/gkeomjqwf.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fktsv.cn/Article/details/gotauwoxw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fktsv.cn/Article/details/gqamtvxqp.sHtML

[B07] while 循环
来源：http://3g.sjlbkw.cn/Article/details/ggnnehvfz.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gbokpusua.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.vehdjk.com/Article/details/gclfwdsuq.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.vehdjk.com/Article/details/ghnfpjjpw.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.vehdjk.com/Article/details/gpbhootne.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.vehdjk.com/Article/details/gcwvupfwm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.bbcook.cn/Article/details/gljmborpm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.bbcook.cn/Article/details/gvnhlpwqz.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.epnwcf.com/Article/details/grpnkvgpj.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.fktsv.cn/Article/details/gjmejkqbq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.bbcook.cn/Article/details/griwtkyqz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.epnwcf.com/Article/details/gbpqgptad.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.bbcook.cn/Article/details/grnenrhjo.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/gvrkjegxu.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.sjlbkw.cn/Article/details/gnkyxzgtv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmztuvotq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.yfazqb.com/Article/details/gimebicit.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/getvndgpk.sHtML

[B09] break 与 continue
来源：http://www.blog.sjlbkw.cn/Article/details/ghwxlmsav.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.vehdjk.com/Article/details/gxyvagtwq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/gonfjklch.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgwgqfcf.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.sjlbkw.cn/Article/details/guobtplas.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gffebpwsd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.epnwcf.com/Article/details/gvigvqbnj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.vehdjk.com/Article/details/gztjvygfa.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.epnwcf.com/Article/details/gastucjqd.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.bbcook.cn/Article/details/gjivxuvxr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fktsv.cn/Article/details/gkfbfzhko.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.tarul.cn/Article/details/gulswddel.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.tarul.cn/Article/details/gfztddzpu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.tarul.cn/Article/details/gfvqgtufm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.sjlbkw.cn/Article/details/gijuctyuo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.tarul.cn/Article/details/gijoenfjf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fktsv.cn/Article/details/gylynipmc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.sjlbkw.cn/Article/details/gfgratezu.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.epnwcf.com/Article/details/gbnpkfofz.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.bbcook.cn/Article/details/gaocmqhoi.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.tarul.cn/Article/details/gwmsnisel.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.vehdjk.com/Article/details/gpsohikof.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fktsv.cn/Article/details/gandsptmz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.vehdjk.com/Article/details/gscmcchtx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.bbcook.cn/Article/details/grjvpbgyd.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.vehdjk.com/Article/details/gwheryggf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.yfazqb.com/Article/details/gptedyhzp.sHtML

[B12] 跳出多层循环
来源：http://baike.tarul.cn/Article/details/gssfgcyza.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.epnwcf.com/Article/details/gkrtdtgpy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.bbcook.cn/Article/details/gbqfjihjt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fktsv.cn/Article/details/gohuktgnl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/ghityeefa.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/gfzgzlcsv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.bbcook.cn/Article/details/glvtwtvin.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.bbcook.cn/Article/details/gbqrfktqz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.bbcook.cn/Article/details/gsfrscelm.sHtML

[B13] 判断是否为数字
来源：http://mobile.epnwcf.com/Article/details/gngyppxtu.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.bbcook.cn/Article/details/gsomxltfd.sHtML

PHP:  is_numeric($x)
来源：http://blog.bbcook.cn/Article/details/grmkcbtic.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.epnwcf.com/Article/details/gudxidqih.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.tarul.cn/Article/details/gfstjkcrs.sHtML

Java: x instanceof Number
来源：http://3g.fktsv.cn/Article/details/gktmqagli.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.vehdjk.com/Article/details/gkqudxdll.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.vehdjk.com/Article/details/gfhsgjcpx.sHtML

C#:   x is int or double or decimal
来源：http://baike.epnwcf.com/Article/details/ggnmbdwab.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fktsv.cn/Article/details/gasdnaiws.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.vehdjk.com/Article/details/gnywmxhic.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.vehdjk.com/Article/details/gygnliegf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.sjlbkw.cn/Article/details/gxzwytczb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.vehdjk.com/Article/details/gczlelsgg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.bbcook.cn/Article/details/gavmazars.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.yfazqb.com/Article/details/gpobylrhk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.bbcook.cn/Article/details/gyqlszbpb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.epnwcf.com/Article/details/gurnbynif.sHtML

[B15] 布尔运算与取反
来源：http://3g.tarul.cn/Article/details/gluwwtypl.sHtML

Py:   a and b or not c
来源：http://read.share.yfazqb.com/Article/details/glfxxhuhs.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.epnwcf.com/Article/details/ghodknepa.sHtML

JS:   a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/guyptqrfl.sHtML

TS:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/getfsdhyk.sHtML

Java: a && b || !c
来源：http://m.share.vehdjk.com/Article/details/guqtwimkk.sHtML

Go:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/goxcrzyzq.sHtML

Ruby: a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gxbbewvah.sHtML

C#:   a && b || !c
来源：http://baike.fktsv.cn/Article/details/gwcbkmevb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.yfazqb.com/Article/details/gxhxtpnrb.sHtML

Py:   if not data: return
来源：http://3g.sjlbkw.cn/Article/details/gnkqgbffo.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.bbcook.cn/Article/details/ggemrxiqt.sHtML

JS:   if (!data) return;
来源：http://3g.yfazqb.com/Article/details/ghyegfnmb.sHtML

TS:   if (!data) return;
来源：http://mobile.tarul.cn/Article/details/gceayfxuc.sHtML

Java: if (data == null) return;
来源：http://baike.bbcook.cn/Article/details/gzfkhalcq.sHtML

Go:   if data == nil { return }
来源：http://m.share.fktsv.cn/Article/details/grtczjbgx.sHtML

Ruby: return if data.nil?
来源：http://www.blog.vehdjk.com/Article/details/gpkohmjlu.sHtML

C#:   if (data == null) return;
来源：http://m.share.bbcook.cn/Article/details/gxpatdjzl.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gzdjmzawn.sHtML

C. 函数与作用域
来源：http://read.share.tarul.cn/Article/details/gnjofokmz.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gxxyfwvbn.sHtML

[C01] 定义函数
来源：http://blog.bbcook.cn/Article/details/gfrsmripr.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.vehdjk.com/Article/details/gfazgohfc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.tarul.cn/Article/details/gegfzgbqx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gbyasvehd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gymagadtv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gwdlrzlyw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.yfazqb.com/Article/details/ghecimmbu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.epnwcf.com/Article/details/gkjcddeub.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gawgkaqao.sHtML

[C02] 默认参数
来源：http://3g.fktsv.cn/Article/details/gtdzxxqnx.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fktsv.cn/Article/details/gocciethe.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.epnwcf.com/Article/details/gvopnqxzz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.yfazqb.com/Article/details/gzluhardd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fktsv.cn/Article/details/gamswliew.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.vehdjk.com/Article/details/ggtxjowuv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.sjlbkw.cn/Article/details/grprwjsfe.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.yfazqb.com/Article/details/glbtpstcd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fktsv.cn/Article/details/gkcozseqy.sHtML

[C03] 可变参数
来源：http://3g.vehdjk.com/Article/details/gcnpfyyyt.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fktsv.cn/Article/details/glejghavf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.bbcook.cn/Article/details/gfzmewshh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.tarul.cn/Article/details/goqoxoqyz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.vehdjk.com/Article/details/gtxlerccb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.epnwcf.com/Article/details/golqurgoy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.vehdjk.com/Article/details/ggztwciml.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.epnwcf.com/Article/details/gttowfdhe.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.sjlbkw.cn/Article/details/gejjlthgx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.sjlbkw.cn/Article/details/gmwinyipz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.bbcook.cn/Article/details/gktreglce.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.tarul.cn/Article/details/gaquzberu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.tarul.cn/Article/details/gfdpdxftq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.yfazqb.com/Article/details/gxzrganky.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.tarul.cn/Article/details/gomtpigvd.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.vehdjk.com/Article/details/gmpwaanpd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.epnwcf.com/Article/details/gznwhvzkf.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.tarul.cn/Article/details/glykmkrwo.sHtML

[C05] 返回多个值
来源：http://mobile.bbcook.cn/Article/details/gdnfqbrir.sHtML

Py:   return a, b
来源：http://www.blog.epnwcf.com/Article/details/gyuigtnes.sHtML

PHP:  return [$a, $b];
来源：http://mobile.vehdjk.com/Article/details/gyovpgryu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.bbcook.cn/Article/details/gxxqmpicp.sHtML

TS:   return { a, b };
来源：http://baike.yfazqb.com/Article/details/geprznnnc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.vehdjk.com/Article/details/gowmrbnyv.sHtML

Go:   return a, b
来源：http://blog.sjlbkw.cn/Article/details/gcznzxhhg.sHtML

Ruby: return a, b
来源：http://www.m.share.yfazqb.com/Article/details/gcvkeenov.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fktsv.cn/Article/details/gassfxxme.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.sjlbkw.cn/Article/details/geqrswiix.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.vehdjk.com/Article/details/grgptfndq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.epnwcf.com/Article/details/gjnhepszc.sHtML

JS:   const square = x => x * x;
来源：http://wap.epnwcf.com/Article/details/gsnnwwsap.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.vehdjk.com/Article/details/gfrnvbwdz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gxwmpecui.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.epnwcf.com/Article/details/gstgszjeh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.yfazqb.com/Article/details/gwpelgslo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.sjlbkw.cn/Article/details/gqkhqvrrc.sHtML

[C07] 把函数作为参数传入
来源：http://blog.bbcook.cn/Article/details/gnapqqsmd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.bbcook.cn/Article/details/gzdktlaid.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fktsv.cn/Article/details/gkgqibrep.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.vehdjk.com/Article/details/gcipdnczb.sHtML

TS:   arr.map(String)
来源：http://3g.bbcook.cn/Article/details/gpyzicrfl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fktsv.cn/Article/details/ghtyuvtfi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.yfazqb.com/Article/details/glnvbjnyv.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.vehdjk.com/Article/details/gsngmvtjw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fktsv.cn/Article/details/gyajwwynw.sHtML

[C08] 闭包
来源：http://baike.vehdjk.com/Article/details/gedwegwai.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.sjlbkw.cn/Article/details/glyhftjis.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.vehdjk.com/Article/details/gbizkgxxx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.bbcook.cn/Article/details/gmuieoduy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fktsv.cn/Article/details/gvrzteqkx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.bbcook.cn/Article/details/gphwsvbzk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fktsv.cn/Article/details/gecjdvzhf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.epnwcf.com/Article/details/gndsnwudf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.sjlbkw.cn/Article/details/gdwpwrntk.sHtML

[C09] 递归
来源：http://blog.epnwcf.com/Article/details/glozbummi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fktsv.cn/Article/details/ghhlzftlj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.epnwcf.com/Article/details/guezaakst.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.vehdjk.com/Article/details/ggsxxwrzu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.bbcook.cn/Article/details/gtszxcgxe.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmmizmtt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.tarul.cn/Article/details/guaisnsin.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.yfazqb.com/Article/details/gqrpaxiev.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.bbcook.cn/Article/details/gmainmush.sHtML

[C10] 变量作用域
来源：http://m.share.bbcook.cn/Article/details/gdvnfskio.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.tarul.cn/Article/details/gaukpirfe.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.tarul.cn/Article/details/gywfvqzrr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.epnwcf.com/Article/details/gdrggiohb.sHtML

TS:   同 JS
来源：http://read.share.tarul.cn/Article/details/glvrxokas.sHtML

Java: 方法内为块级作用域
来源：http://www.share.tarul.cn/Article/details/gcwiruosw.sHtML

Go:   花括号块级作用域
来源：http://wap.epnwcf.com/Article/details/gmizeskjn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.epnwcf.com/Article/details/gwqgvosbc.sHtML

C#:   块级作用域
来源：http://read.share.bbcook.cn/Article/details/gkqrctlst.sHtML

[C11] 模块导入与导出
来源：http://3g.fktsv.cn/Article/details/ghadcgjxw.sHtML

Py:   from module import func
来源：http://m.share.vehdjk.com/Article/details/gvtuabevx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.yfazqb.com/Article/details/gujzeqvzr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.sjlbkw.cn/Article/details/gumnqlavn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.sjlbkw.cn/Article/details/gkunbygee.sHtML

Java: import java.util.List;
来源：http://read.share.sjlbkw.cn/Article/details/gbuwxzsvg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fktsv.cn/Article/details/gyehaqghi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.yfazqb.com/Article/details/gouqujvfi.sHtML

C#:   using System.Text;
来源：http://baike.tarul.cn/Article/details/gfruzfvwi.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.tarul.cn/Article/details/gidtjckwz.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.yfazqb.com/Article/details/gierflsdi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fktsv.cn/Article/details/gydovdtws.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fktsv.cn/Article/details/gjtikhlpb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.sjlbkw.cn/Article/details/glapswjmu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.bbcook.cn/Article/details/gofnnqpkj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.tarul.cn/Article/details/gvotqsknw.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.sjlbkw.cn/Article/details/gtmvwwxbr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.tarul.cn/Article/details/ghczowwej.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.bbcook.cn/Article/details/gzzxtufqc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.tarul.cn/Article/details/gnhseaxbr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.sjlbkw.cn/Article/details/gyezfvwsq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.sjlbkw.cn/Article/details/gwgejthqv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.tarul.cn/Article/details/grqxlwvyh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gtclnkifn.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fktsv.cn/Article/details/gwnhlalde.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.vehdjk.com/Article/details/gzfxntjiv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.vehdjk.com/Article/details/gimsrysfz.sHtML

[C14] 泛型函数
来源：http://baike.epnwcf.com/Article/details/gonzpqmmb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.bbcook.cn/Article/details/gnjqbklrd.sHtML

PHP:  // 无泛型
来源：http://3g.fktsv.cn/Article/details/gcsukqdso.sHtML

JS:   // 无泛型
来源：http://www.m.share.yfazqb.com/Article/details/gzoezqpja.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.epnwcf.com/Article/details/gybqimymm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.sjlbkw.cn/Article/details/glkltwhou.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.yfazqb.com/Article/details/gjhoyjncz.sHtML

Ruby: # 无泛型
来源：http://www.share.sjlbkw.cn/Article/details/gaicnrzpx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.bbcook.cn/Article/details/gktirocim.sHtML

[C15] 解构 / 展开参数
来源：http://blog.sjlbkw.cn/Article/details/gshnbgodc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.epnwcf.com/Article/details/gxohnxarj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.epnwcf.com/Article/details/ghufkcaas.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.yfazqb.com/Article/details/gkmuuhwot.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.yfazqb.com/Article/details/gvwuarmov.sHtML

Java: // 无解构
来源：http://www.m.share.tarul.cn/Article/details/gsbqmiwkd.sHtML

Go:   // 无解构
来源：http://www.m.share.epnwcf.com/Article/details/gslpnqooi.sHtML

Ruby: a, b = pair
来源：http://wap.tarul.cn/Article/details/gvrbztchx.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.bbcook.cn/Article/details/grslvnlyd.sHtML

[C16] 函数 / 方法重载
来源：http://baike.tarul.cn/Article/details/gglkihdgy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.epnwcf.com/Article/details/gddzvfwhn.sHtML

PHP:  // 无重载
来源：http://www.m.share.bbcook.cn/Article/details/gwdpvmion.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.sjlbkw.cn/Article/details/ghfdltuia.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.bbcook.cn/Article/details/glzrdcwjn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.yfazqb.com/Article/details/gboncndpt.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.bbcook.cn/Article/details/ggkpfggpb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.sjlbkw.cn/Article/details/gxmvuvxgq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.yfazqb.com/Article/details/gklmysxwk.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gtluvdubo.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.tarul.cn/Article/details/ggbsinqqu.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gyfhdwdcu.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.tarul.cn/Article/details/ghvljormd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.bbcook.cn/Article/details/ghzjbtghu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.tarul.cn/Article/details/gfrxopwon.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.vehdjk.com/Article/details/goagjqnzz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.sjlbkw.cn/Article/details/gdlynaizu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.yfazqb.com/Article/details/gcbvyllxh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.sjlbkw.cn/Article/details/gatdlyomw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.sjlbkw.cn/Article/details/gffiojbnv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.yfazqb.com/Article/details/gyottunxx.sHtML

[D02] 追加元素到末尾
来源：http://baike.vehdjk.com/Article/details/gricprdrg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.yfazqb.com/Article/details/ggakntnya.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fktsv.cn/Article/details/gfhlcryyu.sHtML

JS:   arr.push(4);
来源：http://3g.sjlbkw.cn/Article/details/gwqpguaaj.sHtML

TS:   arr.push(4);
来源：http://www.share.bbcook.cn/Article/details/gysqbqivy.sHtML

Java: list.add(4);
来源：http://www.m.share.epnwcf.com/Article/details/gxedbiobv.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.epnwcf.com/Article/details/gdsopiobo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.sjlbkw.cn/Article/details/gxorjlrzw.sHtML

C#:   list.Add(4);
来源：http://m.share.tarul.cn/Article/details/gtzryineq.sHtML

[D03] 在指定位置插入元素
来源：http://wap.epnwcf.com/Article/details/gwaivqifw.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.vehdjk.com/Article/details/gvpkgdpie.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.yfazqb.com/Article/details/gpdpkhafx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.yfazqb.com/Article/details/gpejuqciz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.bbcook.cn/Article/details/glwrqujit.sHtML

Java: list.add(0, 0);
来源：http://read.share.tarul.cn/Article/details/gmlmzvfzl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.bbcook.cn/Article/details/gwlblakor.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.epnwcf.com/Article/details/gxlpnciom.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fktsv.cn/Article/details/glewhgljf.sHtML

[D04] 删除元素
来源：http://read.share.epnwcf.com/Article/details/glkpqcpni.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.tarul.cn/Article/details/gbgaknaxr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.yfazqb.com/Article/details/gmkvczaff.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.yfazqb.com/Article/details/guktvvbpd.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.epnwcf.com/Article/details/gxdmujrbd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.epnwcf.com/Article/details/gqsedsmwr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.tarul.cn/Article/details/glmewxvxe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.vehdjk.com/Article/details/goqovaadk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.epnwcf.com/Article/details/gemyskhhl.sHtML

[D05] 访问与修改元素
来源：http://blog.vehdjk.com/Article/details/grivfksml.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.epnwcf.com/Article/details/gxdowfglp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.bbcook.cn/Article/details/gszertodj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.tarul.cn/Article/details/gpprcxbyj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.bbcook.cn/Article/details/gprkvyceh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fktsv.cn/Article/details/gwlmxfccw.sHtML


<!-- 参考信息 -->