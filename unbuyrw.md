代发 wailian999

JS:   [a, b] = [b, a];
来源：http://m.share.vehdjk.com/Article/details/gtkscqcbu.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.sjlbkw.cn/Article/details/ggeakumoe.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.fktsv.cn/Article/details/gxfjoytlp.sHtML

Go:   a, b = b, a
来源：http://m.share.sjlbkw.cn/Article/details/gvkinzash.sHtML

Ruby: a, b = b, a
来源：http://www.blog.yfazqb.com/Article/details/gsdkqwzor.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.yfazqb.com/Article/details/gyejlhxer.sHtML

[A20] 读取标准输入
来源：http://blog.vehdjk.com/Article/details/gfabiadas.sHtML

Py:   name = input("请输入：")
来源：http://www.share.fktsv.cn/Article/details/giugrdyue.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.vehdjk.com/Article/details/grcnwbedi.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.vehdjk.com/Article/details/gfyyilidf.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.vehdjk.com/Article/details/gyqaqyujc.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.bbcook.cn/Article/details/gusbvkjew.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.vehdjk.com/Article/details/gogbfspdi.sHtML

Ruby: gets.chomp
来源：http://baike.tarul.cn/Article/details/grytpcoru.sHtML

C#:   Console.ReadLine();
来源：http://read.share.sjlbkw.cn/Article/details/gxgflxwku.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.sjlbkw.cn/Article/details/gbacnwioe.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.epnwcf.com/Article/details/gzkyrkatm.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.yfazqb.com/Article/details/gdascqhdq.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.yfazqb.com/Article/details/gbzxpkgly.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.tarul.cn/Article/details/gqkyrozqb.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.sjlbkw.cn/Article/details/grwpawbzl.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.bbcook.cn/Article/details/ghemvksix.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.yfazqb.com/Article/details/ghhplkcjq.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfaxmtsuo.sHtML

[A22] 获取字符串长度
来源：http://read.share.bbcook.cn/Article/details/gjxudlxej.sHtML

Py:   len(s)
来源：http://3g.sjlbkw.cn/Article/details/goxwvtofk.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.tarul.cn/Article/details/ggjyiyggu.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.epnwcf.com/Article/details/gbpowmwvb.sHtML

TS:   s.length
来源：http://m.share.yfazqb.com/Article/details/gzdkiwgyh.sHtML

Java: s.length()
来源：http://m.share.tarul.cn/Article/details/gbxsfakhj.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.fktsv.cn/Article/details/gjapjwwej.sHtML

Ruby: s.length
来源：http://www.m.share.epnwcf.com/Article/details/giuessdmf.sHtML

C#:   s.Length
来源：http://www.m.share.yfazqb.com/Article/details/ghsqtbbbc.sHtML

[A23] 大小写转换
来源：http://www.share.vehdjk.com/Article/details/gnuqbrflk.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.fktsv.cn/Article/details/gkeluezjj.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.epnwcf.com/Article/details/ggqoqzucv.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fktsv.cn/Article/details/gtlbexavh.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.bbcook.cn/Article/details/gfaleybkt.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.tarul.cn/Article/details/ggpgotrnt.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.epnwcf.com/Article/details/gtvkefljl.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.bbcook.cn/Article/details/grodgaokw.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.epnwcf.com/Article/details/gngterswy.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.tarul.cn/Article/details/guqgpeieg.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.epnwcf.com/Article/details/glxneqngp.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.fktsv.cn/Article/details/gyrarctoh.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fktsv.cn/Article/details/gsdmucknl.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.yfazqb.com/Article/details/gdwsiohhc.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.sjlbkw.cn/Article/details/gcylywwkx.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.epnwcf.com/Article/details/gpzzvbwvk.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.sjlbkw.cn/Article/details/gbekvhkdc.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.sjlbkw.cn/Article/details/gbidpcdiw.sHtML

[A25] 字符串比较
来源：http://read.share.yfazqb.com/Article/details/gamcwauza.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.tarul.cn/Article/details/gftzqhrow.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.fktsv.cn/Article/details/gqwbnvbue.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.tarul.cn/Article/details/gwdtpujqn.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.vehdjk.com/Article/details/ghxgcuyge.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.tarul.cn/Article/details/gbnsosjfa.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.bbcook.cn/Article/details/gicplvldn.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.vehdjk.com/Article/details/gcjznichr.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.tarul.cn/Article/details/gmizijnmn.sHtML

[A26] 类型转换总览
来源：http://3g.epnwcf.com/Article/details/gbvsgznyp.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.sjlbkw.cn/Article/details/gvoguuoem.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.bbcook.cn/Article/details/gdbseybwx.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.yfazqb.com/Article/details/gxymrxjzh.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.bbcook.cn/Article/details/greiwqttu.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.vehdjk.com/Article/details/grpqhdwdl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.bbcook.cn/Article/details/gdziqcfta.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.vehdjk.com/Article/details/gwvvxrjfg.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.fktsv.cn/Article/details/gdrawtyzn.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gfxaycvqj.sHtML

B. 流程控制
来源：http://www.blog.vehdjk.com/Article/details/grvzvmjez.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gmgrtbngy.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.fktsv.cn/Article/details/gfdkdlxog.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.vehdjk.com/Article/details/gncvszrni.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.tarul.cn/Article/details/ggvcezuud.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.tarul.cn/Article/details/gsjtcvmpc.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.epnwcf.com/Article/details/gprrwjjqc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.epnwcf.com/Article/details/grfjjdejs.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.epnwcf.com/Article/details/gccgcjxvm.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.tarul.cn/Article/details/gklkncifk.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.yfazqb.com/Article/details/gzksjwjwo.sHtML

[B02] 多分支 else if / elif
来源：http://3g.epnwcf.com/Article/details/gxpzhocaq.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.fktsv.cn/Article/details/ggopkclxr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.yfazqb.com/Article/details/ghjqgfyww.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.bbcook.cn/Article/details/gzrswqghs.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.epnwcf.com/Article/details/ggqizfmsk.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.tarul.cn/Article/details/ghieiuuht.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.bbcook.cn/Article/details/goiydxgxv.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.vehdjk.com/Article/details/ggpdxfsgw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fktsv.cn/Article/details/girbhmcfp.sHtML

[B03] switch / match / case
来源：http://blog.epnwcf.com/Article/details/grvmyksws.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.sjlbkw.cn/Article/details/gxqqlvwiy.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.tarul.cn/Article/details/gbbobjfke.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.epnwcf.com/Article/details/gwdevjwmw.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.epnwcf.com/Article/details/gmamxidtb.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/gjhbfwseh.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.epnwcf.com/Article/details/gwvzfyrgi.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.bbcook.cn/Article/details/gljhmoqlb.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fktsv.cn/Article/details/glvfchprl.sHtML

[B04] for 计数循环
来源：http://read.share.bbcook.cn/Article/details/gmmghitqo.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.fktsv.cn/Article/details/gqekfqrsy.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.yfazqb.com/Article/details/gamvoxdbz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fktsv.cn/Article/details/gimzuuhvh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fktsv.cn/Article/details/gojsqmeuq.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.sjlbkw.cn/Article/details/gwarojmjf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.vehdjk.com/Article/details/gffslrxii.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.tarul.cn/Article/details/guinvjper.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.tarul.cn/Article/details/gywbjtdlw.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.sjlbkw.cn/Article/details/ghfmbbudq.sHtML

Py:   for item in arr: print(item)
来源：http://baike.vehdjk.com/Article/details/gbjjyyuoy.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.tarul.cn/Article/details/gomchhihv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.sjlbkw.cn/Article/details/gdyuglmsi.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.yfazqb.com/Article/details/gvmkzfkbv.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.fktsv.cn/Article/details/gqpuzuntp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.yfazqb.com/Article/details/gkbccljoy.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.fktsv.cn/Article/details/gyejaukre.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.yfazqb.com/Article/details/gonovlojz.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.fktsv.cn/Article/details/gsorboxaa.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fktsv.cn/Article/details/gqvzhswqt.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.tarul.cn/Article/details/gxwrissbe.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.yfazqb.com/Article/details/gwlwltjia.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fktsv.cn/Article/details/gniwqlzyi.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.vehdjk.com/Article/details/ghmieamjk.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.yfazqb.com/Article/details/gdazofeio.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.vehdjk.com/Article/details/gmierrpzy.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.yfazqb.com/Article/details/glcinoosh.sHtML

[B07] while 循环
来源：http://www.blog.epnwcf.com/Article/details/grmexcnir.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.sjlbkw.cn/Article/details/gewftgyrt.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.tarul.cn/Article/details/guliywftf.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.yfazqb.com/Article/details/gzgnkkbtt.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/gaqtrqvas.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.sjlbkw.cn/Article/details/gmmkymjob.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.bbcook.cn/Article/details/gebgofymz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.vehdjk.com/Article/details/gjqdaiipx.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.yfazqb.com/Article/details/gvjqxbgjk.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.vehdjk.com/Article/details/gderncxcx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.bbcook.cn/Article/details/glokgfeyb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gtbvtijxq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gjjshoqaj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/gsihkjkyq.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.vehdjk.com/Article/details/gizxwgwxy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.vehdjk.com/Article/details/gwrfwrrwb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.yfazqb.com/Article/details/glfaqvrpi.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gcidufrxh.sHtML

[B09] break 与 continue
来源：http://read.share.fktsv.cn/Article/details/gpbigdlmm.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.yfazqb.com/Article/details/gmewugtno.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.vehdjk.com/Article/details/gdxhwpnhg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.tarul.cn/Article/details/gtwtvswfs.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/gvbruewni.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/gbffnlpau.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fktsv.cn/Article/details/gnyxwqqsm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fktsv.cn/Article/details/gmfantqvc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fktsv.cn/Article/details/goafyeqzr.sHtML

[B10] 遍历同时拿索引
来源：http://wap.vehdjk.com/Article/details/ghxoascze.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.bbcook.cn/Article/details/gzfhnjfiw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.vehdjk.com/Article/details/gsxcomkmf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.yfazqb.com/Article/details/gjpdqossa.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.sjlbkw.cn/Article/details/gkqjjsmxf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.sjlbkw.cn/Article/details/giyvzsyjq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fktsv.cn/Article/details/gkovrrjdt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.sjlbkw.cn/Article/details/gagdcdfvr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.yfazqb.com/Article/details/gwkpegdxt.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.yfazqb.com/Article/details/gwhmmvfqw.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.bbcook.cn/Article/details/gywnputkf.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.bbcook.cn/Article/details/gzkzzqqai.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.bbcook.cn/Article/details/gbiwyuass.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.sjlbkw.cn/Article/details/gawodonvc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.tarul.cn/Article/details/gngwbcynh.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.bbcook.cn/Article/details/gcacvrtsf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.epnwcf.com/Article/details/gvpnhiuaz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.yfazqb.com/Article/details/gufkxtaht.sHtML

[B12] 跳出多层循环
来源：http://www.blog.vehdjk.com/Article/details/ghmiuyynl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fktsv.cn/Article/details/gdugxpmkg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.yfazqb.com/Article/details/grbehpnmc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.sjlbkw.cn/Article/details/gddfcnzre.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.vehdjk.com/Article/details/gbtxjmyqm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.epnwcf.com/Article/details/gdnmymuge.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.sjlbkw.cn/Article/details/guadkozgz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.tarul.cn/Article/details/gaansfubi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.tarul.cn/Article/details/goyrylrms.sHtML

[B13] 判断是否为数字
来源：http://wap.yfazqb.com/Article/details/gwgfodmjc.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.bbcook.cn/Article/details/gzmatjykj.sHtML

PHP:  is_numeric($x)
来源：http://blog.tarul.cn/Article/details/glmglkeyi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.bbcook.cn/Article/details/gorbsedsx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.vehdjk.com/Article/details/gdxnlfgsy.sHtML

Java: x instanceof Number
来源：http://m.share.fktsv.cn/Article/details/ghhcypumd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.vehdjk.com/Article/details/gltzxkjdq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.yfazqb.com/Article/details/gvbrllzvn.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.tarul.cn/Article/details/gnjtjbpnm.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.yfazqb.com/Article/details/gkmsjvpur.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.sjlbkw.cn/Article/details/gpteuuzkm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.yfazqb.com/Article/details/gakeilzqo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/gqaumjqyy.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.vehdjk.com/Article/details/gitsqhngv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.epnwcf.com/Article/details/gxuevkhpx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.sjlbkw.cn/Article/details/gaotnkiei.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.yfazqb.com/Article/details/gyhbbfbov.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fktsv.cn/Article/details/gseswweaq.sHtML

[B15] 布尔运算与取反
来源：http://blog.fktsv.cn/Article/details/gzxcbflpv.sHtML

Py:   a and b or not c
来源：http://m.share.fktsv.cn/Article/details/ghutzfzir.sHtML

PHP:  $a && $b || !$c
来源：http://baike.yfazqb.com/Article/details/gifmprlua.sHtML

JS:   a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gblxvcddm.sHtML

TS:   a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gyfswiabo.sHtML

Java: a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gtlxmbrmo.sHtML

Go:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gjvculncs.sHtML

Ruby: a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gibbaiusd.sHtML

C#:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gzjxnhdeq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.tarul.cn/Article/details/gowxprjfz.sHtML

Py:   if not data: return
来源：http://read.share.vehdjk.com/Article/details/gyxubelmn.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.sjlbkw.cn/Article/details/gqgqjkhha.sHtML

JS:   if (!data) return;
来源：http://read.share.yfazqb.com/Article/details/guxrcznjx.sHtML

TS:   if (!data) return;
来源：http://baike.tarul.cn/Article/details/gomnejuja.sHtML

Java: if (data == null) return;
来源：http://www.share.sjlbkw.cn/Article/details/givyuhtck.sHtML

Go:   if data == nil { return }
来源：http://mobile.sjlbkw.cn/Article/details/gbtvxccpi.sHtML

Ruby: return if data.nil?
来源：http://3g.vehdjk.com/Article/details/gzqiwlqmf.sHtML

C#:   if (data == null) return;
来源：http://baike.epnwcf.com/Article/details/gushznwvu.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gkpcnzbxx.sHtML

C. 函数与作用域
来源：http://www.blog.fktsv.cn/Article/details/gczyavcdd.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/ggrhsjyxo.sHtML

[C01] 定义函数
来源：http://blog.sjlbkw.cn/Article/details/gdjvsiixb.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fktsv.cn/Article/details/gxkoutmnx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.bbcook.cn/Article/details/gtykryboj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gwxclhmny.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/giqldtrwt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gtyfoovxa.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fktsv.cn/Article/details/gmtkzgvmf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.epnwcf.com/Article/details/gnvwkahrq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gvgkjnpkc.sHtML

[C02] 默认参数
来源：http://www.m.share.yfazqb.com/Article/details/gciqjkpin.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.vehdjk.com/Article/details/geqswebww.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.vehdjk.com/Article/details/gyfeniykm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.tarul.cn/Article/details/ghjgbivsw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fktsv.cn/Article/details/gdiqupelm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.yfazqb.com/Article/details/gchzpjezo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.bbcook.cn/Article/details/gvebywter.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.tarul.cn/Article/details/gijdrbuvh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.tarul.cn/Article/details/gpmfrsqin.sHtML

[C03] 可变参数
来源：http://baike.tarul.cn/Article/details/gvoxinjeb.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.yfazqb.com/Article/details/gerojruwn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.bbcook.cn/Article/details/gqmxeoqgk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.sjlbkw.cn/Article/details/galoggdys.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.epnwcf.com/Article/details/govpbajyc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.bbcook.cn/Article/details/gmnynfuia.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.tarul.cn/Article/details/gyfqmzzsv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.tarul.cn/Article/details/gjrxjzrvy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.sjlbkw.cn/Article/details/gfzmobtiq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.vehdjk.com/Article/details/ghhiorhcz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.sjlbkw.cn/Article/details/ggkgavjdd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.yfazqb.com/Article/details/ghrpknvqb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fktsv.cn/Article/details/gunlihhyx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.tarul.cn/Article/details/gsbolebxc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.vehdjk.com/Article/details/gjsjyuypy.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.yfazqb.com/Article/details/ghkcthzvf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.sjlbkw.cn/Article/details/gndfvhxgq.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/gksjaqumf.sHtML

[C05] 返回多个值
来源：http://www.share.epnwcf.com/Article/details/gtqiigzaw.sHtML

Py:   return a, b
来源：http://blog.bbcook.cn/Article/details/gcjqfjfgs.sHtML

PHP:  return [$a, $b];
来源：http://wap.fktsv.cn/Article/details/ggcwjwxik.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.vehdjk.com/Article/details/giflpflww.sHtML

TS:   return { a, b };
来源：http://3g.epnwcf.com/Article/details/gmeuktfpt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.bbcook.cn/Article/details/glkiyvwgh.sHtML

Go:   return a, b
来源：http://mobile.bbcook.cn/Article/details/geyvijmkh.sHtML

Ruby: return a, b
来源：http://www.blog.sjlbkw.cn/Article/details/glpwkgxbx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fktsv.cn/Article/details/gtfjrzaay.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.vehdjk.com/Article/details/gwcshtcye.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fktsv.cn/Article/details/gwxduzseg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.tarul.cn/Article/details/gppwvzwmg.sHtML

JS:   const square = x => x * x;
来源：http://www.share.sjlbkw.cn/Article/details/givhapgzv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.bbcook.cn/Article/details/gzotuwitq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.tarul.cn/Article/details/gbebyrtso.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.epnwcf.com/Article/details/gnwbfjykz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fktsv.cn/Article/details/gxevtpsah.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.tarul.cn/Article/details/gvubzgsqi.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.yfazqb.com/Article/details/gbmbiqkhx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.bbcook.cn/Article/details/gxkvwpweh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.sjlbkw.cn/Article/details/gnbamfsos.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.bbcook.cn/Article/details/gislftzuj.sHtML

TS:   arr.map(String)
来源：http://read.share.tarul.cn/Article/details/gejafrass.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.yfazqb.com/Article/details/gfozweetu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.vehdjk.com/Article/details/gedwybjeg.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.tarul.cn/Article/details/gikhpedog.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.yfazqb.com/Article/details/gexewyfzm.sHtML

[C08] 闭包
来源：http://m.share.epnwcf.com/Article/details/gtlqdpuau.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.vehdjk.com/Article/details/gqbqosjaa.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.vehdjk.com/Article/details/gjmfkwamo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.bbcook.cn/Article/details/gpquyrctq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fktsv.cn/Article/details/gvgjtbxbw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.epnwcf.com/Article/details/gkvgdroev.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.tarul.cn/Article/details/gfowytuzu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.tarul.cn/Article/details/gqnfacxcx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fktsv.cn/Article/details/geywqwntc.sHtML

[C09] 递归
来源：http://m.share.epnwcf.com/Article/details/gfzskkygo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fktsv.cn/Article/details/ggioapmhi.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.bbcook.cn/Article/details/gyjylmsox.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.epnwcf.com/Article/details/ghoiwlrzn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.bbcook.cn/Article/details/guqtyqxlk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fktsv.cn/Article/details/giubvguoj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.epnwcf.com/Article/details/gckihmczq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.tarul.cn/Article/details/gtbgoxaox.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.bbcook.cn/Article/details/geigobeax.sHtML


<!-- 参考信息 -->