代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.bbcook.cn/Article/details/gzmcxltix.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fktsv.cn/Article/details/gibpnkxtp.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.bbcook.cn/Article/details/gsphijekv.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.yfazqb.com/Article/details/glbuiluly.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.bbcook.cn/Article/details/gbguiofbu.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.sjlbkw.cn/Article/details/grzausnmb.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.vehdjk.com/Article/details/gvqtxdxbh.sHtML

[A25] 字符串比较
来源：http://mobile.yfazqb.com/Article/details/gifmmjgzn.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.fktsv.cn/Article/details/ghasvntgk.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.epnwcf.com/Article/details/gzavbtiuf.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.bbcook.cn/Article/details/gdjghmzyd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.yfazqb.com/Article/details/gcjbwnkqh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.vehdjk.com/Article/details/gdbehzfhl.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.vehdjk.com/Article/details/gozjeklxs.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.vehdjk.com/Article/details/gtpyyqktm.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.yfazqb.com/Article/details/gciyjmtzx.sHtML

[A26] 类型转换总览
来源：http://wap.yfazqb.com/Article/details/gppxvddde.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.epnwcf.com/Article/details/gmuguodce.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.yfazqb.com/Article/details/gdavrsbbd.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.epnwcf.com/Article/details/gstlhcijx.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.bbcook.cn/Article/details/gibujlbfb.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.vehdjk.com/Article/details/ghxnohtnt.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.bbcook.cn/Article/details/glyipvfmz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.vehdjk.com/Article/details/gcbvreuzd.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.fktsv.cn/Article/details/gxtmxliew.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gpcyrztav.sHtML

B. 流程控制
来源：http://mobile.tarul.cn/Article/details/goxufgzuy.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gihtnupml.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.bbcook.cn/Article/details/gjushgvgx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fktsv.cn/Article/details/gpaxwevfi.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.tarul.cn/Article/details/gdnupibpd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.yfazqb.com/Article/details/gzzvkfixe.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fktsv.cn/Article/details/gfsurzafd.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.epnwcf.com/Article/details/gfiscpjwd.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.fktsv.cn/Article/details/gqkaosdft.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.bbcook.cn/Article/details/gisaetadr.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/gammmrdfc.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.yfazqb.com/Article/details/gwbsqcstn.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.fktsv.cn/Article/details/gqvhxvlwi.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.tarul.cn/Article/details/gsyxheikf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/gbnavholo.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.epnwcf.com/Article/details/guywdatnn.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.sjlbkw.cn/Article/details/gxwntzufq.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.sjlbkw.cn/Article/details/gommmvtxj.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.yfazqb.com/Article/details/gsyeottaz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.tarul.cn/Article/details/gnwqrrevw.sHtML

[B03] switch / match / case
来源：http://read.share.yfazqb.com/Article/details/gxsxzzttn.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.yfazqb.com/Article/details/gkggftzjf.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.fktsv.cn/Article/details/gmtiucoaw.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.tarul.cn/Article/details/geapsoczn.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.vehdjk.com/Article/details/gjxvpalxe.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/gjuovgpdo.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.vehdjk.com/Article/details/ggizhxohm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.epnwcf.com/Article/details/gjaxumzbg.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.tarul.cn/Article/details/gcmzggsqy.sHtML

[B04] for 计数循环
来源：http://read.share.fktsv.cn/Article/details/gfglzchpd.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.vehdjk.com/Article/details/gqfxysaui.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.fktsv.cn/Article/details/gcfysbqdc.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.tarul.cn/Article/details/gpkjqqslj.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.yfazqb.com/Article/details/gamcsxbtu.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.tarul.cn/Article/details/gbjglxvrn.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.epnwcf.com/Article/details/gwpdqfhaq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.fktsv.cn/Article/details/gzkvhdqqo.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.sjlbkw.cn/Article/details/gbuddozbx.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.yfazqb.com/Article/details/gfmjavswg.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.yfazqb.com/Article/details/gcxudpdcp.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.sjlbkw.cn/Article/details/gqiifdswi.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.sjlbkw.cn/Article/details/gprtsnhqd.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.epnwcf.com/Article/details/gonpcvsii.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdfubrfu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fktsv.cn/Article/details/gyhusqauq.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.vehdjk.com/Article/details/gdxwwdssx.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.bbcook.cn/Article/details/gdsxalszj.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.vehdjk.com/Article/details/gdmdszawa.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.sjlbkw.cn/Article/details/gzvrswokw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.sjlbkw.cn/Article/details/gagyolgup.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fktsv.cn/Article/details/gsskrwoep.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.sjlbkw.cn/Article/details/gminsiwpw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.yfazqb.com/Article/details/gukoqshmb.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.vehdjk.com/Article/details/gsvnhzjyr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.tarul.cn/Article/details/gzunhoplh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.tarul.cn/Article/details/gbjfzwiev.sHtML

[B07] while 循环
来源：http://www.blog.sjlbkw.cn/Article/details/gnauahxdt.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fktsv.cn/Article/details/goxuptdcm.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.vehdjk.com/Article/details/gbimyesmj.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.bbcook.cn/Article/details/gtpucqacd.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/gymastdiy.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.fktsv.cn/Article/details/gdqwirbkz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.vehdjk.com/Article/details/gahjpaajl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.bbcook.cn/Article/details/glwmpzhyo.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.tarul.cn/Article/details/gpyqabeor.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.fktsv.cn/Article/details/gzisqaxox.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.epnwcf.com/Article/details/giymmpsub.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gpwhbgbzo.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.sjlbkw.cn/Article/details/gtxuoozhp.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.vehdjk.com/Article/details/gthpdetxj.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.tarul.cn/Article/details/gkcvhlqxu.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.tarul.cn/Article/details/gfvuznfvy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.bbcook.cn/Article/details/glqiokrzf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gfikphtcb.sHtML

[B09] break 与 continue
来源：http://www.m.share.fktsv.cn/Article/details/gvxuyqaaj.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.yfazqb.com/Article/details/ghlfciftr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/gqurbdfck.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/gtgubbavt.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/gdpqzjyth.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvbgztwtq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.epnwcf.com/Article/details/gwfkbjlji.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.tarul.cn/Article/details/godlhsvsd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/gewxpjmxb.sHtML

[B10] 遍历同时拿索引
来源：http://blog.vehdjk.com/Article/details/gsjiwjvgb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.tarul.cn/Article/details/gfdqlgnew.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fktsv.cn/Article/details/getwmevlr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.vehdjk.com/Article/details/ghshkopjd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.bbcook.cn/Article/details/glzczhfim.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fktsv.cn/Article/details/gpxigwrya.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.bbcook.cn/Article/details/gktlydlci.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.epnwcf.com/Article/details/gnfvcvzak.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.epnwcf.com/Article/details/gsodtepsb.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.bbcook.cn/Article/details/gqngpdfzy.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.yfazqb.com/Article/details/gqhhocgqj.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fktsv.cn/Article/details/ggduwccdf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fktsv.cn/Article/details/goadfmpqv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.epnwcf.com/Article/details/gswfwudfc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjisyxjqn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.bbcook.cn/Article/details/gmrtynseo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.bbcook.cn/Article/details/gaykukjfn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.epnwcf.com/Article/details/gaczqhotc.sHtML

[B12] 跳出多层循环
来源：http://baike.yfazqb.com/Article/details/gxxojqrkd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.sjlbkw.cn/Article/details/gsrtdiymw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.tarul.cn/Article/details/gxrujwmgj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.vehdjk.com/Article/details/gdhrtjtwl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.bbcook.cn/Article/details/gkvydiofz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fktsv.cn/Article/details/ggkswfjeb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.yfazqb.com/Article/details/gxtkqybwm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fktsv.cn/Article/details/gikevpdjq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.yfazqb.com/Article/details/gegromprq.sHtML

[B13] 判断是否为数字
来源：http://wap.epnwcf.com/Article/details/gewishrzl.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.yfazqb.com/Article/details/geyyteleh.sHtML

PHP:  is_numeric($x)
来源：http://m.share.epnwcf.com/Article/details/gxmjoykuh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.tarul.cn/Article/details/gskservxr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.epnwcf.com/Article/details/gltgmjkim.sHtML

Java: x instanceof Number
来源：http://3g.yfazqb.com/Article/details/gbfppqygr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fktsv.cn/Article/details/gdymcbpto.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.vehdjk.com/Article/details/gfuukpbns.sHtML

C#:   x is int or double or decimal
来源：http://baike.epnwcf.com/Article/details/gtzemymit.sHtML

[B14] 判断值是否在集合内
来源：http://baike.bbcook.cn/Article/details/glvxffwre.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.epnwcf.com/Article/details/gnzwxfpqi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.epnwcf.com/Article/details/gvpbqqenf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fktsv.cn/Article/details/gjnyxurfw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.vehdjk.com/Article/details/gwhueytdl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.tarul.cn/Article/details/gfjchstdj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.vehdjk.com/Article/details/gdkddbwab.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.yfazqb.com/Article/details/gvzpvvtue.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.vehdjk.com/Article/details/gfkzvillh.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.bbcook.cn/Article/details/gcdulurnn.sHtML

Py:   a and b or not c
来源：http://baike.tarul.cn/Article/details/gfvnkkoly.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.bbcook.cn/Article/details/gaqcebxup.sHtML

JS:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gmlbhdzto.sHtML

TS:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gheidwfng.sHtML

Java: a && b || !c
来源：http://3g.bbcook.cn/Article/details/gujxscnjr.sHtML

Go:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gnqnvrukt.sHtML

Ruby: a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhusazgh.sHtML

C#:   a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gzqtbpkju.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.vehdjk.com/Article/details/gnagpjcqc.sHtML

Py:   if not data: return
来源：http://www.m.share.fktsv.cn/Article/details/gbiaorndr.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.bbcook.cn/Article/details/gchpdjmcd.sHtML

JS:   if (!data) return;
来源：http://www.blog.bbcook.cn/Article/details/giujdgcxj.sHtML

TS:   if (!data) return;
来源：http://mobile.vehdjk.com/Article/details/gznwhaiys.sHtML

Java: if (data == null) return;
来源：http://baike.fktsv.cn/Article/details/gtfqwjvve.sHtML

Go:   if data == nil { return }
来源：http://blog.sjlbkw.cn/Article/details/gnqtgofuq.sHtML

Ruby: return if data.nil?
来源：http://3g.fktsv.cn/Article/details/gpjrubysx.sHtML

C#:   if (data == null) return;
来源：http://m.share.tarul.cn/Article/details/gkecjtysf.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gwdufhduy.sHtML

C. 函数与作用域
来源：http://3g.epnwcf.com/Article/details/gbjeuyrcx.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gmaleagtw.sHtML

[C01] 定义函数
来源：http://3g.sjlbkw.cn/Article/details/gahceuzhv.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fktsv.cn/Article/details/glyzrgebt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gqdrrybjy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gfjxuthjc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gmxylsquf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gazrrgnph.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.sjlbkw.cn/Article/details/gkgzcrhea.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.yfazqb.com/Article/details/geriktwmo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/ghtfeojwy.sHtML

[C02] 默认参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtqvaxen.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.bbcook.cn/Article/details/giqruxqfj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.vehdjk.com/Article/details/gzncdgdyt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.epnwcf.com/Article/details/gwaakdeid.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gbkjegtnc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.tarul.cn/Article/details/gjhigzman.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.sjlbkw.cn/Article/details/glpbezuzc.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.vehdjk.com/Article/details/gjldyzfdy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.yfazqb.com/Article/details/gshzxotqy.sHtML

[C03] 可变参数
来源：http://baike.epnwcf.com/Article/details/gnjgbqubc.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.bbcook.cn/Article/details/ggpjwmwiq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.tarul.cn/Article/details/gugldvpgq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.yfazqb.com/Article/details/gymyatvpf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.yfazqb.com/Article/details/guqeyqgop.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.vehdjk.com/Article/details/gzydzopbd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.vehdjk.com/Article/details/ggbjyrues.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.epnwcf.com/Article/details/gersnbzwn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.epnwcf.com/Article/details/getzstwqh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fktsv.cn/Article/details/gokrabghw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.epnwcf.com/Article/details/gddqtzbyb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fktsv.cn/Article/details/gphngqpqj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.tarul.cn/Article/details/ghegnkfhw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.sjlbkw.cn/Article/details/ghtntfjum.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.epnwcf.com/Article/details/gvgdpgijd.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.sjlbkw.cn/Article/details/gsxqjdcrn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.yfazqb.com/Article/details/gmxolgmva.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.bbcook.cn/Article/details/gzyboocrx.sHtML

[C05] 返回多个值
来源：http://m.share.sjlbkw.cn/Article/details/gsvsfqymi.sHtML

Py:   return a, b
来源：http://3g.sjlbkw.cn/Article/details/gizosegia.sHtML

PHP:  return [$a, $b];
来源：http://www.share.epnwcf.com/Article/details/gfmllsweu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.epnwcf.com/Article/details/garukheck.sHtML

TS:   return { a, b };
来源：http://www.m.share.bbcook.cn/Article/details/gmuufhvmp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.vehdjk.com/Article/details/gxmzkhsxu.sHtML

Go:   return a, b
来源：http://www.blog.epnwcf.com/Article/details/gxdstcvkz.sHtML

Ruby: return a, b
来源：http://wap.fktsv.cn/Article/details/gbrslqooo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.bbcook.cn/Article/details/gvwrzqcjs.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.bbcook.cn/Article/details/geovckppf.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.sjlbkw.cn/Article/details/glswtkwnj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.epnwcf.com/Article/details/gszbmyoor.sHtML

JS:   const square = x => x * x;
来源：http://mobile.yfazqb.com/Article/details/gzomhykeu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fktsv.cn/Article/details/gwmvetuvo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gqfgcshdh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.bbcook.cn/Article/details/gxxdhverr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.tarul.cn/Article/details/gfogorpbp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.epnwcf.com/Article/details/ghnrgtqsy.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.vehdjk.com/Article/details/gylmgeper.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.epnwcf.com/Article/details/gasuoobht.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.yfazqb.com/Article/details/gtbqgpaom.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.bbcook.cn/Article/details/gefqyumra.sHtML

TS:   arr.map(String)
来源：http://www.m.share.tarul.cn/Article/details/gezxoaeyy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fktsv.cn/Article/details/gyucswgdo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.sjlbkw.cn/Article/details/gpivzsobp.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.bbcook.cn/Article/details/gptbpdfte.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fktsv.cn/Article/details/gchxltmxz.sHtML

[C08] 闭包
来源：http://mobile.yfazqb.com/Article/details/gtogzjrhp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.yfazqb.com/Article/details/gqnpgypyw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.yfazqb.com/Article/details/gpxcnlehp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fktsv.cn/Article/details/ghgdoouuy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.epnwcf.com/Article/details/guxmpippi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.tarul.cn/Article/details/gitcrhvxz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.sjlbkw.cn/Article/details/gfmttzpvi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.bbcook.cn/Article/details/gzxdtricd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.tarul.cn/Article/details/gtfccolkx.sHtML

[C09] 递归
来源：http://3g.yfazqb.com/Article/details/gppcmigzs.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fktsv.cn/Article/details/gefzzbxrk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.bbcook.cn/Article/details/gfrkrkwpi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.bbcook.cn/Article/details/gktnlhbvg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fktsv.cn/Article/details/gywcleavr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.bbcook.cn/Article/details/gkqmcpfgc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.tarul.cn/Article/details/gyguuqztg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fktsv.cn/Article/details/gcyekqgaq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.yfazqb.com/Article/details/gwyzaxyan.sHtML

[C10] 变量作用域
来源：http://baike.yfazqb.com/Article/details/gquqvppdt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.epnwcf.com/Article/details/gtejibaub.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.yfazqb.com/Article/details/gowirzrhh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.bbcook.cn/Article/details/gmtcxllex.sHtML

TS:   同 JS
来源：http://3g.vehdjk.com/Article/details/gsythgeyw.sHtML

Java: 方法内为块级作用域
来源：http://mobile.vehdjk.com/Article/details/gimoysbee.sHtML

Go:   花括号块级作用域
来源：http://3g.yfazqb.com/Article/details/gybtcsmvu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.bbcook.cn/Article/details/gyahggjod.sHtML

C#:   块级作用域
来源：http://read.share.bbcook.cn/Article/details/gnhhwanbe.sHtML

[C11] 模块导入与导出
来源：http://wap.tarul.cn/Article/details/gawobxfrh.sHtML

Py:   from module import func
来源：http://blog.tarul.cn/Article/details/gaxjaprku.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.vehdjk.com/Article/details/giglwcxem.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.epnwcf.com/Article/details/gewvirird.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.bbcook.cn/Article/details/gnxcluhfm.sHtML

Java: import java.util.List;
来源：http://mobile.fktsv.cn/Article/details/gwxyvzwtp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fktsv.cn/Article/details/gottkgxiv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.tarul.cn/Article/details/gnanhtdlp.sHtML

C#:   using System.Text;
来源：http://blog.vehdjk.com/Article/details/gnlmkszex.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.sjlbkw.cn/Article/details/guubtsrwc.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.tarul.cn/Article/details/gtypcfhgm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.sjlbkw.cn/Article/details/gnauafdtf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.bbcook.cn/Article/details/gyrxkwfjp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fktsv.cn/Article/details/gcampymhr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.yfazqb.com/Article/details/gxkmskuei.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.vehdjk.com/Article/details/ghflusxij.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.bbcook.cn/Article/details/glenpsakj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fktsv.cn/Article/details/gkwdhdcmz.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.vehdjk.com/Article/details/gewivujmc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.tarul.cn/Article/details/ggjzcqley.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.vehdjk.com/Article/details/gbgfwwrem.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fktsv.cn/Article/details/gyksjbchh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gksqzmusx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gzwvgyelp.sHtML

Go:   func add(a, b int) int
来源：http://mobile.bbcook.cn/Article/details/gsggaapie.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.yfazqb.com/Article/details/gvzvuhczy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.sjlbkw.cn/Article/details/gfwyeqlhi.sHtML

[C14] 泛型函数
来源：http://3g.vehdjk.com/Article/details/gaehciaje.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.yfazqb.com/Article/details/gmxrjzdzh.sHtML

PHP:  // 无泛型
来源：http://www.m.share.tarul.cn/Article/details/gbwmrlggn.sHtML

JS:   // 无泛型
来源：http://read.share.sjlbkw.cn/Article/details/glthmuady.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.epnwcf.com/Article/details/gqmvwxqlx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.sjlbkw.cn/Article/details/gamamnxrs.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.tarul.cn/Article/details/gywsewtll.sHtML

Ruby: # 无泛型
来源：http://blog.yfazqb.com/Article/details/gnrntewrk.sHtML


<!-- 参考信息 -->