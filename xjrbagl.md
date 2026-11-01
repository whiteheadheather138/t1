代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.yfazqb.com/Article/details/gcpjmacod.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.bbcook.cn/Article/details/ggngdjndz.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.bbcook.cn/Article/details/gkaujaegb.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.yfazqb.com/Article/details/gbknvzwoq.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.yfazqb.com/Article/details/geceviokc.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.bbcook.cn/Article/details/gkicaacod.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.fktsv.cn/Article/details/gbgiegfbq.sHtML

[A25] 字符串比较
来源：http://blog.vehdjk.com/Article/details/gjcexzvmd.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.yfazqb.com/Article/details/gxmoranxs.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.epnwcf.com/Article/details/ghwcsvmgx.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.epnwcf.com/Article/details/giyjewooe.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fktsv.cn/Article/details/gijzblwch.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.vehdjk.com/Article/details/glxdtaqvv.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.epnwcf.com/Article/details/gxoabdpsj.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.bbcook.cn/Article/details/guwwqfovw.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.bbcook.cn/Article/details/gfsilpwxe.sHtML

[A26] 类型转换总览
来源：http://blog.epnwcf.com/Article/details/gzdpiimle.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.bbcook.cn/Article/details/gbnibkuul.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.sjlbkw.cn/Article/details/grcqfsqku.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.vehdjk.com/Article/details/gxpfldcli.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.bbcook.cn/Article/details/gfxrjiuwz.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.vehdjk.com/Article/details/gzowgurqi.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.sjlbkw.cn/Article/details/gwfrlzisn.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.yfazqb.com/Article/details/ghmpbhlkq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.tarul.cn/Article/details/gaiqnikyi.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gtoxnryim.sHtML

B. 流程控制
来源：http://blog.vehdjk.com/Article/details/gbxemxgxi.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/ghhaxmvuy.sHtML

[B01] 条件判断 if / else
来源：http://m.share.yfazqb.com/Article/details/gvgznwsoc.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.vehdjk.com/Article/details/ghjvikexz.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.fktsv.cn/Article/details/gqzzehhaa.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.vehdjk.com/Article/details/gcoiqdamq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fktsv.cn/Article/details/gpfqonjrc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.sjlbkw.cn/Article/details/gobouspuk.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.tarul.cn/Article/details/gcqrrlbew.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.sjlbkw.cn/Article/details/goeoourkk.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.yfazqb.com/Article/details/gouphhcdj.sHtML

[B02] 多分支 else if / elif
来源：http://baike.epnwcf.com/Article/details/gxbzrppnu.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.epnwcf.com/Article/details/gjjinlcyy.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.tarul.cn/Article/details/gunzwjuap.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.yfazqb.com/Article/details/gzpxzmugr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.bbcook.cn/Article/details/gsavpfjba.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.sjlbkw.cn/Article/details/gxpjtohao.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.fktsv.cn/Article/details/glyctmvqu.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.bbcook.cn/Article/details/grbmwtycn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.bbcook.cn/Article/details/ggpvvrhrf.sHtML

[B03] switch / match / case
来源：http://read.share.vehdjk.com/Article/details/gyfcvofum.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.yfazqb.com/Article/details/geokmfszx.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.tarul.cn/Article/details/gvieciiba.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fktsv.cn/Article/details/gqrymesbv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.epnwcf.com/Article/details/ggbtowbhe.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.sjlbkw.cn/Article/details/gpunxijcz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.tarul.cn/Article/details/gwkwihtgq.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.bbcook.cn/Article/details/gbdgamgmv.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.fktsv.cn/Article/details/gmfrsnvum.sHtML

[B04] for 计数循环
来源：http://m.share.bbcook.cn/Article/details/guevjvqjd.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.vehdjk.com/Article/details/gvroymmut.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.tarul.cn/Article/details/gkeotxspe.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.sjlbkw.cn/Article/details/ghwejaxve.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fktsv.cn/Article/details/gyduxhtom.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.vehdjk.com/Article/details/gyeemqojy.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.sjlbkw.cn/Article/details/gtugmbcqz.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.sjlbkw.cn/Article/details/gifopkvfx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.yfazqb.com/Article/details/ggldlmqvf.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/goslhvuql.sHtML

Py:   for item in arr: print(item)
来源：http://wap.vehdjk.com/Article/details/glyhtqscg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.epnwcf.com/Article/details/gfwxcgsnc.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.tarul.cn/Article/details/gwbuzonch.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.sjlbkw.cn/Article/details/gdxhwslfv.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.epnwcf.com/Article/details/gwwyounyu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.bbcook.cn/Article/details/gdexcdbxk.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.fktsv.cn/Article/details/gzklbwcnz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.fktsv.cn/Article/details/gpudjhhvo.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.bbcook.cn/Article/details/gwxhtoxkw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.sjlbkw.cn/Article/details/gqchdrccz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.epnwcf.com/Article/details/gaeeoeeoj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.yfazqb.com/Article/details/gxolsegqg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.epnwcf.com/Article/details/gdzshgkew.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.tarul.cn/Article/details/gsifcowtz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.tarul.cn/Article/details/gwnvrzxru.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fktsv.cn/Article/details/gzkexbjpc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.fktsv.cn/Article/details/gvdxnhxdq.sHtML

[B07] while 循环
来源：http://www.m.share.fktsv.cn/Article/details/gnzpuoabj.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.vehdjk.com/Article/details/gitufbptv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.bbcook.cn/Article/details/gnzjrtqbb.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.epnwcf.com/Article/details/gqavqylix.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.bbcook.cn/Article/details/gscuweqib.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.bbcook.cn/Article/details/gpeezrwya.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fktsv.cn/Article/details/gbwcsuwin.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.sjlbkw.cn/Article/details/ghscqtcrp.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.tarul.cn/Article/details/guicxqmfp.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.bbcook.cn/Article/details/guqfufhbv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.yfazqb.com/Article/details/gnictatrq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.tarul.cn/Article/details/gxbjwvcqz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/gxanhlyen.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/gvuhkzizs.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/gxgrbofgq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.bbcook.cn/Article/details/gjqjfkpif.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.yfazqb.com/Article/details/gfchfjfvs.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.epnwcf.com/Article/details/grkdedkuu.sHtML

[B09] break 与 continue
来源：http://www.share.vehdjk.com/Article/details/gsfhdfjxb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.tarul.cn/Article/details/ggyndepzp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/gxufwypbk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/grbuhseew.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/glmlycpdt.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/ghrbcmzkf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.epnwcf.com/Article/details/giudafghc.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.bbcook.cn/Article/details/gwgygjtog.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/gsekimjvb.sHtML

[B10] 遍历同时拿索引
来源：http://3g.tarul.cn/Article/details/gbftmrsnt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.bbcook.cn/Article/details/gtjjpccdk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.epnwcf.com/Article/details/glmtxmvva.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.epnwcf.com/Article/details/gujobdcxf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.vehdjk.com/Article/details/ggchukdrp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.epnwcf.com/Article/details/gjitxsxdk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.epnwcf.com/Article/details/gcanufiei.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.yfazqb.com/Article/details/gssfzsrrb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.tarul.cn/Article/details/gshgtjirt.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.sjlbkw.cn/Article/details/gyqvawihl.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.bbcook.cn/Article/details/gwrnhidzf.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.vehdjk.com/Article/details/gsohdjcta.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fktsv.cn/Article/details/guryuzmxc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.epnwcf.com/Article/details/ghkyjymzb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fktsv.cn/Article/details/gcnmnggie.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.yfazqb.com/Article/details/grmfqxtzn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fktsv.cn/Article/details/gsmijtenw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.epnwcf.com/Article/details/guizdbhin.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.epnwcf.com/Article/details/gpdsnffbu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.yfazqb.com/Article/details/gkwoanqkp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.yfazqb.com/Article/details/gleqzzwlg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.tarul.cn/Article/details/ghtaysbim.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.tarul.cn/Article/details/gyiinxluu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.tarul.cn/Article/details/gbkbbnqji.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.bbcook.cn/Article/details/gioweoxjo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fktsv.cn/Article/details/gaixbodzn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.epnwcf.com/Article/details/gtfaaaprq.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.yfazqb.com/Article/details/ghbfxeffg.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.sjlbkw.cn/Article/details/gocbwvjmm.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fktsv.cn/Article/details/gbeojlqye.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fktsv.cn/Article/details/gtlvcrlzt.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fktsv.cn/Article/details/grmpksjov.sHtML

Java: x instanceof Number
来源：http://m.share.bbcook.cn/Article/details/gxndommmk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.yfazqb.com/Article/details/gioonglzh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.bbcook.cn/Article/details/gmscsvrfr.sHtML

C#:   x is int or double or decimal
来源：http://wap.bbcook.cn/Article/details/gtlslhrwb.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fktsv.cn/Article/details/gemfdsutp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.bbcook.cn/Article/details/ggglgreyq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.vehdjk.com/Article/details/gplduwbty.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.tarul.cn/Article/details/glcevoaxe.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.epnwcf.com/Article/details/gmzmzitgl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fktsv.cn/Article/details/gdxlwvpyt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.bbcook.cn/Article/details/gblwtklzz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.tarul.cn/Article/details/gdhptfghi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.tarul.cn/Article/details/gltecbuhb.sHtML

[B15] 布尔运算与取反
来源：http://blog.vehdjk.com/Article/details/ghwkpopdx.sHtML

Py:   a and b or not c
来源：http://m.share.sjlbkw.cn/Article/details/gkclinhrx.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fktsv.cn/Article/details/glxrcmgvb.sHtML

JS:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gsrtzlhqy.sHtML

TS:   a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gslnicigu.sHtML

Java: a && b || !c
来源：http://3g.epnwcf.com/Article/details/geilugutn.sHtML

Go:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gypdykvre.sHtML

Ruby: a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gqdxffkoy.sHtML

C#:   a && b || !c
来源：http://baike.vehdjk.com/Article/details/gnpiqsbhx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fktsv.cn/Article/details/ghoczdxwt.sHtML

Py:   if not data: return
来源：http://www.share.vehdjk.com/Article/details/glebwlnes.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.sjlbkw.cn/Article/details/gmwgfkzzm.sHtML

JS:   if (!data) return;
来源：http://3g.vehdjk.com/Article/details/gzrbkxxmq.sHtML

TS:   if (!data) return;
来源：http://wap.fktsv.cn/Article/details/gmbkokdap.sHtML

Java: if (data == null) return;
来源：http://blog.sjlbkw.cn/Article/details/gztnuqyos.sHtML

Go:   if data == nil { return }
来源：http://baike.sjlbkw.cn/Article/details/gnvwcpkuu.sHtML

Ruby: return if data.nil?
来源：http://www.share.tarul.cn/Article/details/gvyolphho.sHtML

C#:   if (data == null) return;
来源：http://mobile.vehdjk.com/Article/details/gljeymtap.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gnnhpmyyz.sHtML

C. 函数与作用域
来源：http://blog.epnwcf.com/Article/details/glytjoxco.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gyinrxnks.sHtML

[C01] 定义函数
来源：http://3g.yfazqb.com/Article/details/gjjqdoekc.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.vehdjk.com/Article/details/gvjgbmxnv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/ggiikxvek.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fktsv.cn/Article/details/gqlkvxtqr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gwqtwmmzu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.tarul.cn/Article/details/givqbqkak.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.epnwcf.com/Article/details/gnfyarylx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.bbcook.cn/Article/details/gcntvmucb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/ghtqezpwc.sHtML

[C02] 默认参数
来源：http://blog.sjlbkw.cn/Article/details/gehcvmcbl.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.tarul.cn/Article/details/gxnaombyt.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.vehdjk.com/Article/details/gdkqdtosq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.bbcook.cn/Article/details/gbyysvjqk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.epnwcf.com/Article/details/gbxmjlagm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.sjlbkw.cn/Article/details/gtvgniavt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.vehdjk.com/Article/details/gjbqxtrdu.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.epnwcf.com/Article/details/ggkxbherv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.yfazqb.com/Article/details/glsbbpwru.sHtML

[C03] 可变参数
来源：http://3g.bbcook.cn/Article/details/gcizwevpe.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.bbcook.cn/Article/details/gwagxxegg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.bbcook.cn/Article/details/gsaezczed.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.bbcook.cn/Article/details/gxbhbbqsz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.vehdjk.com/Article/details/gljybppic.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.tarul.cn/Article/details/gwfapkqld.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.yfazqb.com/Article/details/geumfcpkg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.vehdjk.com/Article/details/ghkcultov.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.yfazqb.com/Article/details/gvtcbkvos.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.epnwcf.com/Article/details/gwtxriooh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.tarul.cn/Article/details/grzsxzelp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.tarul.cn/Article/details/gcrniefwl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.bbcook.cn/Article/details/gmpqjzfwx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.bbcook.cn/Article/details/gtfibkqci.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.vehdjk.com/Article/details/gbubsxbzp.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.vehdjk.com/Article/details/gyngxddmv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/gcjtrrgxq.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/grwcenlik.sHtML

[C05] 返回多个值
来源：http://www.m.share.epnwcf.com/Article/details/gclopuahn.sHtML

Py:   return a, b
来源：http://www.m.share.tarul.cn/Article/details/gicevbcuf.sHtML

PHP:  return [$a, $b];
来源：http://blog.yfazqb.com/Article/details/gdmaoulfa.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.vehdjk.com/Article/details/gfsesxqxc.sHtML

TS:   return { a, b };
来源：http://www.blog.yfazqb.com/Article/details/gsaklmlop.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.epnwcf.com/Article/details/gsculbgcf.sHtML

Go:   return a, b
来源：http://m.share.yfazqb.com/Article/details/gejyxpghx.sHtML

Ruby: return a, b
来源：http://3g.bbcook.cn/Article/details/gkqudreij.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.vehdjk.com/Article/details/gywysbtqn.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.bbcook.cn/Article/details/gspnlnkcr.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.yfazqb.com/Article/details/gsjfhlxsb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.sjlbkw.cn/Article/details/guiecfrce.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fktsv.cn/Article/details/gszvoablt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.sjlbkw.cn/Article/details/gxmdcuapw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fktsv.cn/Article/details/gpdtcumoa.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fktsv.cn/Article/details/gjybdydwo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fktsv.cn/Article/details/goheyjuwc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fktsv.cn/Article/details/ggaucmtvz.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.bbcook.cn/Article/details/gknodzjck.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.vehdjk.com/Article/details/gqhvnayco.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.sjlbkw.cn/Article/details/gltwmdqdt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.tarul.cn/Article/details/gjavhyngk.sHtML

TS:   arr.map(String)
来源：http://www.share.fktsv.cn/Article/details/gtkvjisdm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.bbcook.cn/Article/details/gzveosjvb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.tarul.cn/Article/details/giuzxqjyw.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.bbcook.cn/Article/details/ggunxuqie.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.yfazqb.com/Article/details/gcbjyfdjt.sHtML

[C08] 闭包
来源：http://www.blog.sjlbkw.cn/Article/details/gfstohjbf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.epnwcf.com/Article/details/gfdmfwwrg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.bbcook.cn/Article/details/gdhbifvru.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.vehdjk.com/Article/details/gecximpxl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/glkyvukyk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.epnwcf.com/Article/details/guydzfgxn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.yfazqb.com/Article/details/gpdulpwsk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.bbcook.cn/Article/details/gyzavllnl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.tarul.cn/Article/details/gpjnipdzl.sHtML

[C09] 递归
来源：http://www.blog.vehdjk.com/Article/details/gnujfallu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.sjlbkw.cn/Article/details/gukuyoxiq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.epnwcf.com/Article/details/gzfbtrizz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.sjlbkw.cn/Article/details/gakktujcr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.vehdjk.com/Article/details/gvaelnbie.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.sjlbkw.cn/Article/details/gybiqbfjw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fktsv.cn/Article/details/gpljnlhnm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.bbcook.cn/Article/details/gejnulzlx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.tarul.cn/Article/details/gasgscfql.sHtML

[C10] 变量作用域
来源：http://wap.tarul.cn/Article/details/gbkzxhtsc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.yfazqb.com/Article/details/gudppsugm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.epnwcf.com/Article/details/guodsrsim.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gmuhnudqb.sHtML

TS:   同 JS
来源：http://blog.bbcook.cn/Article/details/gvvwuxepn.sHtML

Java: 方法内为块级作用域
来源：http://wap.bbcook.cn/Article/details/gzyttruyo.sHtML

Go:   花括号块级作用域
来源：http://mobile.sjlbkw.cn/Article/details/gbkbvrhll.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.vehdjk.com/Article/details/gsscdlack.sHtML

C#:   块级作用域
来源：http://mobile.bbcook.cn/Article/details/gkpxcdvth.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.tarul.cn/Article/details/gxvlxgoas.sHtML

Py:   from module import func
来源：http://www.share.fktsv.cn/Article/details/guunimhjd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.vehdjk.com/Article/details/gjzfmzqpa.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.sjlbkw.cn/Article/details/gwyjrldfw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.tarul.cn/Article/details/gdpwxvtfg.sHtML

Java: import java.util.List;
来源：http://mobile.vehdjk.com/Article/details/gcseasefw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.tarul.cn/Article/details/gfnkuncxr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.vehdjk.com/Article/details/gadifomix.sHtML

C#:   using System.Text;
来源：http://blog.sjlbkw.cn/Article/details/grnspjaap.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.epnwcf.com/Article/details/giwlxwslr.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.vehdjk.com/Article/details/gtmjfkibf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fktsv.cn/Article/details/gjfqjemhf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.bbcook.cn/Article/details/gcpbizkak.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.yfazqb.com/Article/details/gadvvtyac.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.yfazqb.com/Article/details/gixsuttuh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fktsv.cn/Article/details/gljzohgxn.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.epnwcf.com/Article/details/gckvkggcn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.bbcook.cn/Article/details/gcjxsamru.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.yfazqb.com/Article/details/giwhjrsuo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.sjlbkw.cn/Article/details/gylsiqzdg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.bbcook.cn/Article/details/ghzjroomt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.yfazqb.com/Article/details/gtujlgvih.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gxhwanvuz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gyhtnpiee.sHtML

Go:   func add(a, b int) int
来源：http://mobile.epnwcf.com/Article/details/giftdmsfs.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.tarul.cn/Article/details/goddgvthc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.vehdjk.com/Article/details/gwjyukrvi.sHtML

[C14] 泛型函数
来源：http://blog.vehdjk.com/Article/details/gsztwusge.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.vehdjk.com/Article/details/gokaesixx.sHtML

PHP:  // 无泛型
来源：http://m.share.yfazqb.com/Article/details/gawiawuga.sHtML

JS:   // 无泛型
来源：http://blog.yfazqb.com/Article/details/gypmzbblr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.vehdjk.com/Article/details/gmeyqcxnd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.epnwcf.com/Article/details/gpfebapeb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.bbcook.cn/Article/details/ghbjpupxd.sHtML

Ruby: # 无泛型
来源：http://blog.fktsv.cn/Article/details/gwxqxxrsc.sHtML


<!-- 参考信息 -->