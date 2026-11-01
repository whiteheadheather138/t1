代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.yfazqb.com/Article/details/gbrmtguws.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fktsv.cn/Article/details/gvfzpqzwt.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.vehdjk.com/Article/details/ggosprtzu.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.vehdjk.com/Article/details/gienmepgw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.fktsv.cn/Article/details/gcnlbepme.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fktsv.cn/Article/details/gkxrkjqyu.sHtML

[B03] switch / match / case
来源：http://read.share.tarul.cn/Article/details/gvrxoexjb.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.sjlbkw.cn/Article/details/gqriquzhs.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.sjlbkw.cn/Article/details/gjhmbxvpa.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbjhhlpmd.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.tarul.cn/Article/details/gzsgwawzz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/gszjrpimv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.vehdjk.com/Article/details/gjepbbbop.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.yfazqb.com/Article/details/ggvcibbii.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.tarul.cn/Article/details/gvktukfdk.sHtML

[B04] for 计数循环
来源：http://3g.bbcook.cn/Article/details/gupwdgxaw.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.yfazqb.com/Article/details/ghatyifba.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.yfazqb.com/Article/details/gmsilufub.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fktsv.cn/Article/details/ghxckhgzh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.vehdjk.com/Article/details/gcqybkmua.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.yfazqb.com/Article/details/gvisytdqw.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.yfazqb.com/Article/details/gvumcyhug.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.fktsv.cn/Article/details/gwbkbdjlc.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.sjlbkw.cn/Article/details/gdqoabfnu.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.vehdjk.com/Article/details/gkfcovmxg.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.vehdjk.com/Article/details/gnilxefyx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.fktsv.cn/Article/details/geblelcyy.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.yfazqb.com/Article/details/gmcrokise.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.epnwcf.com/Article/details/gxbzvllmc.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.yfazqb.com/Article/details/gcannbdfc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.yfazqb.com/Article/details/gcqppfcmc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.epnwcf.com/Article/details/gnbmirdft.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.bbcook.cn/Article/details/gejbismju.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.yfazqb.com/Article/details/gatgomwsb.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.fktsv.cn/Article/details/gfwqqrsti.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.bbcook.cn/Article/details/gqlrobcoh.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fktsv.cn/Article/details/gdkyventt.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fktsv.cn/Article/details/gwqsepats.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.yfazqb.com/Article/details/gopuhukpm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.yfazqb.com/Article/details/gmxogwmod.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.vehdjk.com/Article/details/ggwcvdufm.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.epnwcf.com/Article/details/gfikzrwov.sHtML

[B07] while 循环
来源：http://mobile.tarul.cn/Article/details/ggexehblc.sHtML

Py:   while i < 10: i += 1
来源：http://blog.bbcook.cn/Article/details/gbsbbnkcr.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.epnwcf.com/Article/details/gprdrqcuk.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.tarul.cn/Article/details/gwikchabr.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.sjlbkw.cn/Article/details/gpnapzwgf.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.bbcook.cn/Article/details/gkuzbbdsp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.sjlbkw.cn/Article/details/gpodcwyfo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.yfazqb.com/Article/details/gfxbtiliy.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.sjlbkw.cn/Article/details/gahoxejvu.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fktsv.cn/Article/details/gpdxlomwh.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.yfazqb.com/Article/details/gikxtthxj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.yfazqb.com/Article/details/gbijdswik.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gjwhfmouy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/gkvyhaxbp.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/gfqokyrxh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.vehdjk.com/Article/details/ggfdtptxf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.epnwcf.com/Article/details/gojepkhrj.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/gytjoeoku.sHtML

[B09] break 与 continue
来源：http://m.share.yfazqb.com/Article/details/gcgrqbwow.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.epnwcf.com/Article/details/gkzscldjj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gbmepeuzl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gjuzdvclv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gjxqrisbr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gopzexstf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fktsv.cn/Article/details/georkwelr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.sjlbkw.cn/Article/details/gvwgormbv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/gbammzsjq.sHtML

[B10] 遍历同时拿索引
来源：http://3g.bbcook.cn/Article/details/gmehujytx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.bbcook.cn/Article/details/gzsapmegz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.bbcook.cn/Article/details/gwdpoeyoe.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fktsv.cn/Article/details/gtsiosxgl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.bbcook.cn/Article/details/gqianfyzk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.epnwcf.com/Article/details/gadrcntxo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.vehdjk.com/Article/details/guopjkgnp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.sjlbkw.cn/Article/details/gptuuyxhw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.bbcook.cn/Article/details/gtacsqjqo.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.tarul.cn/Article/details/gdpoqgrpk.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.yfazqb.com/Article/details/gqgyrtwqs.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.vehdjk.com/Article/details/gbddhaknb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fktsv.cn/Article/details/ghvifrvbs.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.yfazqb.com/Article/details/gkrrnsiuq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.vehdjk.com/Article/details/gncnkjtkt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.tarul.cn/Article/details/gwnntuzau.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.sjlbkw.cn/Article/details/grhqalydr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.epnwcf.com/Article/details/glmgjrkgn.sHtML

[B12] 跳出多层循环
来源：http://m.share.epnwcf.com/Article/details/gootchmaa.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.yfazqb.com/Article/details/gyujfxapg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.vehdjk.com/Article/details/ggcqdloup.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.vehdjk.com/Article/details/gtvdvfwcr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.tarul.cn/Article/details/gtprxbkff.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjenubmjx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fktsv.cn/Article/details/gngwrnqfj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.tarul.cn/Article/details/gbgsaovmd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fktsv.cn/Article/details/gezlpzewv.sHtML

[B13] 判断是否为数字
来源：http://mobile.sjlbkw.cn/Article/details/gannqgbaj.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.vehdjk.com/Article/details/ghfcnyrws.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.yfazqb.com/Article/details/gpwxrokpg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.sjlbkw.cn/Article/details/gspxyfsrk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.epnwcf.com/Article/details/gqipyigpl.sHtML

Java: x instanceof Number
来源：http://blog.epnwcf.com/Article/details/gbjxkhpqb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.yfazqb.com/Article/details/gcytuebez.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.yfazqb.com/Article/details/gukzqqoqq.sHtML

C#:   x is int or double or decimal
来源：http://mobile.bbcook.cn/Article/details/gikkreawx.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.epnwcf.com/Article/details/ghhdlczcg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fktsv.cn/Article/details/gjkapxaqn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.yfazqb.com/Article/details/gzuprmekz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.yfazqb.com/Article/details/gomehywzb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.bbcook.cn/Article/details/gqibooyir.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.yfazqb.com/Article/details/gxklvyiyy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gbxydijtm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.yfazqb.com/Article/details/gdqofommy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.tarul.cn/Article/details/gyxymskdr.sHtML

[B15] 布尔运算与取反
来源：http://m.share.epnwcf.com/Article/details/gzwdjqbfm.sHtML

Py:   a and b or not c
来源：http://m.share.bbcook.cn/Article/details/gpdyhojor.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.yfazqb.com/Article/details/gfjqrdxrh.sHtML

JS:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/gjgyqcuht.sHtML

TS:   a && b || !c
来源：http://mobile.epnwcf.com/Article/details/guichiljy.sHtML

Java: a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gvmffxrem.sHtML

Go:   a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gzyxfhlqy.sHtML

Ruby: a && b || !c
来源：http://blog.bbcook.cn/Article/details/gnjniktnv.sHtML

C#:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gwkdfoyux.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.epnwcf.com/Article/details/giialnaqm.sHtML

Py:   if not data: return
来源：http://3g.fktsv.cn/Article/details/guqvqonge.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.tarul.cn/Article/details/gdfpuarve.sHtML

JS:   if (!data) return;
来源：http://baike.sjlbkw.cn/Article/details/gjqlrifsi.sHtML

TS:   if (!data) return;
来源：http://www.m.share.yfazqb.com/Article/details/gkjhdmvru.sHtML

Java: if (data == null) return;
来源：http://read.share.vehdjk.com/Article/details/glxbyqieg.sHtML

Go:   if data == nil { return }
来源：http://wap.tarul.cn/Article/details/ghnqltrzo.sHtML

Ruby: return if data.nil?
来源：http://www.blog.vehdjk.com/Article/details/ghifkibju.sHtML

C#:   if (data == null) return;
来源：http://3g.vehdjk.com/Article/details/gtkknxlpl.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gegsqcbxa.sHtML

C. 函数与作用域
来源：http://baike.sjlbkw.cn/Article/details/gwcpgrxrf.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gbgeuueax.sHtML

[C01] 定义函数
来源：http://www.m.share.sjlbkw.cn/Article/details/ggadopgyh.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.tarul.cn/Article/details/gdsuewnsm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gxqktqpeu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gjjlcukjq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gnhydxlov.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.vehdjk.com/Article/details/gxwbwsxcn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.sjlbkw.cn/Article/details/gvjckdugm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.bbcook.cn/Article/details/gbbjpxgqa.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gzrbcxzvz.sHtML

[C02] 默认参数
来源：http://www.m.share.fktsv.cn/Article/details/gcurjkpad.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.bbcook.cn/Article/details/gzzgxiudl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.tarul.cn/Article/details/gzywwedet.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gybclhbfh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/githuhdnh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.tarul.cn/Article/details/gtbbibfhm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.vehdjk.com/Article/details/glrptjzva.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.epnwcf.com/Article/details/gfganozty.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.vehdjk.com/Article/details/gmzdshfrx.sHtML

[C03] 可变参数
来源：http://www.blog.sjlbkw.cn/Article/details/gfatzhivm.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.tarul.cn/Article/details/gnesuqtxq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.yfazqb.com/Article/details/gfttdtzit.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.tarul.cn/Article/details/gggwtiowy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fktsv.cn/Article/details/gzpdzdaks.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.epnwcf.com/Article/details/goxxgmphl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.bbcook.cn/Article/details/gungtuyfi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.vehdjk.com/Article/details/gevgvmmwg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.bbcook.cn/Article/details/gisdurdvz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.vehdjk.com/Article/details/gzlzpltay.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.sjlbkw.cn/Article/details/gbwooebnu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.epnwcf.com/Article/details/gxjnohflk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.bbcook.cn/Article/details/gznwzzhpl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.epnwcf.com/Article/details/gtazmdrct.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.sjlbkw.cn/Article/details/ginlpnwkh.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.tarul.cn/Article/details/gatizjrrl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.epnwcf.com/Article/details/gaverxkdw.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.tarul.cn/Article/details/gozcqixpd.sHtML

[C05] 返回多个值
来源：http://baike.bbcook.cn/Article/details/gigidgktv.sHtML

Py:   return a, b
来源：http://mobile.yfazqb.com/Article/details/gccjaynwd.sHtML

PHP:  return [$a, $b];
来源：http://baike.sjlbkw.cn/Article/details/gqbrriaub.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.tarul.cn/Article/details/gqpqkzxlv.sHtML

TS:   return { a, b };
来源：http://read.share.yfazqb.com/Article/details/gnaplftmq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.tarul.cn/Article/details/gfxlkkzfp.sHtML

Go:   return a, b
来源：http://read.share.bbcook.cn/Article/details/gcldhrvaf.sHtML

Ruby: return a, b
来源：http://baike.tarul.cn/Article/details/gekcsqkow.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.sjlbkw.cn/Article/details/gdzabjyei.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.sjlbkw.cn/Article/details/guqkmibbs.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.vehdjk.com/Article/details/gmdkykywk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.epnwcf.com/Article/details/gbeclwtar.sHtML

JS:   const square = x => x * x;
来源：http://read.share.vehdjk.com/Article/details/gcjfezkro.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.yfazqb.com/Article/details/grpsuljkd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.sjlbkw.cn/Article/details/giscjbsxx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.epnwcf.com/Article/details/gmmatdjuo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.yfazqb.com/Article/details/gqufagxto.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.sjlbkw.cn/Article/details/gzsupwzvz.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.sjlbkw.cn/Article/details/gexthzubg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.yfazqb.com/Article/details/gfcnddvjq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fktsv.cn/Article/details/gzybhirjf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.vehdjk.com/Article/details/giomozinx.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fktsv.cn/Article/details/gtxxvabed.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.epnwcf.com/Article/details/gkrtdagvu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.epnwcf.com/Article/details/ghezhwkfn.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.sjlbkw.cn/Article/details/gyfyikhgk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.bbcook.cn/Article/details/gwxstkaln.sHtML

[C08] 闭包
来源：http://baike.fktsv.cn/Article/details/ginenbypt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.epnwcf.com/Article/details/gnxmvroyo.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.epnwcf.com/Article/details/gvqmhkhta.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.yfazqb.com/Article/details/gihegivge.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.tarul.cn/Article/details/gkfzjasrz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.tarul.cn/Article/details/gkwveqkqs.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.yfazqb.com/Article/details/gvadqmscr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.sjlbkw.cn/Article/details/goigupzxe.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.yfazqb.com/Article/details/gvvckuvdb.sHtML

[C09] 递归
来源：http://3g.tarul.cn/Article/details/gcfzxigvn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.tarul.cn/Article/details/gcyoiygwx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.epnwcf.com/Article/details/gmaokhckq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.yfazqb.com/Article/details/gvfyxcqhb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.sjlbkw.cn/Article/details/gsstbgcdy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.sjlbkw.cn/Article/details/gaqgsrofn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.sjlbkw.cn/Article/details/gmownhnug.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.vehdjk.com/Article/details/gqtfzwizl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.yfazqb.com/Article/details/gqwbwvpgj.sHtML

[C10] 变量作用域
来源：http://blog.tarul.cn/Article/details/gzpsrkjit.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.bbcook.cn/Article/details/godiqdtpp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.vehdjk.com/Article/details/gbhuodxvh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.bbcook.cn/Article/details/gxhecvtbt.sHtML

TS:   同 JS
来源：http://www.m.share.fktsv.cn/Article/details/ghdjyvnrh.sHtML

Java: 方法内为块级作用域
来源：http://m.share.vehdjk.com/Article/details/gcjrrzaad.sHtML

Go:   花括号块级作用域
来源：http://read.share.bbcook.cn/Article/details/gibzirgrt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.yfazqb.com/Article/details/gpecdqopm.sHtML

C#:   块级作用域
来源：http://3g.yfazqb.com/Article/details/gtzfvsvsl.sHtML

[C11] 模块导入与导出
来源：http://m.share.sjlbkw.cn/Article/details/gjrkozzvb.sHtML

Py:   from module import func
来源：http://m.share.tarul.cn/Article/details/gjmdfabma.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.tarul.cn/Article/details/gjwchpqzn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.yfazqb.com/Article/details/gigcmprgo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.vehdjk.com/Article/details/gzpzctllw.sHtML

Java: import java.util.List;
来源：http://baike.vehdjk.com/Article/details/gxqlpnbhh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.bbcook.cn/Article/details/gboclsxij.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.epnwcf.com/Article/details/gudniuidc.sHtML

C#:   using System.Text;
来源：http://baike.bbcook.cn/Article/details/gznxfiiwt.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.sjlbkw.cn/Article/details/gjieawrmn.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.vehdjk.com/Article/details/gxpctnsrz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.yfazqb.com/Article/details/gushnifow.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.yfazqb.com/Article/details/gmzorfthi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.tarul.cn/Article/details/ggmtvwzym.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.tarul.cn/Article/details/gcwtcmmou.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.epnwcf.com/Article/details/gbzxdfmkz.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.epnwcf.com/Article/details/gcyvudqvr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.sjlbkw.cn/Article/details/gmlavrqfs.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.yfazqb.com/Article/details/gkuukspgl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.epnwcf.com/Article/details/ggbwptjaa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/gtpocxfbl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.vehdjk.com/Article/details/gtgyucwwk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gkmeyhtnp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gmybbnvmh.sHtML

Go:   func add(a, b int) int
来源：http://wap.tarul.cn/Article/details/gaewlezvs.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.tarul.cn/Article/details/gjoifmgum.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.tarul.cn/Article/details/gmexjxsif.sHtML

[C14] 泛型函数
来源：http://baike.sjlbkw.cn/Article/details/gnjylwdnb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fktsv.cn/Article/details/gllxbkkaz.sHtML

PHP:  // 无泛型
来源：http://mobile.yfazqb.com/Article/details/gonpgkefs.sHtML

JS:   // 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/gsslbwtvu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.yfazqb.com/Article/details/gmanbukuf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.bbcook.cn/Article/details/gdqctglvi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.sjlbkw.cn/Article/details/golihfpew.sHtML

Ruby: # 无泛型
来源：http://mobile.fktsv.cn/Article/details/gynlobpbx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.yfazqb.com/Article/details/ghinombjo.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.epnwcf.com/Article/details/gsdnzyrzq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fktsv.cn/Article/details/giilfblrf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.sjlbkw.cn/Article/details/gebgvfbll.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.tarul.cn/Article/details/gczutalih.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.sjlbkw.cn/Article/details/gkggbgjwb.sHtML

Java: // 无解构
来源：http://www.m.share.fktsv.cn/Article/details/gzvrtuvzy.sHtML

Go:   // 无解构
来源：http://blog.sjlbkw.cn/Article/details/gmhxiuddx.sHtML

Ruby: a, b = pair
来源：http://read.share.epnwcf.com/Article/details/gxcanwyjb.sHtML

C#:   var (a, b) = pair;
来源：http://3g.sjlbkw.cn/Article/details/gfabrfjez.sHtML

[C16] 函数 / 方法重载
来源：http://3g.sjlbkw.cn/Article/details/ganjgtpbt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.sjlbkw.cn/Article/details/gogwcseta.sHtML

PHP:  // 无重载
来源：http://www.share.epnwcf.com/Article/details/gargrbmcc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fktsv.cn/Article/details/ghtrjuwns.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.tarul.cn/Article/details/gjlljnntg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.sjlbkw.cn/Article/details/gngyheanx.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.bbcook.cn/Article/details/gglhtkmym.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.vehdjk.com/Article/details/grkktwxra.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.epnwcf.com/Article/details/gngilfcvd.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gowlfxxis.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.epnwcf.com/Article/details/gpmrcrnsj.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gttlobacd.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.sjlbkw.cn/Article/details/gnifzzuon.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fktsv.cn/Article/details/gbbnhsnfq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.tarul.cn/Article/details/gimdwcfso.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fktsv.cn/Article/details/gjrfpycbz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.epnwcf.com/Article/details/grusanfie.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fktsv.cn/Article/details/ghmapkzgc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fktsv.cn/Article/details/giqaojwtn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fktsv.cn/Article/details/gjhxrqajq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.yfazqb.com/Article/details/grsmenqxx.sHtML

[D02] 追加元素到末尾
来源：http://read.share.vehdjk.com/Article/details/grlrhyjdf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.tarul.cn/Article/details/goiigvnrd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fktsv.cn/Article/details/gryuuzwju.sHtML

JS:   arr.push(4);
来源：http://www.m.share.vehdjk.com/Article/details/gnrovrnqt.sHtML

TS:   arr.push(4);
来源：http://m.share.vehdjk.com/Article/details/grfcxappm.sHtML

Java: list.add(4);
来源：http://www.m.share.epnwcf.com/Article/details/gmaohwunz.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.bbcook.cn/Article/details/gnzppsdtx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.tarul.cn/Article/details/goaheaztp.sHtML

C#:   list.Add(4);
来源：http://www.share.bbcook.cn/Article/details/gwbtfdauy.sHtML


<!-- 参考信息 -->