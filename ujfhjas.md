代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://wap.fktsv.cn/Article/details/gpnnmhuht.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.epnwcf.com/Article/details/gzqtmbkwr.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.sjlbkw.cn/Article/details/gexswonhe.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.yfazqb.com/Article/details/gnoigshnj.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.vehdjk.com/Article/details/gpzpghlxm.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.sjlbkw.cn/Article/details/gegvrneyt.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.epnwcf.com/Article/details/gfnziawwf.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.yfazqb.com/Article/details/gtnsspihv.sHtML

[A26] 类型转换总览
来源：http://www.m.share.bbcook.cn/Article/details/gukxdlgmo.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.fktsv.cn/Article/details/ghliekjdj.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.vehdjk.com/Article/details/guswdrkpy.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.yfazqb.com/Article/details/gjesinmba.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.yfazqb.com/Article/details/gqbzywqty.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.tarul.cn/Article/details/gjcvxbyyv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.vehdjk.com/Article/details/gbtxqrgqf.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.sjlbkw.cn/Article/details/gnfgrumqw.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.tarul.cn/Article/details/gutelpjet.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gsgbnfxqh.sHtML

B. 流程控制
来源：http://m.share.fktsv.cn/Article/details/ghoeghqhi.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/grziacmod.sHtML

[B01] 条件判断 if / else
来源：http://wap.yfazqb.com/Article/details/gaoahzwzo.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.vehdjk.com/Article/details/gaekdrvnz.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.vehdjk.com/Article/details/gnvhvxgio.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.tarul.cn/Article/details/gdwogbiai.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.epnwcf.com/Article/details/gwvmhgmrg.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.fktsv.cn/Article/details/gglobikxj.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.bbcook.cn/Article/details/gmeljeahu.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.epnwcf.com/Article/details/grrwabtlj.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/gaijtdylu.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.yfazqb.com/Article/details/gipseyupj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.yfazqb.com/Article/details/gjvhvgqrk.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.sjlbkw.cn/Article/details/gukccrfja.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.bbcook.cn/Article/details/gtetxgpya.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.tarul.cn/Article/details/gichihlcc.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.epnwcf.com/Article/details/gipymupsh.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.tarul.cn/Article/details/gqmdktuif.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fktsv.cn/Article/details/gdfsbdtht.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fktsv.cn/Article/details/gkpozthen.sHtML

[B03] switch / match / case
来源：http://baike.epnwcf.com/Article/details/gjxvfrukk.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.bbcook.cn/Article/details/gzoeovmry.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/gswsjnatf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.bbcook.cn/Article/details/gwcuspdgt.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.sjlbkw.cn/Article/details/gmjdoaqqc.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.tarul.cn/Article/details/gclmiubxe.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.vehdjk.com/Article/details/ghterekhd.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.vehdjk.com/Article/details/gplifvdaf.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.sjlbkw.cn/Article/details/gulaeaaqp.sHtML

[B04] for 计数循环
来源：http://wap.tarul.cn/Article/details/gqghzyzul.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.yfazqb.com/Article/details/gxrmukgdu.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.sjlbkw.cn/Article/details/grkqcuulf.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.vehdjk.com/Article/details/gswdsgfdd.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.yfazqb.com/Article/details/gsbmdbtbr.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.tarul.cn/Article/details/ggwkcuwth.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.sjlbkw.cn/Article/details/gjqrrqtfu.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.fktsv.cn/Article/details/ggortjwtc.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.yfazqb.com/Article/details/gutofjscu.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.tarul.cn/Article/details/gmjtujlvn.sHtML

Py:   for item in arr: print(item)
来源：http://baike.tarul.cn/Article/details/ghodwgrqo.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.vehdjk.com/Article/details/godyvyhmg.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.sjlbkw.cn/Article/details/gcbiwpsfj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.vehdjk.com/Article/details/gtjbijlvy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.yfazqb.com/Article/details/gecydwnjg.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.sjlbkw.cn/Article/details/gepjaywwk.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.fktsv.cn/Article/details/gwxbqohpd.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.yfazqb.com/Article/details/gefajtqjv.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.bbcook.cn/Article/details/gfitdpped.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.yfazqb.com/Article/details/gmkmbpnnj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.epnwcf.com/Article/details/girrzhhub.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.yfazqb.com/Article/details/gxtjyclcb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.vehdjk.com/Article/details/gpbfuqkuz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.sjlbkw.cn/Article/details/gnbgkxykg.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.epnwcf.com/Article/details/ggxjdmdgr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.epnwcf.com/Article/details/gptiqxrfi.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.bbcook.cn/Article/details/gmnlounce.sHtML

[B07] while 循环
来源：http://baike.yfazqb.com/Article/details/gigovgedw.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.vehdjk.com/Article/details/gjxckglfo.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.epnwcf.com/Article/details/ggxfktdzf.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gncgnsuai.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.bbcook.cn/Article/details/gedxazgai.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.epnwcf.com/Article/details/gudodyrst.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.sjlbkw.cn/Article/details/gbpjlbejw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.sjlbkw.cn/Article/details/ghzbnsmwm.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.tarul.cn/Article/details/gwnetktzm.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.tarul.cn/Article/details/gknhwjlid.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.vehdjk.com/Article/details/gbuterktw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.yfazqb.com/Article/details/gvamatzqc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.epnwcf.com/Article/details/gtqpdfzmg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gdwjxlmoj.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gvgghhuyz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.epnwcf.com/Article/details/gqiajuepr.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.bbcook.cn/Article/details/gbsteekvf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.bbcook.cn/Article/details/grfltllnn.sHtML

[B09] break 与 continue
来源：http://baike.yfazqb.com/Article/details/gukskruqy.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.sjlbkw.cn/Article/details/glxoqkyvb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gjbowpjpt.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gdkcbuwgf.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.yfazqb.com/Article/details/gltyejhcv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gordzwkzy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.epnwcf.com/Article/details/gwjxnarll.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.epnwcf.com/Article/details/gbduorgos.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/gykoaxckw.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.tarul.cn/Article/details/ghtueuzbt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.epnwcf.com/Article/details/gfluumdeh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.sjlbkw.cn/Article/details/glrwdasyp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fktsv.cn/Article/details/gbfflgnjx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fktsv.cn/Article/details/gbcpwypir.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.yfazqb.com/Article/details/gmghmldai.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.vehdjk.com/Article/details/ghzrxoqkf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.vehdjk.com/Article/details/gdclypxzu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.vehdjk.com/Article/details/gddjtbqra.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.sjlbkw.cn/Article/details/gvqftlfwd.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.fktsv.cn/Article/details/gzpcwnukl.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fktsv.cn/Article/details/gaambzktz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fktsv.cn/Article/details/gwcmgagwp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.bbcook.cn/Article/details/gkcjurwkg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.vehdjk.com/Article/details/gncpjwykn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.sjlbkw.cn/Article/details/glfbudvqk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fktsv.cn/Article/details/gfvficave.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.sjlbkw.cn/Article/details/goqjwgfev.sHtML

[B12] 跳出多层循环
来源：http://www.blog.vehdjk.com/Article/details/gszsjkihb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.yfazqb.com/Article/details/gvtfebvej.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.yfazqb.com/Article/details/gbqqmdazi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.bbcook.cn/Article/details/gkuhnbija.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/gdonzmebt.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fktsv.cn/Article/details/grfyzjpjz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.yfazqb.com/Article/details/ggjkjldvz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.epnwcf.com/Article/details/galjxaibk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.sjlbkw.cn/Article/details/gasdktxvt.sHtML

[B13] 判断是否为数字
来源：http://www.share.tarul.cn/Article/details/gfvvyyega.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.tarul.cn/Article/details/grgoajout.sHtML

PHP:  is_numeric($x)
来源：http://m.share.tarul.cn/Article/details/gtrmbnffb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fktsv.cn/Article/details/gjbgcpmnd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.epnwcf.com/Article/details/gxaimjaym.sHtML

Java: x instanceof Number
来源：http://mobile.epnwcf.com/Article/details/gtjadljal.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.vehdjk.com/Article/details/gzvqfmuar.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.bbcook.cn/Article/details/ghyxhxksz.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.epnwcf.com/Article/details/glqgfwnwb.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fktsv.cn/Article/details/gnjhsahqz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.bbcook.cn/Article/details/gldslwqxk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.epnwcf.com/Article/details/gfilrntbn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.yfazqb.com/Article/details/glppctmhr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/gvtjxuacm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fktsv.cn/Article/details/gpalagkcr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.sjlbkw.cn/Article/details/gwwkigcap.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.vehdjk.com/Article/details/gfykvvlto.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.sjlbkw.cn/Article/details/gfivgmssn.sHtML

[B15] 布尔运算与取反
来源：http://baike.yfazqb.com/Article/details/gtqjpdqrw.sHtML

Py:   a and b or not c
来源：http://www.m.share.bbcook.cn/Article/details/gsfrzdljg.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.epnwcf.com/Article/details/gkqimvfms.sHtML

JS:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gpbtihtlv.sHtML

TS:   a && b || !c
来源：http://3g.fktsv.cn/Article/details/gwemwcwzv.sHtML

Java: a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gyhayrxoy.sHtML

Go:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gcxxdwofd.sHtML

Ruby: a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gqfdxxjhh.sHtML

C#:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/ggetfbddj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.epnwcf.com/Article/details/gklppsdcp.sHtML

Py:   if not data: return
来源：http://blog.vehdjk.com/Article/details/gkrxikdnr.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.vehdjk.com/Article/details/gsakqhsuh.sHtML

JS:   if (!data) return;
来源：http://m.share.sjlbkw.cn/Article/details/giabttrbm.sHtML

TS:   if (!data) return;
来源：http://mobile.vehdjk.com/Article/details/gocajfyln.sHtML

Java: if (data == null) return;
来源：http://mobile.bbcook.cn/Article/details/gzgmwvqtd.sHtML

Go:   if data == nil { return }
来源：http://m.share.fktsv.cn/Article/details/ggxmauhkd.sHtML

Ruby: return if data.nil?
来源：http://www.blog.yfazqb.com/Article/details/gylhecgpg.sHtML

C#:   if (data == null) return;
来源：http://wap.fktsv.cn/Article/details/gnypkonaa.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gmboasooe.sHtML

C. 函数与作用域
来源：http://mobile.sjlbkw.cn/Article/details/gpukbilik.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gugelqein.sHtML

[C01] 定义函数
来源：http://3g.yfazqb.com/Article/details/gvabinodm.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fktsv.cn/Article/details/gmijobtdp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/gvwvtwwsg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gvlrzbdfj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gqmodenab.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.tarul.cn/Article/details/gsyaatlnr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.yfazqb.com/Article/details/gotdclpze.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.vehdjk.com/Article/details/gcojhlvnl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gwotdlyhx.sHtML

[C02] 默认参数
来源：http://baike.epnwcf.com/Article/details/gexivfhcu.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.epnwcf.com/Article/details/gswajxinv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.sjlbkw.cn/Article/details/gmdfzdwkj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.epnwcf.com/Article/details/gknexxrzi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gahzxmxah.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.epnwcf.com/Article/details/gbbxkfymf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.tarul.cn/Article/details/gceeosajl.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.vehdjk.com/Article/details/glqvxfscs.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.epnwcf.com/Article/details/gsructssv.sHtML

[C03] 可变参数
来源：http://mobile.fktsv.cn/Article/details/guehebfyg.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.bbcook.cn/Article/details/geqxnuzvd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqivvxymn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.vehdjk.com/Article/details/gxvsmtwzt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.tarul.cn/Article/details/gnxglgtxb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.epnwcf.com/Article/details/gvcpqdpwe.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.bbcook.cn/Article/details/gldztpzxa.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.yfazqb.com/Article/details/gvycgjnmf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fktsv.cn/Article/details/gzsiymwuu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.vehdjk.com/Article/details/gcqafkgmv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fktsv.cn/Article/details/gjzwvxwnp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fktsv.cn/Article/details/gevuoohez.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.sjlbkw.cn/Article/details/gutbenpqr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.yfazqb.com/Article/details/gbqrvczyo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fktsv.cn/Article/details/goyqebngh.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.vehdjk.com/Article/details/gxczdylov.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.yfazqb.com/Article/details/gfdshxaaw.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.epnwcf.com/Article/details/gwtzvfpco.sHtML

[C05] 返回多个值
来源：http://www.blog.bbcook.cn/Article/details/ghqmqqoyo.sHtML

Py:   return a, b
来源：http://baike.bbcook.cn/Article/details/gxjyjxhto.sHtML

PHP:  return [$a, $b];
来源：http://blog.yfazqb.com/Article/details/gytsfcgus.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.vehdjk.com/Article/details/glnbouhjc.sHtML

TS:   return { a, b };
来源：http://blog.vehdjk.com/Article/details/glntzqips.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.tarul.cn/Article/details/guuogyzua.sHtML

Go:   return a, b
来源：http://wap.tarul.cn/Article/details/gegnhmyuk.sHtML

Ruby: return a, b
来源：http://3g.epnwcf.com/Article/details/gnrmedooh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.vehdjk.com/Article/details/gpbktbfmr.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.epnwcf.com/Article/details/ghhypgjwh.sHtML

Py:   square = lambda x: x * x
来源：http://3g.tarul.cn/Article/details/gfrffnpyg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fktsv.cn/Article/details/gqenfhfyg.sHtML

JS:   const square = x => x * x;
来源：http://m.share.vehdjk.com/Article/details/ghbtmnjdl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.tarul.cn/Article/details/gcwwfmadq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.vehdjk.com/Article/details/gcbeswtrf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.sjlbkw.cn/Article/details/gwxawpadv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.sjlbkw.cn/Article/details/gmlsrwjqa.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.vehdjk.com/Article/details/gosmvelau.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.epnwcf.com/Article/details/gufuevhmm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.sjlbkw.cn/Article/details/gclldkdja.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.tarul.cn/Article/details/gmclrcgmk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.vehdjk.com/Article/details/gkrejdgfx.sHtML

TS:   arr.map(String)
来源：http://m.share.bbcook.cn/Article/details/goazbpkos.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.yfazqb.com/Article/details/gpbrhridl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.epnwcf.com/Article/details/gtnaddwpq.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.sjlbkw.cn/Article/details/gfzpyvbba.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.tarul.cn/Article/details/gymygpvod.sHtML

[C08] 闭包
来源：http://www.share.epnwcf.com/Article/details/grmrkzpnm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fktsv.cn/Article/details/gcudkchlt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.epnwcf.com/Article/details/gglzgyilk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.sjlbkw.cn/Article/details/gexwtnfvc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.bbcook.cn/Article/details/gefdysxpt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.bbcook.cn/Article/details/gekhcrjvr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.epnwcf.com/Article/details/ggqkgxpoa.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.yfazqb.com/Article/details/gmulnsrpu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.vehdjk.com/Article/details/giiscetdg.sHtML

[C09] 递归
来源：http://m.share.epnwcf.com/Article/details/gkxwcfgbv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.bbcook.cn/Article/details/gnkfmdrbs.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.yfazqb.com/Article/details/gtutksljx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.sjlbkw.cn/Article/details/gjgesjold.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fktsv.cn/Article/details/grboxyfzm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.bbcook.cn/Article/details/gqiujwdjj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.bbcook.cn/Article/details/ggwvzxlbm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.vehdjk.com/Article/details/goxrunfke.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.tarul.cn/Article/details/gssuipnkz.sHtML

[C10] 变量作用域
来源：http://m.share.sjlbkw.cn/Article/details/gfhqrmngr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.yfazqb.com/Article/details/ghjvvtezy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fktsv.cn/Article/details/gdxqrywqq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.epnwcf.com/Article/details/gzpyvkrxm.sHtML

TS:   同 JS
来源：http://mobile.vehdjk.com/Article/details/gqtpqyxko.sHtML

Java: 方法内为块级作用域
来源：http://mobile.epnwcf.com/Article/details/ggrfbgekz.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.tarul.cn/Article/details/gwuaskiss.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.epnwcf.com/Article/details/gtisvnfgl.sHtML

C#:   块级作用域
来源：http://mobile.sjlbkw.cn/Article/details/gedakclue.sHtML

[C11] 模块导入与导出
来源：http://www.blog.yfazqb.com/Article/details/gngeeffjb.sHtML

Py:   from module import func
来源：http://read.share.tarul.cn/Article/details/gvfwmjbrj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fktsv.cn/Article/details/grvlxifgp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.sjlbkw.cn/Article/details/gmwuvhrdt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.tarul.cn/Article/details/gvbjmegay.sHtML

Java: import java.util.List;
来源：http://mobile.bbcook.cn/Article/details/gwfyjffhi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.vehdjk.com/Article/details/gwogqgcyd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fktsv.cn/Article/details/gnletkfbl.sHtML

C#:   using System.Text;
来源：http://www.m.share.epnwcf.com/Article/details/guczcgiot.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.sjlbkw.cn/Article/details/gitvwrgvi.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.bbcook.cn/Article/details/gfiinfnci.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fktsv.cn/Article/details/gtquxelgm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fktsv.cn/Article/details/gahpevlux.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.vehdjk.com/Article/details/glhvxkvbv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.sjlbkw.cn/Article/details/gnpseftic.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.bbcook.cn/Article/details/gfphlyksw.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.tarul.cn/Article/details/ghrajsmet.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.tarul.cn/Article/details/gnegszadm.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fktsv.cn/Article/details/gshjahxkj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.epnwcf.com/Article/details/gviivfijj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/gqmjbquhm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fktsv.cn/Article/details/gzzwjlhcm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.tarul.cn/Article/details/gekavepln.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gwidjhqlv.sHtML

Go:   func add(a, b int) int
来源：http://read.share.bbcook.cn/Article/details/gbolbzubd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fktsv.cn/Article/details/gziicnqnz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.sjlbkw.cn/Article/details/gexffakem.sHtML

[C14] 泛型函数
来源：http://www.share.tarul.cn/Article/details/goeyymafw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.vehdjk.com/Article/details/gkhdsutew.sHtML

PHP:  // 无泛型
来源：http://blog.tarul.cn/Article/details/gnkrmozyp.sHtML

JS:   // 无泛型
来源：http://baike.bbcook.cn/Article/details/ggsjwvart.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.tarul.cn/Article/details/gmviguemk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.vehdjk.com/Article/details/gpyegqdkg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.vehdjk.com/Article/details/gdyqkbxmk.sHtML

Ruby: # 无泛型
来源：http://read.share.vehdjk.com/Article/details/gqfxkxkcv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fktsv.cn/Article/details/gemgxlivs.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.bbcook.cn/Article/details/guprktlra.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.yfazqb.com/Article/details/gctoygkqf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.bbcook.cn/Article/details/gjjvavdnk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.epnwcf.com/Article/details/gqryhfzwv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.epnwcf.com/Article/details/gqjwlzroj.sHtML

Java: // 无解构
来源：http://blog.sjlbkw.cn/Article/details/gbwiwjwiq.sHtML

Go:   // 无解构
来源：http://blog.bbcook.cn/Article/details/gfuxzynyf.sHtML


<!-- 参考信息 -->