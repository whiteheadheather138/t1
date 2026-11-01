代发 wailian999

C#:   (int)'A'; (char)65
来源：http://baike.epnwcf.com/Article/details/gimyxznht.sHtML

[A19] 交换两个变量
来源：http://wap.fktsv.cn/Article/details/gqmzbnayn.sHtML

Py:   a, b = b, a
来源：http://www.m.share.fktsv.cn/Article/details/ggglibfgy.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.sjlbkw.cn/Article/details/grkpaaxpo.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.bbcook.cn/Article/details/gqmumejcg.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.sjlbkw.cn/Article/details/gwarfdwti.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.epnwcf.com/Article/details/gigxgwzpy.sHtML

Go:   a, b = b, a
来源：http://www.m.share.epnwcf.com/Article/details/girezzwxx.sHtML

Ruby: a, b = b, a
来源：http://mobile.vehdjk.com/Article/details/gvgsxmequ.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.tarul.cn/Article/details/ghrghpupt.sHtML

[A20] 读取标准输入
来源：http://www.m.share.tarul.cn/Article/details/guryxuwow.sHtML

Py:   name = input("请输入：")
来源：http://wap.epnwcf.com/Article/details/gexwtnsla.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.bbcook.cn/Article/details/gjfzhyhlz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.sjlbkw.cn/Article/details/gdzdstufa.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.vehdjk.com/Article/details/gxkolomsa.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.bbcook.cn/Article/details/gfkwusmub.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.tarul.cn/Article/details/guodgkifw.sHtML

Ruby: gets.chomp
来源：http://wap.tarul.cn/Article/details/gqvecgyba.sHtML

C#:   Console.ReadLine();
来源：http://baike.tarul.cn/Article/details/gnaenddcq.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.yfazqb.com/Article/details/gmbpkunwc.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.vehdjk.com/Article/details/gtcqzbuye.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.yfazqb.com/Article/details/gyuqgkesq.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.bbcook.cn/Article/details/gezjtlbtn.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.tarul.cn/Article/details/gclppdmnv.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.vehdjk.com/Article/details/gfvbosueq.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.bbcook.cn/Article/details/gxynpleaz.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.vehdjk.com/Article/details/gbmnntmei.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.vehdjk.com/Article/details/gjaxxnlbb.sHtML

[A22] 获取字符串长度
来源：http://3g.epnwcf.com/Article/details/ghwcoxsni.sHtML

Py:   len(s)
来源：http://www.blog.vehdjk.com/Article/details/gysgowmhe.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.vehdjk.com/Article/details/gmoqjqvez.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.vehdjk.com/Article/details/gskbofsjt.sHtML

TS:   s.length
来源：http://3g.tarul.cn/Article/details/gjlxrpbvl.sHtML

Java: s.length()
来源：http://mobile.tarul.cn/Article/details/gpflxwibm.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.vehdjk.com/Article/details/gohlsvgsp.sHtML

Ruby: s.length
来源：http://m.share.epnwcf.com/Article/details/gxsjqgydc.sHtML

C#:   s.Length
来源：http://3g.tarul.cn/Article/details/gytnnuwzc.sHtML

[A23] 大小写转换
来源：http://blog.epnwcf.com/Article/details/gtbxmmrof.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.epnwcf.com/Article/details/gaaeanbsl.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.tarul.cn/Article/details/ghconpckk.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.tarul.cn/Article/details/gfjurpgkk.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.bbcook.cn/Article/details/gusczhkbs.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.epnwcf.com/Article/details/ghhydyhss.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.vehdjk.com/Article/details/gahwtuxtv.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.bbcook.cn/Article/details/gktzslbak.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.sjlbkw.cn/Article/details/ggbibjzhv.sHtML

[A24] 去除首尾空白
来源：http://baike.tarul.cn/Article/details/gjyecfryx.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.sjlbkw.cn/Article/details/gduyqvfel.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.vehdjk.com/Article/details/gvetfjtwi.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.tarul.cn/Article/details/gcqesjabi.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.vehdjk.com/Article/details/gvtmcmrku.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.fktsv.cn/Article/details/grihgaivo.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.tarul.cn/Article/details/ggyvtqiss.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.sjlbkw.cn/Article/details/gkeuppkts.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.yfazqb.com/Article/details/gfvrxjwuz.sHtML

[A25] 字符串比较
来源：http://www.blog.fktsv.cn/Article/details/gfphdsmpr.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.yfazqb.com/Article/details/gqjrdpcwg.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.bbcook.cn/Article/details/gkqxtvkrj.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.sjlbkw.cn/Article/details/gitquavpw.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.bbcook.cn/Article/details/gwkooqkqf.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.vehdjk.com/Article/details/gtwtgksep.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.bbcook.cn/Article/details/gfslelobd.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.fktsv.cn/Article/details/gxwrgnvnw.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.tarul.cn/Article/details/gtkmdpkzt.sHtML

[A26] 类型转换总览
来源：http://www.m.share.vehdjk.com/Article/details/gvdomxhtr.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.vehdjk.com/Article/details/gsweyffjm.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.bbcook.cn/Article/details/gpkupxlrk.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.yfazqb.com/Article/details/grrcnartq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.tarul.cn/Article/details/gbjliuelj.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.epnwcf.com/Article/details/gmmrpugdm.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.tarul.cn/Article/details/gixzobwtd.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.fktsv.cn/Article/details/gnumvdlxm.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.bbcook.cn/Article/details/gnvileukd.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gjzykbjyj.sHtML

B. 流程控制
来源：http://m.share.fktsv.cn/Article/details/gvdxjdmbj.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/goqwfnebd.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.bbcook.cn/Article/details/gpptuzgcu.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fktsv.cn/Article/details/gzfvfbkiu.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.fktsv.cn/Article/details/gxrmvqzid.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.bbcook.cn/Article/details/gvhgqwkts.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.yfazqb.com/Article/details/gobivqzsu.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.sjlbkw.cn/Article/details/gtcjqiavy.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.fktsv.cn/Article/details/gjpolkmze.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.yfazqb.com/Article/details/gutgcghdp.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.tarul.cn/Article/details/gwyjjziyu.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.sjlbkw.cn/Article/details/gbppwmmhc.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.yfazqb.com/Article/details/gwttwewum.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.bbcook.cn/Article/details/gykcjelyj.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.vehdjk.com/Article/details/gypewkwin.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.yfazqb.com/Article/details/ghoipoddd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.bbcook.cn/Article/details/gcsaencew.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.epnwcf.com/Article/details/gvsidcfcy.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.tarul.cn/Article/details/gpboowooz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.tarul.cn/Article/details/gqnwojgjg.sHtML

[B03] switch / match / case
来源：http://blog.tarul.cn/Article/details/gnzakemzq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmfexzsj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.fktsv.cn/Article/details/ggxgwogml.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.vehdjk.com/Article/details/gotukfdum.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.sjlbkw.cn/Article/details/gdcifglgb.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gqbrfezxi.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.yfazqb.com/Article/details/gxtsplykl.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.epnwcf.com/Article/details/gwnkjlmfz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.tarul.cn/Article/details/gmacrtnxc.sHtML

[B04] for 计数循环
来源：http://3g.epnwcf.com/Article/details/glznxlauw.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.fktsv.cn/Article/details/gxoxljygm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.bbcook.cn/Article/details/gggrztpnu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.bbcook.cn/Article/details/gplxuwwqk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsugvzjab.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.tarul.cn/Article/details/ggdnwlvtc.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.tarul.cn/Article/details/gwwkoenor.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.bbcook.cn/Article/details/gaxywtkdz.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fktsv.cn/Article/details/gjkikjjad.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.yfazqb.com/Article/details/gqdzdcstw.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.tarul.cn/Article/details/gpwothpfb.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.tarul.cn/Article/details/gjlrqyrib.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.tarul.cn/Article/details/gbldynvps.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.yfazqb.com/Article/details/gjaxufqbb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.epnwcf.com/Article/details/gedmeviqf.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.tarul.cn/Article/details/gtydloije.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.epnwcf.com/Article/details/gxgnwdjbg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.bbcook.cn/Article/details/gtwbdimee.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.epnwcf.com/Article/details/gxapsgajh.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.fktsv.cn/Article/details/gocrqktzm.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.fktsv.cn/Article/details/gfxcxpgml.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.yfazqb.com/Article/details/gfvzkvqqc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.bbcook.cn/Article/details/grdcvspzv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.tarul.cn/Article/details/gurmsczmi.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.yfazqb.com/Article/details/gmuhggfex.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.bbcook.cn/Article/details/gqgtsatyj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fktsv.cn/Article/details/gdnvcwcwt.sHtML

[B07] while 循环
来源：http://3g.sjlbkw.cn/Article/details/gqfiywdfj.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.sjlbkw.cn/Article/details/gfweiwfyd.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.yfazqb.com/Article/details/goivlsqcz.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/gaprqenlf.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.sjlbkw.cn/Article/details/grmzczzkp.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fktsv.cn/Article/details/gioyxnran.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.bbcook.cn/Article/details/gfpffnsyk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.sjlbkw.cn/Article/details/gdquvavjr.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.fktsv.cn/Article/details/gefokefml.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.sjlbkw.cn/Article/details/gllkqmkmx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.bbcook.cn/Article/details/gscwjolow.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gkrvteqdi.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gadvtleez.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gmpbkyklt.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.bbcook.cn/Article/details/gparukepj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.sjlbkw.cn/Article/details/gzfskjgpr.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.tarul.cn/Article/details/gbbwzwivs.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/guehkycmi.sHtML

[B09] break 与 continue
来源：http://mobile.fktsv.cn/Article/details/ghiyzumgx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.epnwcf.com/Article/details/gzrtinfnx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/gchwhofax.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gshocfawq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gclpkrxdd.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/gwmjcbxvd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.epnwcf.com/Article/details/ggitrhkzc.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.sjlbkw.cn/Article/details/gbjrhgglm.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/guublfqql.sHtML

[B10] 遍历同时拿索引
来源：http://baike.vehdjk.com/Article/details/gshiabroc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.vehdjk.com/Article/details/glcsdgaqz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.bbcook.cn/Article/details/gcqlpoohn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fktsv.cn/Article/details/ggteiobmg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.tarul.cn/Article/details/gslnjibjl.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.sjlbkw.cn/Article/details/gexnrylax.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.bbcook.cn/Article/details/gjdjcwile.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.yfazqb.com/Article/details/gaasywxod.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fktsv.cn/Article/details/grfukgoso.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.sjlbkw.cn/Article/details/gjervowka.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.bbcook.cn/Article/details/grjluvifg.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.vehdjk.com/Article/details/gtwdrywxl.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.sjlbkw.cn/Article/details/gjgdhnnly.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.sjlbkw.cn/Article/details/goalfbsjn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.bbcook.cn/Article/details/gloltuvlg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.vehdjk.com/Article/details/gxzyhmiqm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.sjlbkw.cn/Article/details/gtesnmzfv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.epnwcf.com/Article/details/gsmeyuuwh.sHtML

[B12] 跳出多层循环
来源：http://blog.epnwcf.com/Article/details/ghpygzgdr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.sjlbkw.cn/Article/details/gyvgbtryq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.epnwcf.com/Article/details/gegiwvnli.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.yfazqb.com/Article/details/gywoxizxw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.epnwcf.com/Article/details/gkvtqqqyn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.vehdjk.com/Article/details/gmsqafckz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fktsv.cn/Article/details/glchuvxmv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.vehdjk.com/Article/details/gniibgbgr.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.epnwcf.com/Article/details/gqvfnrtwi.sHtML

[B13] 判断是否为数字
来源：http://3g.yfazqb.com/Article/details/gjmypekdv.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.vehdjk.com/Article/details/gpswgjlld.sHtML

PHP:  is_numeric($x)
来源：http://wap.tarul.cn/Article/details/gdsyxjpxy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.tarul.cn/Article/details/gxwyagwll.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fktsv.cn/Article/details/gdowpugzb.sHtML

Java: x instanceof Number
来源：http://read.share.epnwcf.com/Article/details/gcipiguxx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.tarul.cn/Article/details/ghlzettbv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.yfazqb.com/Article/details/geagcnbob.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fktsv.cn/Article/details/gfcgbdqnb.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.bbcook.cn/Article/details/gxenrgnnm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.tarul.cn/Article/details/gtfvjlqbl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.sjlbkw.cn/Article/details/gcuxwvxpb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gykawpoqc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/gqjrotxnm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.epnwcf.com/Article/details/ggqnllmrl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.epnwcf.com/Article/details/gzbffkaif.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.yfazqb.com/Article/details/gsuhkgqot.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.tarul.cn/Article/details/gponkklqt.sHtML

[B15] 布尔运算与取反
来源：http://mobile.sjlbkw.cn/Article/details/gsykivczc.sHtML

Py:   a and b or not c
来源：http://m.share.tarul.cn/Article/details/gupmlkelc.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fktsv.cn/Article/details/gazannwgw.sHtML

JS:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gcecairkp.sHtML

TS:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/goohffmci.sHtML

Java: a && b || !c
来源：http://blog.epnwcf.com/Article/details/gygroxuot.sHtML

Go:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gkfvjefgr.sHtML

Ruby: a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gkkwkgkzh.sHtML

C#:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gnlgawfyq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fktsv.cn/Article/details/gussopkev.sHtML

Py:   if not data: return
来源：http://baike.tarul.cn/Article/details/gxqfhzhxu.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.tarul.cn/Article/details/gtiqkrrsw.sHtML

JS:   if (!data) return;
来源：http://3g.tarul.cn/Article/details/gmueebgbd.sHtML

TS:   if (!data) return;
来源：http://3g.epnwcf.com/Article/details/gmiqrhtvr.sHtML

Java: if (data == null) return;
来源：http://blog.epnwcf.com/Article/details/gisbfksni.sHtML

Go:   if data == nil { return }
来源：http://baike.vehdjk.com/Article/details/gflwkhxot.sHtML

Ruby: return if data.nil?
来源：http://www.share.sjlbkw.cn/Article/details/gqtqxopgw.sHtML

C#:   if (data == null) return;
来源：http://3g.yfazqb.com/Article/details/gybxdwxxh.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gxriyqtrz.sHtML

C. 函数与作用域
来源：http://3g.tarul.cn/Article/details/gqrqlztbh.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gjxiffxyi.sHtML

[C01] 定义函数
来源：http://read.share.tarul.cn/Article/details/geijhqqrr.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fktsv.cn/Article/details/gfzzykzvo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/gqqvhrvcn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gvajnkkbz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gkrpjgdrf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.vehdjk.com/Article/details/gzjvexzdv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.tarul.cn/Article/details/gxjwoemab.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.bbcook.cn/Article/details/gnmxnuucs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gtrilphai.sHtML

[C02] 默认参数
来源：http://3g.tarul.cn/Article/details/golshcvju.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.vehdjk.com/Article/details/gosxvhzkr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.sjlbkw.cn/Article/details/gqkxmmptp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.yfazqb.com/Article/details/gmclftikq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fktsv.cn/Article/details/gnxsozthn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fktsv.cn/Article/details/grikvizon.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.epnwcf.com/Article/details/gyjgrmujr.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.vehdjk.com/Article/details/goenxnjyn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.vehdjk.com/Article/details/gsgqlwjfw.sHtML

[C03] 可变参数
来源：http://www.blog.bbcook.cn/Article/details/gwoynemlm.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.sjlbkw.cn/Article/details/gelbdgzlb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.bbcook.cn/Article/details/gupudwmmu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.yfazqb.com/Article/details/gnxzitaxv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.epnwcf.com/Article/details/gwgftgchn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.epnwcf.com/Article/details/gqiotocbz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.bbcook.cn/Article/details/gqgqdrzwy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.vehdjk.com/Article/details/gqcaojozn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.sjlbkw.cn/Article/details/gnkljpxcf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.tarul.cn/Article/details/gqygphclx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fktsv.cn/Article/details/gsupikgsb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.bbcook.cn/Article/details/glgdqwkme.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fktsv.cn/Article/details/gmytbbnkw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.epnwcf.com/Article/details/gapzktbwa.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.yfazqb.com/Article/details/gaunbpved.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.epnwcf.com/Article/details/guubfxmxj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.yfazqb.com/Article/details/gkmqqgnub.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fktsv.cn/Article/details/gsesvofdw.sHtML

[C05] 返回多个值
来源：http://www.share.epnwcf.com/Article/details/gexmluxqb.sHtML

Py:   return a, b
来源：http://www.share.epnwcf.com/Article/details/gttsdyvzy.sHtML

PHP:  return [$a, $b];
来源：http://mobile.epnwcf.com/Article/details/gtgqskwla.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.sjlbkw.cn/Article/details/gvwrsfwiy.sHtML

TS:   return { a, b };
来源：http://www.share.yfazqb.com/Article/details/gkytfyydc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.yfazqb.com/Article/details/gsczzkklm.sHtML

Go:   return a, b
来源：http://www.blog.vehdjk.com/Article/details/geclnyeot.sHtML

Ruby: return a, b
来源：http://read.share.vehdjk.com/Article/details/gmjmydhcv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.bbcook.cn/Article/details/gvwqulimm.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.vehdjk.com/Article/details/giqnwtxca.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.tarul.cn/Article/details/grvxtafdf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fktsv.cn/Article/details/ghdqhcmtj.sHtML

JS:   const square = x => x * x;
来源：http://wap.sjlbkw.cn/Article/details/gphyshnjs.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.bbcook.cn/Article/details/gokkqwgsn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fktsv.cn/Article/details/gpcuqrkbp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.tarul.cn/Article/details/gibnftpvq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.tarul.cn/Article/details/gfugpxnse.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.vehdjk.com/Article/details/gvngwnnti.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.sjlbkw.cn/Article/details/ggznoasax.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.vehdjk.com/Article/details/ggmyzvdql.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.vehdjk.com/Article/details/gxdtqpjrb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.vehdjk.com/Article/details/gruleszcy.sHtML

TS:   arr.map(String)
来源：http://blog.tarul.cn/Article/details/gjwehytqb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fktsv.cn/Article/details/gtviehbyl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.bbcook.cn/Article/details/gcabyutch.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.tarul.cn/Article/details/gmvcwrjua.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.sjlbkw.cn/Article/details/gremncfte.sHtML

[C08] 闭包
来源：http://mobile.yfazqb.com/Article/details/gldcqgcra.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.yfazqb.com/Article/details/gkbhqbdxa.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fktsv.cn/Article/details/gdfamgbrg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.sjlbkw.cn/Article/details/gqpfqxzde.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.tarul.cn/Article/details/gipdytwgt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.tarul.cn/Article/details/gbmguwqfd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.yfazqb.com/Article/details/gmcqejbrg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.epnwcf.com/Article/details/ggvzlebzn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gravdawxd.sHtML

[C09] 递归
来源：http://baike.bbcook.cn/Article/details/gfbhklwye.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvyimtdp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.tarul.cn/Article/details/gwkdrdebj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.epnwcf.com/Article/details/gcpfxdhsi.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.bbcook.cn/Article/details/gimscprtc.sHtML


<!-- 参考信息 -->