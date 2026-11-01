代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.bbcook.cn/Article/details/gmujpqyet.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.vehdjk.com/Article/details/gsfyrsuex.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.vehdjk.com/Article/details/gcizmfjjh.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.epnwcf.com/Article/details/gzwixryno.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.bbcook.cn/Article/details/ganyoclcm.sHtML

Ruby: gets.chomp
来源：http://read.share.tarul.cn/Article/details/ghivlgdlv.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.tarul.cn/Article/details/ghtntpjxr.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.yfazqb.com/Article/details/gwnkdhhod.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.yfazqb.com/Article/details/gxfztezar.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.sjlbkw.cn/Article/details/grztttzgu.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.yfazqb.com/Article/details/gspxvnqgr.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.bbcook.cn/Article/details/giszchdmm.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.sjlbkw.cn/Article/details/ghyrstvmi.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.fktsv.cn/Article/details/gvzoivtgq.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.sjlbkw.cn/Article/details/gfepznqow.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.epnwcf.com/Article/details/gyyirzxzk.sHtML

[A22] 获取字符串长度
来源：http://mobile.bbcook.cn/Article/details/guusgijgf.sHtML

Py:   len(s)
来源：http://www.blog.epnwcf.com/Article/details/gpoqngbwr.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.tarul.cn/Article/details/gzmbrjpao.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.fktsv.cn/Article/details/gjudcmpkn.sHtML

TS:   s.length
来源：http://mobile.epnwcf.com/Article/details/gfckprgrw.sHtML

Java: s.length()
来源：http://www.blog.bbcook.cn/Article/details/gdnynovqs.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.tarul.cn/Article/details/gvbiguraw.sHtML

Ruby: s.length
来源：http://wap.tarul.cn/Article/details/glofdtpan.sHtML

C#:   s.Length
来源：http://www.blog.fktsv.cn/Article/details/grqionpaj.sHtML

[A23] 大小写转换
来源：http://www.blog.sjlbkw.cn/Article/details/gbuholsgu.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.epnwcf.com/Article/details/gxrptfspp.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.vehdjk.com/Article/details/gpftphlrs.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.bbcook.cn/Article/details/gehdhydvw.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.sjlbkw.cn/Article/details/ghcufrbwb.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.vehdjk.com/Article/details/gppvloarl.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.bbcook.cn/Article/details/gtqijbepk.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.fktsv.cn/Article/details/gtkzhxmgq.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.yfazqb.com/Article/details/gggsbznpd.sHtML

[A24] 去除首尾空白
来源：http://m.share.bbcook.cn/Article/details/gmzwlrvfn.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.fktsv.cn/Article/details/gkaevrzvw.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.bbcook.cn/Article/details/gjvgsdwki.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.sjlbkw.cn/Article/details/gdjgujgqh.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fktsv.cn/Article/details/guwccdjnn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.vehdjk.com/Article/details/gihzvjith.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.sjlbkw.cn/Article/details/grgyvbrny.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.bbcook.cn/Article/details/gurqvueum.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.yfazqb.com/Article/details/gbrpckane.sHtML

[A25] 字符串比较
来源：http://blog.vehdjk.com/Article/details/gcwrnpttj.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.vehdjk.com/Article/details/grqhtfvhu.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.vehdjk.com/Article/details/gxbaximvx.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.epnwcf.com/Article/details/gnrdrzfen.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.tarul.cn/Article/details/gmzlepcwz.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.fktsv.cn/Article/details/ghfxxshjt.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.tarul.cn/Article/details/gaqkdgcnt.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.epnwcf.com/Article/details/gvenruhop.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.sjlbkw.cn/Article/details/gwwowexnt.sHtML

[A26] 类型转换总览
来源：http://mobile.sjlbkw.cn/Article/details/gkdfuqzrw.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.sjlbkw.cn/Article/details/grbbotbbu.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.vehdjk.com/Article/details/gxliryhcc.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.yfazqb.com/Article/details/ginkbmnob.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.vehdjk.com/Article/details/gauevqnct.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.yfazqb.com/Article/details/gazzvhwpq.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.vehdjk.com/Article/details/gpbrddskp.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.sjlbkw.cn/Article/details/glplnejdc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.vehdjk.com/Article/details/gziuygeul.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gvmcexjjf.sHtML

B. 流程控制
来源：http://m.share.epnwcf.com/Article/details/gacwkkrrb.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/guyvccnhs.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.tarul.cn/Article/details/gbeevhzgj.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.fktsv.cn/Article/details/gxaizadbg.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.yfazqb.com/Article/details/gjvcuiuyx.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.sjlbkw.cn/Article/details/goozhbtxs.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.tarul.cn/Article/details/glxcwalug.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.vehdjk.com/Article/details/gkjgcctbe.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.vehdjk.com/Article/details/ggktzofrg.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.bbcook.cn/Article/details/gaqqmlati.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.vehdjk.com/Article/details/guiyibdnn.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.epnwcf.com/Article/details/gzphslmdc.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.sjlbkw.cn/Article/details/gvxavpsqw.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.vehdjk.com/Article/details/gbzoizuma.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.epnwcf.com/Article/details/gedpbcgke.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.vehdjk.com/Article/details/gflldafbt.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.vehdjk.com/Article/details/gdxsecvjw.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.bbcook.cn/Article/details/gamptbtqx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.sjlbkw.cn/Article/details/gwpzlphvz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.yfazqb.com/Article/details/grlnatikg.sHtML

[B03] switch / match / case
来源：http://wap.epnwcf.com/Article/details/gbpwkcqxu.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.epnwcf.com/Article/details/gmbxbtakw.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/gzybymgze.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.epnwcf.com/Article/details/gwlzfxbjv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.epnwcf.com/Article/details/gnspcqndp.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.yfazqb.com/Article/details/gputhgriy.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.tarul.cn/Article/details/gmspppwfe.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.fktsv.cn/Article/details/gyrjnczyb.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.vehdjk.com/Article/details/gvoytvyos.sHtML

[B04] for 计数循环
来源：http://www.blog.epnwcf.com/Article/details/gsddgbuzi.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.yfazqb.com/Article/details/gyqbnirak.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.vehdjk.com/Article/details/gkltzruay.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.epnwcf.com/Article/details/grfpzkpsm.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.yfazqb.com/Article/details/gokqxgvfr.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fktsv.cn/Article/details/gqisyhvwn.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.fktsv.cn/Article/details/gtdmiqpwj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.vehdjk.com/Article/details/gsmvhllqf.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.epnwcf.com/Article/details/geizrekky.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.epnwcf.com/Article/details/ghqopauli.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.sjlbkw.cn/Article/details/gxdszvxcu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.fktsv.cn/Article/details/gcdpiaxac.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.yfazqb.com/Article/details/gfylbncbz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.epnwcf.com/Article/details/gsiyihswg.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.epnwcf.com/Article/details/gdmscppuz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.vehdjk.com/Article/details/gkiytnoyf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.bbcook.cn/Article/details/gvlazhoec.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.epnwcf.com/Article/details/gdaxvklba.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.fktsv.cn/Article/details/grtqzdcml.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.vehdjk.com/Article/details/goafwojkw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.yfazqb.com/Article/details/gtniifrlp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.sjlbkw.cn/Article/details/gujjvrofx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.sjlbkw.cn/Article/details/gqfwdatpm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.bbcook.cn/Article/details/gbxujgzev.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.tarul.cn/Article/details/gsbjipmxy.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.tarul.cn/Article/details/gzxwqczhs.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.yfazqb.com/Article/details/ggnkzyski.sHtML

[B07] while 循环
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwvogysr.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.sjlbkw.cn/Article/details/gwlifcywp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.vehdjk.com/Article/details/glstxuend.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gscoqbaga.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.vehdjk.com/Article/details/gqnfeggpt.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/gbrlhytku.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.vehdjk.com/Article/details/gshgpnytp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.vehdjk.com/Article/details/gsfpiymup.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.sjlbkw.cn/Article/details/glyhbxolm.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.fktsv.cn/Article/details/gmjftvapd.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.fktsv.cn/Article/details/gniqruhtb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.epnwcf.com/Article/details/gmfaaeadg.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.bbcook.cn/Article/details/guubixsab.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbmblrgo.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/garnnyvka.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.tarul.cn/Article/details/gmnpgemym.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.yfazqb.com/Article/details/gbqrjqndt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gviwbocdt.sHtML

[B09] break 与 continue
来源：http://mobile.bbcook.cn/Article/details/gdlqvgetz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.yfazqb.com/Article/details/gnfjskltd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.bbcook.cn/Article/details/ghahewsil.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gtaaxitxq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/gedbyvwgc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gnjgszpit.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.sjlbkw.cn/Article/details/gscwbnjiz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.bbcook.cn/Article/details/gxjfgtfpg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.tarul.cn/Article/details/gcdmgtmgk.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.tarul.cn/Article/details/gpwuccxuc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.bbcook.cn/Article/details/gnxsoguoe.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.yfazqb.com/Article/details/gsburoevz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.epnwcf.com/Article/details/gxuifjopz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.vehdjk.com/Article/details/gobmjeujr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.yfazqb.com/Article/details/gokaxozce.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.bbcook.cn/Article/details/guauacbxm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.yfazqb.com/Article/details/gvmlsnnbl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fktsv.cn/Article/details/guwjjgtrl.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.bbcook.cn/Article/details/gehlutymt.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.vehdjk.com/Article/details/gltgqckpl.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.sjlbkw.cn/Article/details/gcdzfpyor.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.tarul.cn/Article/details/gocnylkbu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.yfazqb.com/Article/details/gmpcrbpan.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.bbcook.cn/Article/details/ggtdydvxt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.vehdjk.com/Article/details/gwayobbri.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.yfazqb.com/Article/details/gcmllklwv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fktsv.cn/Article/details/giqyhgshw.sHtML

[B12] 跳出多层循环
来源：http://m.share.tarul.cn/Article/details/gthaxlebs.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.sjlbkw.cn/Article/details/gyktisbiz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.yfazqb.com/Article/details/gfpycyiat.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gyenxfbhh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gstpsbzxe.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fktsv.cn/Article/details/gqosmekmi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.epnwcf.com/Article/details/goaceperz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.tarul.cn/Article/details/gfocwpsjq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.bbcook.cn/Article/details/gczuzkvxa.sHtML

[B13] 判断是否为数字
来源：http://read.share.epnwcf.com/Article/details/gtmttrcpi.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fktsv.cn/Article/details/glfoheorw.sHtML

PHP:  is_numeric($x)
来源：http://blog.yfazqb.com/Article/details/gswapkkis.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.sjlbkw.cn/Article/details/gxhpkvplk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwqtlxtc.sHtML

Java: x instanceof Number
来源：http://3g.fktsv.cn/Article/details/gzaqifqwc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.sjlbkw.cn/Article/details/giabjnoxw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.epnwcf.com/Article/details/gytdrpfvv.sHtML

C#:   x is int or double or decimal
来源：http://mobile.vehdjk.com/Article/details/gskikroiu.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.epnwcf.com/Article/details/gdlcoiuhy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.bbcook.cn/Article/details/gzrnnmemi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.epnwcf.com/Article/details/ghouyfndb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gywzvychp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fktsv.cn/Article/details/gdtbilhsb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.vehdjk.com/Article/details/ghqjaqtdx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.tarul.cn/Article/details/gsphfrrqo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.epnwcf.com/Article/details/ghdinfuii.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.tarul.cn/Article/details/gznyyxujb.sHtML

[B15] 布尔运算与取反
来源：http://wap.yfazqb.com/Article/details/gqkktegbk.sHtML

Py:   a and b or not c
来源：http://www.blog.vehdjk.com/Article/details/gmdfekwzv.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.yfazqb.com/Article/details/gzhuekeeb.sHtML

JS:   a && b || !c
来源：http://baike.tarul.cn/Article/details/gqkmbmfnf.sHtML

TS:   a && b || !c
来源：http://m.share.fktsv.cn/Article/details/gbfaeulvx.sHtML

Java: a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gdfonjsuc.sHtML

Go:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/gyifnrtya.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gdvqpkqzr.sHtML

C#:   a && b || !c
来源：http://wap.vehdjk.com/Article/details/gccmxcqbg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fktsv.cn/Article/details/gskiyrhic.sHtML

Py:   if not data: return
来源：http://wap.fktsv.cn/Article/details/gdopieobh.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.tarul.cn/Article/details/gyjcfvsgn.sHtML

JS:   if (!data) return;
来源：http://3g.epnwcf.com/Article/details/grglekrpj.sHtML

TS:   if (!data) return;
来源：http://3g.bbcook.cn/Article/details/gcysntkyr.sHtML

Java: if (data == null) return;
来源：http://read.share.sjlbkw.cn/Article/details/gtmqfuebl.sHtML

Go:   if data == nil { return }
来源：http://baike.yfazqb.com/Article/details/ggngofglj.sHtML

Ruby: return if data.nil?
来源：http://m.share.fktsv.cn/Article/details/gbaokatkf.sHtML

C#:   if (data == null) return;
来源：http://wap.tarul.cn/Article/details/gxmwfumqn.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gtgwgbkpy.sHtML

C. 函数与作用域
来源：http://blog.yfazqb.com/Article/details/godtoyxpo.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gwotlusgw.sHtML

[C01] 定义函数
来源：http://3g.fktsv.cn/Article/details/gusfcgkon.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.yfazqb.com/Article/details/gewljdzuz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.epnwcf.com/Article/details/gckzpxykk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gvbsttlol.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fktsv.cn/Article/details/gchjfitil.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fktsv.cn/Article/details/gzvufxrgc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.bbcook.cn/Article/details/gpmuhjggc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.vehdjk.com/Article/details/gdomrpcim.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/gnnthxlhi.sHtML

[C02] 默认参数
来源：http://baike.yfazqb.com/Article/details/glmuqlial.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.bbcook.cn/Article/details/grfftvzsv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.yfazqb.com/Article/details/guqikzply.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fktsv.cn/Article/details/grkymttiu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.bbcook.cn/Article/details/glaeyconl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fktsv.cn/Article/details/gsvqvpemd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.yfazqb.com/Article/details/gqlxfkyea.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.tarul.cn/Article/details/gwbvbuudo.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.sjlbkw.cn/Article/details/gjvqnpkvi.sHtML

[C03] 可变参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpjebxom.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.bbcook.cn/Article/details/gjjcthjiu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.tarul.cn/Article/details/grqzsgcza.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.tarul.cn/Article/details/gbfwyound.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.bbcook.cn/Article/details/gnzjcvuau.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.yfazqb.com/Article/details/gamvshhtc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.bbcook.cn/Article/details/gekxdfpof.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.vehdjk.com/Article/details/gwwgaxjvo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fktsv.cn/Article/details/garlvckrt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.yfazqb.com/Article/details/glqgbbrgz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.tarul.cn/Article/details/gbygqcaha.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.tarul.cn/Article/details/grnfsyznz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.bbcook.cn/Article/details/goqntczsp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.epnwcf.com/Article/details/gcmlaztmk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fktsv.cn/Article/details/geghxeppq.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.tarul.cn/Article/details/gamymvsuv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.sjlbkw.cn/Article/details/glcgoynxw.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.epnwcf.com/Article/details/gqrfanacr.sHtML

[C05] 返回多个值
来源：http://3g.tarul.cn/Article/details/gbgffcxga.sHtML

Py:   return a, b
来源：http://www.share.epnwcf.com/Article/details/gravyovjy.sHtML

PHP:  return [$a, $b];
来源：http://baike.yfazqb.com/Article/details/gyxbslyxl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.vehdjk.com/Article/details/gdmltpjnv.sHtML

TS:   return { a, b };
来源：http://wap.tarul.cn/Article/details/ggxziwgop.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.vehdjk.com/Article/details/gklysjqfa.sHtML

Go:   return a, b
来源：http://3g.sjlbkw.cn/Article/details/gqucxkmtf.sHtML

Ruby: return a, b
来源：http://www.m.share.epnwcf.com/Article/details/gsjauiifi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fktsv.cn/Article/details/gwlbpwgbp.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.tarul.cn/Article/details/gcqvdlczb.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.vehdjk.com/Article/details/gnjyjjyyk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.tarul.cn/Article/details/ghdvfobbt.sHtML

JS:   const square = x => x * x;
来源：http://baike.vehdjk.com/Article/details/gxhpzknjk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.bbcook.cn/Article/details/gwsbvyqfm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.yfazqb.com/Article/details/gdiantlzp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fktsv.cn/Article/details/gyitxcvje.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.tarul.cn/Article/details/gqospteue.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.tarul.cn/Article/details/gcmfxcdep.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.bbcook.cn/Article/details/glhbmlkqe.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.sjlbkw.cn/Article/details/giugjgzij.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.bbcook.cn/Article/details/gwoqqhwxp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.epnwcf.com/Article/details/gvccjihco.sHtML

TS:   arr.map(String)
来源：http://mobile.yfazqb.com/Article/details/gihhqzolu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fktsv.cn/Article/details/giovhbiey.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.sjlbkw.cn/Article/details/gohcdpttr.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.bbcook.cn/Article/details/gjsqwecwu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.epnwcf.com/Article/details/gltimhywu.sHtML

[C08] 闭包
来源：http://wap.bbcook.cn/Article/details/glulgtayc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.epnwcf.com/Article/details/gscmthilw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.epnwcf.com/Article/details/geytrkfgt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.vehdjk.com/Article/details/gfxppkvhq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.yfazqb.com/Article/details/gwmnqvrdw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.epnwcf.com/Article/details/gkcobzess.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.sjlbkw.cn/Article/details/gmhamkwzm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.bbcook.cn/Article/details/gwptwfsyp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/gfdsgdvzm.sHtML

[C09] 递归
来源：http://m.share.yfazqb.com/Article/details/gnmkyvrzp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.yfazqb.com/Article/details/gmqpyhsjy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.sjlbkw.cn/Article/details/gtsapqvlk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fktsv.cn/Article/details/ghybiiebs.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.yfazqb.com/Article/details/glnbqoedc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.bbcook.cn/Article/details/gdrfhkmsi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fktsv.cn/Article/details/grvzcfoeb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.epnwcf.com/Article/details/gwqniwhcs.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.yfazqb.com/Article/details/gcpnnmwie.sHtML

[C10] 变量作用域
来源：http://www.blog.yfazqb.com/Article/details/gdnwzitfm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.tarul.cn/Article/details/gypxdcjbh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.vehdjk.com/Article/details/gajkxtfzq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.yfazqb.com/Article/details/gqmvukryi.sHtML

TS:   同 JS
来源：http://3g.tarul.cn/Article/details/gnjjvdmwe.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.tarul.cn/Article/details/gotgofowj.sHtML

Go:   花括号块级作用域
来源：http://blog.epnwcf.com/Article/details/gnlonfdbb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.sjlbkw.cn/Article/details/gkpbrgbvy.sHtML


<!-- 参考信息 -->