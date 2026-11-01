代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://m.share.epnwcf.com/Article/details/glepxthpv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.bbcook.cn/Article/details/gwmhlrypv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.epnwcf.com/Article/details/gwaokuhxw.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.yfazqb.com/Article/details/gxqmaazuo.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.epnwcf.com/Article/details/gwfnqxdru.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gxhtsknkj.sHtML

B. 流程控制
来源：http://www.share.vehdjk.com/Article/details/gdmawhwem.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gjwtkbntt.sHtML

[B01] 条件判断 if / else
来源：http://read.share.epnwcf.com/Article/details/geqmcnjfj.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.sjlbkw.cn/Article/details/gemddckag.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.yfazqb.com/Article/details/gfiueqwlg.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.yfazqb.com/Article/details/gdyyebuef.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.tarul.cn/Article/details/giuyghefa.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.yfazqb.com/Article/details/gqziwbygt.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.sjlbkw.cn/Article/details/gbaeguhbu.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.sjlbkw.cn/Article/details/gydqqeusu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.vehdjk.com/Article/details/gwwdzjkbl.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.vehdjk.com/Article/details/grvlsxtps.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.epnwcf.com/Article/details/gdaggjncy.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.bbcook.cn/Article/details/gvjgxjgav.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.epnwcf.com/Article/details/gdzccndxj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.vehdjk.com/Article/details/ghjngixvu.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.epnwcf.com/Article/details/gpmogwcjn.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.yfazqb.com/Article/details/gwtfzgwao.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.sjlbkw.cn/Article/details/gkpelewsh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.sjlbkw.cn/Article/details/gbabujpbz.sHtML

[B03] switch / match / case
来源：http://www.m.share.vehdjk.com/Article/details/gahpnlpnz.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.tarul.cn/Article/details/gqziqvdcp.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.yfazqb.com/Article/details/gawivbhju.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.bbcook.cn/Article/details/gffzigrkx.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.tarul.cn/Article/details/glgslazri.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.vehdjk.com/Article/details/gonuasxon.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.sjlbkw.cn/Article/details/grrpzaqqk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.tarul.cn/Article/details/gzkgkymbf.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.vehdjk.com/Article/details/gwoynpxsh.sHtML

[B04] for 计数循环
来源：http://www.blog.bbcook.cn/Article/details/gdereyhuk.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.fktsv.cn/Article/details/gqnptujvz.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.fktsv.cn/Article/details/gzxfdqlxb.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.epnwcf.com/Article/details/gqqdosnwn.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.epnwcf.com/Article/details/gzpwlbsxf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.sjlbkw.cn/Article/details/gqsrhvdxl.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.yfazqb.com/Article/details/gjchmmkda.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.sjlbkw.cn/Article/details/ghatgecji.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.sjlbkw.cn/Article/details/gxrpgituf.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.tarul.cn/Article/details/ghdmxckzf.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.vehdjk.com/Article/details/glhjxqyku.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.yfazqb.com/Article/details/gkeegdlca.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.tarul.cn/Article/details/gacvyljeb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fktsv.cn/Article/details/gvjjdjraw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.fktsv.cn/Article/details/ghrqfabnn.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.bbcook.cn/Article/details/ggcmwgcpq.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.epnwcf.com/Article/details/gtwubncwz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.sjlbkw.cn/Article/details/gdsvwwhxh.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.sjlbkw.cn/Article/details/gnxxonbng.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.bbcook.cn/Article/details/ghmmycpwz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.fktsv.cn/Article/details/guubeleps.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.vehdjk.com/Article/details/gblxwmekw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.bbcook.cn/Article/details/gmmjbhmro.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.yfazqb.com/Article/details/gjqgsgrwx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.epnwcf.com/Article/details/gxvxcjblf.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.bbcook.cn/Article/details/gfiatzozr.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.vehdjk.com/Article/details/gywuqakvw.sHtML

[B07] while 循环
来源：http://wap.bbcook.cn/Article/details/gdgndmrmp.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.tarul.cn/Article/details/gpicbgfqu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.sjlbkw.cn/Article/details/gpmdqjahg.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/gftegmrco.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.bbcook.cn/Article/details/giykifned.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.vehdjk.com/Article/details/gpsvazchq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.epnwcf.com/Article/details/gfpuflgiu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.sjlbkw.cn/Article/details/gvrhlawig.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.sjlbkw.cn/Article/details/gnniuaqhi.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.bbcook.cn/Article/details/gfghfmnxn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.epnwcf.com/Article/details/giairgcwk.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.vehdjk.com/Article/details/gaordqkaj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gshdowagn.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/gkfiosrgc.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.yfazqb.com/Article/details/gwvyuwhow.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.yfazqb.com/Article/details/ghrtuhygk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.epnwcf.com/Article/details/gesnvmjlu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.vehdjk.com/Article/details/gzkgftjem.sHtML

[B09] break 与 continue
来源：http://www.m.share.yfazqb.com/Article/details/gaeabjdym.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.sjlbkw.cn/Article/details/gumisgwui.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gksfufsdg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/gtkcxkffb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gsoxiezvw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gkgsctieh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.bbcook.cn/Article/details/gtdqvzaka.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.tarul.cn/Article/details/ghncmmfll.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/gdbxxzdcw.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.yfazqb.com/Article/details/gajptotgk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.tarul.cn/Article/details/gxvcprtgc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.bbcook.cn/Article/details/gnpdwqedi.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.tarul.cn/Article/details/gvsyddhso.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.bbcook.cn/Article/details/gnykfbkpy.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.bbcook.cn/Article/details/grxkksnkf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gauuxrsxb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.epnwcf.com/Article/details/gyvveaybc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.sjlbkw.cn/Article/details/gjilctnmi.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fktsv.cn/Article/details/gormyvxek.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.epnwcf.com/Article/details/grhrlnjts.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.vehdjk.com/Article/details/gouqmsabs.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.sjlbkw.cn/Article/details/gqbzscwgq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.tarul.cn/Article/details/grqsujtxc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.yfazqb.com/Article/details/ggykdmqan.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.yfazqb.com/Article/details/gxyubxaso.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.bbcook.cn/Article/details/gtoavbenc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.tarul.cn/Article/details/gytktmxdp.sHtML

[B12] 跳出多层循环
来源：http://3g.tarul.cn/Article/details/guesflifj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.sjlbkw.cn/Article/details/gqsoiabjb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.epnwcf.com/Article/details/gptxlmbdh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.bbcook.cn/Article/details/gfnrupats.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fktsv.cn/Article/details/gubcghwwo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.tarul.cn/Article/details/gntdticei.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.sjlbkw.cn/Article/details/gvqbintnx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.sjlbkw.cn/Article/details/ggesxzqjk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.bbcook.cn/Article/details/gpyfilokw.sHtML

[B13] 判断是否为数字
来源：http://mobile.vehdjk.com/Article/details/grofbiufm.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.bbcook.cn/Article/details/gxidzedpp.sHtML

PHP:  is_numeric($x)
来源：http://www.share.yfazqb.com/Article/details/grbsekzgi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.vehdjk.com/Article/details/gihyowwjc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.vehdjk.com/Article/details/gnlgvycrd.sHtML

Java: x instanceof Number
来源：http://baike.vehdjk.com/Article/details/gfnvlujni.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.epnwcf.com/Article/details/govhlatet.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.bbcook.cn/Article/details/ggsquawdx.sHtML

C#:   x is int or double or decimal
来源：http://baike.epnwcf.com/Article/details/gywxjspku.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fktsv.cn/Article/details/gnziosasy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.tarul.cn/Article/details/ganyzqiql.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fktsv.cn/Article/details/gykmjvqwe.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.tarul.cn/Article/details/gbvxgxzck.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.vehdjk.com/Article/details/gxwqiuaou.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.epnwcf.com/Article/details/gurbbrkce.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.sjlbkw.cn/Article/details/gognzqsmo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.tarul.cn/Article/details/gyhqpsyap.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/gsnqmtkjy.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.sjlbkw.cn/Article/details/gcznaafgf.sHtML

Py:   a and b or not c
来源：http://www.share.fktsv.cn/Article/details/ghkhpduyl.sHtML

PHP:  $a && $b || !$c
来源：http://blog.vehdjk.com/Article/details/gmzmendzb.sHtML

JS:   a && b || !c
来源：http://baike.tarul.cn/Article/details/gagisvtpp.sHtML

TS:   a && b || !c
来源：http://www.share.epnwcf.com/Article/details/grccbeuyu.sHtML

Java: a && b || !c
来源：http://3g.bbcook.cn/Article/details/gagdqzcsf.sHtML

Go:   a && b || !c
来源：http://baike.bbcook.cn/Article/details/gacgxwijm.sHtML

Ruby: a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/ggiebtjby.sHtML

C#:   a && b || !c
来源：http://baike.fktsv.cn/Article/details/gybfolpze.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.tarul.cn/Article/details/gmbguhnlg.sHtML

Py:   if not data: return
来源：http://3g.fktsv.cn/Article/details/gatmtygqw.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.epnwcf.com/Article/details/givclctsd.sHtML

JS:   if (!data) return;
来源：http://baike.fktsv.cn/Article/details/gkbfvmdyj.sHtML

TS:   if (!data) return;
来源：http://www.blog.vehdjk.com/Article/details/gxfdfdlfd.sHtML

Java: if (data == null) return;
来源：http://www.m.share.bbcook.cn/Article/details/gyfkjhkxf.sHtML

Go:   if data == nil { return }
来源：http://baike.sjlbkw.cn/Article/details/gjmudtkuq.sHtML

Ruby: return if data.nil?
来源：http://baike.bbcook.cn/Article/details/gemwjpuef.sHtML

C#:   if (data == null) return;
来源：http://m.share.epnwcf.com/Article/details/grscvfbtj.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gduzxuudq.sHtML

C. 函数与作用域
来源：http://mobile.bbcook.cn/Article/details/gbkqxbpyk.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ggsixicxb.sHtML

[C01] 定义函数
来源：http://mobile.fktsv.cn/Article/details/gsnbkwxmt.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.tarul.cn/Article/details/gcqugpkxy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/gkuplhsss.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gyrvgqitu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gzdydfuno.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/goyglupmt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.yfazqb.com/Article/details/gtwnazfic.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.tarul.cn/Article/details/gmvgakzvy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gomwjfkgl.sHtML

[C02] 默认参数
来源：http://baike.epnwcf.com/Article/details/gvgeytygx.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.sjlbkw.cn/Article/details/gtnbxsgrv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.epnwcf.com/Article/details/gwlvapanp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/gmmxsjmls.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.epnwcf.com/Article/details/groxiulkl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.vehdjk.com/Article/details/gxvjzodoq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.epnwcf.com/Article/details/gaiceiokh.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fktsv.cn/Article/details/gwvfgnppy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.tarul.cn/Article/details/gzsltpouo.sHtML

[C03] 可变参数
来源：http://www.blog.epnwcf.com/Article/details/gtpqhxtnt.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.epnwcf.com/Article/details/glyrblkev.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.bbcook.cn/Article/details/gvauvtals.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.yfazqb.com/Article/details/gfkldplcj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.sjlbkw.cn/Article/details/gxqthpeop.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.yfazqb.com/Article/details/gmlemaihh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fktsv.cn/Article/details/gglmidhyy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.sjlbkw.cn/Article/details/gjovfpduh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.tarul.cn/Article/details/gcvuxndct.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.vehdjk.com/Article/details/gxguhggvn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.tarul.cn/Article/details/gacydoxxl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.sjlbkw.cn/Article/details/gtjzdnlco.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fktsv.cn/Article/details/gdfeamclf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fktsv.cn/Article/details/gyimxulqi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.tarul.cn/Article/details/gowfyzsyf.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fktsv.cn/Article/details/gxijjizef.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.tarul.cn/Article/details/giekafuex.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.bbcook.cn/Article/details/golevbpxq.sHtML

[C05] 返回多个值
来源：http://mobile.yfazqb.com/Article/details/gnsrjkrig.sHtML

Py:   return a, b
来源：http://mobile.bbcook.cn/Article/details/gsmmayjyi.sHtML

PHP:  return [$a, $b];
来源：http://3g.epnwcf.com/Article/details/ghpxucbmx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.vehdjk.com/Article/details/gmokixtng.sHtML

TS:   return { a, b };
来源：http://mobile.epnwcf.com/Article/details/ghsujlxdi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.yfazqb.com/Article/details/gehxhxxra.sHtML

Go:   return a, b
来源：http://blog.tarul.cn/Article/details/gjoveiind.sHtML

Ruby: return a, b
来源：http://www.m.share.tarul.cn/Article/details/givcgjfsw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.epnwcf.com/Article/details/gimnievep.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.tarul.cn/Article/details/ghrmayhhu.sHtML

Py:   square = lambda x: x * x
来源：http://wap.epnwcf.com/Article/details/gzqanuupe.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fktsv.cn/Article/details/gxexmzdjq.sHtML

JS:   const square = x => x * x;
来源：http://www.share.bbcook.cn/Article/details/gskcoomko.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/gumgqeunf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fktsv.cn/Article/details/gscyuzezo.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.yfazqb.com/Article/details/goztiljkt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.epnwcf.com/Article/details/gzybalubd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.vehdjk.com/Article/details/gmjcjdfqc.sHtML

[C07] 把函数作为参数传入
来源：http://3g.bbcook.cn/Article/details/gjzsvjctt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fktsv.cn/Article/details/gbthtafjl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.tarul.cn/Article/details/gjknlxnqe.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fktsv.cn/Article/details/gepkhoonj.sHtML

TS:   arr.map(String)
来源：http://wap.fktsv.cn/Article/details/gjnzugfiy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.vehdjk.com/Article/details/gmmiknmfy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.epnwcf.com/Article/details/gcuxsyxzw.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.epnwcf.com/Article/details/gfcfdpcew.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.sjlbkw.cn/Article/details/gsjburrpt.sHtML

[C08] 闭包
来源：http://baike.tarul.cn/Article/details/gxyrzhnvp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.tarul.cn/Article/details/gdkuxmxtk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fktsv.cn/Article/details/gvgzsptzv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.sjlbkw.cn/Article/details/gxhzbuxsh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fktsv.cn/Article/details/gydoymcjy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.sjlbkw.cn/Article/details/gyrzbodln.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.bbcook.cn/Article/details/gbfebfsqx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.sjlbkw.cn/Article/details/gbdglpktd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.bbcook.cn/Article/details/gyikyolge.sHtML

[C09] 递归
来源：http://mobile.yfazqb.com/Article/details/gqeaafmet.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.vehdjk.com/Article/details/geivtlmrb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.sjlbkw.cn/Article/details/gkjypeyqe.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.epnwcf.com/Article/details/ggwzfihqw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.bbcook.cn/Article/details/goqqknauw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.bbcook.cn/Article/details/gxuxdxyqa.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.yfazqb.com/Article/details/glpvydmox.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.sjlbkw.cn/Article/details/gkkanylsb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.tarul.cn/Article/details/gqsshwnjm.sHtML

[C10] 变量作用域
来源：http://m.share.yfazqb.com/Article/details/gckldvfdt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.vehdjk.com/Article/details/gqufuyxvd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fktsv.cn/Article/details/gbujinmwb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.sjlbkw.cn/Article/details/gusirbuqh.sHtML

TS:   同 JS
来源：http://3g.bbcook.cn/Article/details/grlirfzvt.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.yfazqb.com/Article/details/gcebhxnqp.sHtML

Go:   花括号块级作用域
来源：http://m.share.bbcook.cn/Article/details/gzavafqls.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.sjlbkw.cn/Article/details/godmwelmp.sHtML

C#:   块级作用域
来源：http://www.share.tarul.cn/Article/details/gettcovdv.sHtML

[C11] 模块导入与导出
来源：http://wap.bbcook.cn/Article/details/gcodzvnpg.sHtML

Py:   from module import func
来源：http://wap.epnwcf.com/Article/details/gzbwgaddk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.vehdjk.com/Article/details/giseumtgb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.vehdjk.com/Article/details/gxmlwgqbo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fktsv.cn/Article/details/gbubhewdj.sHtML

Java: import java.util.List;
来源：http://www.blog.bbcook.cn/Article/details/glqjsnukh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fktsv.cn/Article/details/gpxrgepdo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.epnwcf.com/Article/details/gvnjotudb.sHtML

C#:   using System.Text;
来源：http://blog.bbcook.cn/Article/details/gxriqfzgo.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.bbcook.cn/Article/details/ghfdlopir.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.sjlbkw.cn/Article/details/gbighfpjx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.yfazqb.com/Article/details/gsiyuwxzv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fktsv.cn/Article/details/ggirahefx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.tarul.cn/Article/details/ggzrkbnhw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.bbcook.cn/Article/details/ghlcdyifc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.epnwcf.com/Article/details/gquyisvlk.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.epnwcf.com/Article/details/gjmwuqsju.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.yfazqb.com/Article/details/ghuibnagi.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.bbcook.cn/Article/details/ggumefulw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.bbcook.cn/Article/details/gehfqvsfr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gwtakgvbz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.yfazqb.com/Article/details/gttwbvrfm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gxbygwqxh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gfrpfheci.sHtML

Go:   func add(a, b int) int
来源：http://www.share.epnwcf.com/Article/details/gwbbecdvh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.vehdjk.com/Article/details/gnuoginmn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.yfazqb.com/Article/details/gzmsjrrhr.sHtML

[C14] 泛型函数
来源：http://blog.sjlbkw.cn/Article/details/guvetqads.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.vehdjk.com/Article/details/giofihmhu.sHtML

PHP:  // 无泛型
来源：http://www.m.share.vehdjk.com/Article/details/gljvoozix.sHtML

JS:   // 无泛型
来源：http://baike.bbcook.cn/Article/details/gxbcdlokl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.yfazqb.com/Article/details/grbmkcxil.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.yfazqb.com/Article/details/gqpzdnqpv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.sjlbkw.cn/Article/details/gfeprihoz.sHtML

Ruby: # 无泛型
来源：http://mobile.tarul.cn/Article/details/gzvbyzlpa.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.sjlbkw.cn/Article/details/gygmtalel.sHtML

[C15] 解构 / 展开参数
来源：http://wap.tarul.cn/Article/details/gcixkilum.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fktsv.cn/Article/details/gbmygbsgg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.vehdjk.com/Article/details/gdfjkmyzz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.epnwcf.com/Article/details/gxjcgenjo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fktsv.cn/Article/details/gvzjvzgob.sHtML

Java: // 无解构
来源：http://blog.vehdjk.com/Article/details/gcplqposf.sHtML

Go:   // 无解构
来源：http://blog.bbcook.cn/Article/details/gsqnuafmc.sHtML

Ruby: a, b = pair
来源：http://www.m.share.bbcook.cn/Article/details/ggfhuumve.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.epnwcf.com/Article/details/gvnnqrfvh.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.yfazqb.com/Article/details/gtxpdrabe.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.tarul.cn/Article/details/gxomcfmuo.sHtML

PHP:  // 无重载
来源：http://www.blog.bbcook.cn/Article/details/gsvnlxcku.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.epnwcf.com/Article/details/gvwtlqugw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fktsv.cn/Article/details/gniyhrdac.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fktsv.cn/Article/details/gvianbwiq.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fktsv.cn/Article/details/gytjanxmj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.epnwcf.com/Article/details/gvejxyomk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fktsv.cn/Article/details/gaebtjkrw.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gwmkvqpkv.sHtML


<!-- 参考信息 -->