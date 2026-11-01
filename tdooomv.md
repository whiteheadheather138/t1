代发 wailian999

[A22] 获取字符串长度
来源：http://read.share.tarul.cn/Article/details/gdenpasew.sHtML

Py:   len(s)
来源：http://read.share.epnwcf.com/Article/details/giucxuuqe.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.epnwcf.com/Article/details/gwwjvapeo.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.tarul.cn/Article/details/grpyphfbj.sHtML

TS:   s.length
来源：http://m.share.vehdjk.com/Article/details/gooalgkej.sHtML

Java: s.length()
来源：http://m.share.tarul.cn/Article/details/gqzmuovmj.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.fktsv.cn/Article/details/gnmgwlshh.sHtML

Ruby: s.length
来源：http://blog.bbcook.cn/Article/details/gyobktlma.sHtML

C#:   s.Length
来源：http://blog.vehdjk.com/Article/details/getsruaqt.sHtML

[A23] 大小写转换
来源：http://www.m.share.tarul.cn/Article/details/gdzokracb.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.sjlbkw.cn/Article/details/gmhlzmcmn.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.vehdjk.com/Article/details/gegylvlbk.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.sjlbkw.cn/Article/details/gukfjopdn.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.sjlbkw.cn/Article/details/gfqgryhgi.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.sjlbkw.cn/Article/details/gcxwdmwww.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.tarul.cn/Article/details/gmybkqkar.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.tarul.cn/Article/details/gegeofeyv.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.epnwcf.com/Article/details/gpebcvqri.sHtML

[A24] 去除首尾空白
来源：http://baike.tarul.cn/Article/details/gpreaqwcz.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.tarul.cn/Article/details/grcmypobs.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.fktsv.cn/Article/details/gkihpdtch.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.bbcook.cn/Article/details/gnhxgovej.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.epnwcf.com/Article/details/gzlamdtfv.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.fktsv.cn/Article/details/gdmdrbyvc.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.yfazqb.com/Article/details/gebqkuajy.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.epnwcf.com/Article/details/gpeghuxhm.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.tarul.cn/Article/details/gofzplqvl.sHtML

[A25] 字符串比较
来源：http://blog.sjlbkw.cn/Article/details/gitargbso.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.bbcook.cn/Article/details/goyvmxmyd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.sjlbkw.cn/Article/details/gmzuyqeva.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.vehdjk.com/Article/details/gmsfpqtcc.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.yfazqb.com/Article/details/ghdgukeqo.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.sjlbkw.cn/Article/details/gkkyfdxaa.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.fktsv.cn/Article/details/giflpalfl.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.tarul.cn/Article/details/ghifapchu.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.vehdjk.com/Article/details/ghlgztqxk.sHtML

[A26] 类型转换总览
来源：http://baike.vehdjk.com/Article/details/gtctszkjy.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.tarul.cn/Article/details/ggoajrxzr.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.vehdjk.com/Article/details/gxzlcwprp.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.vehdjk.com/Article/details/gghhosnld.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.vehdjk.com/Article/details/gzuwpuhrd.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.vehdjk.com/Article/details/glcniknzi.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.fktsv.cn/Article/details/godohnvjp.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.tarul.cn/Article/details/gglmxfwip.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.bbcook.cn/Article/details/gyoczlpad.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gezcznrcu.sHtML

B. 流程控制
来源：http://baike.yfazqb.com/Article/details/gtkhnhesh.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/glyponkpl.sHtML

[B01] 条件判断 if / else
来源：http://www.share.fktsv.cn/Article/details/ghqlsvqsb.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.bbcook.cn/Article/details/grhiapdmi.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.yfazqb.com/Article/details/genbocwzs.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.sjlbkw.cn/Article/details/gnhjwvgfd.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.sjlbkw.cn/Article/details/gzntiixke.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.fktsv.cn/Article/details/gjiuvavyc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.vehdjk.com/Article/details/gavrsasur.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.fktsv.cn/Article/details/gdifzbalv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.bbcook.cn/Article/details/gtxyyxrwh.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.bbcook.cn/Article/details/guwlpugxs.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.fktsv.cn/Article/details/gdifbbedm.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.yfazqb.com/Article/details/gcxqwtwpy.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.yfazqb.com/Article/details/gqiaybexa.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.vehdjk.com/Article/details/gchxkndbq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.bbcook.cn/Article/details/gkltqcoro.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.fktsv.cn/Article/details/gxtfznvkb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.tarul.cn/Article/details/gnykrorfi.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.sjlbkw.cn/Article/details/gcejpjemv.sHtML

[B03] switch / match / case
来源：http://mobile.vehdjk.com/Article/details/gtbpajbru.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.vehdjk.com/Article/details/gmgxjqdjx.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.yfazqb.com/Article/details/gyqpqijpy.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.sjlbkw.cn/Article/details/gfhblrxla.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.tarul.cn/Article/details/guqpwxzsl.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/gtqqlosmp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.fktsv.cn/Article/details/gfpdilzsi.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.vehdjk.com/Article/details/gtoctcxtj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.sjlbkw.cn/Article/details/ghrqwlzfb.sHtML

[B04] for 计数循环
来源：http://baike.epnwcf.com/Article/details/gizcxxreo.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.yfazqb.com/Article/details/gcejocdvt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.epnwcf.com/Article/details/guvzacpgb.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.yfazqb.com/Article/details/gkqikngpq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.sjlbkw.cn/Article/details/gojvrdbox.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.epnwcf.com/Article/details/gydvyifbz.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.bbcook.cn/Article/details/gklzelabt.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.epnwcf.com/Article/details/gbakvdthf.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.epnwcf.com/Article/details/gwmsorbvq.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.fktsv.cn/Article/details/gwxjxkuty.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.vehdjk.com/Article/details/gcgmovjsi.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.vehdjk.com/Article/details/gaimfsyji.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.fktsv.cn/Article/details/gjitisxgu.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.tarul.cn/Article/details/gvyrgfbbs.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.yfazqb.com/Article/details/gflcvwhgp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.yfazqb.com/Article/details/gxxxayorw.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.yfazqb.com/Article/details/gbzwsfbor.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.tarul.cn/Article/details/grdbcybbt.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.sjlbkw.cn/Article/details/gvkascrpv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.epnwcf.com/Article/details/gmbdvfwmn.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.bbcook.cn/Article/details/gjvdtjkmt.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.sjlbkw.cn/Article/details/gklxnhbbs.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.epnwcf.com/Article/details/gnfaxzxks.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.yfazqb.com/Article/details/ghycqtwdx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.epnwcf.com/Article/details/giujknpmm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.yfazqb.com/Article/details/gdpgadcnl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.yfazqb.com/Article/details/gmtmfcgdl.sHtML

[B07] while 循环
来源：http://mobile.fktsv.cn/Article/details/gztnwyddh.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.yfazqb.com/Article/details/gpkmcgicx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.epnwcf.com/Article/details/gavwkghmw.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.epnwcf.com/Article/details/gggdjrceh.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/gunfcvbcq.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/gjuxzgiuv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.epnwcf.com/Article/details/gtmwguors.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fktsv.cn/Article/details/ggfczmhei.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.tarul.cn/Article/details/gwnmpwkmz.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.epnwcf.com/Article/details/gcdfkjnda.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.sjlbkw.cn/Article/details/gmuanvirw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.fktsv.cn/Article/details/grwilsdbb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.tarul.cn/Article/details/gbnrdxvzk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gyefyfycw.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gzlwpeymc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.vehdjk.com/Article/details/gusxiuuew.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.fktsv.cn/Article/details/gxfbzelrv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/gutxgoulb.sHtML

[B09] break 与 continue
来源：http://blog.fktsv.cn/Article/details/gesfnlluw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.epnwcf.com/Article/details/ggsmbwlgi.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gfhldmrcl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fktsv.cn/Article/details/glgwrsgtc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/gsusymmwb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/gxwloexne.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.epnwcf.com/Article/details/gzqakahbj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.bbcook.cn/Article/details/gyldzzsvp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/gnbkqugrl.sHtML

[B10] 遍历同时拿索引
来源：http://3g.vehdjk.com/Article/details/gmgzarywm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.sjlbkw.cn/Article/details/gjskhuqth.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.tarul.cn/Article/details/gfhjtvkin.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fktsv.cn/Article/details/gilbnhppx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.vehdjk.com/Article/details/gcumansvo.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.epnwcf.com/Article/details/gytnwcpnn.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.tarul.cn/Article/details/gmqpdmlqk.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.yfazqb.com/Article/details/gihktnulu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.epnwcf.com/Article/details/ggxzesvzx.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.yfazqb.com/Article/details/ghuuhbztd.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.epnwcf.com/Article/details/gjqqtvurf.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.bbcook.cn/Article/details/gwtoqmwav.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.bbcook.cn/Article/details/gknorjkrn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.sjlbkw.cn/Article/details/guefmhevm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gaxzjeivs.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.sjlbkw.cn/Article/details/gmenivyhb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.epnwcf.com/Article/details/gtduykgyu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.bbcook.cn/Article/details/gkvhjaadc.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.epnwcf.com/Article/details/gsqmxpjjs.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.epnwcf.com/Article/details/gsebekzlv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.yfazqb.com/Article/details/gzdipdvkx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.bbcook.cn/Article/details/gvshqsdwn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fktsv.cn/Article/details/gjgddiovd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.epnwcf.com/Article/details/gqlutbflr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.epnwcf.com/Article/details/gdnfiyfhl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.yfazqb.com/Article/details/gwgcnndqj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fktsv.cn/Article/details/gymqgqhwn.sHtML

[B13] 判断是否为数字
来源：http://3g.bbcook.cn/Article/details/gkigvnqxd.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.vehdjk.com/Article/details/gywiiedbz.sHtML

PHP:  is_numeric($x)
来源：http://3g.bbcook.cn/Article/details/gqvtrfkxd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwukticij.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.epnwcf.com/Article/details/gqhhgczaj.sHtML

Java: x instanceof Number
来源：http://m.share.bbcook.cn/Article/details/gnrgsgmsa.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.sjlbkw.cn/Article/details/guihhebik.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.vehdjk.com/Article/details/gihenieep.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.vehdjk.com/Article/details/gfgvxuhgh.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.bbcook.cn/Article/details/gsibfzqix.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.bbcook.cn/Article/details/gtetgqvgh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.bbcook.cn/Article/details/goxrloxlk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.vehdjk.com/Article/details/gkgcgpuwc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.vehdjk.com/Article/details/grvilkzjw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gvrwbiisr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.vehdjk.com/Article/details/gxflyuxvo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.tarul.cn/Article/details/gcolrdcfb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/gjiktcweg.sHtML

[B15] 布尔运算与取反
来源：http://baike.yfazqb.com/Article/details/gmuhmfmxs.sHtML

Py:   a and b or not c
来源：http://mobile.epnwcf.com/Article/details/gcnajdsjg.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fktsv.cn/Article/details/gfkvqqynx.sHtML

JS:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/goicuoott.sHtML

TS:   a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gumsrfark.sHtML

Java: a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gkuuoycql.sHtML

Go:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/grdcbpvni.sHtML

Ruby: a && b || !c
来源：http://www.share.yfazqb.com/Article/details/genxobshj.sHtML

C#:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gudapphra.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fktsv.cn/Article/details/goqedhxfo.sHtML

Py:   if not data: return
来源：http://read.share.tarul.cn/Article/details/gdpudbukr.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.bbcook.cn/Article/details/gdvvkiclt.sHtML

JS:   if (!data) return;
来源：http://www.m.share.sjlbkw.cn/Article/details/gyemykkhh.sHtML

TS:   if (!data) return;
来源：http://www.blog.bbcook.cn/Article/details/gfvwtrset.sHtML

Java: if (data == null) return;
来源：http://baike.yfazqb.com/Article/details/gcrbmutpb.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.bbcook.cn/Article/details/gifpzddcs.sHtML

Ruby: return if data.nil?
来源：http://mobile.tarul.cn/Article/details/ggovaqmhp.sHtML

C#:   if (data == null) return;
来源：http://m.share.epnwcf.com/Article/details/gpjliwpkg.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gebgwdoib.sHtML

C. 函数与作用域
来源：http://baike.epnwcf.com/Article/details/gmvnfauwk.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gtuxsuhns.sHtML

[C01] 定义函数
来源：http://wap.tarul.cn/Article/details/gtjsfncay.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.bbcook.cn/Article/details/gumdubkrk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.epnwcf.com/Article/details/gujgkboyk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/giwokbyky.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/gnujbbyvn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gzrsnpypn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.yfazqb.com/Article/details/gcpydaprg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.epnwcf.com/Article/details/gxmarxjfo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gmdgqbqzp.sHtML

[C02] 默认参数
来源：http://m.share.bbcook.cn/Article/details/gzqmwkjlc.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.yfazqb.com/Article/details/gafdgaiam.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.vehdjk.com/Article/details/goegsrgkr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.vehdjk.com/Article/details/ghrhpoqeu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.vehdjk.com/Article/details/ghhqgmupl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.bbcook.cn/Article/details/gnrngtdoi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.vehdjk.com/Article/details/grxxlzihy.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.bbcook.cn/Article/details/gqsccklov.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fktsv.cn/Article/details/gwcacnhxm.sHtML

[C03] 可变参数
来源：http://www.share.sjlbkw.cn/Article/details/guxejrwfd.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.bbcook.cn/Article/details/gcldnpbqn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.bbcook.cn/Article/details/gdbpwdktu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.vehdjk.com/Article/details/gzgjxkaiz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.vehdjk.com/Article/details/gdbxlcryx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.vehdjk.com/Article/details/gqprtmvxm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.bbcook.cn/Article/details/glmfhhhya.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.yfazqb.com/Article/details/grpzwsykg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.bbcook.cn/Article/details/gfcexyutf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.sjlbkw.cn/Article/details/gwyapqsvn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fktsv.cn/Article/details/gnvunwmxd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fktsv.cn/Article/details/greponqvm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.vehdjk.com/Article/details/glyyhbcza.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.sjlbkw.cn/Article/details/gmetahnsj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.tarul.cn/Article/details/gteixlkft.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.vehdjk.com/Article/details/glrcaxlgq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.tarul.cn/Article/details/gkpijbunb.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.tarul.cn/Article/details/gkuszqyga.sHtML

[C05] 返回多个值
来源：http://www.blog.epnwcf.com/Article/details/grchdswka.sHtML

Py:   return a, b
来源：http://www.share.epnwcf.com/Article/details/gsinyfsne.sHtML

PHP:  return [$a, $b];
来源：http://mobile.sjlbkw.cn/Article/details/gwjmcyeca.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.vehdjk.com/Article/details/gjjuidztc.sHtML

TS:   return { a, b };
来源：http://m.share.bbcook.cn/Article/details/gpmmlqeal.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.yfazqb.com/Article/details/gochsuira.sHtML

Go:   return a, b
来源：http://m.share.vehdjk.com/Article/details/gqcdviqyr.sHtML

Ruby: return a, b
来源：http://www.share.fktsv.cn/Article/details/gdjvepjws.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.bbcook.cn/Article/details/guwhlhtci.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fktsv.cn/Article/details/gjlmnfqnt.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.bbcook.cn/Article/details/gwippxdke.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.tarul.cn/Article/details/gygmbohpr.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fktsv.cn/Article/details/gowvuqbuy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gwqayoxqw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.bbcook.cn/Article/details/gcqauqehe.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.tarul.cn/Article/details/grllbgekc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fktsv.cn/Article/details/gggqguqiz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gauyusuxc.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.epnwcf.com/Article/details/ggpmxvimq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.vehdjk.com/Article/details/gbdpscxee.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.tarul.cn/Article/details/gakvvammz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.sjlbkw.cn/Article/details/grnydwvsh.sHtML

TS:   arr.map(String)
来源：http://blog.epnwcf.com/Article/details/ghnchwvuj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.epnwcf.com/Article/details/gvoigwhnw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.sjlbkw.cn/Article/details/gtyhvtkce.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.yfazqb.com/Article/details/gcbafinyo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.sjlbkw.cn/Article/details/ggnynxebn.sHtML

[C08] 闭包
来源：http://baike.yfazqb.com/Article/details/gbbgecsog.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.yfazqb.com/Article/details/gtznwpcja.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.vehdjk.com/Article/details/gccraxhcn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/gcsnycvbh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.tarul.cn/Article/details/gefxxxljt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.bbcook.cn/Article/details/gvoifnccs.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.vehdjk.com/Article/details/gvkfwsqai.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.vehdjk.com/Article/details/geshxnepu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fktsv.cn/Article/details/gyhgpzpcd.sHtML

[C09] 递归
来源：http://read.share.fktsv.cn/Article/details/godsijvjz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.yfazqb.com/Article/details/gtgidxyol.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.yfazqb.com/Article/details/gawvdrxng.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.epnwcf.com/Article/details/gyywwrqij.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.sjlbkw.cn/Article/details/gjdskbbfj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.bbcook.cn/Article/details/ggqkwwngx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.sjlbkw.cn/Article/details/gndcdkyrx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.sjlbkw.cn/Article/details/gvmrlxyqc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.sjlbkw.cn/Article/details/gyzmkqsix.sHtML

[C10] 变量作用域
来源：http://www.blog.tarul.cn/Article/details/gdrxgysck.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.yfazqb.com/Article/details/gcerimiyx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.vehdjk.com/Article/details/gnkysltcw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.yfazqb.com/Article/details/gupweaamb.sHtML

TS:   同 JS
来源：http://m.share.sjlbkw.cn/Article/details/gjaqxhxgm.sHtML

Java: 方法内为块级作用域
来源：http://mobile.epnwcf.com/Article/details/goerapyme.sHtML

Go:   花括号块级作用域
来源：http://3g.vehdjk.com/Article/details/gtvzkyfri.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.yfazqb.com/Article/details/gumrirutt.sHtML

C#:   块级作用域
来源：http://www.blog.tarul.cn/Article/details/gvwkzozpl.sHtML

[C11] 模块导入与导出
来源：http://m.share.fktsv.cn/Article/details/gcowqdwdl.sHtML

Py:   from module import func
来源：http://www.share.yfazqb.com/Article/details/gegbzcunu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.epnwcf.com/Article/details/gknbixdal.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.sjlbkw.cn/Article/details/gxiogxcqq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.yfazqb.com/Article/details/gqxxfjyyy.sHtML

Java: import java.util.List;
来源：http://blog.epnwcf.com/Article/details/gejafhghb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.yfazqb.com/Article/details/gwehyhxuj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.yfazqb.com/Article/details/gmdrgzbun.sHtML

C#:   using System.Text;
来源：http://3g.sjlbkw.cn/Article/details/gaiprcszt.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.sjlbkw.cn/Article/details/gjhzshyfa.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.vehdjk.com/Article/details/grhrypixj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.vehdjk.com/Article/details/geahwekje.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.vehdjk.com/Article/details/gqmwcgtug.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.yfazqb.com/Article/details/ghywuwuxw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.tarul.cn/Article/details/gavxpqgxd.sHtML


<!-- 参考信息 -->