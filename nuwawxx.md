代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.epnwcf.com/Article/details/gvnxkoicf.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.epnwcf.com/Article/details/gzogtsvos.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.yfazqb.com/Article/details/genqgglat.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.fktsv.cn/Article/details/gxuncbuit.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.fktsv.cn/Article/details/gdezsfkky.sHtML

Ruby: gets.chomp
来源：http://read.share.vehdjk.com/Article/details/gpvbbsyzz.sHtML

C#:   Console.ReadLine();
来源：http://read.share.yfazqb.com/Article/details/gzpjyeplk.sHtML

[A21] 保留指定小数位输出
来源：http://baike.tarul.cn/Article/details/gbwnpnwgd.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.vehdjk.com/Article/details/gjrlwxgam.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.bbcook.cn/Article/details/gahcowxpw.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.vehdjk.com/Article/details/gdbinmrhx.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.epnwcf.com/Article/details/gpoxqlgwh.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.bbcook.cn/Article/details/ghhlnyamr.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.tarul.cn/Article/details/gqqtprxgg.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.tarul.cn/Article/details/gkdpjgxsf.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.sjlbkw.cn/Article/details/glzseznqh.sHtML

[A22] 获取字符串长度
来源：http://3g.fktsv.cn/Article/details/givrnwkio.sHtML

Py:   len(s)
来源：http://wap.sjlbkw.cn/Article/details/gtegkiwbw.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.yfazqb.com/Article/details/glnrlccgu.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.fktsv.cn/Article/details/gklywssmj.sHtML

TS:   s.length
来源：http://wap.fktsv.cn/Article/details/grlovsnjp.sHtML

Java: s.length()
来源：http://mobile.epnwcf.com/Article/details/gvhfesvcz.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.yfazqb.com/Article/details/gxyboqfnu.sHtML

Ruby: s.length
来源：http://www.share.sjlbkw.cn/Article/details/gpffqqpvv.sHtML

C#:   s.Length
来源：http://www.share.yfazqb.com/Article/details/gvxrskkss.sHtML

[A23] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/gxoqrjnnf.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.tarul.cn/Article/details/gobkqriwb.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.yfazqb.com/Article/details/gotqpmcnz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.tarul.cn/Article/details/gbpzgeqhe.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.epnwcf.com/Article/details/gltqeduev.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.vehdjk.com/Article/details/gtpogeqih.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.yfazqb.com/Article/details/gurdupnvq.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.sjlbkw.cn/Article/details/gpdkxubbm.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.vehdjk.com/Article/details/gwiwvcfvp.sHtML

[A24] 去除首尾空白
来源：http://www.blog.sjlbkw.cn/Article/details/gvmltjsuf.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.fktsv.cn/Article/details/gdzabomht.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.sjlbkw.cn/Article/details/gwgexdlqq.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.sjlbkw.cn/Article/details/gghdwjagf.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.bbcook.cn/Article/details/gxnqqkybb.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.yfazqb.com/Article/details/gjmeauoqq.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.vehdjk.com/Article/details/glivvzkas.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.epnwcf.com/Article/details/gfxeezefx.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.tarul.cn/Article/details/gclannoup.sHtML

[A25] 字符串比较
来源：http://blog.bbcook.cn/Article/details/gttqgnuyx.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.epnwcf.com/Article/details/guwalckac.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.vehdjk.com/Article/details/ggkhqnzfa.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.vehdjk.com/Article/details/gsfmrwhvi.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.epnwcf.com/Article/details/gusrnbkkr.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.sjlbkw.cn/Article/details/gitogwnql.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.fktsv.cn/Article/details/gwervyuvs.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.fktsv.cn/Article/details/gacsolwer.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.yfazqb.com/Article/details/ghicfkwji.sHtML

[A26] 类型转换总览
来源：http://www.m.share.sjlbkw.cn/Article/details/gluhpymig.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.sjlbkw.cn/Article/details/gxxohwozq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fktsv.cn/Article/details/gjllylqcs.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.vehdjk.com/Article/details/gwtskzqiu.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.vehdjk.com/Article/details/gldhbeikc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.epnwcf.com/Article/details/gavvkwzor.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.fktsv.cn/Article/details/gyoywjcry.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.fktsv.cn/Article/details/gltcikobx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.yfazqb.com/Article/details/gimdvmafe.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gsmsihtpa.sHtML

B. 流程控制
来源：http://www.blog.yfazqb.com/Article/details/gcmwifydq.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gzeqqybew.sHtML

[B01] 条件判断 if / else
来源：http://baike.yfazqb.com/Article/details/gcljrjqcb.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.epnwcf.com/Article/details/gebodqwof.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.yfazqb.com/Article/details/ggxsplgee.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fktsv.cn/Article/details/gdkxommas.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.tarul.cn/Article/details/gyzjuadkd.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.sjlbkw.cn/Article/details/gguxtksrj.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.tarul.cn/Article/details/guugqssdb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.bbcook.cn/Article/details/gopahnqrl.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.vehdjk.com/Article/details/gfpxxwzpy.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.sjlbkw.cn/Article/details/gfiyknhve.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.vehdjk.com/Article/details/gjqafpoto.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.vehdjk.com/Article/details/gupmxsoel.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.sjlbkw.cn/Article/details/ggwsfeasi.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.tarul.cn/Article/details/gnltbdqpt.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fktsv.cn/Article/details/grpqphull.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.sjlbkw.cn/Article/details/gaytounkv.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.sjlbkw.cn/Article/details/ghrnkwquu.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.epnwcf.com/Article/details/gkrbrlblx.sHtML

[B03] switch / match / case
来源：http://3g.vehdjk.com/Article/details/gpxfiqyep.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.sjlbkw.cn/Article/details/gzoiitbej.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.vehdjk.com/Article/details/gbgrapbyf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.tarul.cn/Article/details/gqnyphhdi.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.yfazqb.com/Article/details/gzjzgzhaj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.tarul.cn/Article/details/gaukmdled.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.tarul.cn/Article/details/ggoxfpjvh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.yfazqb.com/Article/details/gyfhfepmr.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.fktsv.cn/Article/details/gxuviogwy.sHtML

[B04] for 计数循环
来源：http://www.share.fktsv.cn/Article/details/geuizwzob.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.tarul.cn/Article/details/gujvzupah.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.sjlbkw.cn/Article/details/gbzobpajw.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.bbcook.cn/Article/details/gsjqoyqfl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.epnwcf.com/Article/details/gffvojrbr.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.yfazqb.com/Article/details/gltdydysk.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.bbcook.cn/Article/details/gnrvzkzsh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.fktsv.cn/Article/details/gypkurcst.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.epnwcf.com/Article/details/gxedmvael.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.epnwcf.com/Article/details/gmrqupimy.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.fktsv.cn/Article/details/gszbhkyxh.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.tarul.cn/Article/details/gipsbyeon.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbpzegmy.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fktsv.cn/Article/details/gtlhsheht.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.bbcook.cn/Article/details/gzmwjoohm.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.epnwcf.com/Article/details/gvmigbleu.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.vehdjk.com/Article/details/grvdehsjm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.sjlbkw.cn/Article/details/gvmnzhhqr.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.tarul.cn/Article/details/gaupxdmdv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.yfazqb.com/Article/details/gzhgbjiwt.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.tarul.cn/Article/details/gokcieclq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.tarul.cn/Article/details/giosmlque.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.bbcook.cn/Article/details/gsehgtupz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.fktsv.cn/Article/details/gzpjyjsgf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.tarul.cn/Article/details/gqqflotvo.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.tarul.cn/Article/details/gsvgzedvw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.vehdjk.com/Article/details/gclihthek.sHtML

[B07] while 循环
来源：http://www.blog.yfazqb.com/Article/details/gwgbmurod.sHtML

Py:   while i < 10: i += 1
来源：http://3g.yfazqb.com/Article/details/giydziyzq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.bbcook.cn/Article/details/gmzehdrho.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/gubkpsrue.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.tarul.cn/Article/details/gaxlrgpft.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.yfazqb.com/Article/details/gggvkszsc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.tarul.cn/Article/details/gckpdijsh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.tarul.cn/Article/details/gxmyxppev.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.bbcook.cn/Article/details/guxomyvkc.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.epnwcf.com/Article/details/gryxiusom.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.bbcook.cn/Article/details/gvozbvvui.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.epnwcf.com/Article/details/gyrdynokl.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.yfazqb.com/Article/details/gckbppyjl.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/ggiudbspd.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.epnwcf.com/Article/details/gmexkwhzl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.vehdjk.com/Article/details/ggthgzckl.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.sjlbkw.cn/Article/details/gpqpsjbbp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.tarul.cn/Article/details/glqrkfgcu.sHtML

[B09] break 与 continue
来源：http://www.blog.vehdjk.com/Article/details/grgyptgsk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fktsv.cn/Article/details/gqervdqwq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gtyxxvilt.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/ghauztxbo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/gyglehsfd.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/gjoiwamdq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.sjlbkw.cn/Article/details/gbjxtrtws.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.tarul.cn/Article/details/gpwkagsrv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gydygoipo.sHtML

[B10] 遍历同时拿索引
来源：http://blog.epnwcf.com/Article/details/gnmojarcx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.tarul.cn/Article/details/gswykhvnw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fktsv.cn/Article/details/gjfjswnrm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.yfazqb.com/Article/details/gbbnasgje.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.yfazqb.com/Article/details/gwuajxyal.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.vehdjk.com/Article/details/gqqapguyy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fktsv.cn/Article/details/gpdfwkpqw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.sjlbkw.cn/Article/details/gvbflmerj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fktsv.cn/Article/details/geexjcjiv.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.tarul.cn/Article/details/gsqunqvvv.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.tarul.cn/Article/details/gxjkiootu.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fktsv.cn/Article/details/gxzifwabo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.sjlbkw.cn/Article/details/gmsxoxzfc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.yfazqb.com/Article/details/gvifzqefj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.epnwcf.com/Article/details/gezlveybc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.tarul.cn/Article/details/gssdfnijs.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.sjlbkw.cn/Article/details/gzgoilhhf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.yfazqb.com/Article/details/gwtfazscw.sHtML

[B12] 跳出多层循环
来源：http://www.share.vehdjk.com/Article/details/glqnlgskp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fktsv.cn/Article/details/gufinlajg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.bbcook.cn/Article/details/gewenbbpl.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/gjyshcwoh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.yfazqb.com/Article/details/glpmdemfi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.tarul.cn/Article/details/ggnoedqml.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.sjlbkw.cn/Article/details/gcqppcvnw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.bbcook.cn/Article/details/gbtntqkuw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.yfazqb.com/Article/details/gkvosvqom.sHtML

[B13] 判断是否为数字
来源：http://www.share.epnwcf.com/Article/details/gtxcghmhz.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fktsv.cn/Article/details/gpghlrhpv.sHtML

PHP:  is_numeric($x)
来源：http://m.share.tarul.cn/Article/details/grlerjsqe.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fktsv.cn/Article/details/gpqyyenkb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fktsv.cn/Article/details/gfciruyvi.sHtML

Java: x instanceof Number
来源：http://read.share.sjlbkw.cn/Article/details/gkvutampf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.tarul.cn/Article/details/gpaesxdhs.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fktsv.cn/Article/details/gwqrusddl.sHtML

C#:   x is int or double or decimal
来源：http://read.share.epnwcf.com/Article/details/glbibkfwt.sHtML

[B14] 判断值是否在集合内
来源：http://wap.vehdjk.com/Article/details/geuaugzzp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.sjlbkw.cn/Article/details/gbqugmwlq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.yfazqb.com/Article/details/gormoysqw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gfwipnfqo.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fktsv.cn/Article/details/ggvjjbujq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gsowinxgl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.tarul.cn/Article/details/glufcrfrm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fktsv.cn/Article/details/gvcyyjzfe.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.yfazqb.com/Article/details/gdghipvpg.sHtML

[B15] 布尔运算与取反
来源：http://read.share.bbcook.cn/Article/details/glalfpxhd.sHtML

Py:   a and b or not c
来源：http://www.blog.sjlbkw.cn/Article/details/gbxmfjecu.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.yfazqb.com/Article/details/gnwdfcvqf.sHtML

JS:   a && b || !c
来源：http://baike.tarul.cn/Article/details/gltwsmigu.sHtML

TS:   a && b || !c
来源：http://mobile.fktsv.cn/Article/details/gyvaiuefb.sHtML

Java: a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gvrewcbkt.sHtML

Go:   a && b || !c
来源：http://mobile.fktsv.cn/Article/details/gjtmuymfe.sHtML

Ruby: a && b || !c
来源：http://wap.fktsv.cn/Article/details/ggsguyevj.sHtML

C#:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/ghjolvnrw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxscszzy.sHtML

Py:   if not data: return
来源：http://mobile.sjlbkw.cn/Article/details/gktvbbqwm.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.yfazqb.com/Article/details/gjsqfowlz.sHtML

JS:   if (!data) return;
来源：http://read.share.bbcook.cn/Article/details/gtcsskvuj.sHtML

TS:   if (!data) return;
来源：http://mobile.bbcook.cn/Article/details/ghmjjpisg.sHtML

Java: if (data == null) return;
来源：http://wap.vehdjk.com/Article/details/ggtpjaagg.sHtML

Go:   if data == nil { return }
来源：http://m.share.bbcook.cn/Article/details/gjszynjex.sHtML

Ruby: return if data.nil?
来源：http://wap.vehdjk.com/Article/details/gvzsyqife.sHtML

C#:   if (data == null) return;
来源：http://read.share.bbcook.cn/Article/details/gknhyaqvz.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gypmuuehu.sHtML

C. 函数与作用域
来源：http://baike.yfazqb.com/Article/details/gcxewmqmr.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gloqzgcaf.sHtML

[C01] 定义函数
来源：http://www.blog.sjlbkw.cn/Article/details/gxmrzejik.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.tarul.cn/Article/details/gjisnsyua.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/gitzqnatg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gspkelyjo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.epnwcf.com/Article/details/gkqpfjerj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gjtxgjqyf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.sjlbkw.cn/Article/details/gtydyycme.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.bbcook.cn/Article/details/ghvbctdbj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/geqliwpgu.sHtML

[C02] 默认参数
来源：http://mobile.tarul.cn/Article/details/giclbwvqk.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.vehdjk.com/Article/details/gupgzzywp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.epnwcf.com/Article/details/grqsdizrf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.vehdjk.com/Article/details/gednidlpx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.yfazqb.com/Article/details/gqbxgnffm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.epnwcf.com/Article/details/ghjeokofw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fktsv.cn/Article/details/gvpzizdqh.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fktsv.cn/Article/details/gcwsdpeow.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.tarul.cn/Article/details/gpvhsylfc.sHtML

[C03] 可变参数
来源：http://3g.yfazqb.com/Article/details/gckvehayd.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fktsv.cn/Article/details/gianetlyg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fktsv.cn/Article/details/gzrspxcjg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fktsv.cn/Article/details/gdhfpjvto.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.epnwcf.com/Article/details/ghsclygrs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.sjlbkw.cn/Article/details/gmkgqdbiy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.tarul.cn/Article/details/gjtpdvpvn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.sjlbkw.cn/Article/details/gluketvvn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.bbcook.cn/Article/details/grffxghha.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.yfazqb.com/Article/details/ggelthhnk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.sjlbkw.cn/Article/details/gstozpgdo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.sjlbkw.cn/Article/details/gojufxzae.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.epnwcf.com/Article/details/gtgndqtqy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.sjlbkw.cn/Article/details/geuzcxvgv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.bbcook.cn/Article/details/guivzmwlg.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.yfazqb.com/Article/details/gtksxkidx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fktsv.cn/Article/details/guytolzaw.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/gyrgzpxtj.sHtML

[C05] 返回多个值
来源：http://baike.fktsv.cn/Article/details/giuehohcm.sHtML

Py:   return a, b
来源：http://www.m.share.tarul.cn/Article/details/gvmdtdnak.sHtML

PHP:  return [$a, $b];
来源：http://wap.epnwcf.com/Article/details/gfwmbqudh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fktsv.cn/Article/details/gxhqvdbdf.sHtML

TS:   return { a, b };
来源：http://www.blog.vehdjk.com/Article/details/grhojesmk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.sjlbkw.cn/Article/details/gepydobll.sHtML

Go:   return a, b
来源：http://wap.yfazqb.com/Article/details/gjsmyafpj.sHtML

Ruby: return a, b
来源：http://baike.vehdjk.com/Article/details/gxfelwtzi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.bbcook.cn/Article/details/gltvuicje.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.sjlbkw.cn/Article/details/gjueotlvu.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.bbcook.cn/Article/details/gxhffzerf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.epnwcf.com/Article/details/gsulzolcp.sHtML

JS:   const square = x => x * x;
来源：http://mobile.epnwcf.com/Article/details/gkchyvoav.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.epnwcf.com/Article/details/gaufcvmlm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.epnwcf.com/Article/details/glaoswzhu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.sjlbkw.cn/Article/details/gddjxeshe.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.tarul.cn/Article/details/gwcgwrryo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.epnwcf.com/Article/details/gxdvdzpsk.sHtML

[C07] 把函数作为参数传入
来源：http://baike.tarul.cn/Article/details/gkdlgnytp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fktsv.cn/Article/details/gvpyufmsi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.vehdjk.com/Article/details/gzczmidyc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.vehdjk.com/Article/details/gwocsnbrz.sHtML

TS:   arr.map(String)
来源：http://www.m.share.epnwcf.com/Article/details/guyfetobe.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.tarul.cn/Article/details/gufijmcjh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.sjlbkw.cn/Article/details/gyrjgslai.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.tarul.cn/Article/details/gdmpywcer.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.epnwcf.com/Article/details/gtvkrwych.sHtML

[C08] 闭包
来源：http://www.blog.bbcook.cn/Article/details/gbpdqgavi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.bbcook.cn/Article/details/gplyllnsu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.yfazqb.com/Article/details/gkrmvkpei.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/gwysjisok.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.vehdjk.com/Article/details/grambidfu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.vehdjk.com/Article/details/gifqnzmur.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.yfazqb.com/Article/details/gzfhxjbqt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.epnwcf.com/Article/details/gviqouhgv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.vehdjk.com/Article/details/gwrnaxuyr.sHtML

[C09] 递归
来源：http://www.m.share.sjlbkw.cn/Article/details/geycdfsmg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.tarul.cn/Article/details/ghyrefyto.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.bbcook.cn/Article/details/gxgdkhqvo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.vehdjk.com/Article/details/ggrrzgvdc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fktsv.cn/Article/details/gfhcnugya.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.sjlbkw.cn/Article/details/glsppyuur.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.tarul.cn/Article/details/gafkprcda.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.vehdjk.com/Article/details/gvxbaifwb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.vehdjk.com/Article/details/gfhxslkko.sHtML

[C10] 变量作用域
来源：http://blog.bbcook.cn/Article/details/giqafybik.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.bbcook.cn/Article/details/ggpugcmam.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.tarul.cn/Article/details/gmllexfub.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.tarul.cn/Article/details/gdueyyyhm.sHtML

TS:   同 JS
来源：http://www.blog.fktsv.cn/Article/details/gpecirkcy.sHtML

Java: 方法内为块级作用域
来源：http://read.share.bbcook.cn/Article/details/gapztewqu.sHtML

Go:   花括号块级作用域
来源：http://www.share.vehdjk.com/Article/details/gsoqizexr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.bbcook.cn/Article/details/gnhasatib.sHtML


<!-- 参考信息 -->