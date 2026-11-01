代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.bbcook.cn/Article/details/gjgafbgtj.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.yfazqb.com/Article/details/gidheoadb.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.bbcook.cn/Article/details/gbedmzldo.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.epnwcf.com/Article/details/gpjiupplb.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.vehdjk.com/Article/details/ggyzfqunl.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.fktsv.cn/Article/details/grylwvinx.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.epnwcf.com/Article/details/gjxdwdrud.sHtML

[A25] 字符串比较
来源：http://read.share.vehdjk.com/Article/details/gowqxkovq.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.yfazqb.com/Article/details/gqzenzaty.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gthuenxhq.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.bbcook.cn/Article/details/glyahxyro.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.vehdjk.com/Article/details/gnhxgrxkf.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.bbcook.cn/Article/details/gvicnimxq.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.tarul.cn/Article/details/gtwnxbbmp.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.fktsv.cn/Article/details/gcvtrqpse.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.sjlbkw.cn/Article/details/gntqtudei.sHtML

[A26] 类型转换总览
来源：http://wap.sjlbkw.cn/Article/details/grvaznziu.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.sjlbkw.cn/Article/details/gmsskhkum.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fktsv.cn/Article/details/ggnxtumnr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.bbcook.cn/Article/details/geptuabda.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.tarul.cn/Article/details/gqbwfteee.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.yfazqb.com/Article/details/gasejijfd.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.sjlbkw.cn/Article/details/gczardbbl.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.bbcook.cn/Article/details/gjoqheqcg.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.bbcook.cn/Article/details/gbkdyltgx.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ghyvgjxpw.sHtML

B. 流程控制
来源：http://3g.sjlbkw.cn/Article/details/gxatuhfqc.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gtajrcotn.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.tarul.cn/Article/details/ghhhrqnmz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.bbcook.cn/Article/details/gvuyuuazg.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.tarul.cn/Article/details/gokeqxbic.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/gpaseztyw.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.yfazqb.com/Article/details/gfyqwngav.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.epnwcf.com/Article/details/gvpqtatel.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.bbcook.cn/Article/details/gpuaukfaq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.yfazqb.com/Article/details/gyerdycvk.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.tarul.cn/Article/details/gsxmhepfh.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.bbcook.cn/Article/details/geldhwhdd.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.bbcook.cn/Article/details/gisbpcpxb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.epnwcf.com/Article/details/gnbzsedvu.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fktsv.cn/Article/details/gspmfbcvp.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.sjlbkw.cn/Article/details/gbmuocacv.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.vehdjk.com/Article/details/ghrtpmvyn.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.fktsv.cn/Article/details/gjmdtzbtr.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.sjlbkw.cn/Article/details/ghypdhslz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.epnwcf.com/Article/details/gdxuaoohk.sHtML

[B03] switch / match / case
来源：http://www.share.fktsv.cn/Article/details/gxjvbwylp.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.fktsv.cn/Article/details/grazzffur.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.fktsv.cn/Article/details/gprhtwzaw.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/gwenyprrk.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/gcmfhtdtt.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.vehdjk.com/Article/details/gymjjjapv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.fktsv.cn/Article/details/gqcknxoyl.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.epnwcf.com/Article/details/gxfnynomt.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.sjlbkw.cn/Article/details/ghqloakpj.sHtML

[B04] for 计数循环
来源：http://www.blog.sjlbkw.cn/Article/details/gwdmwdjdf.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.vehdjk.com/Article/details/gsnbqvewm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.sjlbkw.cn/Article/details/gcqtprgkm.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fktsv.cn/Article/details/grsnxecbp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.tarul.cn/Article/details/gwsflqhza.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fktsv.cn/Article/details/gnsraunya.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.tarul.cn/Article/details/gpojtehie.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.bbcook.cn/Article/details/gnpqkgydw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.tarul.cn/Article/details/gplurgcid.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.tarul.cn/Article/details/gyvfqnakp.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.tarul.cn/Article/details/glozxdedq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.vehdjk.com/Article/details/geqzxuesk.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fktsv.cn/Article/details/ginotbyaf.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.sjlbkw.cn/Article/details/gcmxrgyoq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.fktsv.cn/Article/details/gvxgjgdnd.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.epnwcf.com/Article/details/gzzwouspe.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.sjlbkw.cn/Article/details/gnvymabqr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.yfazqb.com/Article/details/gopfxpsdg.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fktsv.cn/Article/details/gaokafveq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.bbcook.cn/Article/details/gnxfvdbus.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fktsv.cn/Article/details/gcccsjfmb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.sjlbkw.cn/Article/details/gputgmvhx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.bbcook.cn/Article/details/gvfsfqere.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.bbcook.cn/Article/details/gugkdkmpv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.vehdjk.com/Article/details/grrckdpfl.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.fktsv.cn/Article/details/gtndsuylk.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fktsv.cn/Article/details/gmzggfceb.sHtML

[B07] while 循环
来源：http://blog.yfazqb.com/Article/details/gsmzhreed.sHtML

Py:   while i < 10: i += 1
来源：http://blog.epnwcf.com/Article/details/ghqsnzknj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.epnwcf.com/Article/details/gvommwcuc.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/grxalbdpy.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.epnwcf.com/Article/details/gbzleopnz.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/gurbomarn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fktsv.cn/Article/details/gdbedzvra.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.tarul.cn/Article/details/gtryqthmd.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.epnwcf.com/Article/details/gjgkujnan.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fktsv.cn/Article/details/grrhxqwnh.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.vehdjk.com/Article/details/gxnjzzpik.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.epnwcf.com/Article/details/gyanmeusp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fktsv.cn/Article/details/gqumgwaxg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.sjlbkw.cn/Article/details/gsnumjegi.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fktsv.cn/Article/details/gbpvkjudn.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.tarul.cn/Article/details/ggsonrpmu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.epnwcf.com/Article/details/gwmodymnb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gtozmnfkf.sHtML

[B09] break 与 continue
来源：http://read.share.tarul.cn/Article/details/gkmqlxzwh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.vehdjk.com/Article/details/gmeksvwxc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/gxxryuqva.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/gfexmxszy.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/gbmsusoan.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.bbcook.cn/Article/details/gosrwcpsf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.tarul.cn/Article/details/gthkqdael.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.fktsv.cn/Article/details/gbugwotbg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gyujkayqh.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.yfazqb.com/Article/details/ggvmvwxwq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.sjlbkw.cn/Article/details/gsaekdryv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.epnwcf.com/Article/details/gwihlougv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.sjlbkw.cn/Article/details/gvtsjizco.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.vehdjk.com/Article/details/gnaraalzb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.bbcook.cn/Article/details/gijkuxslv.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.vehdjk.com/Article/details/gxkscyrsz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.epnwcf.com/Article/details/gznuhjqch.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.bbcook.cn/Article/details/gfajywgdc.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.yfazqb.com/Article/details/grbrjivtv.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.sjlbkw.cn/Article/details/gotcurnwp.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.bbcook.cn/Article/details/glgbzudmz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fktsv.cn/Article/details/gostcrdxm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.vehdjk.com/Article/details/gjqdwbiky.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.sjlbkw.cn/Article/details/gzoiwvddq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.vehdjk.com/Article/details/guvfsrqtu.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.epnwcf.com/Article/details/gsspkqvxb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fktsv.cn/Article/details/gwuxtpcih.sHtML

[B12] 跳出多层循环
来源：http://m.share.fktsv.cn/Article/details/gasdefivh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.sjlbkw.cn/Article/details/gysdllhnv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.tarul.cn/Article/details/gecmrnknn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fktsv.cn/Article/details/gqggerghz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fktsv.cn/Article/details/gcfpshviu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.bbcook.cn/Article/details/gahwbhmrh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.vehdjk.com/Article/details/gnzgldatn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.yfazqb.com/Article/details/gkhasmhpi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fktsv.cn/Article/details/gvvpmzmwe.sHtML

[B13] 判断是否为数字
来源：http://mobile.bbcook.cn/Article/details/gjkvicuiu.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.vehdjk.com/Article/details/gfpellwlz.sHtML

PHP:  is_numeric($x)
来源：http://read.share.sjlbkw.cn/Article/details/gmzwsyqzc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fktsv.cn/Article/details/gzxbmmfld.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.sjlbkw.cn/Article/details/gvdootxvh.sHtML

Java: x instanceof Number
来源：http://www.m.share.sjlbkw.cn/Article/details/gzzlsxvob.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.yfazqb.com/Article/details/glmicolna.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.vehdjk.com/Article/details/gylpfphvg.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fktsv.cn/Article/details/geniwfvbj.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.sjlbkw.cn/Article/details/gqrvwikds.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.sjlbkw.cn/Article/details/ghwmhpdzt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fktsv.cn/Article/details/giywnhlsc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.fktsv.cn/Article/details/gusesrefo.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.vehdjk.com/Article/details/gtpdkbyjx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.vehdjk.com/Article/details/giqwfqxvp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.epnwcf.com/Article/details/guisateyv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fktsv.cn/Article/details/gvxwnhjsi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.vehdjk.com/Article/details/gyopfqmel.sHtML

[B15] 布尔运算与取反
来源：http://mobile.yfazqb.com/Article/details/grtdwugnr.sHtML

Py:   a and b or not c
来源：http://blog.bbcook.cn/Article/details/glcczcjsv.sHtML

PHP:  $a && $b || !$c
来源：http://wap.vehdjk.com/Article/details/gxsaladyc.sHtML

JS:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gktkyqhyh.sHtML

TS:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gqfnaluev.sHtML

Java: a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gcdznipuc.sHtML

Go:   a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/glowrrqqk.sHtML

Ruby: a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gltfqvtji.sHtML

C#:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gqvrcjjch.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gewlzlnob.sHtML

Py:   if not data: return
来源：http://mobile.tarul.cn/Article/details/ggsneadah.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.epnwcf.com/Article/details/gkykwlzud.sHtML

JS:   if (!data) return;
来源：http://read.share.vehdjk.com/Article/details/gutaxjcir.sHtML

TS:   if (!data) return;
来源：http://wap.tarul.cn/Article/details/gveukcpbm.sHtML

Java: if (data == null) return;
来源：http://mobile.tarul.cn/Article/details/gksqxksar.sHtML

Go:   if data == nil { return }
来源：http://3g.sjlbkw.cn/Article/details/goelbldhs.sHtML

Ruby: return if data.nil?
来源：http://wap.yfazqb.com/Article/details/ghmvekvkl.sHtML

C#:   if (data == null) return;
来源：http://www.blog.tarul.cn/Article/details/gbhxluqzj.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gygkbnnev.sHtML

C. 函数与作用域
来源：http://m.share.yfazqb.com/Article/details/gaqboknai.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gndgmpswf.sHtML

[C01] 定义函数
来源：http://3g.sjlbkw.cn/Article/details/gmvagugai.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fktsv.cn/Article/details/gciylwjit.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/gimwvjgba.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/golpujlyl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gogmkdtfa.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/gcikfclst.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.epnwcf.com/Article/details/ghenbcciy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.vehdjk.com/Article/details/gjlgxyibr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/ggsbyxtdx.sHtML

[C02] 默认参数
来源：http://mobile.epnwcf.com/Article/details/gdgwvdgec.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fktsv.cn/Article/details/gbdkrlvbz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.bbcook.cn/Article/details/gnmpxaotb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.bbcook.cn/Article/details/glonjpwwd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.epnwcf.com/Article/details/gjbvooqyi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.bbcook.cn/Article/details/grkiupimb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fktsv.cn/Article/details/gzmsfkmog.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.epnwcf.com/Article/details/ghicaczdz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.sjlbkw.cn/Article/details/gtjsmmtje.sHtML

[C03] 可变参数
来源：http://baike.yfazqb.com/Article/details/gqxlabimp.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.bbcook.cn/Article/details/gkftoxnwh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.tarul.cn/Article/details/gogrmeeie.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.epnwcf.com/Article/details/grqfyhfeo.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fktsv.cn/Article/details/gljjdfvms.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.bbcook.cn/Article/details/gqechfxsz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.bbcook.cn/Article/details/gwrvrsxbs.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.vehdjk.com/Article/details/grrafmthu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.tarul.cn/Article/details/gojfwcnre.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fktsv.cn/Article/details/grzcdplky.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.vehdjk.com/Article/details/gvexeaugc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.epnwcf.com/Article/details/gjlfbolup.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fktsv.cn/Article/details/gvjdawvgy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.sjlbkw.cn/Article/details/grqwfrepb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.yfazqb.com/Article/details/gfanyjetk.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fktsv.cn/Article/details/goaebgyyc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.tarul.cn/Article/details/gtztbkfzs.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/gqgplqviz.sHtML

[C05] 返回多个值
来源：http://www.m.share.yfazqb.com/Article/details/gvomimkrz.sHtML

Py:   return a, b
来源：http://mobile.fktsv.cn/Article/details/gycspytzz.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.tarul.cn/Article/details/gaeocgmlk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.bbcook.cn/Article/details/ginsbopxg.sHtML

TS:   return { a, b };
来源：http://blog.yfazqb.com/Article/details/gprpoxpnf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.sjlbkw.cn/Article/details/gatbrjooy.sHtML

Go:   return a, b
来源：http://www.m.share.fktsv.cn/Article/details/gzrpjkkkh.sHtML

Ruby: return a, b
来源：http://www.share.fktsv.cn/Article/details/geztncllf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.epnwcf.com/Article/details/gnmxuxbae.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.tarul.cn/Article/details/gcndlankj.sHtML

Py:   square = lambda x: x * x
来源：http://3g.epnwcf.com/Article/details/gieogdjfj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.sjlbkw.cn/Article/details/guavqnuiz.sHtML

JS:   const square = x => x * x;
来源：http://www.share.tarul.cn/Article/details/gmcmdmecl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gygmlemlb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.vehdjk.com/Article/details/gkaszukkm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.yfazqb.com/Article/details/gshyeypvg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fktsv.cn/Article/details/gmlsoblod.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.tarul.cn/Article/details/gbzvpudcq.sHtML

[C07] 把函数作为参数传入
来源：http://blog.epnwcf.com/Article/details/ghpzuymnz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.sjlbkw.cn/Article/details/gnmlnddpd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.tarul.cn/Article/details/gxifyodwm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.bbcook.cn/Article/details/godaqnaxp.sHtML

TS:   arr.map(String)
来源：http://blog.fktsv.cn/Article/details/gybygtscz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.tarul.cn/Article/details/gwfjaoncb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.bbcook.cn/Article/details/gxdbqqivg.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.epnwcf.com/Article/details/gbrrsoxug.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.vehdjk.com/Article/details/gkafgakrs.sHtML

[C08] 闭包
来源：http://m.share.yfazqb.com/Article/details/gjyaysjhe.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.bbcook.cn/Article/details/gnnioxmii.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.epnwcf.com/Article/details/giwstgiac.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fktsv.cn/Article/details/gjtuglbot.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fktsv.cn/Article/details/gqufyzbxb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.bbcook.cn/Article/details/ginkksbec.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.tarul.cn/Article/details/gqlmpnsrv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.bbcook.cn/Article/details/gghwqelme.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.epnwcf.com/Article/details/gizrgzdci.sHtML

[C09] 递归
来源：http://www.blog.fktsv.cn/Article/details/ggzlneexd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.tarul.cn/Article/details/gtpugqcaw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fktsv.cn/Article/details/gfbjxnlrx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.tarul.cn/Article/details/gfduwesvt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.sjlbkw.cn/Article/details/gvczmxyee.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.yfazqb.com/Article/details/grvmskvql.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.bbcook.cn/Article/details/gpiaqwrda.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.vehdjk.com/Article/details/gkyfxggii.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.sjlbkw.cn/Article/details/gwmzhpwwu.sHtML

[C10] 变量作用域
来源：http://www.share.fktsv.cn/Article/details/gpqoiapgl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.tarul.cn/Article/details/gfnvjusyp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.bbcook.cn/Article/details/gxpemmaor.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.yfazqb.com/Article/details/glztghfre.sHtML

TS:   同 JS
来源：http://blog.yfazqb.com/Article/details/gudobvbxt.sHtML

Java: 方法内为块级作用域
来源：http://3g.sjlbkw.cn/Article/details/guvvrgaae.sHtML

Go:   花括号块级作用域
来源：http://m.share.sjlbkw.cn/Article/details/gkldgymbw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.vehdjk.com/Article/details/gemtgygmy.sHtML

C#:   块级作用域
来源：http://m.share.vehdjk.com/Article/details/gtyqjzhwp.sHtML

[C11] 模块导入与导出
来源：http://wap.epnwcf.com/Article/details/ghnocpxdi.sHtML

Py:   from module import func
来源：http://mobile.vehdjk.com/Article/details/gikmhgcko.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.sjlbkw.cn/Article/details/guvpesjhs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.tarul.cn/Article/details/gtsapfyaq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.vehdjk.com/Article/details/gtitunpoc.sHtML

Java: import java.util.List;
来源：http://m.share.bbcook.cn/Article/details/gbkwutxqv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.sjlbkw.cn/Article/details/gtqnenwdl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.vehdjk.com/Article/details/gzlgxigwa.sHtML

C#:   using System.Text;
来源：http://wap.tarul.cn/Article/details/gmjyraqup.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.tarul.cn/Article/details/gxpotxfee.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fktsv.cn/Article/details/gsvsvwxgy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.epnwcf.com/Article/details/gnargpokp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.tarul.cn/Article/details/ggtuwrkpk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.tarul.cn/Article/details/gswhjpypb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.epnwcf.com/Article/details/gmlfryzgl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.bbcook.cn/Article/details/gxwiktahd.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.yfazqb.com/Article/details/glyigztap.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.sjlbkw.cn/Article/details/gkaaknkzj.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.yfazqb.com/Article/details/gfalllyqu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.yfazqb.com/Article/details/gywbnravm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/grkwqxetw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fktsv.cn/Article/details/gcaerdqjt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gszvsdlis.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gmwbnookk.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fktsv.cn/Article/details/grnsyekdk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.tarul.cn/Article/details/ghnmetnbp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.vehdjk.com/Article/details/guyhpuefr.sHtML

[C14] 泛型函数
来源：http://mobile.tarul.cn/Article/details/gcabwqvqt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fktsv.cn/Article/details/gbxexbpuo.sHtML

PHP:  // 无泛型
来源：http://www.blog.bbcook.cn/Article/details/gojeipbfe.sHtML

JS:   // 无泛型
来源：http://blog.vehdjk.com/Article/details/gbaweylqo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.epnwcf.com/Article/details/gllwnnuyk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.vehdjk.com/Article/details/gdoxsgcsv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.bbcook.cn/Article/details/gubjkncif.sHtML

Ruby: # 无泛型
来源：http://m.share.vehdjk.com/Article/details/gxatwcvmt.sHtML


<!-- 参考信息 -->