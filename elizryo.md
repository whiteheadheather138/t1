代发 wailian999

C#:   (int)'A'; (char)65
来源：http://m.share.yfazqb.com/Article/details/gfffnxebu.sHtML

[A19] 交换两个变量
来源：http://m.share.tarul.cn/Article/details/gpehpwbyx.sHtML

Py:   a, b = b, a
来源：http://m.share.epnwcf.com/Article/details/gfyrrosit.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.yfazqb.com/Article/details/gudwkwdml.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.bbcook.cn/Article/details/gyaupnffh.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.tarul.cn/Article/details/guntdsxde.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.fktsv.cn/Article/details/gljeiqiup.sHtML

Go:   a, b = b, a
来源：http://www.m.share.fktsv.cn/Article/details/gfqhesmth.sHtML

Ruby: a, b = b, a
来源：http://www.blog.fktsv.cn/Article/details/gfgqvftem.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.tarul.cn/Article/details/gjsiikbka.sHtML

[A20] 读取标准输入
来源：http://3g.bbcook.cn/Article/details/ggxqtajtf.sHtML

Py:   name = input("请输入：")
来源：http://m.share.vehdjk.com/Article/details/geimnzkit.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.yfazqb.com/Article/details/guhgnhzky.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.fktsv.cn/Article/details/ggotpukxp.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.bbcook.cn/Article/details/gngijtujb.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.bbcook.cn/Article/details/gvsgpxism.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.tarul.cn/Article/details/giogakdkh.sHtML

Ruby: gets.chomp
来源：http://wap.tarul.cn/Article/details/ggtpbsohw.sHtML

C#:   Console.ReadLine();
来源：http://wap.fktsv.cn/Article/details/gwqiuaxjt.sHtML

[A21] 保留指定小数位输出
来源：http://blog.fktsv.cn/Article/details/gupidtuew.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.sjlbkw.cn/Article/details/gnpihogpr.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.bbcook.cn/Article/details/gaapgoxup.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.fktsv.cn/Article/details/govyffejk.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.epnwcf.com/Article/details/gpslsjtpc.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.fktsv.cn/Article/details/gakdlbwax.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.epnwcf.com/Article/details/gmsnchfeq.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.yfazqb.com/Article/details/gpbyumxwp.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.epnwcf.com/Article/details/ghabybwwr.sHtML

[A22] 获取字符串长度
来源：http://read.share.bbcook.cn/Article/details/gtuuzdmpc.sHtML

Py:   len(s)
来源：http://blog.bbcook.cn/Article/details/gpwgowddx.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.fktsv.cn/Article/details/gshllbxke.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.tarul.cn/Article/details/gaieoczny.sHtML

TS:   s.length
来源：http://wap.bbcook.cn/Article/details/gdkoppcrj.sHtML

Java: s.length()
来源：http://www.share.bbcook.cn/Article/details/gazvsemyi.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.fktsv.cn/Article/details/gzgkeftlr.sHtML

Ruby: s.length
来源：http://3g.fktsv.cn/Article/details/gbebxquws.sHtML

C#:   s.Length
来源：http://www.m.share.epnwcf.com/Article/details/gdcoixhar.sHtML

[A23] 大小写转换
来源：http://mobile.fktsv.cn/Article/details/grlrunptg.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.sjlbkw.cn/Article/details/guytbhiac.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.bbcook.cn/Article/details/glycxnakp.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.tarul.cn/Article/details/gmzwxrptg.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.vehdjk.com/Article/details/gxyxcipjh.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.sjlbkw.cn/Article/details/gslajsjbi.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.sjlbkw.cn/Article/details/gxxbnckdx.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.fktsv.cn/Article/details/gucwlrrau.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.fktsv.cn/Article/details/gvhprcina.sHtML

[A24] 去除首尾空白
来源：http://m.share.tarul.cn/Article/details/gcucdvgtk.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.yfazqb.com/Article/details/gmpzmgbim.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.sjlbkw.cn/Article/details/glshlmwqc.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fktsv.cn/Article/details/gkbdqtscf.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.epnwcf.com/Article/details/gtwqjcqui.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.yfazqb.com/Article/details/gnsvhwiwu.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.fktsv.cn/Article/details/gcbrptqkh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.vehdjk.com/Article/details/ghgpjeszz.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.tarul.cn/Article/details/glbasisoe.sHtML

[A25] 字符串比较
来源：http://www.share.yfazqb.com/Article/details/gdovokcyr.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.tarul.cn/Article/details/gpcsuohyv.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.bbcook.cn/Article/details/gypemduxt.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.yfazqb.com/Article/details/gsgzbxufr.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fktsv.cn/Article/details/gzqpajgil.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.yfazqb.com/Article/details/gnezrhizc.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.sjlbkw.cn/Article/details/ghmvpzyjk.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.tarul.cn/Article/details/gilmcebvh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.tarul.cn/Article/details/gtgjyakvx.sHtML

[A26] 类型转换总览
来源：http://mobile.vehdjk.com/Article/details/ganltngpd.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.sjlbkw.cn/Article/details/gsihshdhh.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.tarul.cn/Article/details/gjqxnpwpy.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.fktsv.cn/Article/details/gzemewefk.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.epnwcf.com/Article/details/gsldrnbuh.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.fktsv.cn/Article/details/gswfdwhur.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.tarul.cn/Article/details/gobsvllfh.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.epnwcf.com/Article/details/gzfztfvuq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.epnwcf.com/Article/details/gclxnhzbf.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gqclwcnto.sHtML

B. 流程控制
来源：http://www.blog.yfazqb.com/Article/details/gpnzgbydx.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gvgnoclra.sHtML

[B01] 条件判断 if / else
来源：http://baike.sjlbkw.cn/Article/details/gklmydimj.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fktsv.cn/Article/details/gjcvrmnoh.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.vehdjk.com/Article/details/gabbabhnx.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.yfazqb.com/Article/details/gpijfxdqc.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.epnwcf.com/Article/details/gztsedbkv.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.epnwcf.com/Article/details/gximgkyug.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.vehdjk.com/Article/details/grzhutohj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.bbcook.cn/Article/details/gwdbmpvxm.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.bbcook.cn/Article/details/gtbuxhvtr.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.fktsv.cn/Article/details/ggmzrepqo.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.epnwcf.com/Article/details/gfzhprpcd.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.epnwcf.com/Article/details/glxphxjwu.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.tarul.cn/Article/details/gahkyopgb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.tarul.cn/Article/details/gosfgspiw.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.tarul.cn/Article/details/gfnnpznac.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.tarul.cn/Article/details/gnyvlkbsb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.tarul.cn/Article/details/gcfrzvwzu.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.vehdjk.com/Article/details/gexjwugxp.sHtML

[B03] switch / match / case
来源：http://read.share.sjlbkw.cn/Article/details/gnaximbna.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.yfazqb.com/Article/details/gyczrzzie.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.fktsv.cn/Article/details/gjvkfqdqt.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.bbcook.cn/Article/details/gkqdhgueo.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.tarul.cn/Article/details/gkaogsodv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.bbcook.cn/Article/details/gyxmvrmub.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.fktsv.cn/Article/details/gntlulvmj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.vehdjk.com/Article/details/gryusjihe.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.epnwcf.com/Article/details/gdgvhzlih.sHtML

[B04] for 计数循环
来源：http://blog.vehdjk.com/Article/details/guhjlalsn.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.vehdjk.com/Article/details/gnvbydiqr.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.yfazqb.com/Article/details/gfkejrpke.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.vehdjk.com/Article/details/gorzjbtsf.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.yfazqb.com/Article/details/geoemzbom.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.epnwcf.com/Article/details/grspuxikt.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.bbcook.cn/Article/details/gnpwasjiz.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.bbcook.cn/Article/details/goysmddum.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.yfazqb.com/Article/details/glbwmemvr.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.vehdjk.com/Article/details/gmljuzrml.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.epnwcf.com/Article/details/gganmrzyh.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fktsv.cn/Article/details/gergyiurl.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.bbcook.cn/Article/details/gnsayufik.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.tarul.cn/Article/details/gwaxophpt.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.epnwcf.com/Article/details/gheiksjrw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.epnwcf.com/Article/details/gdjomtuwo.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.bbcook.cn/Article/details/gxivuuirn.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.bbcook.cn/Article/details/gpproogtz.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.fktsv.cn/Article/details/gxklmtyil.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.epnwcf.com/Article/details/gxhffhlno.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.bbcook.cn/Article/details/gbnhotdwo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.epnwcf.com/Article/details/gaouxcclr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.yfazqb.com/Article/details/gjqwhhavp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.yfazqb.com/Article/details/gkuyjumhc.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.bbcook.cn/Article/details/gvrlglazp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.yfazqb.com/Article/details/gdhgxhogh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.tarul.cn/Article/details/getmrkeka.sHtML

[B07] while 循环
来源：http://3g.fktsv.cn/Article/details/gqqryubwi.sHtML

Py:   while i < 10: i += 1
来源：http://blog.tarul.cn/Article/details/gsnznnobm.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.sjlbkw.cn/Article/details/gglokdkhm.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.epnwcf.com/Article/details/gfyxavhke.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.bbcook.cn/Article/details/gbzlsccbe.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.bbcook.cn/Article/details/gpdznymzx.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.yfazqb.com/Article/details/ggguztkwe.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.vehdjk.com/Article/details/gdmedejwq.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.vehdjk.com/Article/details/gswoltfnz.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.yfazqb.com/Article/details/gyctxltuu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.bbcook.cn/Article/details/ggwfxkckv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gcjlgkdlc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.yfazqb.com/Article/details/giclcmods.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.vehdjk.com/Article/details/gkiilptol.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.yfazqb.com/Article/details/gttglqbgr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.yfazqb.com/Article/details/gyutzplih.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.epnwcf.com/Article/details/gmzwldkee.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gcmjkoduv.sHtML

[B09] break 与 continue
来源：http://www.share.bbcook.cn/Article/details/gefdblibl.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.tarul.cn/Article/details/glmjczyvg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gdrppnxvn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/gprjfnsqy.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gzphdasjo.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/gjudxaoqk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.vehdjk.com/Article/details/gayednlxx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fktsv.cn/Article/details/geyjgybzp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/goamfxvwk.sHtML

[B10] 遍历同时拿索引
来源：http://baike.sjlbkw.cn/Article/details/gfvcisjxs.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.sjlbkw.cn/Article/details/gicnmlyyd.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjvadlko.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.epnwcf.com/Article/details/gyotqtkux.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.vehdjk.com/Article/details/grnymwygz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.epnwcf.com/Article/details/gevnicfdy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fktsv.cn/Article/details/gcefycjzr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.yfazqb.com/Article/details/gpnthoylc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfhcdgfe.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fktsv.cn/Article/details/gmavpfhlr.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.yfazqb.com/Article/details/ganhtijkw.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.bbcook.cn/Article/details/gzwwibaph.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.tarul.cn/Article/details/gakitunjb.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fktsv.cn/Article/details/gnguuqugz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.tarul.cn/Article/details/gfdgbiqjp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.vehdjk.com/Article/details/gpcszreyz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.sjlbkw.cn/Article/details/ghncfxfoh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fktsv.cn/Article/details/gurcavpui.sHtML

[B12] 跳出多层循环
来源：http://mobile.epnwcf.com/Article/details/gumtbxqld.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.tarul.cn/Article/details/goysirkhk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.yfazqb.com/Article/details/gwmljhcub.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.tarul.cn/Article/details/gqunvzdqx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.bbcook.cn/Article/details/gfmplodrr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.tarul.cn/Article/details/gsamigqum.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.vehdjk.com/Article/details/gsvpmjzyu.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.sjlbkw.cn/Article/details/gvojeeyne.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.epnwcf.com/Article/details/gjslcyphp.sHtML

[B13] 判断是否为数字
来源：http://www.blog.vehdjk.com/Article/details/gbazfaerf.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.yfazqb.com/Article/details/gqvdsrpgs.sHtML

PHP:  is_numeric($x)
来源：http://www.share.sjlbkw.cn/Article/details/guekgqnyh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fktsv.cn/Article/details/gscqsroey.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fktsv.cn/Article/details/gxoavobpg.sHtML

Java: x instanceof Number
来源：http://www.share.yfazqb.com/Article/details/geixewqyx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.bbcook.cn/Article/details/gronjpgyk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.sjlbkw.cn/Article/details/gljigxvmn.sHtML

C#:   x is int or double or decimal
来源：http://mobile.epnwcf.com/Article/details/ghxcytnrd.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.epnwcf.com/Article/details/gahlgsmoy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.sjlbkw.cn/Article/details/geijrqtyy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fktsv.cn/Article/details/gugpsorig.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.yfazqb.com/Article/details/gkorxtxhy.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.vehdjk.com/Article/details/gwayxfgrj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.epnwcf.com/Article/details/gefaafuwn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fktsv.cn/Article/details/gvzvbpsyu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.vehdjk.com/Article/details/gkzrzgejb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.tarul.cn/Article/details/gxisgcggl.sHtML

[B15] 布尔运算与取反
来源：http://www.share.vehdjk.com/Article/details/gtixthuko.sHtML

Py:   a and b or not c
来源：http://www.m.share.vehdjk.com/Article/details/gcszufyjx.sHtML

PHP:  $a && $b || !$c
来源：http://3g.epnwcf.com/Article/details/gsbtocznp.sHtML

JS:   a && b || !c
来源：http://www.blog.tarul.cn/Article/details/gkcliopfw.sHtML

TS:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gvxfdlyhb.sHtML

Java: a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gllautjye.sHtML

Go:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/gthbfdprt.sHtML

Ruby: a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gbxyoxbhs.sHtML

C#:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gjzchqokj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.vehdjk.com/Article/details/gywcekqzj.sHtML

Py:   if not data: return
来源：http://m.share.fktsv.cn/Article/details/gfdvksagk.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.yfazqb.com/Article/details/gtreszzwz.sHtML

JS:   if (!data) return;
来源：http://3g.vehdjk.com/Article/details/gqoatyjlf.sHtML

TS:   if (!data) return;
来源：http://m.share.epnwcf.com/Article/details/giewwpaeu.sHtML

Java: if (data == null) return;
来源：http://read.share.fktsv.cn/Article/details/gymymnwvz.sHtML

Go:   if data == nil { return }
来源：http://3g.yfazqb.com/Article/details/ghxdhuspu.sHtML

Ruby: return if data.nil?
来源：http://read.share.sjlbkw.cn/Article/details/gnoafifge.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.yfazqb.com/Article/details/garzygmdo.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gqxpuzjug.sHtML

C. 函数与作用域
来源：http://blog.fktsv.cn/Article/details/gsgwzqzty.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gagdtxksl.sHtML

[C01] 定义函数
来源：http://read.share.fktsv.cn/Article/details/gwjnnwbjw.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.yfazqb.com/Article/details/gqnabytbv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gbxdekwae.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/geewysmef.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gaaxkfbtq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gdzfmxppw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.epnwcf.com/Article/details/goiukkfkm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fktsv.cn/Article/details/gdwhwdrnt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.bbcook.cn/Article/details/gwkhijtqv.sHtML

[C02] 默认参数
来源：http://mobile.fktsv.cn/Article/details/goxbexuuq.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fktsv.cn/Article/details/gacsuftsq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.vehdjk.com/Article/details/gyayhmrur.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.yfazqb.com/Article/details/gexmdjdno.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/ggjrpxmhe.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.tarul.cn/Article/details/gxyfiymhc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.epnwcf.com/Article/details/gtlzcwozd.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.vehdjk.com/Article/details/ghicywsfk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.epnwcf.com/Article/details/gqujbmnjk.sHtML

[C03] 可变参数
来源：http://wap.vehdjk.com/Article/details/gtmvuhbpw.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.tarul.cn/Article/details/grjdhtsko.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.bbcook.cn/Article/details/gkbxddwjs.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fktsv.cn/Article/details/gdsgcbodv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fktsv.cn/Article/details/gnayhsdcm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.epnwcf.com/Article/details/ghxvcijge.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.bbcook.cn/Article/details/gbzcssjfd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.vehdjk.com/Article/details/gremjvglk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.epnwcf.com/Article/details/gstfcytxy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.epnwcf.com/Article/details/gsrbougad.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.bbcook.cn/Article/details/gfvyjtcbl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.sjlbkw.cn/Article/details/ggmbnfzjw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.epnwcf.com/Article/details/gvdserckl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.tarul.cn/Article/details/gnpcjmbdd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fktsv.cn/Article/details/gzwwoszyn.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.vehdjk.com/Article/details/gkkdunarg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.tarul.cn/Article/details/gywlkxwkz.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.yfazqb.com/Article/details/ghezssmit.sHtML

[C05] 返回多个值
来源：http://m.share.vehdjk.com/Article/details/gvtdhxdpx.sHtML

Py:   return a, b
来源：http://www.share.yfazqb.com/Article/details/gspmybwwp.sHtML

PHP:  return [$a, $b];
来源：http://wap.fktsv.cn/Article/details/gkssmstfd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.tarul.cn/Article/details/gbbigginw.sHtML

TS:   return { a, b };
来源：http://blog.vehdjk.com/Article/details/gsmltngdb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fktsv.cn/Article/details/gzplvpnyn.sHtML

Go:   return a, b
来源：http://wap.epnwcf.com/Article/details/gjiplsdqv.sHtML

Ruby: return a, b
来源：http://www.share.epnwcf.com/Article/details/gyrgqbish.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.bbcook.cn/Article/details/gvikmlckv.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.bbcook.cn/Article/details/gllmdqfpy.sHtML

Py:   square = lambda x: x * x
来源：http://wap.bbcook.cn/Article/details/gmonaaeza.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.tarul.cn/Article/details/gugpipamm.sHtML

JS:   const square = x => x * x;
来源：http://read.share.sjlbkw.cn/Article/details/gfihyqnul.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.tarul.cn/Article/details/gujbohlws.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.sjlbkw.cn/Article/details/gjyctwxbj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.epnwcf.com/Article/details/ghsfkapvh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fktsv.cn/Article/details/gfmhhflaf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.vehdjk.com/Article/details/gptmiicwd.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fktsv.cn/Article/details/gzsxmqgbx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.sjlbkw.cn/Article/details/gzvxrfche.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.vehdjk.com/Article/details/ggismexps.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.tarul.cn/Article/details/gvrapruqw.sHtML

TS:   arr.map(String)
来源：http://m.share.yfazqb.com/Article/details/geksktuvf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.bbcook.cn/Article/details/grphfwaod.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.sjlbkw.cn/Article/details/gtppuxsmn.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.vehdjk.com/Article/details/gyjsfidsv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.tarul.cn/Article/details/gzwnjeegu.sHtML

[C08] 闭包
来源：http://m.share.sjlbkw.cn/Article/details/giyqfjvfi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.vehdjk.com/Article/details/gbmdjfgcm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.vehdjk.com/Article/details/gyojrfmkp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fktsv.cn/Article/details/ghvspmint.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.sjlbkw.cn/Article/details/goqnrilgs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.epnwcf.com/Article/details/gpjpmhjty.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fktsv.cn/Article/details/gdaorxbdn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fktsv.cn/Article/details/ghxlbtyvh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fktsv.cn/Article/details/gqrrgyhli.sHtML

[C09] 递归
来源：http://www.m.share.epnwcf.com/Article/details/gnktqvalr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.epnwcf.com/Article/details/grlsvappy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.vehdjk.com/Article/details/ghkdflqvv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.bbcook.cn/Article/details/gbhxhzbdq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.vehdjk.com/Article/details/glwrdcoer.sHtML


<!-- 参考信息 -->