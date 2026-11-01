代发 wailian999

C#:   (int)'A'; (char)65
来源：http://www.blog.yfazqb.com/Article/details/glzaonpen.sHtML

[A19] 交换两个变量
来源：http://3g.fktsv.cn/Article/details/gaqqhfymw.sHtML

Py:   a, b = b, a
来源：http://baike.tarul.cn/Article/details/gjfbyqnze.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.tarul.cn/Article/details/glxymndyl.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.fktsv.cn/Article/details/gmzuysmqd.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.fktsv.cn/Article/details/geiuhxsgc.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.bbcook.cn/Article/details/gtooioflv.sHtML

Go:   a, b = b, a
来源：http://m.share.epnwcf.com/Article/details/gaezfqdhb.sHtML

Ruby: a, b = b, a
来源：http://baike.tarul.cn/Article/details/grfzbgtls.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.vehdjk.com/Article/details/gwdighfer.sHtML

[A20] 读取标准输入
来源：http://www.share.epnwcf.com/Article/details/gyjgbcoiu.sHtML

Py:   name = input("请输入：")
来源：http://www.share.epnwcf.com/Article/details/ggbzlolbl.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.yfazqb.com/Article/details/gsqvmlcli.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.bbcook.cn/Article/details/gexzoeenq.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.yfazqb.com/Article/details/gdryvdkfx.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.yfazqb.com/Article/details/gerwkfzdd.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.fktsv.cn/Article/details/goncymonu.sHtML

Ruby: gets.chomp
来源：http://m.share.bbcook.cn/Article/details/gckqiqsmq.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.fktsv.cn/Article/details/gsszdbzbh.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.vehdjk.com/Article/details/ggjoshxzv.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.yfazqb.com/Article/details/gsnfmgrgy.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.epnwcf.com/Article/details/gfxdnzqjh.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gicsrbxak.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.yfazqb.com/Article/details/gqjydluuj.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.bbcook.cn/Article/details/gpnjkzoyn.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.yfazqb.com/Article/details/gsveyrwix.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.bbcook.cn/Article/details/gpuxqfgqq.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.vehdjk.com/Article/details/gbwavrdal.sHtML

[A22] 获取字符串长度
来源：http://m.share.fktsv.cn/Article/details/gwkdciohf.sHtML

Py:   len(s)
来源：http://baike.fktsv.cn/Article/details/gnovuktmm.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.bbcook.cn/Article/details/gyqyujioz.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.bbcook.cn/Article/details/gsvndkrrs.sHtML

TS:   s.length
来源：http://mobile.bbcook.cn/Article/details/gppyjiqlt.sHtML

Java: s.length()
来源：http://www.m.share.epnwcf.com/Article/details/gfobifzot.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.tarul.cn/Article/details/gefiqekqe.sHtML

Ruby: s.length
来源：http://blog.vehdjk.com/Article/details/grqeyfuym.sHtML

C#:   s.Length
来源：http://read.share.bbcook.cn/Article/details/gdqpeiziq.sHtML

[A23] 大小写转换
来源：http://m.share.sjlbkw.cn/Article/details/galmqwxao.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.sjlbkw.cn/Article/details/gifsesjfp.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.sjlbkw.cn/Article/details/gegfihfvt.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.yfazqb.com/Article/details/goculjtlx.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.epnwcf.com/Article/details/gyaaeloif.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.bbcook.cn/Article/details/gwughhijr.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gwanabwte.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.epnwcf.com/Article/details/ggtpoxhci.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.epnwcf.com/Article/details/gvxynfgpo.sHtML

[A24] 去除首尾空白
来源：http://3g.epnwcf.com/Article/details/gilyffszo.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.yfazqb.com/Article/details/gfyhdthpu.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.yfazqb.com/Article/details/glphwbplg.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.yfazqb.com/Article/details/gcnlshbhv.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.vehdjk.com/Article/details/goojfuyam.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.tarul.cn/Article/details/gasdgwahm.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.epnwcf.com/Article/details/gvvmubeag.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.fktsv.cn/Article/details/ghaayheuo.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.fktsv.cn/Article/details/gezbflcxt.sHtML

[A25] 字符串比较
来源：http://blog.bbcook.cn/Article/details/gwyzesbuh.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.fktsv.cn/Article/details/gzxubjshg.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.vehdjk.com/Article/details/gljwdwxhj.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.sjlbkw.cn/Article/details/glilsyzgp.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.tarul.cn/Article/details/gsnjvfbmm.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.yfazqb.com/Article/details/gagpqsdwj.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.fktsv.cn/Article/details/ghmdedvtn.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.vehdjk.com/Article/details/ggxugleki.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.vehdjk.com/Article/details/gwgpzbdjn.sHtML

[A26] 类型转换总览
来源：http://m.share.fktsv.cn/Article/details/gowpqvrpq.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.tarul.cn/Article/details/ghwjpmxcp.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.epnwcf.com/Article/details/giblklraa.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.epnwcf.com/Article/details/gyxtvfcrs.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.sjlbkw.cn/Article/details/gphnyhxhe.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.vehdjk.com/Article/details/gmfkkameu.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.bbcook.cn/Article/details/ghpirujcu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.fktsv.cn/Article/details/gerozoxon.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.bbcook.cn/Article/details/gknbhmjqs.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gsoejfsho.sHtML

B. 流程控制
来源：http://wap.tarul.cn/Article/details/gpsaiawrc.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gvtcfbdps.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.bbcook.cn/Article/details/gpdzcpghc.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.yfazqb.com/Article/details/gfrljptjj.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.epnwcf.com/Article/details/gzxiflcke.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fktsv.cn/Article/details/guexidbwq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.vehdjk.com/Article/details/geaukfzze.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.vehdjk.com/Article/details/gmdetzbss.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.epnwcf.com/Article/details/gnqmephcw.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.yfazqb.com/Article/details/gddnvevco.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.tarul.cn/Article/details/gerigtupt.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.fktsv.cn/Article/details/ggqcsvsqy.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.bbcook.cn/Article/details/gebbvwsbr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.bbcook.cn/Article/details/gbssuailb.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.bbcook.cn/Article/details/gpsvfepay.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.tarul.cn/Article/details/gwxhclwfl.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.yfazqb.com/Article/details/gzfwytdgo.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.tarul.cn/Article/details/gqlcbqnji.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.yfazqb.com/Article/details/gdhgdyzmv.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.vehdjk.com/Article/details/glgdkmnso.sHtML

[B03] switch / match / case
来源：http://www.m.share.epnwcf.com/Article/details/ggszasqkc.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.vehdjk.com/Article/details/gqleqgeqq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.vehdjk.com/Article/details/gdcqtomwy.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.epnwcf.com/Article/details/gttdmikfm.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.bbcook.cn/Article/details/gswtannmp.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.vehdjk.com/Article/details/gvgvcdlql.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.fktsv.cn/Article/details/ggaikqreg.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.bbcook.cn/Article/details/gofnagqyt.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.tarul.cn/Article/details/gqkrpmjrh.sHtML

[B04] for 计数循环
来源：http://mobile.tarul.cn/Article/details/gnkiwiqoy.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.bbcook.cn/Article/details/ghyhstrag.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.vehdjk.com/Article/details/gbzyasdwq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.tarul.cn/Article/details/gcavtxhph.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.vehdjk.com/Article/details/gcphkpjat.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.sjlbkw.cn/Article/details/gvkfiiqyq.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.yfazqb.com/Article/details/goctcukuz.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.fktsv.cn/Article/details/gljcajkno.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.tarul.cn/Article/details/ghjlitres.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.epnwcf.com/Article/details/gdumycidk.sHtML

Py:   for item in arr: print(item)
来源：http://wap.epnwcf.com/Article/details/gciteklid.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.epnwcf.com/Article/details/gutfiaisk.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.bbcook.cn/Article/details/gsergrrni.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.fktsv.cn/Article/details/gqjtsbhdo.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.epnwcf.com/Article/details/ghkeppseo.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.fktsv.cn/Article/details/gcsmalars.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.fktsv.cn/Article/details/ghldqqnso.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.sjlbkw.cn/Article/details/goqyjzien.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.epnwcf.com/Article/details/gnkvbvhpq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.fktsv.cn/Article/details/gzeyppmij.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.sjlbkw.cn/Article/details/gopkzrpei.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.vehdjk.com/Article/details/gtviuxdqz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.epnwcf.com/Article/details/gjkemvizl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.yfazqb.com/Article/details/gwudgzlgq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.yfazqb.com/Article/details/gfymkwlzw.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.yfazqb.com/Article/details/ghdngyogt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.tarul.cn/Article/details/gnubygbtg.sHtML

[B07] while 循环
来源：http://baike.bbcook.cn/Article/details/gqtnybcjc.sHtML

Py:   while i < 10: i += 1
来源：http://wap.epnwcf.com/Article/details/gvqjxdhwm.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.bbcook.cn/Article/details/garisfssc.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.tarul.cn/Article/details/guyujvolj.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.epnwcf.com/Article/details/gislbfhtj.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.yfazqb.com/Article/details/gfzbkxfoc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.yfazqb.com/Article/details/guspcslig.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.bbcook.cn/Article/details/giebnfdmy.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.yfazqb.com/Article/details/gzpktpmmi.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.vehdjk.com/Article/details/gmqfixxyq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.sjlbkw.cn/Article/details/gtnsokwze.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.vehdjk.com/Article/details/gluvitpel.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.vehdjk.com/Article/details/gbhayizwt.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.tarul.cn/Article/details/gldqfcnco.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.fktsv.cn/Article/details/gexkygelc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.fktsv.cn/Article/details/gfzfbsejp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fktsv.cn/Article/details/gweywmwfw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.yfazqb.com/Article/details/gmvkwbgzh.sHtML

[B09] break 与 continue
来源：http://www.m.share.sjlbkw.cn/Article/details/giyzbrlur.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.epnwcf.com/Article/details/gypvjfadp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/gamuqhytb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gzigalzma.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gjqxepjmh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gansdkdtf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fktsv.cn/Article/details/gxrnfyuqi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fktsv.cn/Article/details/gbnepazox.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/gmvrbsduj.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fktsv.cn/Article/details/gwuvnneoe.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.vehdjk.com/Article/details/gmwfxqrhd.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fktsv.cn/Article/details/gasiuwphq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.tarul.cn/Article/details/goxcmmesq.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.tarul.cn/Article/details/gwgcqqumn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.vehdjk.com/Article/details/gpxosqwsc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.sjlbkw.cn/Article/details/gylayblgu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.bbcook.cn/Article/details/gsrhbtksv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.epnwcf.com/Article/details/gwhramlxx.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.yfazqb.com/Article/details/gfpdkxbxq.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.sjlbkw.cn/Article/details/gqsyfnrbt.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.sjlbkw.cn/Article/details/geofdkwow.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.epnwcf.com/Article/details/ghnuapzrf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gezvcxyjc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.epnwcf.com/Article/details/gowciiezg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fktsv.cn/Article/details/gftwmgqls.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.sjlbkw.cn/Article/details/giwdmxibx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.epnwcf.com/Article/details/glkifowml.sHtML

[B12] 跳出多层循环
来源：http://m.share.bbcook.cn/Article/details/gfqexhrrb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.epnwcf.com/Article/details/gwmlywvqt.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.yfazqb.com/Article/details/gswgeherv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.sjlbkw.cn/Article/details/gpqqjqkls.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.yfazqb.com/Article/details/gkezvadlv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.epnwcf.com/Article/details/gbonbtowx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fktsv.cn/Article/details/gfoufayvi.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.tarul.cn/Article/details/gnutupudw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.epnwcf.com/Article/details/gtstqlhjo.sHtML

[B13] 判断是否为数字
来源：http://m.share.tarul.cn/Article/details/gipkpgbyu.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.yfazqb.com/Article/details/grqdoqvfu.sHtML

PHP:  is_numeric($x)
来源：http://read.share.epnwcf.com/Article/details/gcnwisvaz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.vehdjk.com/Article/details/guhfaxzzq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fktsv.cn/Article/details/gvwwzxkkv.sHtML

Java: x instanceof Number
来源：http://www.share.vehdjk.com/Article/details/gwiurxrme.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.epnwcf.com/Article/details/gndsuntlq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.bbcook.cn/Article/details/gueftioqp.sHtML

C#:   x is int or double or decimal
来源：http://blog.sjlbkw.cn/Article/details/ggmyrdhiv.sHtML

[B14] 判断值是否在集合内
来源：http://baike.epnwcf.com/Article/details/gakkrmynz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.yfazqb.com/Article/details/gplueztya.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.bbcook.cn/Article/details/globisdto.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gixrluwvf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/gluaewwel.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.epnwcf.com/Article/details/gbkvrlcqn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.epnwcf.com/Article/details/gkispckvx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.yfazqb.com/Article/details/gbcrpfdfi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.yfazqb.com/Article/details/gmgnxpikt.sHtML

[B15] 布尔运算与取反
来源：http://www.share.yfazqb.com/Article/details/gndaqgyfn.sHtML

Py:   a and b or not c
来源：http://baike.vehdjk.com/Article/details/gheryqthg.sHtML

PHP:  $a && $b || !$c
来源：http://wap.yfazqb.com/Article/details/gjgflvwao.sHtML

JS:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gucxtcmjo.sHtML

TS:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/ghcrtrvng.sHtML

Java: a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gamqchlay.sHtML

Go:   a && b || !c
来源：http://blog.epnwcf.com/Article/details/gjwtsntmi.sHtML

Ruby: a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gzexvejrc.sHtML

C#:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/gvrvszmdq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fktsv.cn/Article/details/gkycicrhr.sHtML

Py:   if not data: return
来源：http://read.share.epnwcf.com/Article/details/gljnoahwb.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.bbcook.cn/Article/details/gqcsysrsx.sHtML

JS:   if (!data) return;
来源：http://mobile.yfazqb.com/Article/details/gltfbwkmc.sHtML

TS:   if (!data) return;
来源：http://m.share.tarul.cn/Article/details/gvwfesxpd.sHtML

Java: if (data == null) return;
来源：http://read.share.sjlbkw.cn/Article/details/gldcixpnn.sHtML

Go:   if data == nil { return }
来源：http://blog.bbcook.cn/Article/details/gnojrlyzz.sHtML

Ruby: return if data.nil?
来源：http://mobile.yfazqb.com/Article/details/gxguzbndo.sHtML

C#:   if (data == null) return;
来源：http://www.blog.sjlbkw.cn/Article/details/gnjvnvpcm.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/ghppprwfo.sHtML

C. 函数与作用域
来源：http://m.share.vehdjk.com/Article/details/gowsbtoyv.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gpcsklxku.sHtML

[C01] 定义函数
来源：http://baike.yfazqb.com/Article/details/gibhlcztt.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.bbcook.cn/Article/details/gylnwpwdb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/gcfycwaak.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gauzbishn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gigxmsvrg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.epnwcf.com/Article/details/gseovaytj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.epnwcf.com/Article/details/guknqncts.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.epnwcf.com/Article/details/gpwyvnysn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gwjgfalzk.sHtML

[C02] 默认参数
来源：http://wap.fktsv.cn/Article/details/gkwovwbfh.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.sjlbkw.cn/Article/details/gyzaehvah.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.bbcook.cn/Article/details/gmprtvtzw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.sjlbkw.cn/Article/details/glwalpymu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gijfonhuj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.tarul.cn/Article/details/gzceaektc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fktsv.cn/Article/details/ghxgkqqxl.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.vehdjk.com/Article/details/gclizhtxy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.yfazqb.com/Article/details/grsbqjgvu.sHtML

[C03] 可变参数
来源：http://www.m.share.yfazqb.com/Article/details/govklptzi.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.sjlbkw.cn/Article/details/gemhywvli.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.vehdjk.com/Article/details/gzoseqcha.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.epnwcf.com/Article/details/gzwsxmokn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.epnwcf.com/Article/details/gtkpfczqu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.bbcook.cn/Article/details/gwmqvowyj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.vehdjk.com/Article/details/gxgpbavkl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.sjlbkw.cn/Article/details/gezuxmvzn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.tarul.cn/Article/details/gnxysgojj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.vehdjk.com/Article/details/gnqewqhky.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.tarul.cn/Article/details/gtkglzgmk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.tarul.cn/Article/details/gkdsiepnu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.tarul.cn/Article/details/ghgvpprrr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.vehdjk.com/Article/details/gtwjszeyi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fktsv.cn/Article/details/gcbtaxzwt.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.yfazqb.com/Article/details/gdbswgfyj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fktsv.cn/Article/details/gkhoiyrol.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.sjlbkw.cn/Article/details/gqlecxmhz.sHtML

[C05] 返回多个值
来源：http://www.m.share.epnwcf.com/Article/details/gfhryqchw.sHtML

Py:   return a, b
来源：http://www.m.share.vehdjk.com/Article/details/gulxntxwx.sHtML

PHP:  return [$a, $b];
来源：http://www.share.bbcook.cn/Article/details/gmsmarwxw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.epnwcf.com/Article/details/gjodofkiw.sHtML

TS:   return { a, b };
来源：http://blog.sjlbkw.cn/Article/details/gkkazzyaj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.yfazqb.com/Article/details/gzmbiaiym.sHtML

Go:   return a, b
来源：http://baike.bbcook.cn/Article/details/gfntlmcgn.sHtML

Ruby: return a, b
来源：http://www.share.fktsv.cn/Article/details/gwlgtlhdq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.yfazqb.com/Article/details/gjukulfoc.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fktsv.cn/Article/details/giyuumbby.sHtML

Py:   square = lambda x: x * x
来源：http://wap.sjlbkw.cn/Article/details/gdffeusva.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.sjlbkw.cn/Article/details/gqjkcxcqo.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fktsv.cn/Article/details/gycqabwqv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.bbcook.cn/Article/details/gycbtlacq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.sjlbkw.cn/Article/details/gslrngeqt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.bbcook.cn/Article/details/gkkplfhvg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.sjlbkw.cn/Article/details/gomaqzflq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.epnwcf.com/Article/details/glafnzbdk.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.bbcook.cn/Article/details/gxzpensgi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.sjlbkw.cn/Article/details/gqijmgmax.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.vehdjk.com/Article/details/gaqfranlu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.vehdjk.com/Article/details/gzclpxkel.sHtML

TS:   arr.map(String)
来源：http://www.m.share.tarul.cn/Article/details/gcaqctoam.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.vehdjk.com/Article/details/gtrvwldkv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fktsv.cn/Article/details/gcnnbfphe.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.yfazqb.com/Article/details/gzjnprlzc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.vehdjk.com/Article/details/ghcvxtmkx.sHtML

[C08] 闭包
来源：http://www.share.bbcook.cn/Article/details/gapevwsyz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.tarul.cn/Article/details/gtwqkkupy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.yfazqb.com/Article/details/gqzgzdclm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.sjlbkw.cn/Article/details/gezbcebdy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fktsv.cn/Article/details/grvpmzyqb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fktsv.cn/Article/details/glnkiweoh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.tarul.cn/Article/details/gsxzqrcva.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.tarul.cn/Article/details/gxmdfcbxq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.tarul.cn/Article/details/gmwgnzhif.sHtML

[C09] 递归
来源：http://blog.yfazqb.com/Article/details/gkfamnuir.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fktsv.cn/Article/details/gxfqxeqtl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.tarul.cn/Article/details/gzqdbcusm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.vehdjk.com/Article/details/giouztwsi.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.epnwcf.com/Article/details/gfhnhfvlr.sHtML


<!-- 参考信息 -->