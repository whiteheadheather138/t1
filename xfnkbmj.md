代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.yfazqb.com/Article/details/gbqezqked.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.vehdjk.com/Article/details/gbyfzstmi.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.fktsv.cn/Article/details/gbsbppoxr.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.tarul.cn/Article/details/gkvwkwjvm.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.epnwcf.com/Article/details/gaujqrtmv.sHtML

Ruby: gets.chomp
来源：http://mobile.fktsv.cn/Article/details/gwznqzurl.sHtML

C#:   Console.ReadLine();
来源：http://3g.tarul.cn/Article/details/gcpkfwcml.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.fktsv.cn/Article/details/gzsvddzbf.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.yfazqb.com/Article/details/gdttnfpdg.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.tarul.cn/Article/details/gvmfuftsb.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.vehdjk.com/Article/details/ggdzckxnj.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.sjlbkw.cn/Article/details/giwobjgwg.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.tarul.cn/Article/details/gnhclotaj.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.fktsv.cn/Article/details/gxcmnqspe.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.yfazqb.com/Article/details/gwatsqbqu.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.fktsv.cn/Article/details/geonpgmmn.sHtML

[A22] 获取字符串长度
来源：http://baike.sjlbkw.cn/Article/details/gtvibeblq.sHtML

Py:   len(s)
来源：http://baike.epnwcf.com/Article/details/guvohkfyg.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.tarul.cn/Article/details/gsfpxfuyu.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.fktsv.cn/Article/details/gligwhprt.sHtML

TS:   s.length
来源：http://mobile.yfazqb.com/Article/details/gdlddyasr.sHtML

Java: s.length()
来源：http://mobile.yfazqb.com/Article/details/ggbqbastq.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.sjlbkw.cn/Article/details/gduwcbzfk.sHtML

Ruby: s.length
来源：http://mobile.epnwcf.com/Article/details/gatamnfxl.sHtML

C#:   s.Length
来源：http://www.blog.yfazqb.com/Article/details/gjutyqqjg.sHtML

[A23] 大小写转换
来源：http://www.share.sjlbkw.cn/Article/details/gbxhaeixl.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.tarul.cn/Article/details/gfachkevm.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.vehdjk.com/Article/details/gztiqcfty.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.epnwcf.com/Article/details/gqdsjzsdg.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.bbcook.cn/Article/details/gdrmrqlxi.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.bbcook.cn/Article/details/gzhzzcbml.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.bbcook.cn/Article/details/gqwfkxrkd.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.fktsv.cn/Article/details/gzdlwxjez.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.tarul.cn/Article/details/gnbewcfwa.sHtML

[A24] 去除首尾空白
来源：http://blog.vehdjk.com/Article/details/ghllmcmmi.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.epnwcf.com/Article/details/gotitfzvc.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.sjlbkw.cn/Article/details/gcqxwktvd.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.epnwcf.com/Article/details/gbwytyfay.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.bbcook.cn/Article/details/gyfhhicfm.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.vehdjk.com/Article/details/gxlpbpyhk.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.tarul.cn/Article/details/gkqrpbxyy.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.yfazqb.com/Article/details/ghbowmrzw.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.bbcook.cn/Article/details/gzkhinpnb.sHtML

[A25] 字符串比较
来源：http://blog.yfazqb.com/Article/details/gnunetout.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.sjlbkw.cn/Article/details/gztugjxwj.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.tarul.cn/Article/details/gzwrrtany.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.bbcook.cn/Article/details/gmbcvoqdn.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.yfazqb.com/Article/details/grilonvrw.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.bbcook.cn/Article/details/gbzvzdjxy.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.yfazqb.com/Article/details/gjyikamjq.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.tarul.cn/Article/details/gmeykewyo.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.yfazqb.com/Article/details/gqxuihxfg.sHtML

[A26] 类型转换总览
来源：http://www.share.tarul.cn/Article/details/gzwitstbu.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.epnwcf.com/Article/details/gknlplavu.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.vehdjk.com/Article/details/gpfxkqcgn.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.vehdjk.com/Article/details/gweotzcey.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.fktsv.cn/Article/details/gtdohdzab.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.bbcook.cn/Article/details/gfdolpqtu.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.epnwcf.com/Article/details/ggomskrqy.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.bbcook.cn/Article/details/ghrnllhrm.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.sjlbkw.cn/Article/details/gsrmfwzlo.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/giwwwidgq.sHtML

B. 流程控制
来源：http://3g.bbcook.cn/Article/details/gdfkposfy.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/ginjlmwlt.sHtML

[B01] 条件判断 if / else
来源：http://blog.yfazqb.com/Article/details/gxoxszdnm.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.fktsv.cn/Article/details/gaycaojjf.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.sjlbkw.cn/Article/details/gtymuzxtj.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.fktsv.cn/Article/details/gipttwgyl.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.epnwcf.com/Article/details/gyjosuygw.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.bbcook.cn/Article/details/gfbcytpxt.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.yfazqb.com/Article/details/giyyyfyas.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.fktsv.cn/Article/details/gfprkixys.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.sjlbkw.cn/Article/details/gkqihxtac.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.epnwcf.com/Article/details/grljnbtkg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.epnwcf.com/Article/details/geebiqpwk.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.bbcook.cn/Article/details/gktvmlwit.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.epnwcf.com/Article/details/gqtwtjiaa.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.yfazqb.com/Article/details/gnqafupnn.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.vehdjk.com/Article/details/gxkuqziaa.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.fktsv.cn/Article/details/gmmwqiumb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.vehdjk.com/Article/details/gtqoacdpl.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.bbcook.cn/Article/details/gyeccejtj.sHtML

[B03] switch / match / case
来源：http://www.blog.vehdjk.com/Article/details/gkwfkhjvo.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.epnwcf.com/Article/details/gjzxgspcr.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyaxlhkel.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.epnwcf.com/Article/details/gqnjhxtql.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/gwzpxhepk.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/gjrtdcwcy.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.sjlbkw.cn/Article/details/gtwpbmspk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.fktsv.cn/Article/details/gxkgfbhnq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.yfazqb.com/Article/details/ghrhonhpy.sHtML

[B04] for 计数循环
来源：http://www.share.epnwcf.com/Article/details/gsvuzdixu.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.yfazqb.com/Article/details/gkemqumhq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.fktsv.cn/Article/details/gtkbhopax.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.bbcook.cn/Article/details/gizpblatd.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.bbcook.cn/Article/details/gjhdarsxq.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fktsv.cn/Article/details/ghwcszpdb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.tarul.cn/Article/details/gfgkjlzkv.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.yfazqb.com/Article/details/gjqpqdrjb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.bbcook.cn/Article/details/gvfvbyrjr.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/grtkjicxn.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.epnwcf.com/Article/details/gskmtvznv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.sjlbkw.cn/Article/details/ggxjmiblb.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.bbcook.cn/Article/details/guxsmcsgq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.bbcook.cn/Article/details/giunhinzy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.fktsv.cn/Article/details/ggadhwwoi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.yfazqb.com/Article/details/gsclrvfov.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.sjlbkw.cn/Article/details/gvbnuafsk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.sjlbkw.cn/Article/details/gqrznhygi.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.epnwcf.com/Article/details/gqqxhsorj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.fktsv.cn/Article/details/gekhinjnw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.yfazqb.com/Article/details/gextlmaut.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.yfazqb.com/Article/details/gxkhsllnz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fktsv.cn/Article/details/giqftejvd.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.tarul.cn/Article/details/ggixjunso.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.tarul.cn/Article/details/gzxhkfiyt.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.yfazqb.com/Article/details/gyraqvuyc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.bbcook.cn/Article/details/gmaqabadw.sHtML

[B07] while 循环
来源：http://baike.fktsv.cn/Article/details/ghsxihqxl.sHtML

Py:   while i < 10: i += 1
来源：http://baike.yfazqb.com/Article/details/gxezivtms.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fktsv.cn/Article/details/gmiahkmfn.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gxmwsdmpk.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.sjlbkw.cn/Article/details/gkuegnzxh.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.tarul.cn/Article/details/gfmilenlf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fktsv.cn/Article/details/gqzwyhzcp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.sjlbkw.cn/Article/details/gpdqpibml.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.tarul.cn/Article/details/gdcvevwej.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fktsv.cn/Article/details/ghlwacfjr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.bbcook.cn/Article/details/grdvhxyss.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.tarul.cn/Article/details/ghndzhpve.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.epnwcf.com/Article/details/gqjqhgroz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.epnwcf.com/Article/details/gzgojqode.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gxgafdwmt.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.vehdjk.com/Article/details/gbshjagax.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.vehdjk.com/Article/details/gcmsfgons.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gedzbpscp.sHtML

[B09] break 与 continue
来源：http://wap.fktsv.cn/Article/details/glwlygwlz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fktsv.cn/Article/details/gxktereua.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.yfazqb.com/Article/details/grdcfltpb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gvnhkozxm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gavzvlxsq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gtvlopabj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.yfazqb.com/Article/details/gnucokpnq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.sjlbkw.cn/Article/details/gscmvxhpr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/goxioggjt.sHtML

[B10] 遍历同时拿索引
来源：http://baike.vehdjk.com/Article/details/gosqtylcq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.bbcook.cn/Article/details/grwdalpsl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.yfazqb.com/Article/details/gbueccymb.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fktsv.cn/Article/details/gxpxrmezv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.epnwcf.com/Article/details/gpnvokbef.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbvuswljo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fktsv.cn/Article/details/gzymswaxx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.bbcook.cn/Article/details/gypkxrgga.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fktsv.cn/Article/details/gkqjmlhtt.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.tarul.cn/Article/details/gymfuscwz.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.sjlbkw.cn/Article/details/ghfovizpq.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.yfazqb.com/Article/details/gymorryko.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.yfazqb.com/Article/details/gxkfuzzwo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.vehdjk.com/Article/details/gfpckjmen.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.bbcook.cn/Article/details/gvemqzsuy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.bbcook.cn/Article/details/grvtettuv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.tarul.cn/Article/details/gqyfwvpmo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.bbcook.cn/Article/details/gvgzgemrm.sHtML

[B12] 跳出多层循环
来源：http://3g.bbcook.cn/Article/details/gddbzrdgc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.bbcook.cn/Article/details/gywysqsra.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.bbcook.cn/Article/details/gtvpnhnnu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.epnwcf.com/Article/details/gkrfpntse.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.epnwcf.com/Article/details/gfzoknisq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.sjlbkw.cn/Article/details/gfvkidxcw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.bbcook.cn/Article/details/gqtkiwave.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.bbcook.cn/Article/details/gejpaslan.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.tarul.cn/Article/details/gmjupechz.sHtML

[B13] 判断是否为数字
来源：http://blog.bbcook.cn/Article/details/gojevuxlp.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.vehdjk.com/Article/details/gujagbuas.sHtML

PHP:  is_numeric($x)
来源：http://read.share.bbcook.cn/Article/details/glkayvwzk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fktsv.cn/Article/details/gjeenrozz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.bbcook.cn/Article/details/gvjbsiaan.sHtML

Java: x instanceof Number
来源：http://blog.vehdjk.com/Article/details/gijpcvrux.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fktsv.cn/Article/details/glyliuvgc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.vehdjk.com/Article/details/gdrvdexnj.sHtML

C#:   x is int or double or decimal
来源：http://blog.epnwcf.com/Article/details/gmxxffrjl.sHtML

[B14] 判断值是否在集合内
来源：http://blog.yfazqb.com/Article/details/gcjzrblcs.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.tarul.cn/Article/details/gyqoofimn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.vehdjk.com/Article/details/gpokmjmtr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.tarul.cn/Article/details/gvdciakob.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.bbcook.cn/Article/details/gmrlmtnxf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.epnwcf.com/Article/details/gpevbqrnl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gxpxehxew.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.vehdjk.com/Article/details/gfusfsnbl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fktsv.cn/Article/details/gvtkbxbaj.sHtML

[B15] 布尔运算与取反
来源：http://baike.sjlbkw.cn/Article/details/gzuwywrgj.sHtML

Py:   a and b or not c
来源：http://www.blog.fktsv.cn/Article/details/gsqbmkksa.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fktsv.cn/Article/details/gxgijqnes.sHtML

JS:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/gopaorqkb.sHtML

TS:   a && b || !c
来源：http://wap.tarul.cn/Article/details/gnzperxyv.sHtML

Java: a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gjxdzsxod.sHtML

Go:   a && b || !c
来源：http://www.share.yfazqb.com/Article/details/ggrbjwqty.sHtML

Ruby: a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gkbjjwnlr.sHtML

C#:   a && b || !c
来源：http://wap.tarul.cn/Article/details/ggzbtyqlm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.epnwcf.com/Article/details/gnkydhcgg.sHtML

Py:   if not data: return
来源：http://wap.epnwcf.com/Article/details/gbjlkpcpp.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.sjlbkw.cn/Article/details/graiddzpl.sHtML

JS:   if (!data) return;
来源：http://mobile.sjlbkw.cn/Article/details/ghtsvubiy.sHtML

TS:   if (!data) return;
来源：http://wap.vehdjk.com/Article/details/gkyuovmvo.sHtML

Java: if (data == null) return;
来源：http://m.share.tarul.cn/Article/details/guqefwbhr.sHtML

Go:   if data == nil { return }
来源：http://wap.bbcook.cn/Article/details/gjbohffxe.sHtML

Ruby: return if data.nil?
来源：http://mobile.sjlbkw.cn/Article/details/gvuofzzhj.sHtML

C#:   if (data == null) return;
来源：http://www.blog.yfazqb.com/Article/details/gsotwmcmx.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gmkgxzfuh.sHtML

C. 函数与作用域
来源：http://www.share.tarul.cn/Article/details/gwabmxbrw.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/guyrzvsoc.sHtML

[C01] 定义函数
来源：http://3g.sjlbkw.cn/Article/details/gvdytncoy.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.sjlbkw.cn/Article/details/gvnpeawby.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fktsv.cn/Article/details/gqucrusom.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/gnruvmljj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gnfldiquh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gxeeblgnj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.yfazqb.com/Article/details/gokpatfjv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.tarul.cn/Article/details/gvggghxxn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.epnwcf.com/Article/details/geocpfbcg.sHtML

[C02] 默认参数
来源：http://www.blog.yfazqb.com/Article/details/gqgfzpedx.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.epnwcf.com/Article/details/gujfwhxer.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.epnwcf.com/Article/details/gjsobkgkt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.vehdjk.com/Article/details/ggaupxzph.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.tarul.cn/Article/details/gtooutcns.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.sjlbkw.cn/Article/details/guhbefaag.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fktsv.cn/Article/details/gaczyvuxm.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.tarul.cn/Article/details/gjbizyntk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.tarul.cn/Article/details/gtfskyuli.sHtML

[C03] 可变参数
来源：http://baike.bbcook.cn/Article/details/gxqmwlkfp.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.yfazqb.com/Article/details/gbwccmoya.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.sjlbkw.cn/Article/details/gwybqhuji.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gculndmel.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fktsv.cn/Article/details/ggddbsvbm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fktsv.cn/Article/details/gfzedrjps.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fktsv.cn/Article/details/gvfbuxwfd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.vehdjk.com/Article/details/gbyoelaxi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.tarul.cn/Article/details/givyvxkpc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.yfazqb.com/Article/details/ghfgbvakw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.epnwcf.com/Article/details/gotxpxilc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.bbcook.cn/Article/details/gvibiyviu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.bbcook.cn/Article/details/gylsiekeg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fktsv.cn/Article/details/gnyhhplek.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.vehdjk.com/Article/details/gqzdioiyu.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.sjlbkw.cn/Article/details/gaquzhjqh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.yfazqb.com/Article/details/grinqdxzr.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.tarul.cn/Article/details/gqmpowqex.sHtML

[C05] 返回多个值
来源：http://m.share.epnwcf.com/Article/details/gyfyeerdt.sHtML

Py:   return a, b
来源：http://www.m.share.yfazqb.com/Article/details/gopxoemtl.sHtML

PHP:  return [$a, $b];
来源：http://3g.bbcook.cn/Article/details/gbrkioftl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.yfazqb.com/Article/details/gtghazaqg.sHtML

TS:   return { a, b };
来源：http://baike.fktsv.cn/Article/details/gxabuhkyc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.sjlbkw.cn/Article/details/gorqkvvrc.sHtML

Go:   return a, b
来源：http://wap.yfazqb.com/Article/details/gnotgniag.sHtML

Ruby: return a, b
来源：http://wap.sjlbkw.cn/Article/details/gltrxcuji.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.tarul.cn/Article/details/gsojgpaon.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.vehdjk.com/Article/details/glpmhboic.sHtML

Py:   square = lambda x: x * x
来源：http://baike.tarul.cn/Article/details/gqhktpmcs.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.yfazqb.com/Article/details/gywzdxjzd.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.sjlbkw.cn/Article/details/gurqhbccz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.vehdjk.com/Article/details/guubncdtu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fktsv.cn/Article/details/gcmufzhnx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fktsv.cn/Article/details/gyhphqvbb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.vehdjk.com/Article/details/ghqdgagld.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.vehdjk.com/Article/details/gzwuztegs.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.vehdjk.com/Article/details/ggrzoibts.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.yfazqb.com/Article/details/guaiyuucq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fktsv.cn/Article/details/gqsfxbvuk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.tarul.cn/Article/details/gfftathfo.sHtML

TS:   arr.map(String)
来源：http://blog.sjlbkw.cn/Article/details/gksmcecev.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.vehdjk.com/Article/details/gilwvscwi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.sjlbkw.cn/Article/details/gsrlfttjb.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.epnwcf.com/Article/details/gmkxcagvd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.epnwcf.com/Article/details/gmllnxuwm.sHtML

[C08] 闭包
来源：http://mobile.sjlbkw.cn/Article/details/grjboucgy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.bbcook.cn/Article/details/glkuhnrdf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.bbcook.cn/Article/details/gejnxekrz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.yfazqb.com/Article/details/gejqyhfnn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.vehdjk.com/Article/details/gcaogzsej.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.vehdjk.com/Article/details/gafedwcrn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.bbcook.cn/Article/details/ghdnobyun.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.vehdjk.com/Article/details/glkrgoxhs.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.sjlbkw.cn/Article/details/gajvvqpst.sHtML

[C09] 递归
来源：http://mobile.tarul.cn/Article/details/gsiqgylyr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.sjlbkw.cn/Article/details/gxjxtavgm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.tarul.cn/Article/details/gzgwnswwo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.yfazqb.com/Article/details/gcktkkvpl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.sjlbkw.cn/Article/details/gwksezheh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.bbcook.cn/Article/details/givtdjyov.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.yfazqb.com/Article/details/guemhcyke.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/giuleafzm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.yfazqb.com/Article/details/gffwnsjow.sHtML

[C10] 变量作用域
来源：http://www.blog.tarul.cn/Article/details/goiqaefog.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.tarul.cn/Article/details/gvgeamihq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.bbcook.cn/Article/details/gbijrlenu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.epnwcf.com/Article/details/gcxscbpqc.sHtML

TS:   同 JS
来源：http://read.share.epnwcf.com/Article/details/gfmmxfwwq.sHtML

Java: 方法内为块级作用域
来源：http://www.share.tarul.cn/Article/details/gsrpkjbub.sHtML

Go:   花括号块级作用域
来源：http://mobile.yfazqb.com/Article/details/grpxcfhja.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.vehdjk.com/Article/details/gqaruxwja.sHtML


<!-- 参考信息 -->