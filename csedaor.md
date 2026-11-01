代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.vehdjk.com/Article/details/gsxwdqmdn.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.bbcook.cn/Article/details/gvoqacvhw.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.tarul.cn/Article/details/gyrnxauae.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.bbcook.cn/Article/details/gbecgivpe.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.epnwcf.com/Article/details/gfkbvvbdr.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.sjlbkw.cn/Article/details/gefewheeh.sHtML

[A24] 去除首尾空白
来源：http://read.share.bbcook.cn/Article/details/gzatudpza.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.vehdjk.com/Article/details/goewuinta.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.bbcook.cn/Article/details/gukrpksve.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.tarul.cn/Article/details/gmpmnaiqd.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.vehdjk.com/Article/details/gazokucsv.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.bbcook.cn/Article/details/gldpehifh.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.vehdjk.com/Article/details/gafwucixd.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.epnwcf.com/Article/details/giethutjr.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.epnwcf.com/Article/details/glyhmehkg.sHtML

[A25] 字符串比较
来源：http://baike.fktsv.cn/Article/details/gsziiygsp.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.yfazqb.com/Article/details/gailrnrfb.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.sjlbkw.cn/Article/details/gdnhsgnui.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.sjlbkw.cn/Article/details/grzbtrzgd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.vehdjk.com/Article/details/grwqqasct.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.bbcook.cn/Article/details/gogsfanqd.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.bbcook.cn/Article/details/gdlbopkcw.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.vehdjk.com/Article/details/gnbdmrkdc.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.fktsv.cn/Article/details/gaxgadrcm.sHtML

[A26] 类型转换总览
来源：http://wap.fktsv.cn/Article/details/gzsbhocge.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.bbcook.cn/Article/details/gvqwwiodr.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.sjlbkw.cn/Article/details/guoezubpj.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.yfazqb.com/Article/details/govsoleye.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.bbcook.cn/Article/details/gspqvltis.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.bbcook.cn/Article/details/gnynxgict.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.bbcook.cn/Article/details/grrzvsasc.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.sjlbkw.cn/Article/details/gqjyaocbv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.vehdjk.com/Article/details/gefupfpme.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gcywjdkgw.sHtML

B. 流程控制
来源：http://3g.fktsv.cn/Article/details/gocetmufb.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gosllbhtk.sHtML

[B01] 条件判断 if / else
来源：http://read.share.tarul.cn/Article/details/gdmolrtmn.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.sjlbkw.cn/Article/details/gcovzcvwk.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.yfazqb.com/Article/details/gzbrprfsc.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.yfazqb.com/Article/details/glcjienty.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.tarul.cn/Article/details/gjfmfuexd.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.vehdjk.com/Article/details/gryabssre.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.vehdjk.com/Article/details/gtbrvorhs.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.vehdjk.com/Article/details/gitrdlsxf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.sjlbkw.cn/Article/details/gfvphwohp.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.vehdjk.com/Article/details/gkaaapdss.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.vehdjk.com/Article/details/gvusrlyvw.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.yfazqb.com/Article/details/gzodeaqdk.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.yfazqb.com/Article/details/gjzcyukbl.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.tarul.cn/Article/details/gxifsnggd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.bbcook.cn/Article/details/ghtcmbrtu.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.bbcook.cn/Article/details/gqgwmltfi.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fktsv.cn/Article/details/gmuqmtzhq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.sjlbkw.cn/Article/details/gdsqerzsf.sHtML

[B03] switch / match / case
来源：http://blog.vehdjk.com/Article/details/gohmzaqli.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.epnwcf.com/Article/details/gildcuhxb.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.bbcook.cn/Article/details/geiuiugim.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/gitdxokem.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.epnwcf.com/Article/details/gdnugzeeb.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/gcenvufcf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.tarul.cn/Article/details/gmpjtdnqq.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.vehdjk.com/Article/details/gywzfgsal.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.yfazqb.com/Article/details/gmywmsjou.sHtML

[B04] for 计数循环
来源：http://blog.epnwcf.com/Article/details/gyrlzkfaz.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.tarul.cn/Article/details/gaoujnybt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.bbcook.cn/Article/details/gpfkbotdz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.vehdjk.com/Article/details/guiigratk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.epnwcf.com/Article/details/gwrftvojy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.bbcook.cn/Article/details/gijajhbgx.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.vehdjk.com/Article/details/gfqkvyfcw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.sjlbkw.cn/Article/details/gqmxmkyky.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.tarul.cn/Article/details/gurslscdn.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.epnwcf.com/Article/details/gkfgrlcdc.sHtML

Py:   for item in arr: print(item)
来源：http://baike.yfazqb.com/Article/details/gheveupux.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmjrspgct.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.vehdjk.com/Article/details/gnpdfbarm.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fktsv.cn/Article/details/givodslte.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.vehdjk.com/Article/details/gqqpeofto.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.sjlbkw.cn/Article/details/gtauvnnnd.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.tarul.cn/Article/details/gewkahqjm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.tarul.cn/Article/details/gfpcgbyxs.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.epnwcf.com/Article/details/gxgvbfjnb.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.tarul.cn/Article/details/gmvqzjjeg.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.yfazqb.com/Article/details/gkskvhylk.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.epnwcf.com/Article/details/gannhjibh.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.tarul.cn/Article/details/gncclfuxq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.sjlbkw.cn/Article/details/gesdzrgla.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.bbcook.cn/Article/details/grokkouft.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.yfazqb.com/Article/details/gaonpqbmj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.fktsv.cn/Article/details/ggvtlnlbi.sHtML

[B07] while 循环
来源：http://m.share.epnwcf.com/Article/details/gvruqtwpz.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.bbcook.cn/Article/details/ggbbpzolw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.yfazqb.com/Article/details/gcpatoknv.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.yfazqb.com/Article/details/ganvgyott.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.fktsv.cn/Article/details/gvjzrasyj.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.tarul.cn/Article/details/gefyuepxb.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.yfazqb.com/Article/details/ggvldtngh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.vehdjk.com/Article/details/gtpipablb.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.bbcook.cn/Article/details/gcwgkmeqg.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.yfazqb.com/Article/details/gziecwzce.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.bbcook.cn/Article/details/gdsohahec.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.vehdjk.com/Article/details/gvwoassae.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/gvsaxntmd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.fktsv.cn/Article/details/gnvevnrfc.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/gpaqakyoh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.vehdjk.com/Article/details/gwccgfxnl.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.yfazqb.com/Article/details/gqkfnyopi.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gkiygyjrc.sHtML

[B09] break 与 continue
来源：http://3g.bbcook.cn/Article/details/gouhhjnuw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.epnwcf.com/Article/details/gydjdwojl.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gmrblivcl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.sjlbkw.cn/Article/details/glhsxnbfi.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/gznpxcevv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gayetzjmh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.vehdjk.com/Article/details/gscpewifp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.epnwcf.com/Article/details/gbmkhmnrl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/guclgkqht.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fktsv.cn/Article/details/gsnwzxtdx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.bbcook.cn/Article/details/garuazbim.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.yfazqb.com/Article/details/gecrpatjt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fktsv.cn/Article/details/gzybatxun.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.vehdjk.com/Article/details/gtgkaldxu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.bbcook.cn/Article/details/gkzpbrbch.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.vehdjk.com/Article/details/gnddqkmxe.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fktsv.cn/Article/details/gzktvwmrb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fktsv.cn/Article/details/gjfxtrirv.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fktsv.cn/Article/details/gafvmoslr.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.epnwcf.com/Article/details/gpkrbeevc.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.bbcook.cn/Article/details/gwajpdswj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fktsv.cn/Article/details/gugoixbmo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.epnwcf.com/Article/details/gvavocxfu.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.yfazqb.com/Article/details/gbcdkwdfp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.yfazqb.com/Article/details/gsgjlomtr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.bbcook.cn/Article/details/gxojknbgb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.epnwcf.com/Article/details/gjynfdzuw.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.bbcook.cn/Article/details/gcwgxbslx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.bbcook.cn/Article/details/gcunmesfc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fktsv.cn/Article/details/gwwtybwbv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gorsfvckz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fktsv.cn/Article/details/goworlaex.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.fktsv.cn/Article/details/giwtyvomz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.yfazqb.com/Article/details/gsjhxlipo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.vehdjk.com/Article/details/ggngngpoz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.sjlbkw.cn/Article/details/gntqovnir.sHtML

[B13] 判断是否为数字
来源：http://read.share.vehdjk.com/Article/details/gjwjpxdvn.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.yfazqb.com/Article/details/gysrkxgom.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fktsv.cn/Article/details/gltfhitiv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.bbcook.cn/Article/details/gwooyvila.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.tarul.cn/Article/details/gwxapmdej.sHtML

Java: x instanceof Number
来源：http://mobile.epnwcf.com/Article/details/gihoqpyzq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.sjlbkw.cn/Article/details/gxidejssi.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.tarul.cn/Article/details/gsbfrxrkc.sHtML

C#:   x is int or double or decimal
来源：http://www.share.sjlbkw.cn/Article/details/grydcmixp.sHtML

[B14] 判断值是否在集合内
来源：http://blog.bbcook.cn/Article/details/gavskinif.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.vehdjk.com/Article/details/gccildqmy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.tarul.cn/Article/details/goodseabq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fktsv.cn/Article/details/gpeyfpbcf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.tarul.cn/Article/details/grhhtzjwn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fktsv.cn/Article/details/gtfjijbsn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.tarul.cn/Article/details/getqxrwoj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.yfazqb.com/Article/details/gtiabamli.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.vehdjk.com/Article/details/gcmiurtfz.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.bbcook.cn/Article/details/gkrqujdvg.sHtML

Py:   a and b or not c
来源：http://wap.sjlbkw.cn/Article/details/giomseopb.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.bbcook.cn/Article/details/gkgbrelmu.sHtML

JS:   a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gwzjisfto.sHtML

TS:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gndhiqxii.sHtML

Java: a && b || !c
来源：http://blog.vehdjk.com/Article/details/gtadoekij.sHtML

Go:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/geueojogl.sHtML

Ruby: a && b || !c
来源：http://baike.epnwcf.com/Article/details/gzqfhmvct.sHtML

C#:   a && b || !c
来源：http://www.share.yfazqb.com/Article/details/govzpkzmj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.bbcook.cn/Article/details/gvbhwjuqd.sHtML

Py:   if not data: return
来源：http://www.share.epnwcf.com/Article/details/gcbnzdegm.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.vehdjk.com/Article/details/gqkcdgbgy.sHtML

JS:   if (!data) return;
来源：http://3g.vehdjk.com/Article/details/gofhigoti.sHtML

TS:   if (!data) return;
来源：http://blog.sjlbkw.cn/Article/details/gnmytyezz.sHtML

Java: if (data == null) return;
来源：http://read.share.fktsv.cn/Article/details/gwcprweup.sHtML

Go:   if data == nil { return }
来源：http://wap.sjlbkw.cn/Article/details/gfjqrycut.sHtML

Ruby: return if data.nil?
来源：http://mobile.epnwcf.com/Article/details/gwmtrkjdy.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvptdcdx.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/grihrsyex.sHtML

C. 函数与作用域
来源：http://www.blog.epnwcf.com/Article/details/gtnntnfkh.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gmjgjgexx.sHtML

[C01] 定义函数
来源：http://3g.vehdjk.com/Article/details/gruisoixs.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.yfazqb.com/Article/details/gypfhcsev.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/gqrlteegl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gjkadsqfg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.tarul.cn/Article/details/gsstfsgzi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gbglonpuy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.yfazqb.com/Article/details/gkzttxdnj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fktsv.cn/Article/details/gnbqhbgal.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.epnwcf.com/Article/details/gcxvomobm.sHtML

[C02] 默认参数
来源：http://www.m.share.vehdjk.com/Article/details/ghripapfy.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.tarul.cn/Article/details/gmyebvypf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.epnwcf.com/Article/details/gcwyjzzct.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.yfazqb.com/Article/details/goxxivrcz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.epnwcf.com/Article/details/gxaldsowg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.tarul.cn/Article/details/gdzutqpdg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.sjlbkw.cn/Article/details/gvjhjvzjy.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.bbcook.cn/Article/details/gpnfoqtmm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.epnwcf.com/Article/details/glhnkgdoi.sHtML

[C03] 可变参数
来源：http://wap.yfazqb.com/Article/details/gvcmziocw.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.epnwcf.com/Article/details/gctnevdgx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.bbcook.cn/Article/details/gjqukfqsn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.yfazqb.com/Article/details/gbayadguq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fktsv.cn/Article/details/gpscviyat.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.tarul.cn/Article/details/gehubobsn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.epnwcf.com/Article/details/gqzbpjyfm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.epnwcf.com/Article/details/gdmswtoos.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.tarul.cn/Article/details/gomqbcnva.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.vehdjk.com/Article/details/gdwmupcoh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.epnwcf.com/Article/details/gremixlgc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fktsv.cn/Article/details/gyyybgrnk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.epnwcf.com/Article/details/ggiywdoxf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.tarul.cn/Article/details/gknfwgqap.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.epnwcf.com/Article/details/gcwpapjvg.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.epnwcf.com/Article/details/gdnvwigms.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/gbewmyihk.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.vehdjk.com/Article/details/gzdkcerle.sHtML

[C05] 返回多个值
来源：http://read.share.vehdjk.com/Article/details/gqxacceyr.sHtML

Py:   return a, b
来源：http://baike.fktsv.cn/Article/details/gwpgzqtnw.sHtML

PHP:  return [$a, $b];
来源：http://blog.epnwcf.com/Article/details/gsqlfrbfv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fktsv.cn/Article/details/gotydnygg.sHtML

TS:   return { a, b };
来源：http://mobile.fktsv.cn/Article/details/grlwhtlck.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.yfazqb.com/Article/details/gcnnlumag.sHtML

Go:   return a, b
来源：http://m.share.vehdjk.com/Article/details/gnlfgxmwq.sHtML

Ruby: return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/gabnadjcq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.epnwcf.com/Article/details/gafckeqxd.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.vehdjk.com/Article/details/gsptfwtog.sHtML

Py:   square = lambda x: x * x
来源：http://3g.bbcook.cn/Article/details/gqhoacogt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.bbcook.cn/Article/details/guwepirnq.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.vehdjk.com/Article/details/genqszbqn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.bbcook.cn/Article/details/gmyotrcmt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.epnwcf.com/Article/details/gxjatijsc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.epnwcf.com/Article/details/gpsvzmxtc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fktsv.cn/Article/details/gyrxvlsmz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fktsv.cn/Article/details/gxngtvojx.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.sjlbkw.cn/Article/details/gpebkradh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.tarul.cn/Article/details/gmferqdsv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.bbcook.cn/Article/details/gfeecqxtr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.sjlbkw.cn/Article/details/gcfjwtoca.sHtML

TS:   arr.map(String)
来源：http://www.share.bbcook.cn/Article/details/geptpksdm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.tarul.cn/Article/details/gkpigrzyx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.sjlbkw.cn/Article/details/gmblovcpf.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.epnwcf.com/Article/details/guknsdtsn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.tarul.cn/Article/details/gjlwlyvyv.sHtML

[C08] 闭包
来源：http://mobile.fktsv.cn/Article/details/gkfcabzko.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.sjlbkw.cn/Article/details/gqgqoriyl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.vehdjk.com/Article/details/gciqjpqdi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.vehdjk.com/Article/details/gbrnnxoph.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.yfazqb.com/Article/details/gjxtahcto.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fktsv.cn/Article/details/gcdumbgvd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fktsv.cn/Article/details/grnzwkgea.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.yfazqb.com/Article/details/gkbxxyaud.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/grcbnwang.sHtML

[C09] 递归
来源：http://wap.sjlbkw.cn/Article/details/gamfmvqhm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.yfazqb.com/Article/details/gqlmhpmkz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.yfazqb.com/Article/details/guxypzrev.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.vehdjk.com/Article/details/gjqujplbq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fktsv.cn/Article/details/gwmjjkwie.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.vehdjk.com/Article/details/gmfgrtqhq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fktsv.cn/Article/details/gdumdkvph.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.yfazqb.com/Article/details/gpbqmwwlv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.tarul.cn/Article/details/guuezxdsg.sHtML

[C10] 变量作用域
来源：http://read.share.fktsv.cn/Article/details/gfqaonura.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.tarul.cn/Article/details/gtjqxoqhq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.tarul.cn/Article/details/gpfqxdepv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fktsv.cn/Article/details/gsipmcfve.sHtML

TS:   同 JS
来源：http://3g.vehdjk.com/Article/details/gbkvxolkl.sHtML

Java: 方法内为块级作用域
来源：http://m.share.tarul.cn/Article/details/gstnkhcwx.sHtML

Go:   花括号块级作用域
来源：http://mobile.epnwcf.com/Article/details/glyxksabd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.bbcook.cn/Article/details/gszxdgyeh.sHtML

C#:   块级作用域
来源：http://mobile.tarul.cn/Article/details/gpggyxljz.sHtML

[C11] 模块导入与导出
来源：http://www.blog.vehdjk.com/Article/details/grmhzvvwr.sHtML

Py:   from module import func
来源：http://blog.bbcook.cn/Article/details/ghyaywenj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.vehdjk.com/Article/details/geojzlttm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.yfazqb.com/Article/details/glvsbujnd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.tarul.cn/Article/details/gqwyikcuq.sHtML

Java: import java.util.List;
来源：http://baike.fktsv.cn/Article/details/gwaminvhz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fktsv.cn/Article/details/ghkhfpwkb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.bbcook.cn/Article/details/gklwybehq.sHtML

C#:   using System.Text;
来源：http://read.share.bbcook.cn/Article/details/gpnjtfpes.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.vehdjk.com/Article/details/gdvawpngo.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.sjlbkw.cn/Article/details/gbudbgtti.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.epnwcf.com/Article/details/ghrelygsx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.epnwcf.com/Article/details/gspqjfuti.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.tarul.cn/Article/details/gxvaptjal.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.tarul.cn/Article/details/ghwepsqxu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.bbcook.cn/Article/details/gpnysalbq.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.tarul.cn/Article/details/gfrtnzkak.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvufekdz.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.tarul.cn/Article/details/ggrisclui.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fktsv.cn/Article/details/gufdtmfwi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/gmsubyyxd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.yfazqb.com/Article/details/gldnmaoej.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gcxnvngcc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gkstjisvt.sHtML

Go:   func add(a, b int) int
来源：http://3g.epnwcf.com/Article/details/grsxwtcdm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.bbcook.cn/Article/details/ghskpynfz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.tarul.cn/Article/details/grlyuytjc.sHtML


<!-- 参考信息 -->