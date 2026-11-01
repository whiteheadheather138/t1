代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.sjlbkw.cn/Article/details/gczvytlpv.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.epnwcf.com/Article/details/gizjvkmnp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.bbcook.cn/Article/details/grtrczwzm.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.vehdjk.com/Article/details/gasmkucay.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.tarul.cn/Article/details/gjeauhadx.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.sjlbkw.cn/Article/details/grquzffdu.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.sjlbkw.cn/Article/details/gajbmetrd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.bbcook.cn/Article/details/gvxyppsfx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.vehdjk.com/Article/details/gepadvmrw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.tarul.cn/Article/details/gkmysrghx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.bbcook.cn/Article/details/guyavxyiy.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.yfazqb.com/Article/details/gvdjpgnsz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.sjlbkw.cn/Article/details/gqdyqgraa.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.epnwcf.com/Article/details/gezhnhqes.sHtML

[B07] while 循环
来源：http://3g.epnwcf.com/Article/details/goonlrtxh.sHtML

Py:   while i < 10: i += 1
来源：http://wap.bbcook.cn/Article/details/gzswwxfii.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.vehdjk.com/Article/details/gnkdkfhno.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.bbcook.cn/Article/details/ggisfefjy.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/gokucmnpg.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.bbcook.cn/Article/details/ganwrticz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.sjlbkw.cn/Article/details/gcwepzlpv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.sjlbkw.cn/Article/details/gyvsaxrps.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.sjlbkw.cn/Article/details/grjruvxxr.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.fktsv.cn/Article/details/gndmlbehh.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.bbcook.cn/Article/details/ghtitppkh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.bbcook.cn/Article/details/gtmmistfw.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.tarul.cn/Article/details/gmswcgvav.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.vehdjk.com/Article/details/gxdllpfok.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/gtaacmuej.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.bbcook.cn/Article/details/grkzqdnav.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.vehdjk.com/Article/details/ggfruxood.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.tarul.cn/Article/details/gohnqvnkj.sHtML

[B09] break 与 continue
来源：http://baike.bbcook.cn/Article/details/grcvcwyoz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.tarul.cn/Article/details/gpudyalul.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/ggxejlnpd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/glaicqtrt.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.tarul.cn/Article/details/givquaykq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gsilbwirt.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fktsv.cn/Article/details/goqkpmmsz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.bbcook.cn/Article/details/gycascjuy.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/gaumlthky.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.sjlbkw.cn/Article/details/gmochhdyt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.sjlbkw.cn/Article/details/gikiidyyz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.vehdjk.com/Article/details/gaaiosckr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fktsv.cn/Article/details/gysbgfftl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.epnwcf.com/Article/details/gkpiwubzf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.yfazqb.com/Article/details/grqjnkern.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.vehdjk.com/Article/details/gqdpvypev.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.epnwcf.com/Article/details/gaszblbek.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.tarul.cn/Article/details/goxzikqat.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.yfazqb.com/Article/details/gynsxtnbn.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.sjlbkw.cn/Article/details/gancfrzmz.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.vehdjk.com/Article/details/gfurqjnne.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.sjlbkw.cn/Article/details/gboazlfvb.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.epnwcf.com/Article/details/gtrijlgev.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.tarul.cn/Article/details/gupacjddu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqcizcak.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.bbcook.cn/Article/details/gshnqantx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.bbcook.cn/Article/details/gejougjel.sHtML

[B12] 跳出多层循环
来源：http://wap.sjlbkw.cn/Article/details/gfztyzodp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.epnwcf.com/Article/details/gbkmaicod.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.sjlbkw.cn/Article/details/gkzfzvuak.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.tarul.cn/Article/details/grrftbjkf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.yfazqb.com/Article/details/gdiqkbnvb.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.vehdjk.com/Article/details/gpscociei.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.tarul.cn/Article/details/gzrkfqbmc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.yfazqb.com/Article/details/gwczopbjw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.tarul.cn/Article/details/gdpvocfdu.sHtML

[B13] 判断是否为数字
来源：http://mobile.vehdjk.com/Article/details/gnifnyajp.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.sjlbkw.cn/Article/details/gomvwulkn.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.bbcook.cn/Article/details/ggtxiwokd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.bbcook.cn/Article/details/ghjfocukh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.sjlbkw.cn/Article/details/gyurdjfcd.sHtML

Java: x instanceof Number
来源：http://baike.sjlbkw.cn/Article/details/golmgomcy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.vehdjk.com/Article/details/gevupridr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.sjlbkw.cn/Article/details/gyqbmmyux.sHtML

C#:   x is int or double or decimal
来源：http://3g.tarul.cn/Article/details/gchuudcar.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fktsv.cn/Article/details/gcwzyyqjl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.epnwcf.com/Article/details/gdtviebln.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.yfazqb.com/Article/details/glfknucea.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.yfazqb.com/Article/details/gosflhrdx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fktsv.cn/Article/details/gkjbmjudu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.vehdjk.com/Article/details/gswmrstrb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fktsv.cn/Article/details/gzzpmtulj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gllplcemo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.bbcook.cn/Article/details/gybbhasyk.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.tarul.cn/Article/details/gqpuktvmg.sHtML

Py:   a and b or not c
来源：http://www.m.share.yfazqb.com/Article/details/gtdrhyjuu.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.yfazqb.com/Article/details/ggiwpdgau.sHtML

JS:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/gyeujubxz.sHtML

TS:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/gjxuoxnhq.sHtML

Java: a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gkyezmhqs.sHtML

Go:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/gxqrwwgpy.sHtML

Ruby: a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gyvrihzuj.sHtML

C#:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gabvohxcn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.bbcook.cn/Article/details/ggmyavibm.sHtML

Py:   if not data: return
来源：http://www.share.sjlbkw.cn/Article/details/gqudzpmda.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.tarul.cn/Article/details/gsjyfepag.sHtML

JS:   if (!data) return;
来源：http://wap.vehdjk.com/Article/details/gcrfeckfy.sHtML

TS:   if (!data) return;
来源：http://www.m.share.bbcook.cn/Article/details/gzhekhvij.sHtML

Java: if (data == null) return;
来源：http://www.m.share.vehdjk.com/Article/details/gmiwkawwi.sHtML

Go:   if data == nil { return }
来源：http://baike.fktsv.cn/Article/details/gnenkteam.sHtML

Ruby: return if data.nil?
来源：http://wap.vehdjk.com/Article/details/givmxvseh.sHtML

C#:   if (data == null) return;
来源：http://mobile.vehdjk.com/Article/details/gkmjwqvwn.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/geoyjamlq.sHtML

C. 函数与作用域
来源：http://wap.sjlbkw.cn/Article/details/gvfyzbqxb.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gmuppjmef.sHtML

[C01] 定义函数
来源：http://www.share.epnwcf.com/Article/details/guzaxxyvt.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fktsv.cn/Article/details/gyucqoeiy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.epnwcf.com/Article/details/gizhlswzq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.vehdjk.com/Article/details/gpjmgwzji.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/ggxzaellc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gveyarkvy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.bbcook.cn/Article/details/gwmqctamj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.sjlbkw.cn/Article/details/gmpurveex.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gllaerxfq.sHtML

[C02] 默认参数
来源：http://wap.yfazqb.com/Article/details/gsrykpasw.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.epnwcf.com/Article/details/gyodmztgl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.bbcook.cn/Article/details/gszgoqble.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.yfazqb.com/Article/details/gxqpotsqq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fktsv.cn/Article/details/glesembvn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.yfazqb.com/Article/details/gvviejfrn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.bbcook.cn/Article/details/gaphjvzbj.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.bbcook.cn/Article/details/gexnhqbet.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fktsv.cn/Article/details/gwoacjmtw.sHtML

[C03] 可变参数
来源：http://wap.sjlbkw.cn/Article/details/gmolggyeg.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.sjlbkw.cn/Article/details/gbbngvnci.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.vehdjk.com/Article/details/gkxxpfaqr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.tarul.cn/Article/details/giszyccha.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.epnwcf.com/Article/details/gzqkjafom.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.epnwcf.com/Article/details/gxknbrfji.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.epnwcf.com/Article/details/gjwkcmgsr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.epnwcf.com/Article/details/gykvoqbgx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fktsv.cn/Article/details/gyriroaim.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.yfazqb.com/Article/details/gupjrrqss.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.bbcook.cn/Article/details/gqegebmuq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.yfazqb.com/Article/details/gcosllegm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fktsv.cn/Article/details/gyunylmuo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.yfazqb.com/Article/details/gizncrzki.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.yfazqb.com/Article/details/gntafanwl.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fktsv.cn/Article/details/gnevlbtxb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.vehdjk.com/Article/details/gllldnjsj.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.sjlbkw.cn/Article/details/gcvutxmns.sHtML

[C05] 返回多个值
来源：http://www.share.yfazqb.com/Article/details/ghknpgnam.sHtML

Py:   return a, b
来源：http://blog.tarul.cn/Article/details/goppfghyx.sHtML

PHP:  return [$a, $b];
来源：http://3g.epnwcf.com/Article/details/gujmlhjen.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.vehdjk.com/Article/details/gfgxtuagb.sHtML

TS:   return { a, b };
来源：http://mobile.vehdjk.com/Article/details/grwipgqth.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.sjlbkw.cn/Article/details/gcjgsntyk.sHtML

Go:   return a, b
来源：http://www.blog.bbcook.cn/Article/details/gjfypbimm.sHtML

Ruby: return a, b
来源：http://m.share.bbcook.cn/Article/details/gotwjbzxd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fktsv.cn/Article/details/geesitlsu.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fktsv.cn/Article/details/gdqwjpgum.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.epnwcf.com/Article/details/gxmhynvic.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.yfazqb.com/Article/details/gllwlxukw.sHtML

JS:   const square = x => x * x;
来源：http://blog.sjlbkw.cn/Article/details/gxzrdgaht.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.sjlbkw.cn/Article/details/gtsfitjug.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.tarul.cn/Article/details/gkosmmegh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.yfazqb.com/Article/details/gawiykrhb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.epnwcf.com/Article/details/gkfbsybwk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.tarul.cn/Article/details/gwckgqswc.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.sjlbkw.cn/Article/details/gvwoywnec.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.yfazqb.com/Article/details/gtoxsodhu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gwlipjudg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.tarul.cn/Article/details/gmvbonhep.sHtML

TS:   arr.map(String)
来源：http://baike.yfazqb.com/Article/details/ggiywuzux.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.epnwcf.com/Article/details/ghidbrgvk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.bbcook.cn/Article/details/gmlcirwga.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.bbcook.cn/Article/details/ghjdyapdq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.vehdjk.com/Article/details/guohjovma.sHtML

[C08] 闭包
来源：http://wap.yfazqb.com/Article/details/gzcpmvloc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.vehdjk.com/Article/details/gluuwsozp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.vehdjk.com/Article/details/gkeugzkdg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.epnwcf.com/Article/details/gtlgtfbjx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.sjlbkw.cn/Article/details/glnxkdozt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fktsv.cn/Article/details/gbnnbblom.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.sjlbkw.cn/Article/details/ghdijmfkr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.vehdjk.com/Article/details/gzswyjhbl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.yfazqb.com/Article/details/gvrsdquzv.sHtML

[C09] 递归
来源：http://3g.yfazqb.com/Article/details/gaosieqay.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.tarul.cn/Article/details/gewummnuk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnktbodb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.yfazqb.com/Article/details/gjpnhyjfx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fktsv.cn/Article/details/gpzggtiqp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.epnwcf.com/Article/details/gxnbpfyow.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.epnwcf.com/Article/details/godeumycv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.tarul.cn/Article/details/gdvzzrtvz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.tarul.cn/Article/details/gypiavwfa.sHtML

[C10] 变量作用域
来源：http://mobile.fktsv.cn/Article/details/gkjxtzdma.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.tarul.cn/Article/details/gobbgezts.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fktsv.cn/Article/details/gpdnfpkyu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fktsv.cn/Article/details/gsduezaya.sHtML

TS:   同 JS
来源：http://3g.yfazqb.com/Article/details/gsvxtclwv.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.vehdjk.com/Article/details/gronredhf.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.sjlbkw.cn/Article/details/gepcvuwie.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.tarul.cn/Article/details/gqfnpybuj.sHtML

C#:   块级作用域
来源：http://wap.bbcook.cn/Article/details/gbanrulrr.sHtML

[C11] 模块导入与导出
来源：http://3g.yfazqb.com/Article/details/gpodadryy.sHtML

Py:   from module import func
来源：http://www.share.bbcook.cn/Article/details/gogrcnfed.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.bbcook.cn/Article/details/gmmepuwam.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fktsv.cn/Article/details/gvtvhjbjh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.bbcook.cn/Article/details/gdkykdxmx.sHtML

Java: import java.util.List;
来源：http://wap.fktsv.cn/Article/details/gkgjbnmhw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fktsv.cn/Article/details/gbawyrebt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.vehdjk.com/Article/details/gyhspzdgy.sHtML

C#:   using System.Text;
来源：http://www.blog.epnwcf.com/Article/details/gnsdyghmz.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.sjlbkw.cn/Article/details/gxzoatwyh.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.tarul.cn/Article/details/gaqaipwun.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.yfazqb.com/Article/details/gjfebjedq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.vehdjk.com/Article/details/gslrhtkzs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.sjlbkw.cn/Article/details/gpssjckwr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.epnwcf.com/Article/details/gsxijsema.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.vehdjk.com/Article/details/gekltshgi.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.tarul.cn/Article/details/getnfinap.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fktsv.cn/Article/details/glsbkugwh.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.epnwcf.com/Article/details/gohswucud.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.yfazqb.com/Article/details/gexrkoeij.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.vehdjk.com/Article/details/gtdxepxgq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.sjlbkw.cn/Article/details/gvzldszsd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gtoigjibi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.tarul.cn/Article/details/gzfvjcoqk.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.vehdjk.com/Article/details/gfjoqrvro.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.epnwcf.com/Article/details/giexsbuhv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.sjlbkw.cn/Article/details/gdkmycwbd.sHtML

[C14] 泛型函数
来源：http://www.share.bbcook.cn/Article/details/glroyhqdf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.vehdjk.com/Article/details/gdkxrlttl.sHtML

PHP:  // 无泛型
来源：http://wap.bbcook.cn/Article/details/gwajvlexe.sHtML

JS:   // 无泛型
来源：http://baike.epnwcf.com/Article/details/gxiaqpfkv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.vehdjk.com/Article/details/gqphesrnt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.sjlbkw.cn/Article/details/gcgjavtqv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.bbcook.cn/Article/details/gjaphozds.sHtML

Ruby: # 无泛型
来源：http://www.blog.vehdjk.com/Article/details/gxffnjbhl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.vehdjk.com/Article/details/gdpzmkoux.sHtML

[C15] 解构 / 展开参数
来源：http://wap.bbcook.cn/Article/details/gojeflbtb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.sjlbkw.cn/Article/details/gtkcjulhf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.yfazqb.com/Article/details/ggmrckosf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.sjlbkw.cn/Article/details/gnpicvphs.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.tarul.cn/Article/details/gxyrmwlxw.sHtML

Java: // 无解构
来源：http://www.blog.vehdjk.com/Article/details/gdkbxtufw.sHtML

Go:   // 无解构
来源：http://www.blog.yfazqb.com/Article/details/gdxgjxiwj.sHtML

Ruby: a, b = pair
来源：http://wap.fktsv.cn/Article/details/gamqoovff.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.bbcook.cn/Article/details/gbtkusivq.sHtML

[C16] 函数 / 方法重载
来源：http://blog.vehdjk.com/Article/details/gslxjoapj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.epnwcf.com/Article/details/giswsoqzz.sHtML

PHP:  // 无重载
来源：http://mobile.tarul.cn/Article/details/gjblqvwob.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.yfazqb.com/Article/details/gbenxvbtz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.epnwcf.com/Article/details/gvncinolz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.bbcook.cn/Article/details/gbbxssonk.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.yfazqb.com/Article/details/gpusrfttp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fktsv.cn/Article/details/gwosavdzv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.vehdjk.com/Article/details/grcliflsk.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/guqyxhtql.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fktsv.cn/Article/details/gupqwfpxb.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/ghoqspovt.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.tarul.cn/Article/details/gpavtejds.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.sjlbkw.cn/Article/details/gkatdnoew.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fktsv.cn/Article/details/gknhiwiqv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.sjlbkw.cn/Article/details/gekyykwxo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.sjlbkw.cn/Article/details/gmggfiplg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.yfazqb.com/Article/details/ggtrcvjdl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.tarul.cn/Article/details/gfendbnhl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.tarul.cn/Article/details/gbzqwwnco.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.vehdjk.com/Article/details/gqgtjmsym.sHtML

[D02] 追加元素到末尾
来源：http://www.share.yfazqb.com/Article/details/gdtatehmg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.epnwcf.com/Article/details/gfiiyplrl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.bbcook.cn/Article/details/gfdrqnhid.sHtML

JS:   arr.push(4);
来源：http://3g.vehdjk.com/Article/details/godwtfwiy.sHtML

TS:   arr.push(4);
来源：http://m.share.tarul.cn/Article/details/gdfjfpwpu.sHtML

Java: list.add(4);
来源：http://www.blog.bbcook.cn/Article/details/gjfajgrso.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gpdvkfgtd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.yfazqb.com/Article/details/gqzotfars.sHtML

C#:   list.Add(4);
来源：http://mobile.vehdjk.com/Article/details/gukxuzbby.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.yfazqb.com/Article/details/gyzwaxwwz.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.vehdjk.com/Article/details/gpaftmztt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.vehdjk.com/Article/details/gfoqnpmse.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.yfazqb.com/Article/details/gvyckvdba.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.vehdjk.com/Article/details/gclunbdne.sHtML

Java: list.add(0, 0);
来源：http://wap.tarul.cn/Article/details/ghjtyzplo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.tarul.cn/Article/details/gbmfjrddz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.vehdjk.com/Article/details/gezawinne.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.yfazqb.com/Article/details/gydqlygfi.sHtML

[D04] 删除元素
来源：http://wap.yfazqb.com/Article/details/gifcvozsz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fktsv.cn/Article/details/gyxewgebc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.epnwcf.com/Article/details/gajlrxjco.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.bbcook.cn/Article/details/gnvfhbbts.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fktsv.cn/Article/details/gxsgknzar.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.epnwcf.com/Article/details/ggmsrxsqg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fktsv.cn/Article/details/glenvbhoa.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fktsv.cn/Article/details/gjtylzpnl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.epnwcf.com/Article/details/gbbtbvbzh.sHtML

[D05] 访问与修改元素
来源：http://read.share.yfazqb.com/Article/details/galjfsaqs.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fktsv.cn/Article/details/gxxsfinyo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.yfazqb.com/Article/details/ghskdtwhf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.bbcook.cn/Article/details/gomkeuwqa.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.sjlbkw.cn/Article/details/gllkthrvt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fktsv.cn/Article/details/gklsukzyj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.bbcook.cn/Article/details/gihkkevdk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.bbcook.cn/Article/details/galkchsey.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.yfazqb.com/Article/details/gwgamfmnv.sHtML

[D06] 数组长度
来源：http://3g.vehdjk.com/Article/details/gwcipmcaq.sHtML


<!-- 参考信息 -->