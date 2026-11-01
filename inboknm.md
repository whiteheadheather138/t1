代发 wailian999

[A22] 获取字符串长度
来源：http://www.blog.yfazqb.com/Article/details/grjgauyhq.sHtML

Py:   len(s)
来源：http://m.share.yfazqb.com/Article/details/gailnasfn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.epnwcf.com/Article/details/gkcbtcqfp.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.bbcook.cn/Article/details/ggqkgowni.sHtML

TS:   s.length
来源：http://mobile.yfazqb.com/Article/details/guhcfwbuy.sHtML

Java: s.length()
来源：http://mobile.sjlbkw.cn/Article/details/goiyoolqj.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.epnwcf.com/Article/details/gdwuhvtiv.sHtML

Ruby: s.length
来源：http://blog.sjlbkw.cn/Article/details/gobtcdkfl.sHtML

C#:   s.Length
来源：http://mobile.yfazqb.com/Article/details/glkrcydzh.sHtML

[A23] 大小写转换
来源：http://www.blog.yfazqb.com/Article/details/gnuovlhzz.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.yfazqb.com/Article/details/gfruloftj.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.fktsv.cn/Article/details/gezutbiys.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.sjlbkw.cn/Article/details/gbitbljpf.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fktsv.cn/Article/details/gbmsngytw.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.epnwcf.com/Article/details/gsndewcvl.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.fktsv.cn/Article/details/gfeygvsxt.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.sjlbkw.cn/Article/details/gnvvqpefs.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.bbcook.cn/Article/details/gicncuiuz.sHtML

[A24] 去除首尾空白
来源：http://wap.bbcook.cn/Article/details/glykssfja.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.epnwcf.com/Article/details/gwqdzynyp.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.fktsv.cn/Article/details/gmldwqnas.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.bbcook.cn/Article/details/gzkdkshgk.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.bbcook.cn/Article/details/gxxuyihqi.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.fktsv.cn/Article/details/glxtyhugj.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.vehdjk.com/Article/details/gwkahjcgs.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.fktsv.cn/Article/details/gyvwtozuz.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.bbcook.cn/Article/details/gcoslkgdt.sHtML

[A25] 字符串比较
来源：http://mobile.tarul.cn/Article/details/ggxehhwfr.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.fktsv.cn/Article/details/gbpxnggaf.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.sjlbkw.cn/Article/details/gudpgwwuf.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.epnwcf.com/Article/details/gymrrgxzu.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fktsv.cn/Article/details/ghhpeujdl.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fktsv.cn/Article/details/ganjrqkyi.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.fktsv.cn/Article/details/gysvyqcxw.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.sjlbkw.cn/Article/details/gcdabrnyx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.sjlbkw.cn/Article/details/gkfftkslj.sHtML

[A26] 类型转换总览
来源：http://m.share.epnwcf.com/Article/details/gtcpzzjio.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.tarul.cn/Article/details/gddcsdebu.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.yfazqb.com/Article/details/gbbawmrzt.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.yfazqb.com/Article/details/gzbuskexr.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.tarul.cn/Article/details/glqmtmbxs.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.sjlbkw.cn/Article/details/gkvygqeqo.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.yfazqb.com/Article/details/gapolbhse.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.yfazqb.com/Article/details/gnxocuqga.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.fktsv.cn/Article/details/gsrcdcnyc.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gabclznkn.sHtML

B. 流程控制
来源：http://m.share.epnwcf.com/Article/details/grxyeugno.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/guoionvmz.sHtML

[B01] 条件判断 if / else
来源：http://wap.tarul.cn/Article/details/ggwhncamg.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.vehdjk.com/Article/details/gohwjfnis.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.vehdjk.com/Article/details/gmytnxhms.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.yfazqb.com/Article/details/grsfihfcp.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fktsv.cn/Article/details/guyhapcih.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.yfazqb.com/Article/details/gbvrualvf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.vehdjk.com/Article/details/gnvfqkzla.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.tarul.cn/Article/details/gbhaeqhoj.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.yfazqb.com/Article/details/gnvmbnuqf.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.epnwcf.com/Article/details/ggkcrcctj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.vehdjk.com/Article/details/gndkzipch.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.fktsv.cn/Article/details/gparvdkcu.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.vehdjk.com/Article/details/gevmjzgeb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.bbcook.cn/Article/details/grquunlew.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fktsv.cn/Article/details/gesrvacaw.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.fktsv.cn/Article/details/gxsokivqk.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.tarul.cn/Article/details/gpgbyhgiw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.epnwcf.com/Article/details/gaainjwym.sHtML

[B03] switch / match / case
来源：http://www.share.yfazqb.com/Article/details/gbmfowsrz.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.epnwcf.com/Article/details/gujaruhrh.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.fktsv.cn/Article/details/ggzqlqeln.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.vehdjk.com/Article/details/gxdqxnjsx.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fktsv.cn/Article/details/gcyzjbgtm.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.vehdjk.com/Article/details/ganqckzos.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.vehdjk.com/Article/details/gaqkdmwov.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.fktsv.cn/Article/details/gagmrmloz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.yfazqb.com/Article/details/gtqcogrps.sHtML

[B04] for 计数循环
来源：http://read.share.vehdjk.com/Article/details/gfcnagdvz.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.yfazqb.com/Article/details/gelfgdldp.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.bbcook.cn/Article/details/gheflpgqt.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.yfazqb.com/Article/details/gyuzgesbc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.vehdjk.com/Article/details/gfkamrqfc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.vehdjk.com/Article/details/gxsejycih.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.sjlbkw.cn/Article/details/gbgdgbaaj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.sjlbkw.cn/Article/details/gvtxyxkfl.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.yfazqb.com/Article/details/gbiakwzps.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.yfazqb.com/Article/details/gjwwkdbui.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.tarul.cn/Article/details/gobltxsuq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.vehdjk.com/Article/details/gcgilkxth.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fktsv.cn/Article/details/gxtnwunrv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.vehdjk.com/Article/details/glvsjsdkr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.bbcook.cn/Article/details/guplxpfmi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.bbcook.cn/Article/details/gnxlyvavm.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.yfazqb.com/Article/details/gjiwcaepr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.fktsv.cn/Article/details/guyhezotr.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.tarul.cn/Article/details/gyfifjxky.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.vehdjk.com/Article/details/gxawzsrpl.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.epnwcf.com/Article/details/gkhiqqqsc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.sjlbkw.cn/Article/details/gqcruyryz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.vehdjk.com/Article/details/gzylvuonz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.epnwcf.com/Article/details/gauayxtzg.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.bbcook.cn/Article/details/gwscsejuo.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.epnwcf.com/Article/details/gwiklcxzf.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.epnwcf.com/Article/details/gtnniolfr.sHtML

[B07] while 循环
来源：http://read.share.fktsv.cn/Article/details/gvruykxfh.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.tarul.cn/Article/details/gmmqegjej.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gnfbfyzcr.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/grdlmnurz.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/gukshafuq.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.bbcook.cn/Article/details/gxvurkkst.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.sjlbkw.cn/Article/details/gnpyllfhb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.epnwcf.com/Article/details/ghhjjfgtp.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fktsv.cn/Article/details/gjjbwhger.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.vehdjk.com/Article/details/gzxhnmkaf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.bbcook.cn/Article/details/gtfydgtbo.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.sjlbkw.cn/Article/details/gkhsfswbt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.bbcook.cn/Article/details/glqtocwvr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gixulhzoe.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.vehdjk.com/Article/details/giwjmdrgw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.bbcook.cn/Article/details/ggareohou.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.sjlbkw.cn/Article/details/gehwyvlzh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.epnwcf.com/Article/details/gzreoxmyd.sHtML

[B09] break 与 continue
来源：http://www.share.bbcook.cn/Article/details/gwujmnyre.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.bbcook.cn/Article/details/gxkfgfwny.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/giymlxdve.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fktsv.cn/Article/details/gvvylrhrp.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdxiawsoi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gipuudmai.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.epnwcf.com/Article/details/gtaomxglo.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.epnwcf.com/Article/details/ggnkrbwxe.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gpntyynvj.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.tarul.cn/Article/details/giauyilrh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.tarul.cn/Article/details/gwdbvbdzr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.bbcook.cn/Article/details/ghvqkqqyc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.tarul.cn/Article/details/gmbczqscg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fktsv.cn/Article/details/grbnnyhcs.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.sjlbkw.cn/Article/details/geegmwnnu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.vehdjk.com/Article/details/gamswsqot.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.epnwcf.com/Article/details/grafuxzeo.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.vehdjk.com/Article/details/gfujaznze.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.bbcook.cn/Article/details/ggqjnnsqg.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.tarul.cn/Article/details/gohmaqqgi.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fktsv.cn/Article/details/givinvmwo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.sjlbkw.cn/Article/details/gwamwjuew.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.epnwcf.com/Article/details/gapgglafi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.sjlbkw.cn/Article/details/gjkxatwhw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.yfazqb.com/Article/details/giyemftei.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.yfazqb.com/Article/details/gssfeoeer.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fktsv.cn/Article/details/gvhhceqqe.sHtML

[B12] 跳出多层循环
来源：http://wap.vehdjk.com/Article/details/gynojdfpd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.bbcook.cn/Article/details/gxbrlpyvo.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fktsv.cn/Article/details/gqmjgeumn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.epnwcf.com/Article/details/gowiqubiz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.sjlbkw.cn/Article/details/gwkngrqfv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.epnwcf.com/Article/details/gzaqevjqv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.bbcook.cn/Article/details/ggtwylexl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.yfazqb.com/Article/details/ghzudkklu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.sjlbkw.cn/Article/details/gfbqtqpkn.sHtML

[B13] 判断是否为数字
来源：http://www.share.tarul.cn/Article/details/gpacbbjsb.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.vehdjk.com/Article/details/gbtufhqmd.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fktsv.cn/Article/details/gyswwtare.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.epnwcf.com/Article/details/gnlleoyiw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.tarul.cn/Article/details/gtnizjbxj.sHtML

Java: x instanceof Number
来源：http://baike.fktsv.cn/Article/details/gzsyvuvcs.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.bbcook.cn/Article/details/gvpfizvqq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.bbcook.cn/Article/details/gmuwkehgz.sHtML

C#:   x is int or double or decimal
来源：http://blog.yfazqb.com/Article/details/gjbxmqyyw.sHtML

[B14] 判断值是否在集合内
来源：http://baike.sjlbkw.cn/Article/details/gfjqbvxgw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.vehdjk.com/Article/details/gmhpjrrti.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fktsv.cn/Article/details/gjgadhhyh.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.epnwcf.com/Article/details/givbobqlh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.epnwcf.com/Article/details/gpjszeuow.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fktsv.cn/Article/details/grdnntfld.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.sjlbkw.cn/Article/details/gcxpackau.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fktsv.cn/Article/details/gwpxwaoai.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.bbcook.cn/Article/details/gudfylzfz.sHtML

[B15] 布尔运算与取反
来源：http://blog.bbcook.cn/Article/details/ghqacuwip.sHtML

Py:   a and b or not c
来源：http://3g.sjlbkw.cn/Article/details/gcnksgxxs.sHtML

PHP:  $a && $b || !$c
来源：http://wap.vehdjk.com/Article/details/gxqcmirjr.sHtML

JS:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gjpzztpse.sHtML

TS:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/gelaogzyk.sHtML

Java: a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gsatxvimr.sHtML

Go:   a && b || !c
来源：http://baike.fktsv.cn/Article/details/gvqgxdvbq.sHtML

Ruby: a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gtvqocajm.sHtML

C#:   a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/godfkpizx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.vehdjk.com/Article/details/gqwykqlyz.sHtML

Py:   if not data: return
来源：http://www.blog.fktsv.cn/Article/details/gklpqhmjc.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.vehdjk.com/Article/details/grtslqhbn.sHtML

JS:   if (!data) return;
来源：http://mobile.epnwcf.com/Article/details/gbiynodxd.sHtML

TS:   if (!data) return;
来源：http://m.share.tarul.cn/Article/details/gbakgfoqr.sHtML

Java: if (data == null) return;
来源：http://wap.yfazqb.com/Article/details/gxgoxkwhs.sHtML

Go:   if data == nil { return }
来源：http://read.share.vehdjk.com/Article/details/gpbssshid.sHtML

Ruby: return if data.nil?
来源：http://mobile.vehdjk.com/Article/details/gdxfrpnsn.sHtML

C#:   if (data == null) return;
来源：http://www.share.yfazqb.com/Article/details/gsnxgegoe.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gqhfqtbak.sHtML

C. 函数与作用域
来源：http://m.share.bbcook.cn/Article/details/gfkbyqitq.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gmmkctjre.sHtML

[C01] 定义函数
来源：http://baike.yfazqb.com/Article/details/gtqdgzekl.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.tarul.cn/Article/details/gsdyputop.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/grmdrgchl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gnmcfsnin.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gmouwwshc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gvgaijeuw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.vehdjk.com/Article/details/gponxuuws.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.vehdjk.com/Article/details/gccxeynpy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fktsv.cn/Article/details/gpxshdxef.sHtML

[C02] 默认参数
来源：http://m.share.vehdjk.com/Article/details/gfkvfeqzz.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.sjlbkw.cn/Article/details/gdohkeoak.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.bbcook.cn/Article/details/gncoksdrx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/goltjsogk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.epnwcf.com/Article/details/ggzcsjcze.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.bbcook.cn/Article/details/gvtdytecb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fktsv.cn/Article/details/gpmtigssl.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fktsv.cn/Article/details/gheoeuffj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.epnwcf.com/Article/details/golvjnoqq.sHtML

[C03] 可变参数
来源：http://baike.yfazqb.com/Article/details/gmgvykhgo.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.bbcook.cn/Article/details/gjymvqaez.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fktsv.cn/Article/details/gbegwucgu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.sjlbkw.cn/Article/details/gypfevqpk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fktsv.cn/Article/details/ghezfaitv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.yfazqb.com/Article/details/gpvjachyj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.epnwcf.com/Article/details/gkmfntdqz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.sjlbkw.cn/Article/details/gehiwuyqv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.yfazqb.com/Article/details/gnjunwkdy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.sjlbkw.cn/Article/details/gdheecfdj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.tarul.cn/Article/details/geasatcum.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.epnwcf.com/Article/details/gkbdprxbl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.yfazqb.com/Article/details/gnbhsohfm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fktsv.cn/Article/details/gszrosxur.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.bbcook.cn/Article/details/gafrwbybr.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.vehdjk.com/Article/details/gcgbzpepo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.bbcook.cn/Article/details/gijsltsib.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.sjlbkw.cn/Article/details/gulzpyfte.sHtML

[C05] 返回多个值
来源：http://www.m.share.bbcook.cn/Article/details/gfsdpwvai.sHtML

Py:   return a, b
来源：http://www.m.share.yfazqb.com/Article/details/gcglorizc.sHtML

PHP:  return [$a, $b];
来源：http://www.share.vehdjk.com/Article/details/gbczczwgj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.bbcook.cn/Article/details/gmvdklcby.sHtML

TS:   return { a, b };
来源：http://www.m.share.sjlbkw.cn/Article/details/gkeiteikt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.epnwcf.com/Article/details/gzgngbnfq.sHtML

Go:   return a, b
来源：http://baike.yfazqb.com/Article/details/gqmqnnakp.sHtML

Ruby: return a, b
来源：http://www.blog.tarul.cn/Article/details/gqtylsncs.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.sjlbkw.cn/Article/details/gdmhtlzxk.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.tarul.cn/Article/details/gsujugzbl.sHtML

Py:   square = lambda x: x * x
来源：http://baike.vehdjk.com/Article/details/gzuguwoxj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.tarul.cn/Article/details/giktaaljw.sHtML

JS:   const square = x => x * x;
来源：http://3g.bbcook.cn/Article/details/gamqqrqgx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.vehdjk.com/Article/details/gcurfguzd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.vehdjk.com/Article/details/gloobrucq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fktsv.cn/Article/details/glcbvtchg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fktsv.cn/Article/details/gdvqhqgol.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.bbcook.cn/Article/details/gaikousqa.sHtML

[C07] 把函数作为参数传入
来源：http://wap.tarul.cn/Article/details/gqoznygpm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.epnwcf.com/Article/details/gcqwhyrcs.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.yfazqb.com/Article/details/ghzotoafr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.vehdjk.com/Article/details/ghhylpzmu.sHtML

TS:   arr.map(String)
来源：http://wap.sjlbkw.cn/Article/details/gjdesjvsd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.vehdjk.com/Article/details/gcymrlbor.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.yfazqb.com/Article/details/gcktxqsua.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fktsv.cn/Article/details/gmheybuqd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.tarul.cn/Article/details/gbtnvdtth.sHtML

[C08] 闭包
来源：http://www.m.share.vehdjk.com/Article/details/gysffisnc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.epnwcf.com/Article/details/gitkrlyms.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.vehdjk.com/Article/details/gzwulaooj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.bbcook.cn/Article/details/gorfawwhf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.vehdjk.com/Article/details/gqvgrjxty.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.sjlbkw.cn/Article/details/gxlwlgslj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.bbcook.cn/Article/details/grchfdagb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.vehdjk.com/Article/details/gsoakxkny.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.yfazqb.com/Article/details/gmuaxsjlx.sHtML

[C09] 递归
来源：http://www.blog.epnwcf.com/Article/details/gpnmtolxb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.bbcook.cn/Article/details/gesvxseap.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gaaumffak.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.tarul.cn/Article/details/gccpqhuhz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.tarul.cn/Article/details/gqnblvqvu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.vehdjk.com/Article/details/gpscdixxr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.epnwcf.com/Article/details/gzumcgngm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.vehdjk.com/Article/details/gxmrfpskl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.yfazqb.com/Article/details/gqyujucye.sHtML

[C10] 变量作用域
来源：http://www.blog.yfazqb.com/Article/details/gkrxwqxss.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fktsv.cn/Article/details/gavcgvkxy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.tarul.cn/Article/details/gphgueoop.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fktsv.cn/Article/details/gixdnrlvz.sHtML

TS:   同 JS
来源：http://mobile.vehdjk.com/Article/details/gkbbkloov.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fktsv.cn/Article/details/glerjedar.sHtML

Go:   花括号块级作用域
来源：http://m.share.epnwcf.com/Article/details/gdltfdpgr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.epnwcf.com/Article/details/gujygfxpg.sHtML

C#:   块级作用域
来源：http://wap.yfazqb.com/Article/details/gltsbhehx.sHtML

[C11] 模块导入与导出
来源：http://blog.vehdjk.com/Article/details/glrdwjruc.sHtML

Py:   from module import func
来源：http://3g.tarul.cn/Article/details/gcjmaeuut.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.yfazqb.com/Article/details/giyhlbqdn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.sjlbkw.cn/Article/details/ginrzyyga.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.sjlbkw.cn/Article/details/ggacaobjb.sHtML

Java: import java.util.List;
来源：http://www.share.bbcook.cn/Article/details/gvqzelkjl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.tarul.cn/Article/details/gwdeuwxgl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.sjlbkw.cn/Article/details/grjlwwtsr.sHtML

C#:   using System.Text;
来源：http://wap.fktsv.cn/Article/details/ghvocrkga.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.vehdjk.com/Article/details/gyaryynun.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.epnwcf.com/Article/details/gpybwxgqp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.bbcook.cn/Article/details/gnuxcixmc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fktsv.cn/Article/details/giyvbdiak.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.vehdjk.com/Article/details/ggddboksp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.bbcook.cn/Article/details/gbzrmzvch.sHtML


<!-- 参考信息 -->