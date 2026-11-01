代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fktsv.cn/Article/details/grcoyuikb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.epnwcf.com/Article/details/gqibjbyll.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.epnwcf.com/Article/details/ggniinetn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.epnwcf.com/Article/details/gfbqifrvo.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fktsv.cn/Article/details/ghyergcrn.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.tarul.cn/Article/details/gqcfreesm.sHtML

[B07] while 循环
来源：http://baike.sjlbkw.cn/Article/details/gdzwctozj.sHtML

Py:   while i < 10: i += 1
来源：http://baike.vehdjk.com/Article/details/gwhkmvdxc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.epnwcf.com/Article/details/gotajvkxu.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.epnwcf.com/Article/details/gucomruuv.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.tarul.cn/Article/details/gpkamckon.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.bbcook.cn/Article/details/gphpytwkk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhrduryl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.yfazqb.com/Article/details/gxxfgnmfk.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.tarul.cn/Article/details/gnbpkhugu.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.sjlbkw.cn/Article/details/gojxjsshe.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.bbcook.cn/Article/details/gwvtkwanc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.vehdjk.com/Article/details/gaimvdnha.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.vehdjk.com/Article/details/gkdjqhtzs.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.sjlbkw.cn/Article/details/gqcszmzev.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.yfazqb.com/Article/details/gueshgysz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.epnwcf.com/Article/details/ggdsditmu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fktsv.cn/Article/details/gqbrhgxkk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.yfazqb.com/Article/details/gelttzmmr.sHtML

[B09] break 与 continue
来源：http://wap.fktsv.cn/Article/details/gbdzyvqsz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.yfazqb.com/Article/details/gzcduzyaw.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gxsxxiamw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/grgyxoudg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/gxsxacacm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/ghbhdqdgk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.bbcook.cn/Article/details/ghaiddiik.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.fktsv.cn/Article/details/gyhznghek.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/gzuxsogan.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.vehdjk.com/Article/details/gtulshyvu.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.tarul.cn/Article/details/gjpdgjlrr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.bbcook.cn/Article/details/gxrmpzgnx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.sjlbkw.cn/Article/details/geokqoive.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fktsv.cn/Article/details/gnwabhcum.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.yfazqb.com/Article/details/gwsbfjmtt.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fktsv.cn/Article/details/gwngkdgpx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.sjlbkw.cn/Article/details/ghfyzdwig.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.tarul.cn/Article/details/ggsxiswco.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.tarul.cn/Article/details/goryimkui.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.vehdjk.com/Article/details/gcuaycznh.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.yfazqb.com/Article/details/gbkirdhvf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gpruiinvj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.epnwcf.com/Article/details/gdbupfjpj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fktsv.cn/Article/details/gvwqlpfkf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.vehdjk.com/Article/details/gxhbljwkd.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.sjlbkw.cn/Article/details/golrmjbcu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fktsv.cn/Article/details/glwpavhlp.sHtML

[B12] 跳出多层循环
来源：http://mobile.vehdjk.com/Article/details/gvdlsrmtn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.sjlbkw.cn/Article/details/goishqdqe.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.vehdjk.com/Article/details/gemlrjwhl.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyobclpwl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.yfazqb.com/Article/details/gexjebfth.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdayaqmpq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.vehdjk.com/Article/details/gmvifzkdl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.epnwcf.com/Article/details/goqvvwjsj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.yfazqb.com/Article/details/gchvuztyf.sHtML

[B13] 判断是否为数字
来源：http://read.share.sjlbkw.cn/Article/details/gxlfxapkb.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.yfazqb.com/Article/details/gbmbsckym.sHtML

PHP:  is_numeric($x)
来源：http://blog.fktsv.cn/Article/details/gqefvhzwn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fktsv.cn/Article/details/gffdpreto.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.yfazqb.com/Article/details/gwqlenjbc.sHtML

Java: x instanceof Number
来源：http://wap.vehdjk.com/Article/details/gvjbsdzhg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.vehdjk.com/Article/details/gnblnzixl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.yfazqb.com/Article/details/gaeybigmn.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fktsv.cn/Article/details/gludnbquw.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.yfazqb.com/Article/details/gxwwzfjmo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.bbcook.cn/Article/details/gzrhqxeut.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fktsv.cn/Article/details/gyyclbmpm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gxnhqrhxn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.tarul.cn/Article/details/gxyvqhsuz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.yfazqb.com/Article/details/gicueysha.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.vehdjk.com/Article/details/gjyasjewy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.bbcook.cn/Article/details/gekaxuvum.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkwvjxra.sHtML

[B15] 布尔运算与取反
来源：http://baike.sjlbkw.cn/Article/details/gwdhngixr.sHtML

Py:   a and b or not c
来源：http://baike.epnwcf.com/Article/details/gpzizbmea.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fktsv.cn/Article/details/gktlmnrud.sHtML

JS:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gendopnev.sHtML

TS:   a && b || !c
来源：http://blog.fktsv.cn/Article/details/gomlgcrlk.sHtML

Java: a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gpofoaltq.sHtML

Go:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gprvsmwjx.sHtML

Ruby: a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gncxnulbi.sHtML

C#:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gxkgpubbo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.bbcook.cn/Article/details/gapxrgwxq.sHtML

Py:   if not data: return
来源：http://www.m.share.tarul.cn/Article/details/ggsuplmui.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.epnwcf.com/Article/details/gaiagiuar.sHtML

JS:   if (!data) return;
来源：http://www.blog.epnwcf.com/Article/details/gomoowtlg.sHtML

TS:   if (!data) return;
来源：http://www.m.share.tarul.cn/Article/details/gtdsamens.sHtML

Java: if (data == null) return;
来源：http://mobile.epnwcf.com/Article/details/gcixkxgqt.sHtML

Go:   if data == nil { return }
来源：http://m.share.sjlbkw.cn/Article/details/ggvqwmmht.sHtML

Ruby: return if data.nil?
来源：http://blog.bbcook.cn/Article/details/ggyxerydp.sHtML

C#:   if (data == null) return;
来源：http://3g.bbcook.cn/Article/details/gmsphdxyo.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gqgqhnxae.sHtML

C. 函数与作用域
来源：http://mobile.vehdjk.com/Article/details/ggfnersvr.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gsfqqkqez.sHtML

[C01] 定义函数
来源：http://www.m.share.tarul.cn/Article/details/gxwtczxct.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fktsv.cn/Article/details/gdxgupgia.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/gjtqsrbcr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gkkhrwmbp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gunjjswmk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.bbcook.cn/Article/details/gfacxkvsg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.yfazqb.com/Article/details/gbrmgngla.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.vehdjk.com/Article/details/gxcokgmeo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gqqlptodb.sHtML

[C02] 默认参数
来源：http://mobile.vehdjk.com/Article/details/gdypoigqs.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.vehdjk.com/Article/details/gtajfpnbn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.yfazqb.com/Article/details/gjnmdvozd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.yfazqb.com/Article/details/gqebfkibe.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.bbcook.cn/Article/details/gkmbjicfz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.bbcook.cn/Article/details/gotfgbsxt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.vehdjk.com/Article/details/gtlgsxnkt.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.bbcook.cn/Article/details/gwjgqjknv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.bbcook.cn/Article/details/gozdzfoce.sHtML

[C03] 可变参数
来源：http://mobile.yfazqb.com/Article/details/govzpoplz.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.sjlbkw.cn/Article/details/guvznyjwh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.yfazqb.com/Article/details/gxzlkdiia.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.epnwcf.com/Article/details/gpcaiuhyi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.tarul.cn/Article/details/grhkxjvaa.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fktsv.cn/Article/details/gtlaplzcn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fktsv.cn/Article/details/gnkrolcvb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.vehdjk.com/Article/details/geuqwtxhy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.sjlbkw.cn/Article/details/gnxhyrwjz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.epnwcf.com/Article/details/gydnollvc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.yfazqb.com/Article/details/gvvnzeygl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.sjlbkw.cn/Article/details/gjaheoxpo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fktsv.cn/Article/details/ghllkozvo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fktsv.cn/Article/details/gnnagscse.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.bbcook.cn/Article/details/gpiccieuh.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.yfazqb.com/Article/details/guwpdxyrj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.vehdjk.com/Article/details/geaxfsqug.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/gsrwzpsoq.sHtML

[C05] 返回多个值
来源：http://wap.bbcook.cn/Article/details/gqxbdnkgu.sHtML

Py:   return a, b
来源：http://m.share.fktsv.cn/Article/details/gyyjnjztv.sHtML

PHP:  return [$a, $b];
来源：http://baike.bbcook.cn/Article/details/gprcunwfz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.bbcook.cn/Article/details/gucytzjbt.sHtML

TS:   return { a, b };
来源：http://baike.tarul.cn/Article/details/gypffdjpz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.epnwcf.com/Article/details/gclujeqme.sHtML

Go:   return a, b
来源：http://baike.yfazqb.com/Article/details/gsndvmmxz.sHtML

Ruby: return a, b
来源：http://baike.tarul.cn/Article/details/ghypcyrgi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.bbcook.cn/Article/details/glyodkykg.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.yfazqb.com/Article/details/gjyxtgikw.sHtML

Py:   square = lambda x: x * x
来源：http://blog.epnwcf.com/Article/details/gafmwhstb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fktsv.cn/Article/details/ghdjlcmhi.sHtML

JS:   const square = x => x * x;
来源：http://m.share.sjlbkw.cn/Article/details/gmzhqgxtj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.yfazqb.com/Article/details/gaajcttkr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.bbcook.cn/Article/details/gnurngdii.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.sjlbkw.cn/Article/details/gdpjgqcmv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.bbcook.cn/Article/details/gesfdbdez.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.tarul.cn/Article/details/gkcytqhpl.sHtML

[C07] 把函数作为参数传入
来源：http://wap.epnwcf.com/Article/details/gttyhxlbf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.tarul.cn/Article/details/gbwesoyru.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.epnwcf.com/Article/details/gvwstrjhs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.tarul.cn/Article/details/gjjjngspc.sHtML

TS:   arr.map(String)
来源：http://3g.bbcook.cn/Article/details/gviyfavje.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gfruntwaw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fktsv.cn/Article/details/gmdgdnzop.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.sjlbkw.cn/Article/details/grbigssts.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fktsv.cn/Article/details/gwhjkpevr.sHtML

[C08] 闭包
来源：http://mobile.fktsv.cn/Article/details/gddhkdrun.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.epnwcf.com/Article/details/gblntapfm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.vehdjk.com/Article/details/gmajdrjcn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.yfazqb.com/Article/details/grbxzvueb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.yfazqb.com/Article/details/gervvrmxu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.yfazqb.com/Article/details/glaoaxqgy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.bbcook.cn/Article/details/gjesuecoy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrjwkrpe.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/gxxdihstn.sHtML

[C09] 递归
来源：http://www.share.sjlbkw.cn/Article/details/gmcghxlxk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.vehdjk.com/Article/details/gogdtbjgt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fktsv.cn/Article/details/gvrhzocio.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.tarul.cn/Article/details/gnbckdweh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.vehdjk.com/Article/details/gjswuczam.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.tarul.cn/Article/details/gqmwqfywm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.yfazqb.com/Article/details/gbbrrbtzo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.sjlbkw.cn/Article/details/ghjlzjcjx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.tarul.cn/Article/details/gafwhnfrl.sHtML

[C10] 变量作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gpgzeszjs.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fktsv.cn/Article/details/gleynkfqd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.vehdjk.com/Article/details/gkfxwzzil.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.vehdjk.com/Article/details/gwihdijjv.sHtML

TS:   同 JS
来源：http://mobile.vehdjk.com/Article/details/gcedqezcc.sHtML

Java: 方法内为块级作用域
来源：http://baike.sjlbkw.cn/Article/details/gepifgtlr.sHtML

Go:   花括号块级作用域
来源：http://3g.bbcook.cn/Article/details/gargbikek.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.epnwcf.com/Article/details/gthamombc.sHtML

C#:   块级作用域
来源：http://baike.bbcook.cn/Article/details/gpmxpjlwt.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.bbcook.cn/Article/details/gnkqghwhr.sHtML

Py:   from module import func
来源：http://read.share.tarul.cn/Article/details/ggpduzwks.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.tarul.cn/Article/details/gbgzqptzp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fktsv.cn/Article/details/gvokzbzpl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.sjlbkw.cn/Article/details/gxtrezdoa.sHtML

Java: import java.util.List;
来源：http://www.m.share.fktsv.cn/Article/details/gncnhcsbr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.epnwcf.com/Article/details/gmuxmqwjr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.vehdjk.com/Article/details/gxmtffmbc.sHtML

C#:   using System.Text;
来源：http://mobile.fktsv.cn/Article/details/gcrzkusuq.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fktsv.cn/Article/details/gnundyuuy.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.epnwcf.com/Article/details/gqkaggkgn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.yfazqb.com/Article/details/gbknayswp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.sjlbkw.cn/Article/details/gqtvbkilk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.sjlbkw.cn/Article/details/gzkkjjjuj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.bbcook.cn/Article/details/gkjtcmzgo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.yfazqb.com/Article/details/gxwubfswk.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fktsv.cn/Article/details/gsvvnuskz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.bbcook.cn/Article/details/gambamwvf.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.epnwcf.com/Article/details/gedyqpkev.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.yfazqb.com/Article/details/gogttbiea.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/giecvhjug.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.epnwcf.com/Article/details/glntdjuay.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gurropzbm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gzktklnef.sHtML

Go:   func add(a, b int) int
来源：http://baike.bbcook.cn/Article/details/ghzkyxctd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.epnwcf.com/Article/details/giidxvayv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.yfazqb.com/Article/details/gsggvndrb.sHtML

[C14] 泛型函数
来源：http://mobile.yfazqb.com/Article/details/gvepkqidq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.sjlbkw.cn/Article/details/gssnkekkr.sHtML

PHP:  // 无泛型
来源：http://www.m.share.yfazqb.com/Article/details/gajiagbfm.sHtML

JS:   // 无泛型
来源：http://mobile.vehdjk.com/Article/details/gaxpyckwz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.sjlbkw.cn/Article/details/gezhgyuea.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.vehdjk.com/Article/details/gqumammyd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.epnwcf.com/Article/details/gxvrxltkq.sHtML

Ruby: # 无泛型
来源：http://www.m.share.yfazqb.com/Article/details/glzjniixq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.tarul.cn/Article/details/gtceecono.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fktsv.cn/Article/details/gexwuuucc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.bbcook.cn/Article/details/glrcltjoz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.epnwcf.com/Article/details/gzgvgyiut.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.sjlbkw.cn/Article/details/gvtusryyw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fktsv.cn/Article/details/gduvlsxym.sHtML

Java: // 无解构
来源：http://3g.epnwcf.com/Article/details/gbxbdacqd.sHtML

Go:   // 无解构
来源：http://read.share.epnwcf.com/Article/details/giowyrsra.sHtML

Ruby: a, b = pair
来源：http://mobile.fktsv.cn/Article/details/gnkesawoc.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.yfazqb.com/Article/details/gyufewhad.sHtML

[C16] 函数 / 方法重载
来源：http://blog.sjlbkw.cn/Article/details/glaiwytsi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.epnwcf.com/Article/details/ghdupjesx.sHtML

PHP:  // 无重载
来源：http://baike.fktsv.cn/Article/details/gockrzjrq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.vehdjk.com/Article/details/ganzoydti.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.sjlbkw.cn/Article/details/gnzbyugxq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fktsv.cn/Article/details/gfynokiua.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.tarul.cn/Article/details/gttaiwmqx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.sjlbkw.cn/Article/details/gzhgluqbp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.sjlbkw.cn/Article/details/gldfxbhyx.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gxqcmugmc.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.bbcook.cn/Article/details/gzmnyegrx.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gyncoipsc.sHtML

[D01] 创建数组 / 列表
来源：http://3g.epnwcf.com/Article/details/gxbyxpfuh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.vehdjk.com/Article/details/gbahgjnlr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.sjlbkw.cn/Article/details/glrcmfgkw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.tarul.cn/Article/details/gnmxnzgoi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fktsv.cn/Article/details/gifelchbk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.bbcook.cn/Article/details/ghuzuhxcf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fktsv.cn/Article/details/gasodxjly.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fktsv.cn/Article/details/gtzmnywiq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.yfazqb.com/Article/details/ggcizzyon.sHtML

[D02] 追加元素到末尾
来源：http://blog.vehdjk.com/Article/details/gxedjlcfw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.epnwcf.com/Article/details/girsbgeen.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.sjlbkw.cn/Article/details/gdlufudcx.sHtML

JS:   arr.push(4);
来源：http://mobile.yfazqb.com/Article/details/gzcvemwik.sHtML

TS:   arr.push(4);
来源：http://3g.sjlbkw.cn/Article/details/ganhxdjfg.sHtML

Java: list.add(4);
来源：http://baike.yfazqb.com/Article/details/gkggpdowl.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gytomctmi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.sjlbkw.cn/Article/details/gjoyhsuiz.sHtML

C#:   list.Add(4);
来源：http://baike.tarul.cn/Article/details/gxfzfnsxz.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.epnwcf.com/Article/details/goslalmea.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.bbcook.cn/Article/details/guxsxywpu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.tarul.cn/Article/details/gdlixkwtq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.tarul.cn/Article/details/gayqkzduk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.yfazqb.com/Article/details/gdqwadroz.sHtML

Java: list.add(0, 0);
来源：http://www.blog.tarul.cn/Article/details/guxfjglei.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.yfazqb.com/Article/details/ghfrefdpr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.tarul.cn/Article/details/gssgviqfh.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.vehdjk.com/Article/details/gwbouiugh.sHtML

[D04] 删除元素
来源：http://www.m.share.tarul.cn/Article/details/gqfrairft.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fktsv.cn/Article/details/gvuwmysbj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.epnwcf.com/Article/details/grgbpqzcw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fktsv.cn/Article/details/giaffllje.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.bbcook.cn/Article/details/guumfbjmd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fktsv.cn/Article/details/gtohwggvr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.tarul.cn/Article/details/gbhinzoox.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.bbcook.cn/Article/details/ghbvobacy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.sjlbkw.cn/Article/details/gmixrjflt.sHtML

[D05] 访问与修改元素
来源：http://m.share.sjlbkw.cn/Article/details/gwutkhhir.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.sjlbkw.cn/Article/details/ghshzuniq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.tarul.cn/Article/details/gacoqqqpr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.tarul.cn/Article/details/glsvrrdfy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.vehdjk.com/Article/details/gzmurmhkt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.yfazqb.com/Article/details/guhqcdofw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.sjlbkw.cn/Article/details/gbiskrufe.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.bbcook.cn/Article/details/gggdqwvhz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.bbcook.cn/Article/details/grkjwbnyr.sHtML

[D06] 数组长度
来源：http://www.share.yfazqb.com/Article/details/goldzttpc.sHtML

Py:   len(arr)
来源：http://wap.vehdjk.com/Article/details/gpkxpwpzy.sHtML

PHP:  count($arr);
来源：http://blog.epnwcf.com/Article/details/gcgqglhko.sHtML

JS:   arr.length
来源：http://www.share.bbcook.cn/Article/details/gxgryrxki.sHtML

TS:   arr.length
来源：http://blog.vehdjk.com/Article/details/gvtzounbt.sHtML

Java: list.size();
来源：http://read.share.yfazqb.com/Article/details/gtabbupkc.sHtML

Go:   len(arr)
来源：http://3g.sjlbkw.cn/Article/details/gcmqciixz.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.vehdjk.com/Article/details/gyizgwicq.sHtML

C#:   list.Count;
来源：http://wap.fktsv.cn/Article/details/giuqhdvzy.sHtML


<!-- 参考信息 -->