代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.vehdjk.com/Article/details/gmthpsdnq.sHtML

Ruby: gets.chomp
来源：http://mobile.vehdjk.com/Article/details/gpuwqemlu.sHtML

C#:   Console.ReadLine();
来源：http://mobile.tarul.cn/Article/details/gtxqtebjo.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.yfazqb.com/Article/details/gdjmufivc.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.fktsv.cn/Article/details/gnefkkrmc.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.yfazqb.com/Article/details/gxmzkcbzw.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.vehdjk.com/Article/details/gknvvsljv.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.bbcook.cn/Article/details/gasnmwkwy.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.vehdjk.com/Article/details/gtggtnbzn.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.epnwcf.com/Article/details/ggeriexzx.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.epnwcf.com/Article/details/gqwqhrjsl.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.yfazqb.com/Article/details/gkohgoyts.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.bbcook.cn/Article/details/gymgbutei.sHtML

Py:   len(s)
来源：http://3g.vehdjk.com/Article/details/gwtqosmml.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.tarul.cn/Article/details/givovdqlm.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.vehdjk.com/Article/details/gcivjxoak.sHtML

TS:   s.length
来源：http://www.share.fktsv.cn/Article/details/gfeadirud.sHtML

Java: s.length()
来源：http://mobile.epnwcf.com/Article/details/gsjzoyuoj.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.sjlbkw.cn/Article/details/gjmsbvinf.sHtML

Ruby: s.length
来源：http://www.m.share.yfazqb.com/Article/details/gzxqykpqb.sHtML

C#:   s.Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmupghnw.sHtML

[A23] 大小写转换
来源：http://m.share.yfazqb.com/Article/details/gbdbyqrmn.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.sjlbkw.cn/Article/details/gasfmbsac.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gabhaalkj.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.vehdjk.com/Article/details/gjkrbgccz.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fktsv.cn/Article/details/gdauxevdu.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.epnwcf.com/Article/details/gmmuulivt.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.yfazqb.com/Article/details/gvpomfsgh.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.vehdjk.com/Article/details/gzlefbnsr.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.tarul.cn/Article/details/gugjfryxy.sHtML

[A24] 去除首尾空白
来源：http://wap.fktsv.cn/Article/details/ghbgyzcvf.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.vehdjk.com/Article/details/gaznjsguw.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.tarul.cn/Article/details/gsqafyxfs.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fktsv.cn/Article/details/gzwbgqsqm.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fktsv.cn/Article/details/gvtintcly.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.bbcook.cn/Article/details/grhwiawlb.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.tarul.cn/Article/details/gavnwukhw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.epnwcf.com/Article/details/gsvrewcrb.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.yfazqb.com/Article/details/gwoverchh.sHtML

[A25] 字符串比较
来源：http://read.share.epnwcf.com/Article/details/gewfivckn.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.tarul.cn/Article/details/gbjbqhmeu.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.fktsv.cn/Article/details/gjvarrqav.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.tarul.cn/Article/details/gyretrorb.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.sjlbkw.cn/Article/details/gqiddurcm.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.vehdjk.com/Article/details/gjzgasdqw.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.bbcook.cn/Article/details/gsyaompjq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.sjlbkw.cn/Article/details/gycdlmqtq.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.yfazqb.com/Article/details/geksgitmi.sHtML

[A26] 类型转换总览
来源：http://3g.sjlbkw.cn/Article/details/gleflbjbv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.sjlbkw.cn/Article/details/gvcyepvex.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.vehdjk.com/Article/details/grkcvvlya.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.bbcook.cn/Article/details/gidzyxebd.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.epnwcf.com/Article/details/ggkkdlpxv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.fktsv.cn/Article/details/gqmsbffxu.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.fktsv.cn/Article/details/grwqwpbjq.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.tarul.cn/Article/details/gzupufdvv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.bbcook.cn/Article/details/gomgjyhrn.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/guyulcjaj.sHtML

B. 流程控制
来源：http://mobile.epnwcf.com/Article/details/gaslxozfx.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gdqvaefaj.sHtML

[B01] 条件判断 if / else
来源：http://mobile.epnwcf.com/Article/details/glmsottdj.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.bbcook.cn/Article/details/gtsinoqvo.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.sjlbkw.cn/Article/details/geqbsymjx.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.epnwcf.com/Article/details/gnetbbzgu.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.vehdjk.com/Article/details/ghhocqlmb.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/gqpntkmho.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.bbcook.cn/Article/details/gloqhmdrf.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.epnwcf.com/Article/details/gtjdoilth.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.bbcook.cn/Article/details/ggtqqzjfs.sHtML

[B02] 多分支 else if / elif
来源：http://wap.yfazqb.com/Article/details/gxikdwbax.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.yfazqb.com/Article/details/gyvskkcvk.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.fktsv.cn/Article/details/gibwifzky.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.tarul.cn/Article/details/gfgrfzufd.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.tarul.cn/Article/details/gayrxlvne.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fktsv.cn/Article/details/gdaapogge.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.vehdjk.com/Article/details/goumfnnce.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.fktsv.cn/Article/details/gthhayeft.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.sjlbkw.cn/Article/details/gwcyixest.sHtML

[B03] switch / match / case
来源：http://blog.fktsv.cn/Article/details/gpisisaea.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.epnwcf.com/Article/details/gfwauutyp.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.vehdjk.com/Article/details/gclebocld.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/gvrwjidoo.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.yfazqb.com/Article/details/giczsyfqb.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.sjlbkw.cn/Article/details/grckodpxp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.tarul.cn/Article/details/grsrutwyn.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.bbcook.cn/Article/details/gbtwldywt.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.sjlbkw.cn/Article/details/gjavglwvz.sHtML

[B04] for 计数循环
来源：http://blog.sjlbkw.cn/Article/details/gbkhemwsc.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.fktsv.cn/Article/details/gypmsohjl.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.vehdjk.com/Article/details/glhwpdovv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.vehdjk.com/Article/details/gtyyuwamg.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.epnwcf.com/Article/details/gecbvirjg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.vehdjk.com/Article/details/gdpodwhhi.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.tarul.cn/Article/details/gxzniwdbl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.fktsv.cn/Article/details/guiizexcx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.vehdjk.com/Article/details/ghkzwrfgg.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.tarul.cn/Article/details/gcvxpngwx.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.sjlbkw.cn/Article/details/grryqijye.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fktsv.cn/Article/details/gvravqofs.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.yfazqb.com/Article/details/gccacgcnb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fktsv.cn/Article/details/gysyaymbd.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.sjlbkw.cn/Article/details/gmvqpzost.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.fktsv.cn/Article/details/gnyyekxzz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.vehdjk.com/Article/details/gijpwnaoo.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.tarul.cn/Article/details/gscfronav.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.epnwcf.com/Article/details/giwlcgixt.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.yfazqb.com/Article/details/gjbnsiuaw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gspnndome.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.sjlbkw.cn/Article/details/gmsgyjkpf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.yfazqb.com/Article/details/gueojdmka.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.epnwcf.com/Article/details/gaicoifea.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.tarul.cn/Article/details/groahxwof.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.vehdjk.com/Article/details/grhvqyyol.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.epnwcf.com/Article/details/gdshoaowy.sHtML

[B07] while 循环
来源：http://www.share.bbcook.cn/Article/details/gitcndtex.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.sjlbkw.cn/Article/details/gemkqlwlf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gzrqbjvuk.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/grfkwxbbu.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.vehdjk.com/Article/details/ggevturmr.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.vehdjk.com/Article/details/gzmthbzab.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fktsv.cn/Article/details/gqerbikyh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.bbcook.cn/Article/details/gjueqqmcm.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.bbcook.cn/Article/details/glyjuuytm.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.sjlbkw.cn/Article/details/gnffoxtqi.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.sjlbkw.cn/Article/details/gdpirkvhs.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.vehdjk.com/Article/details/gskvvhdwu.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gowkphqcp.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.yfazqb.com/Article/details/gjwnebvgx.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gacypvnht.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.tarul.cn/Article/details/gughuwlhb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fktsv.cn/Article/details/gkswrewxx.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.tarul.cn/Article/details/gxhhyrkvl.sHtML

[B09] break 与 continue
来源：http://wap.yfazqb.com/Article/details/gbavdvzkg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.tarul.cn/Article/details/gcqyntxqt.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gcyoadhly.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gwbahlukj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/gpramepiy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.tarul.cn/Article/details/gcayuigqi.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.sjlbkw.cn/Article/details/gmpewzvoq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.bbcook.cn/Article/details/gpgzchgzm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/goxauddcc.sHtML

[B10] 遍历同时拿索引
来源：http://3g.yfazqb.com/Article/details/gyomjxjvs.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnbvrggk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.tarul.cn/Article/details/gftgcervn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fktsv.cn/Article/details/gggjemovc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.yfazqb.com/Article/details/gmejixoep.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.yfazqb.com/Article/details/gqnxlbkzu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.epnwcf.com/Article/details/gkchysdtu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.sjlbkw.cn/Article/details/gkvrvnhct.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.epnwcf.com/Article/details/gnuwvniwy.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.bbcook.cn/Article/details/gxqyfnsyd.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.vehdjk.com/Article/details/gzzckajir.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.tarul.cn/Article/details/gzjzwjqav.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.epnwcf.com/Article/details/gzfqsuvpa.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.tarul.cn/Article/details/gqwsfvwzk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.sjlbkw.cn/Article/details/gauigoaic.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.bbcook.cn/Article/details/gzujdzlfu.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.sjlbkw.cn/Article/details/gwrllncjv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.tarul.cn/Article/details/gsdzkwviw.sHtML

[B12] 跳出多层循环
来源：http://3g.tarul.cn/Article/details/gjxdxnckx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.epnwcf.com/Article/details/grojysewb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.tarul.cn/Article/details/ggetmzahm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/gwqwaacfu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fktsv.cn/Article/details/goixyrivu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/gnhubxhkh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.vehdjk.com/Article/details/gpguttbhi.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.vehdjk.com/Article/details/gfpubliqt.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.vehdjk.com/Article/details/gwarmtkad.sHtML

[B13] 判断是否为数字
来源：http://m.share.bbcook.cn/Article/details/gptazetso.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.sjlbkw.cn/Article/details/gbknoycyx.sHtML

PHP:  is_numeric($x)
来源：http://www.share.bbcook.cn/Article/details/gerfyqsyv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.yfazqb.com/Article/details/gfigtbreo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.yfazqb.com/Article/details/grfflbzdk.sHtML

Java: x instanceof Number
来源：http://www.blog.vehdjk.com/Article/details/gzxuazrdw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.vehdjk.com/Article/details/guhabyiyk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.epnwcf.com/Article/details/ggivutsqh.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.bbcook.cn/Article/details/gxiyoghkm.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.tarul.cn/Article/details/gwycxgwwm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.tarul.cn/Article/details/gdwtqgjaz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fktsv.cn/Article/details/gjjdfztpu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.vehdjk.com/Article/details/geenhrsmv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/gjegnpnon.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gbkurgzqv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.bbcook.cn/Article/details/ghnakugvl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.bbcook.cn/Article/details/gbokdihcy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/gvmgzasiy.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fktsv.cn/Article/details/gvmsgdwlz.sHtML

Py:   a and b or not c
来源：http://3g.sjlbkw.cn/Article/details/gweyjsbam.sHtML

PHP:  $a && $b || !$c
来源：http://baike.yfazqb.com/Article/details/gzxqbwtwf.sHtML

JS:   a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gehxsjplo.sHtML

TS:   a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gdwgqdtya.sHtML

Java: a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gdcgameyc.sHtML

Go:   a && b || !c
来源：http://www.blog.fktsv.cn/Article/details/geihmqgkq.sHtML

Ruby: a && b || !c
来源：http://blog.fktsv.cn/Article/details/gnqxekbct.sHtML

C#:   a && b || !c
来源：http://3g.epnwcf.com/Article/details/gvgcwbrto.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.vehdjk.com/Article/details/glgqbryuv.sHtML

Py:   if not data: return
来源：http://m.share.tarul.cn/Article/details/gzayzfdpa.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fktsv.cn/Article/details/ggvnzzlaq.sHtML

JS:   if (!data) return;
来源：http://baike.yfazqb.com/Article/details/gexrwxkis.sHtML

TS:   if (!data) return;
来源：http://wap.vehdjk.com/Article/details/gzyyijxhb.sHtML

Java: if (data == null) return;
来源：http://baike.epnwcf.com/Article/details/gvhsbmkxj.sHtML

Go:   if data == nil { return }
来源：http://baike.tarul.cn/Article/details/gqmneedie.sHtML

Ruby: return if data.nil?
来源：http://mobile.yfazqb.com/Article/details/gsixoreja.sHtML

C#:   if (data == null) return;
来源：http://www.blog.sjlbkw.cn/Article/details/gdjqbtdsb.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gzhfkplmm.sHtML

C. 函数与作用域
来源：http://www.blog.tarul.cn/Article/details/gqcyslexg.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gvpltwbbb.sHtML

[C01] 定义函数
来源：http://www.blog.epnwcf.com/Article/details/goajenwjh.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.yfazqb.com/Article/details/gkgnwuqjg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/glkqsrxjw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/girilkvqm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gubugejrn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/glyqbdjmj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.bbcook.cn/Article/details/grnaxolrm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.vehdjk.com/Article/details/gphafvlha.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gnobijfvw.sHtML

[C02] 默认参数
来源：http://www.share.epnwcf.com/Article/details/gggxnqwqa.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fktsv.cn/Article/details/gvizssltc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fktsv.cn/Article/details/glopmycof.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.epnwcf.com/Article/details/gegejyovf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.epnwcf.com/Article/details/ghrarxmtx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.tarul.cn/Article/details/gxihceiws.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.bbcook.cn/Article/details/gosgwfkur.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.epnwcf.com/Article/details/gamtilwzm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.sjlbkw.cn/Article/details/gekjcdqfx.sHtML

[C03] 可变参数
来源：http://blog.sjlbkw.cn/Article/details/gjrhjqcpl.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fktsv.cn/Article/details/gbmshywls.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.bbcook.cn/Article/details/glaqjewkk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.vehdjk.com/Article/details/gkqlitbyc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.sjlbkw.cn/Article/details/gmrsfpkgc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.tarul.cn/Article/details/gvvtguypw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.vehdjk.com/Article/details/gntthsdhx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.epnwcf.com/Article/details/gvcialday.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.sjlbkw.cn/Article/details/glaqsuoff.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.bbcook.cn/Article/details/gbvkclure.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.vehdjk.com/Article/details/gqepkkxzn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.bbcook.cn/Article/details/gfgjjstlo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.vehdjk.com/Article/details/grnldtrjc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fktsv.cn/Article/details/gkzhsflel.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.epnwcf.com/Article/details/glsapvgqm.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.vehdjk.com/Article/details/grwyjluqo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.yfazqb.com/Article/details/ghhzqyfun.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fktsv.cn/Article/details/ghzgcdyss.sHtML

[C05] 返回多个值
来源：http://www.m.share.fktsv.cn/Article/details/gqanrgwef.sHtML

Py:   return a, b
来源：http://read.share.fktsv.cn/Article/details/gjhohbrow.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.epnwcf.com/Article/details/gqsjrxczo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.vehdjk.com/Article/details/gxyhshqcd.sHtML

TS:   return { a, b };
来源：http://www.m.share.vehdjk.com/Article/details/guonbiwut.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fktsv.cn/Article/details/gogliewbk.sHtML

Go:   return a, b
来源：http://wap.tarul.cn/Article/details/glnltejyp.sHtML

Ruby: return a, b
来源：http://www.m.share.epnwcf.com/Article/details/goieywgae.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.tarul.cn/Article/details/gcvpmziyo.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.tarul.cn/Article/details/gainkbpvc.sHtML

Py:   square = lambda x: x * x
来源：http://3g.sjlbkw.cn/Article/details/gfkmypoch.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.vehdjk.com/Article/details/gazoqccqu.sHtML

JS:   const square = x => x * x;
来源：http://baike.sjlbkw.cn/Article/details/gpvzxulfg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.vehdjk.com/Article/details/gkwknqxzb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.sjlbkw.cn/Article/details/gluidlnlm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.tarul.cn/Article/details/gplzzckwy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.tarul.cn/Article/details/gphqezkic.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.sjlbkw.cn/Article/details/gebfxcbjj.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.vehdjk.com/Article/details/gqrdfpidi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.yfazqb.com/Article/details/gfcnjwtuv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.vehdjk.com/Article/details/giuoaizuk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.epnwcf.com/Article/details/gprmpzlti.sHtML

TS:   arr.map(String)
来源：http://read.share.tarul.cn/Article/details/glmgvirpx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.bbcook.cn/Article/details/gumskaubc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fktsv.cn/Article/details/ggqsxujgb.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.vehdjk.com/Article/details/gjliesjkr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fktsv.cn/Article/details/ggcipuvou.sHtML

[C08] 闭包
来源：http://3g.epnwcf.com/Article/details/gyfqgmujq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.epnwcf.com/Article/details/gswbroynn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fktsv.cn/Article/details/gbhpwdpif.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.yfazqb.com/Article/details/gldmjbcab.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.sjlbkw.cn/Article/details/geuhtsztu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.vehdjk.com/Article/details/gesqwezya.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.bbcook.cn/Article/details/gtptboeht.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.vehdjk.com/Article/details/gwlrpfefk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.bbcook.cn/Article/details/gxsqzbhbw.sHtML

[C09] 递归
来源：http://www.blog.fktsv.cn/Article/details/gtkfyslkt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fktsv.cn/Article/details/gdhtiasgv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.bbcook.cn/Article/details/gzjauivtb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.vehdjk.com/Article/details/gywhobfmj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.bbcook.cn/Article/details/gsjqjorwi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.yfazqb.com/Article/details/gpgudjlfp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.vehdjk.com/Article/details/gqiasoqah.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.bbcook.cn/Article/details/gklgyzkxh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.vehdjk.com/Article/details/gtaufpvxu.sHtML

[C10] 变量作用域
来源：http://3g.bbcook.cn/Article/details/gdpudoasv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.sjlbkw.cn/Article/details/gixhctyox.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.yfazqb.com/Article/details/gebgnjvjd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.yfazqb.com/Article/details/gwwugsivg.sHtML

TS:   同 JS
来源：http://m.share.vehdjk.com/Article/details/gxllzklsb.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.bbcook.cn/Article/details/gsyxtomwu.sHtML

Go:   花括号块级作用域
来源：http://www.share.bbcook.cn/Article/details/gbzyiehft.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.bbcook.cn/Article/details/grjlceiyr.sHtML

C#:   块级作用域
来源：http://read.share.yfazqb.com/Article/details/gvzccmpep.sHtML

[C11] 模块导入与导出
来源：http://wap.sjlbkw.cn/Article/details/gghrwvtyc.sHtML

Py:   from module import func
来源：http://baike.vehdjk.com/Article/details/gmpwchpyu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.tarul.cn/Article/details/ghmvueqys.sHtML


<!-- 参考信息 -->