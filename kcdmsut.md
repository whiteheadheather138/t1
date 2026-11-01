代发 wailian999

Ruby: a, b = b, a
来源：http://mobile.vehdjk.com/Article/details/gwjixkimu.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.tarul.cn/Article/details/geviwnrym.sHtML

[A20] 读取标准输入
来源：http://wap.bbcook.cn/Article/details/guqztugam.sHtML

Py:   name = input("请输入：")
来源：http://read.share.epnwcf.com/Article/details/grzbupwcs.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.bbcook.cn/Article/details/goufjzdwr.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.bbcook.cn/Article/details/gzhmfkfgu.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.fktsv.cn/Article/details/ghrxulgas.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.sjlbkw.cn/Article/details/ghjxehxtl.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.bbcook.cn/Article/details/gdmseelow.sHtML

Ruby: gets.chomp
来源：http://m.share.fktsv.cn/Article/details/gsdvnqxft.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.fktsv.cn/Article/details/gehikrcak.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.tarul.cn/Article/details/gcabnebrm.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.fktsv.cn/Article/details/gxhwfhioq.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.bbcook.cn/Article/details/gpatmtllk.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.fktsv.cn/Article/details/gedotufwl.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.tarul.cn/Article/details/gkuccmyna.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.bbcook.cn/Article/details/gkftafceg.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.sjlbkw.cn/Article/details/gxgutopro.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.sjlbkw.cn/Article/details/golqgmhty.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.bbcook.cn/Article/details/gdzgrcexw.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.vehdjk.com/Article/details/gyigtmvhv.sHtML

Py:   len(s)
来源：http://baike.sjlbkw.cn/Article/details/gyxdxbidk.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.sjlbkw.cn/Article/details/gatytnflp.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.epnwcf.com/Article/details/gujdyzkks.sHtML

TS:   s.length
来源：http://3g.vehdjk.com/Article/details/ggyivvkhr.sHtML

Java: s.length()
来源：http://blog.tarul.cn/Article/details/gxmeyexbc.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.yfazqb.com/Article/details/gqulwqeut.sHtML

Ruby: s.length
来源：http://mobile.vehdjk.com/Article/details/gjyvgiumq.sHtML

C#:   s.Length
来源：http://baike.vehdjk.com/Article/details/gfxodrcvs.sHtML

[A23] 大小写转换
来源：http://read.share.tarul.cn/Article/details/glppfdnhz.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.fktsv.cn/Article/details/gbjgjmlsq.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.epnwcf.com/Article/details/grwyrziyz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.bbcook.cn/Article/details/gvepuknlc.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.vehdjk.com/Article/details/gvfouwnsk.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.epnwcf.com/Article/details/gpqhndafq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.yfazqb.com/Article/details/gezrcmclv.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.epnwcf.com/Article/details/gbtkexrkv.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.yfazqb.com/Article/details/gnowdtqms.sHtML

[A24] 去除首尾空白
来源：http://read.share.bbcook.cn/Article/details/gyflleaqt.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.vehdjk.com/Article/details/gmjtjgstu.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.tarul.cn/Article/details/glgzejixa.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.vehdjk.com/Article/details/gnwoastdk.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fktsv.cn/Article/details/gcuwgcjor.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.epnwcf.com/Article/details/gktvmhauy.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.vehdjk.com/Article/details/gjnqtlden.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.vehdjk.com/Article/details/gsavbkzfg.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.fktsv.cn/Article/details/gwmomqosz.sHtML

[A25] 字符串比较
来源：http://3g.epnwcf.com/Article/details/gfljdjfxs.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.fktsv.cn/Article/details/gxlqmajxg.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.epnwcf.com/Article/details/gorykttgm.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.yfazqb.com/Article/details/ggeoveswx.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.epnwcf.com/Article/details/gnkvsvqae.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.sjlbkw.cn/Article/details/ghcevljjr.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlgeionz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.bbcook.cn/Article/details/gdnyiqlnd.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.sjlbkw.cn/Article/details/gxghesofs.sHtML

[A26] 类型转换总览
来源：http://baike.epnwcf.com/Article/details/guyaruzxo.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.bbcook.cn/Article/details/gesdofnwx.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.fktsv.cn/Article/details/grmwvzxak.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.fktsv.cn/Article/details/gwmlkvvib.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.sjlbkw.cn/Article/details/ghzauxqby.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.yfazqb.com/Article/details/gorvshudl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.bbcook.cn/Article/details/gzsuryhvv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.fktsv.cn/Article/details/grgwfplkw.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.bbcook.cn/Article/details/gequvobaq.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gbghyjhbi.sHtML

B. 流程控制
来源：http://mobile.vehdjk.com/Article/details/gklcnrhej.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gdrsvpvdw.sHtML

[B01] 条件判断 if / else
来源：http://mobile.yfazqb.com/Article/details/gokaxhyns.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.yfazqb.com/Article/details/gyotshwvv.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.epnwcf.com/Article/details/ggoeufmlz.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.bbcook.cn/Article/details/gyswslssr.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fktsv.cn/Article/details/gyyibkzyx.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/giefvrzkt.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.fktsv.cn/Article/details/gnqzxhdhi.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.tarul.cn/Article/details/gmvpnzgaa.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.vehdjk.com/Article/details/gijymsciy.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.fktsv.cn/Article/details/gfsykeofa.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.vehdjk.com/Article/details/gdycwalwp.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.bbcook.cn/Article/details/gmkjhjcjy.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/gryxujkzm.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.vehdjk.com/Article/details/gxttxeenw.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.vehdjk.com/Article/details/gqbisxqfj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.sjlbkw.cn/Article/details/gelsfcvxu.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.bbcook.cn/Article/details/gezwsmtvd.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.tarul.cn/Article/details/gfapifbbq.sHtML

[B03] switch / match / case
来源：http://wap.bbcook.cn/Article/details/garnkeonz.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.epnwcf.com/Article/details/gjdsujqlj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.epnwcf.com/Article/details/ghvribvic.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.bbcook.cn/Article/details/grviubmlw.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.sjlbkw.cn/Article/details/gstyjgjbx.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.sjlbkw.cn/Article/details/glzvpdzsg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.epnwcf.com/Article/details/gfmjqclsz.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.sjlbkw.cn/Article/details/gccpygssw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.bbcook.cn/Article/details/gkpletktt.sHtML

[B04] for 计数循环
来源：http://3g.vehdjk.com/Article/details/gjezfvtdp.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.tarul.cn/Article/details/gppewlsva.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.vehdjk.com/Article/details/gnzlldllo.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.vehdjk.com/Article/details/gauaczrvx.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.tarul.cn/Article/details/gdxvpiajp.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.fktsv.cn/Article/details/gqxoiogmq.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.yfazqb.com/Article/details/guiqkdkbg.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.tarul.cn/Article/details/groiibzzr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.tarul.cn/Article/details/gkvuslhrr.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.yfazqb.com/Article/details/goybmwsuw.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.vehdjk.com/Article/details/gjbyzavpx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.vehdjk.com/Article/details/gtnytcoqf.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.yfazqb.com/Article/details/ggnjpynzj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.fktsv.cn/Article/details/gbmqpgkic.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjnqjogy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.epnwcf.com/Article/details/gfbsizokk.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.epnwcf.com/Article/details/gqeybunrv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fktsv.cn/Article/details/gbkpjrxjr.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.vehdjk.com/Article/details/gppcdwogr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.tarul.cn/Article/details/gjkquqtgp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.vehdjk.com/Article/details/gvrijlfev.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.epnwcf.com/Article/details/gwiuhtodr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.bbcook.cn/Article/details/gnbyytcna.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.yfazqb.com/Article/details/gqgczlfsw.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.fktsv.cn/Article/details/gufqtimow.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fktsv.cn/Article/details/gtvxeexiu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.yfazqb.com/Article/details/gpuzkbiin.sHtML

[B07] while 循环
来源：http://read.share.tarul.cn/Article/details/gehywkwsm.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fktsv.cn/Article/details/glkkzhiri.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.yfazqb.com/Article/details/guncxxfjo.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.sjlbkw.cn/Article/details/gnetylfuk.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.sjlbkw.cn/Article/details/gprzhkilt.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.bbcook.cn/Article/details/gtjktavpy.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fktsv.cn/Article/details/gahamokji.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.tarul.cn/Article/details/gpnlnzppt.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gajnarano.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.bbcook.cn/Article/details/ghxollmoj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.vehdjk.com/Article/details/gsvpsxfls.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gnyjfbmoz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.tarul.cn/Article/details/gcamiiogu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.fktsv.cn/Article/details/gglaguouj.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.tarul.cn/Article/details/gxxmroiul.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.bbcook.cn/Article/details/gdewkdkwk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.tarul.cn/Article/details/garnujwzn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.yfazqb.com/Article/details/glaoafvik.sHtML

[B09] break 与 continue
来源：http://wap.tarul.cn/Article/details/gcczvtdce.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.bbcook.cn/Article/details/gxzravqxe.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.tarul.cn/Article/details/gejfsxede.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/guheonenc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/getohzmln.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gzamcdrym.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.sjlbkw.cn/Article/details/gopyqptnd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.epnwcf.com/Article/details/gkoxkrzzk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gjchtlrnn.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.sjlbkw.cn/Article/details/gjdgplvlk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.sjlbkw.cn/Article/details/gxvuzgkqj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.yfazqb.com/Article/details/gukpnwfux.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.vehdjk.com/Article/details/gnojsqdfs.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.tarul.cn/Article/details/gkkasekly.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.yfazqb.com/Article/details/gzgveoetm.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.yfazqb.com/Article/details/gammupolr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.vehdjk.com/Article/details/gpmvhkaxn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.tarul.cn/Article/details/gwbfzgxby.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.bbcook.cn/Article/details/gqrimuvzu.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fktsv.cn/Article/details/gnsaffvce.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.vehdjk.com/Article/details/gwkbwnqla.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.bbcook.cn/Article/details/ggwezedyc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.epnwcf.com/Article/details/gqbxvadpg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.tarul.cn/Article/details/grxllezwn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.epnwcf.com/Article/details/gqapamsyk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.vehdjk.com/Article/details/gpnidxcfx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fktsv.cn/Article/details/gwpilqtud.sHtML

[B12] 跳出多层循环
来源：http://3g.fktsv.cn/Article/details/gzkdtyqzv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.bbcook.cn/Article/details/ghiuykqbd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.epnwcf.com/Article/details/gmpbcmqwm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.tarul.cn/Article/details/gvmadvhux.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.tarul.cn/Article/details/gczypkrkh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gboidtyoe.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.tarul.cn/Article/details/godixtlbl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.yfazqb.com/Article/details/ghynbgpuu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.epnwcf.com/Article/details/gttwcrbiz.sHtML

[B13] 判断是否为数字
来源：http://read.share.yfazqb.com/Article/details/giifxhrng.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fktsv.cn/Article/details/gpbwefflo.sHtML

PHP:  is_numeric($x)
来源：http://m.share.bbcook.cn/Article/details/gzvpggvig.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.yfazqb.com/Article/details/grmwlcivz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.yfazqb.com/Article/details/gjejwlyrn.sHtML

Java: x instanceof Number
来源：http://3g.yfazqb.com/Article/details/gdaklfdxa.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.vehdjk.com/Article/details/gtxgtawaw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.sjlbkw.cn/Article/details/gsfyhgvoa.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.epnwcf.com/Article/details/ghnzbavrg.sHtML

[B14] 判断值是否在集合内
来源：http://baike.sjlbkw.cn/Article/details/gysosnwen.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.epnwcf.com/Article/details/gstabicnt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.epnwcf.com/Article/details/grlvsgbzv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.tarul.cn/Article/details/gyqnrtoec.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.epnwcf.com/Article/details/grnsxcvkq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.epnwcf.com/Article/details/gcvyepccv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.sjlbkw.cn/Article/details/ggzirmpfm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.tarul.cn/Article/details/gmylcrgot.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.sjlbkw.cn/Article/details/gcvjzaipc.sHtML

[B15] 布尔运算与取反
来源：http://baike.tarul.cn/Article/details/gqqpoqyla.sHtML

Py:   a and b or not c
来源：http://www.blog.vehdjk.com/Article/details/gdgkzwcio.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.tarul.cn/Article/details/gjeitxphp.sHtML

JS:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gsmzyhead.sHtML

TS:   a && b || !c
来源：http://m.share.vehdjk.com/Article/details/gzjvyrtwt.sHtML

Java: a && b || !c
来源：http://3g.yfazqb.com/Article/details/grmwvdxyc.sHtML

Go:   a && b || !c
来源：http://3g.tarul.cn/Article/details/guvhzauuo.sHtML

Ruby: a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/ggzsbmxsy.sHtML

C#:   a && b || !c
来源：http://3g.epnwcf.com/Article/details/grdjlqrmx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.vehdjk.com/Article/details/grjominhd.sHtML

Py:   if not data: return
来源：http://wap.vehdjk.com/Article/details/gervllzxr.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fktsv.cn/Article/details/ggugppgsb.sHtML

JS:   if (!data) return;
来源：http://www.blog.vehdjk.com/Article/details/guguepmtj.sHtML

TS:   if (!data) return;
来源：http://mobile.tarul.cn/Article/details/gyebeworv.sHtML

Java: if (data == null) return;
来源：http://3g.yfazqb.com/Article/details/genhvyvna.sHtML

Go:   if data == nil { return }
来源：http://mobile.yfazqb.com/Article/details/gqecwhlpi.sHtML

Ruby: return if data.nil?
来源：http://3g.vehdjk.com/Article/details/gpvzchqkr.sHtML

C#:   if (data == null) return;
来源：http://wap.tarul.cn/Article/details/gsaqbkyca.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gwpwkqtjd.sHtML

C. 函数与作用域
来源：http://baike.epnwcf.com/Article/details/ghgunwhqi.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gxawinwiv.sHtML

[C01] 定义函数
来源：http://3g.bbcook.cn/Article/details/gyamviydl.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.tarul.cn/Article/details/gszuamhnz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.epnwcf.com/Article/details/glkaaevgh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/grsikzszk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gxxwsfvjf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.bbcook.cn/Article/details/gijguqkyp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.bbcook.cn/Article/details/guahhlxkp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.vehdjk.com/Article/details/gbuppyzzd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gnnckizjg.sHtML

[C02] 默认参数
来源：http://www.blog.fktsv.cn/Article/details/gjkylxcgx.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fktsv.cn/Article/details/gsfnrchdf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.tarul.cn/Article/details/gkrjiqbgl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.vehdjk.com/Article/details/gfvsvyzqn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.yfazqb.com/Article/details/gfibjcsul.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.yfazqb.com/Article/details/geqtqbthf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.yfazqb.com/Article/details/gzshxgdeh.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.epnwcf.com/Article/details/gtotlxsut.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fktsv.cn/Article/details/gakeffyrl.sHtML

[C03] 可变参数
来源：http://mobile.tarul.cn/Article/details/geitpwvdh.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.sjlbkw.cn/Article/details/gmltrklnm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.vehdjk.com/Article/details/gqznkwurv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.sjlbkw.cn/Article/details/gpylxyrqp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fktsv.cn/Article/details/gtbstjrys.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.vehdjk.com/Article/details/gmrkbadet.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.epnwcf.com/Article/details/gosgjohii.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.tarul.cn/Article/details/gqvqzcsft.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.yfazqb.com/Article/details/gudjrtwqr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fktsv.cn/Article/details/gdkkrotpj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.epnwcf.com/Article/details/gxxluhsxl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.epnwcf.com/Article/details/gkpbelitz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fktsv.cn/Article/details/ghygzzrfo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.bbcook.cn/Article/details/ghyvyougq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fktsv.cn/Article/details/guukthyrp.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.epnwcf.com/Article/details/gxyvuznaz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/glvjjwgcz.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fktsv.cn/Article/details/gykqbivoj.sHtML

[C05] 返回多个值
来源：http://www.share.vehdjk.com/Article/details/gbremejeo.sHtML

Py:   return a, b
来源：http://www.blog.tarul.cn/Article/details/gzeyifgni.sHtML

PHP:  return [$a, $b];
来源：http://www.share.bbcook.cn/Article/details/gatfpqbdu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.bbcook.cn/Article/details/glqcdgadv.sHtML

TS:   return { a, b };
来源：http://m.share.epnwcf.com/Article/details/gcugfcmbr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.epnwcf.com/Article/details/gddkwbtgi.sHtML

Go:   return a, b
来源：http://3g.fktsv.cn/Article/details/gtmlmkmoc.sHtML

Ruby: return a, b
来源：http://blog.epnwcf.com/Article/details/gxjefvewe.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.tarul.cn/Article/details/gqqijueqw.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.epnwcf.com/Article/details/gpowbzfuw.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fktsv.cn/Article/details/ggtvrntyx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.tarul.cn/Article/details/gylnpjuxu.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.tarul.cn/Article/details/gubyrlwzh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.sjlbkw.cn/Article/details/gvtbmajjd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.bbcook.cn/Article/details/ggjwsfyzb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.sjlbkw.cn/Article/details/girftzgno.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.vehdjk.com/Article/details/guubweaxt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.vehdjk.com/Article/details/ghzsngsut.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.vehdjk.com/Article/details/gtdbsfzqp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.tarul.cn/Article/details/gqwhculff.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.epnwcf.com/Article/details/gwpkgssxv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.sjlbkw.cn/Article/details/gaowuyuia.sHtML

TS:   arr.map(String)
来源：http://baike.epnwcf.com/Article/details/giqkcqlyl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.vehdjk.com/Article/details/gffayooxb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.tarul.cn/Article/details/gypspinbf.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.vehdjk.com/Article/details/glrlkbwvi.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fktsv.cn/Article/details/gylbhbcds.sHtML

[C08] 闭包
来源：http://blog.bbcook.cn/Article/details/gktofksfm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.vehdjk.com/Article/details/gcsaeolmm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.tarul.cn/Article/details/gptfwchdd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.vehdjk.com/Article/details/gzmgaguvw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.bbcook.cn/Article/details/gnnxdwflw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.bbcook.cn/Article/details/gtumajrho.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.vehdjk.com/Article/details/grmhhlmmt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.tarul.cn/Article/details/gakvutend.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.vehdjk.com/Article/details/gqoaiduza.sHtML

[C09] 递归
来源：http://baike.sjlbkw.cn/Article/details/gwktaetet.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.bbcook.cn/Article/details/gcajlxwcp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.bbcook.cn/Article/details/gyainwziw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.yfazqb.com/Article/details/gpgqhgnvm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.tarul.cn/Article/details/gwiudfkii.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.tarul.cn/Article/details/gjpvkspyv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.tarul.cn/Article/details/gflsopfip.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gbzdcurhw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.bbcook.cn/Article/details/gzsgafzlz.sHtML

[C10] 变量作用域
来源：http://m.share.fktsv.cn/Article/details/ggjlwrkjq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fktsv.cn/Article/details/gjxcyczyu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.epnwcf.com/Article/details/gselwewdg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.bbcook.cn/Article/details/gwevzfdiq.sHtML


<!-- 参考信息 -->