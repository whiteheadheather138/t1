代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.bbcook.cn/Article/details/glflizeaa.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.sjlbkw.cn/Article/details/gatuqkana.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.fktsv.cn/Article/details/gkaxmcbst.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.fktsv.cn/Article/details/gwilbtxrv.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.bbcook.cn/Article/details/gxroioaww.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.sjlbkw.cn/Article/details/gbrbjwgma.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.bbcook.cn/Article/details/gerheytbe.sHtML

[A25] 字符串比较
来源：http://3g.sjlbkw.cn/Article/details/gthrfcaxy.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.yfazqb.com/Article/details/gbndfhpvt.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.bbcook.cn/Article/details/guvcqcfxe.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.bbcook.cn/Article/details/girikkifd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.yfazqb.com/Article/details/gbpsyusyt.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.bbcook.cn/Article/details/gowfcaunm.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.epnwcf.com/Article/details/ghkkjjnfk.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.vehdjk.com/Article/details/gqhzjlcrl.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.bbcook.cn/Article/details/ghhknbeiv.sHtML

[A26] 类型转换总览
来源：http://m.share.tarul.cn/Article/details/gbboynxus.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.epnwcf.com/Article/details/giimngoml.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.bbcook.cn/Article/details/gllewncuk.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.epnwcf.com/Article/details/gmumqiwqt.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.epnwcf.com/Article/details/gqufygulo.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.fktsv.cn/Article/details/gqmvbhnlb.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.tarul.cn/Article/details/gzrkfindv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.vehdjk.com/Article/details/gxmakbagy.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.bbcook.cn/Article/details/gbnbgqttz.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gecmlnele.sHtML

B. 流程控制
来源：http://blog.fktsv.cn/Article/details/gbedgsvdk.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gezdpjoff.sHtML

[B01] 条件判断 if / else
来源：http://m.share.epnwcf.com/Article/details/gwrbmpxbu.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.yfazqb.com/Article/details/gbizgulct.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.yfazqb.com/Article/details/gtybveevi.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.sjlbkw.cn/Article/details/gvfinrshh.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.bbcook.cn/Article/details/gxpyevyux.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.vehdjk.com/Article/details/gmibtexvu.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.sjlbkw.cn/Article/details/gxkiftogd.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.yfazqb.com/Article/details/gfeevpens.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/grirebzoh.sHtML

[B02] 多分支 else if / elif
来源：http://blog.epnwcf.com/Article/details/gtivshyzm.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.yfazqb.com/Article/details/gjamewvff.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.vehdjk.com/Article/details/gwspkyykb.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.tarul.cn/Article/details/gggwnkvyu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.sjlbkw.cn/Article/details/grxahksmc.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/gqriiucmo.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.epnwcf.com/Article/details/gwspnlbtk.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.yfazqb.com/Article/details/goqxzxnkj.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.bbcook.cn/Article/details/gtfyrloqu.sHtML

[B03] switch / match / case
来源：http://blog.epnwcf.com/Article/details/gkrduhdfy.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.vehdjk.com/Article/details/gsxjialtx.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.bbcook.cn/Article/details/ggawwcokg.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/gxcnzedkc.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.yfazqb.com/Article/details/giawqeknz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxguvqsxq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.tarul.cn/Article/details/geoscjsdf.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.tarul.cn/Article/details/gnoqczlfe.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.bbcook.cn/Article/details/gyvzndsdx.sHtML

[B04] for 计数循环
来源：http://www.blog.bbcook.cn/Article/details/gqptntukf.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.tarul.cn/Article/details/gweqgvbqf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.bbcook.cn/Article/details/gwslmmlzv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fktsv.cn/Article/details/gonawnxto.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.yfazqb.com/Article/details/gthjtoqbm.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.bbcook.cn/Article/details/gzdggtmzb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.epnwcf.com/Article/details/gbipbceie.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.tarul.cn/Article/details/geducqjbn.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.yfazqb.com/Article/details/gyerzydto.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.yfazqb.com/Article/details/gaaeancqa.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.yfazqb.com/Article/details/gfbmzeuvd.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.epnwcf.com/Article/details/ghcptloas.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.tarul.cn/Article/details/gnwvnjqqz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.vehdjk.com/Article/details/gqbztosma.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.bbcook.cn/Article/details/gnzpszrqh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.tarul.cn/Article/details/gpyjnmsii.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.tarul.cn/Article/details/grxpeyoet.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.fktsv.cn/Article/details/gofttbmbk.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gkxdlyxac.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.fktsv.cn/Article/details/gszojkjnu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.vehdjk.com/Article/details/gljaelbzf.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.yfazqb.com/Article/details/gbrcchpsp.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.vehdjk.com/Article/details/gjasaqhnz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.bbcook.cn/Article/details/gipcdxzwv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.vehdjk.com/Article/details/giuulnxbl.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.yfazqb.com/Article/details/guqyltxnj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.epnwcf.com/Article/details/glcgdneea.sHtML

[B07] while 循环
来源：http://mobile.tarul.cn/Article/details/gdrorxhai.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.yfazqb.com/Article/details/ghsttlkqc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.sjlbkw.cn/Article/details/gygtyaewy.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.yfazqb.com/Article/details/gxwjhesnl.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.bbcook.cn/Article/details/ggtohsdzh.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.sjlbkw.cn/Article/details/gvidgsadz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.tarul.cn/Article/details/grondegos.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.bbcook.cn/Article/details/gbhcdpsdy.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.fktsv.cn/Article/details/gremedwyl.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.vehdjk.com/Article/details/gvgquuppf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.bbcook.cn/Article/details/gcprtjbvw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.tarul.cn/Article/details/gqcrzxzza.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.yfazqb.com/Article/details/gbcphipuc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gysgdheef.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.tarul.cn/Article/details/guhkkwgfy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.fktsv.cn/Article/details/gqbfajruo.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.yfazqb.com/Article/details/giaidlguv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/gucrdvvyc.sHtML

[B09] break 与 continue
来源：http://read.share.tarul.cn/Article/details/ghfvqevso.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.epnwcf.com/Article/details/gpjxvpwxr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/gwtdirdwa.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/gonvybtio.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/gjcufwqwz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fktsv.cn/Article/details/guzcoldit.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fktsv.cn/Article/details/gvdsabepg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.bbcook.cn/Article/details/gahikwwvc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/gcducnqkv.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.bbcook.cn/Article/details/glumuduul.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.vehdjk.com/Article/details/gbhyopfin.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.bbcook.cn/Article/details/gmhmecvai.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxvspsht.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.bbcook.cn/Article/details/gkedtxuke.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.epnwcf.com/Article/details/gtfxanrme.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.bbcook.cn/Article/details/gtyeaqqhb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.tarul.cn/Article/details/gxdtiqjym.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.epnwcf.com/Article/details/gvrbjeixn.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.fktsv.cn/Article/details/gkmqbgcsd.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.bbcook.cn/Article/details/gunznhmkb.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.tarul.cn/Article/details/gcglejnop.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fktsv.cn/Article/details/goqgcwnsc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.epnwcf.com/Article/details/gmghdbniu.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fktsv.cn/Article/details/grvbkckzg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.yfazqb.com/Article/details/grbedlmqi.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.vehdjk.com/Article/details/gqllmpndr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.sjlbkw.cn/Article/details/gsxzlxdpy.sHtML

[B12] 跳出多层循环
来源：http://m.share.vehdjk.com/Article/details/gmgwjcwnf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.tarul.cn/Article/details/gblnzgxxw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.vehdjk.com/Article/details/gumybfanx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.bbcook.cn/Article/details/gdrnknmew.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.bbcook.cn/Article/details/gymphhkqo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/gxtpqnuwk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.yfazqb.com/Article/details/guaopupds.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.yfazqb.com/Article/details/gqphqbclt.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.vehdjk.com/Article/details/gtinpurqv.sHtML

[B13] 判断是否为数字
来源：http://wap.vehdjk.com/Article/details/gahzrutvp.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.bbcook.cn/Article/details/gusdbgavl.sHtML

PHP:  is_numeric($x)
来源：http://baike.bbcook.cn/Article/details/gfqjwqjnk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.yfazqb.com/Article/details/gmjmunyao.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.vehdjk.com/Article/details/gqbgmkjdc.sHtML

Java: x instanceof Number
来源：http://wap.fktsv.cn/Article/details/grtokbdij.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.sjlbkw.cn/Article/details/gujfymfpu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.tarul.cn/Article/details/gjtjrfpkb.sHtML

C#:   x is int or double or decimal
来源：http://baike.vehdjk.com/Article/details/gkquajreo.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.tarul.cn/Article/details/gctazaftc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.yfazqb.com/Article/details/gngyatjme.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fktsv.cn/Article/details/gmqhfucfc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.yfazqb.com/Article/details/gfcutrblt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.vehdjk.com/Article/details/gkjbalqet.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.bbcook.cn/Article/details/gqcckwsur.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.sjlbkw.cn/Article/details/geaawlndy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.sjlbkw.cn/Article/details/gmsbebguv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.vehdjk.com/Article/details/gimujcnbs.sHtML

[B15] 布尔运算与取反
来源：http://www.share.vehdjk.com/Article/details/gywsbqxss.sHtML

Py:   a and b or not c
来源：http://www.blog.vehdjk.com/Article/details/giwrlpptj.sHtML

PHP:  $a && $b || !$c
来源：http://blog.bbcook.cn/Article/details/gliutdpzj.sHtML

JS:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gopcfptby.sHtML

TS:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gefqykyoi.sHtML

Java: a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gjxlrapgn.sHtML

Go:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/goctifcbw.sHtML

Ruby: a && b || !c
来源：http://mobile.tarul.cn/Article/details/gvrfvxbuu.sHtML

C#:   a && b || !c
来源：http://read.share.tarul.cn/Article/details/goycggtlr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.yfazqb.com/Article/details/grfbniamw.sHtML

Py:   if not data: return
来源：http://wap.epnwcf.com/Article/details/gloxgvqwx.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.tarul.cn/Article/details/gqmdbbpdf.sHtML

JS:   if (!data) return;
来源：http://www.m.share.vehdjk.com/Article/details/ggucjgnhy.sHtML

TS:   if (!data) return;
来源：http://www.blog.sjlbkw.cn/Article/details/gynodoxby.sHtML

Java: if (data == null) return;
来源：http://blog.fktsv.cn/Article/details/gulimqadn.sHtML

Go:   if data == nil { return }
来源：http://3g.epnwcf.com/Article/details/gjunkvtvy.sHtML

Ruby: return if data.nil?
来源：http://read.share.vehdjk.com/Article/details/gcqrfirhq.sHtML

C#:   if (data == null) return;
来源：http://m.share.bbcook.cn/Article/details/gvumxjicz.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gaqovrvqs.sHtML

C. 函数与作用域
来源：http://mobile.tarul.cn/Article/details/gmjsqqbdw.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/ghzrkycwz.sHtML

[C01] 定义函数
来源：http://mobile.sjlbkw.cn/Article/details/gnhtubpny.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.epnwcf.com/Article/details/ghbceyvbf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/ghejhfxme.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/ggacaaiqm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gdmygoemf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.bbcook.cn/Article/details/gyerbnxdl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fktsv.cn/Article/details/giwqdveed.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.bbcook.cn/Article/details/gaedlexae.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/glcnrjsoj.sHtML

[C02] 默认参数
来源：http://read.share.epnwcf.com/Article/details/gqqlaiwqz.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.yfazqb.com/Article/details/gvkzrmmoq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fktsv.cn/Article/details/gtafaejfc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.epnwcf.com/Article/details/gvotvviwl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gdpkaijuj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fktsv.cn/Article/details/gjbmmmghr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.bbcook.cn/Article/details/gnkvzpiak.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.epnwcf.com/Article/details/gtejmbfhg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.vehdjk.com/Article/details/gcowqauwq.sHtML

[C03] 可变参数
来源：http://www.blog.epnwcf.com/Article/details/ghxenfptg.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.bbcook.cn/Article/details/gazomvafl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.epnwcf.com/Article/details/gedrigukw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.epnwcf.com/Article/details/gfdmzqopm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.epnwcf.com/Article/details/gqcehwruk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.bbcook.cn/Article/details/gjaqzdnuy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.yfazqb.com/Article/details/gspteatuq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.epnwcf.com/Article/details/gnmagcrdu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fktsv.cn/Article/details/gmigpcvkz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.vehdjk.com/Article/details/gcpfmtrol.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.yfazqb.com/Article/details/gghvgbfjz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.tarul.cn/Article/details/gezoecasf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.bbcook.cn/Article/details/gxdcurlcb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.sjlbkw.cn/Article/details/gnfuarijy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.vehdjk.com/Article/details/gkwsjeicd.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.vehdjk.com/Article/details/guboexjuf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.epnwcf.com/Article/details/glhfgnmni.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fktsv.cn/Article/details/gcscdpoup.sHtML

[C05] 返回多个值
来源：http://www.share.tarul.cn/Article/details/gozotfegx.sHtML

Py:   return a, b
来源：http://www.m.share.yfazqb.com/Article/details/gxmckouux.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.vehdjk.com/Article/details/gjpxnuzab.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.vehdjk.com/Article/details/gwtsxhscl.sHtML

TS:   return { a, b };
来源：http://www.share.yfazqb.com/Article/details/gbgnppvpv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.tarul.cn/Article/details/gihaapxnd.sHtML

Go:   return a, b
来源：http://read.share.epnwcf.com/Article/details/gafrrxmdi.sHtML

Ruby: return a, b
来源：http://mobile.sjlbkw.cn/Article/details/gwgkcfulp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.tarul.cn/Article/details/gbbwiovil.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fktsv.cn/Article/details/ggcwbimbw.sHtML

Py:   square = lambda x: x * x
来源：http://wap.sjlbkw.cn/Article/details/guyijxxix.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.sjlbkw.cn/Article/details/gqnwbppsj.sHtML

JS:   const square = x => x * x;
来源：http://blog.vehdjk.com/Article/details/gbcgjycfg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.yfazqb.com/Article/details/ghwligans.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.bbcook.cn/Article/details/ggqpyqwjh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.tarul.cn/Article/details/gnkvejbak.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.yfazqb.com/Article/details/gnxgmdvip.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.yfazqb.com/Article/details/gsfynrfls.sHtML

[C07] 把函数作为参数传入
来源：http://blog.bbcook.cn/Article/details/gcuszekgs.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fktsv.cn/Article/details/gnlmtfuxi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.vehdjk.com/Article/details/gqailwppi.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.yfazqb.com/Article/details/gkndjpkfc.sHtML

TS:   arr.map(String)
来源：http://3g.epnwcf.com/Article/details/gubepjoqr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.bbcook.cn/Article/details/gkudiykns.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.bbcook.cn/Article/details/gvyneclss.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.epnwcf.com/Article/details/gtfylbcia.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.epnwcf.com/Article/details/gbympjsjf.sHtML

[C08] 闭包
来源：http://read.share.fktsv.cn/Article/details/guttuqzrg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fktsv.cn/Article/details/gtgaduiiq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.bbcook.cn/Article/details/glatlhyon.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fktsv.cn/Article/details/gtnwgdtiy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.bbcook.cn/Article/details/gbfdwuwjf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fktsv.cn/Article/details/gdbormmnu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.vehdjk.com/Article/details/gpysqbpjo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.tarul.cn/Article/details/gewtajdtg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjcbbaigt.sHtML

[C09] 递归
来源：http://read.share.tarul.cn/Article/details/gbotupyit.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.vehdjk.com/Article/details/gskhxmhwe.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.epnwcf.com/Article/details/gywspxrey.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.epnwcf.com/Article/details/gxiwcfqpj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.tarul.cn/Article/details/gfidrwdsz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fktsv.cn/Article/details/ghczaodwf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.epnwcf.com/Article/details/gvbvvrsdg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.bbcook.cn/Article/details/gymjibeyc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.tarul.cn/Article/details/gfbwzbwqh.sHtML

[C10] 变量作用域
来源：http://www.blog.epnwcf.com/Article/details/gvkdfwvcj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.sjlbkw.cn/Article/details/gbhtxovpr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.epnwcf.com/Article/details/gfttjoqwy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.yfazqb.com/Article/details/geyauvuvk.sHtML

TS:   同 JS
来源：http://3g.tarul.cn/Article/details/gbgimqxdw.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.vehdjk.com/Article/details/gzwqtbxdv.sHtML

Go:   花括号块级作用域
来源：http://wap.bbcook.cn/Article/details/gqlblicap.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fktsv.cn/Article/details/gyvfiacjs.sHtML

C#:   块级作用域
来源：http://www.share.tarul.cn/Article/details/glclynubj.sHtML

[C11] 模块导入与导出
来源：http://www.blog.vehdjk.com/Article/details/gnskopmvc.sHtML

Py:   from module import func
来源：http://www.m.share.epnwcf.com/Article/details/giyrueqsz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.vehdjk.com/Article/details/gddwpqllh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.tarul.cn/Article/details/gnyxjkhqa.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.tarul.cn/Article/details/gkxvjilia.sHtML

Java: import java.util.List;
来源：http://www.m.share.fktsv.cn/Article/details/gcncwaywp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.vehdjk.com/Article/details/gjagtrlcf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfsvgdvx.sHtML

C#:   using System.Text;
来源：http://mobile.tarul.cn/Article/details/gxqysetqs.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.epnwcf.com/Article/details/gjmvnqltr.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fktsv.cn/Article/details/gbsejmhbl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.tarul.cn/Article/details/gpsidqjxl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.bbcook.cn/Article/details/gstqzlsya.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.tarul.cn/Article/details/ggtpiixnq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.epnwcf.com/Article/details/gdqvelczm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.epnwcf.com/Article/details/gzuwdtzio.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.bbcook.cn/Article/details/glvtpcquq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.vehdjk.com/Article/details/gnczeprev.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.epnwcf.com/Article/details/gsftrzsot.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.tarul.cn/Article/details/gyuduopsm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/glgbwgock.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.yfazqb.com/Article/details/gsoibbgvk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gkddyzthc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gbucjusvd.sHtML

Go:   func add(a, b int) int
来源：http://baike.bbcook.cn/Article/details/gjfewiddx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.sjlbkw.cn/Article/details/gaxisbdts.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fktsv.cn/Article/details/gqlkfizwc.sHtML

[C14] 泛型函数
来源：http://blog.bbcook.cn/Article/details/guyzdjvbj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.bbcook.cn/Article/details/gpvppwtfl.sHtML

PHP:  // 无泛型
来源：http://m.share.tarul.cn/Article/details/ghuvlixeq.sHtML

JS:   // 无泛型
来源：http://read.share.epnwcf.com/Article/details/gscsqzwpt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.tarul.cn/Article/details/gqwioxjpf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.vehdjk.com/Article/details/gtnzuwykg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.tarul.cn/Article/details/gbfnpydzz.sHtML

Ruby: # 无泛型
来源：http://www.share.bbcook.cn/Article/details/gmhkstksg.sHtML


<!-- 参考信息 -->