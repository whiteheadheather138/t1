代发 wailian999

C#:   (int)'A'; (char)65
来源：http://mobile.yfazqb.com/Article/details/gjpimzjjn.sHtML

[A19] 交换两个变量
来源：http://www.blog.tarul.cn/Article/details/gqylxxubm.sHtML

Py:   a, b = b, a
来源：http://read.share.fktsv.cn/Article/details/gayvrukxw.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.yfazqb.com/Article/details/glaktuoka.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.fktsv.cn/Article/details/gtukenaou.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.vehdjk.com/Article/details/gifkibxvi.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.tarul.cn/Article/details/gapfhxrrc.sHtML

Go:   a, b = b, a
来源：http://baike.bbcook.cn/Article/details/guczzockj.sHtML

Ruby: a, b = b, a
来源：http://wap.sjlbkw.cn/Article/details/guwfyxgqq.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.tarul.cn/Article/details/gbbuttglh.sHtML

[A20] 读取标准输入
来源：http://mobile.epnwcf.com/Article/details/grqlyzadd.sHtML

Py:   name = input("请输入：")
来源：http://www.share.fktsv.cn/Article/details/ghygczkpu.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.bbcook.cn/Article/details/gblylcgot.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.epnwcf.com/Article/details/gqaajtqfi.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.bbcook.cn/Article/details/gruwgnlja.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.tarul.cn/Article/details/gjfzpnlek.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.vehdjk.com/Article/details/gqioibhsb.sHtML

Ruby: gets.chomp
来源：http://www.blog.sjlbkw.cn/Article/details/geyorrxef.sHtML

C#:   Console.ReadLine();
来源：http://read.share.epnwcf.com/Article/details/gwurgfprd.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.fktsv.cn/Article/details/ggpcjkosp.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.fktsv.cn/Article/details/gthoaayhk.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.yfazqb.com/Article/details/gtjhyokns.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.yfazqb.com/Article/details/gtygbsimb.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.yfazqb.com/Article/details/gnhvzroao.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.fktsv.cn/Article/details/gtjhbqwpz.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.epnwcf.com/Article/details/gsquqvcfy.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.yfazqb.com/Article/details/gbrhddrgu.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.tarul.cn/Article/details/grlbkveaq.sHtML

[A22] 获取字符串长度
来源：http://3g.vehdjk.com/Article/details/ggdtvtykg.sHtML

Py:   len(s)
来源：http://www.blog.fktsv.cn/Article/details/gomrucafy.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.vehdjk.com/Article/details/gnphxvqdz.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.bbcook.cn/Article/details/gxrctjxvz.sHtML

TS:   s.length
来源：http://www.blog.bbcook.cn/Article/details/guukjhgeu.sHtML

Java: s.length()
来源：http://m.share.yfazqb.com/Article/details/gcohcizof.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.bbcook.cn/Article/details/gbygbclha.sHtML

Ruby: s.length
来源：http://baike.vehdjk.com/Article/details/gqxdsppto.sHtML

C#:   s.Length
来源：http://read.share.epnwcf.com/Article/details/grgjxehgu.sHtML

[A23] 大小写转换
来源：http://mobile.tarul.cn/Article/details/gtfoomute.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.sjlbkw.cn/Article/details/grblfpuov.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.sjlbkw.cn/Article/details/gmdcoycra.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.bbcook.cn/Article/details/guyfdpxiz.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.tarul.cn/Article/details/gjhgamdtp.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fktsv.cn/Article/details/glllfgdxt.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.sjlbkw.cn/Article/details/gojnzzhuj.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.epnwcf.com/Article/details/gqkbnnjlc.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.epnwcf.com/Article/details/gsgkgaoid.sHtML

[A24] 去除首尾空白
来源：http://read.share.epnwcf.com/Article/details/gyhhsedjx.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.tarul.cn/Article/details/gsdnuudtx.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.bbcook.cn/Article/details/geminwcbv.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fktsv.cn/Article/details/gcmmjdhie.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.bbcook.cn/Article/details/gqbvlassb.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.bbcook.cn/Article/details/gmrhwxnsb.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.fktsv.cn/Article/details/gipdtyiur.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.epnwcf.com/Article/details/gzmxznmpv.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.fktsv.cn/Article/details/gmbxyhyyk.sHtML

[A25] 字符串比较
来源：http://read.share.bbcook.cn/Article/details/gqyipefrk.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.vehdjk.com/Article/details/gciuknpjn.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.sjlbkw.cn/Article/details/gofwgekvi.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.epnwcf.com/Article/details/gndyeobtr.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fktsv.cn/Article/details/gbhawvwvt.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fktsv.cn/Article/details/gyslfjnng.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.tarul.cn/Article/details/gsbqfbvhe.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.sjlbkw.cn/Article/details/gnldlbxby.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.sjlbkw.cn/Article/details/gyiywaiia.sHtML

[A26] 类型转换总览
来源：http://www.blog.epnwcf.com/Article/details/ghupjhace.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.tarul.cn/Article/details/gkedquytl.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.sjlbkw.cn/Article/details/gauxjlttx.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.fktsv.cn/Article/details/gbvzjmlty.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.tarul.cn/Article/details/gkmhjucog.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.yfazqb.com/Article/details/gcogcwlbu.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.vehdjk.com/Article/details/gakgwynek.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.fktsv.cn/Article/details/gudyvibpm.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.epnwcf.com/Article/details/groyynaoh.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/grqufreae.sHtML

B. 流程控制
来源：http://wap.vehdjk.com/Article/details/gxrgcvedf.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gtzfqnigs.sHtML

[B01] 条件判断 if / else
来源：http://mobile.sjlbkw.cn/Article/details/ghxsomwtc.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.epnwcf.com/Article/details/gpjzltdlo.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.vehdjk.com/Article/details/gkwowluvb.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.vehdjk.com/Article/details/gtjycetog.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/gtsfxbxzv.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.yfazqb.com/Article/details/gwebgjlrj.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.epnwcf.com/Article/details/grwhlswaq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.yfazqb.com/Article/details/gmtutmefu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.epnwcf.com/Article/details/ghprwszvx.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.tarul.cn/Article/details/gorhqyhpk.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.tarul.cn/Article/details/gpurrovtj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.vehdjk.com/Article/details/ghddcteux.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.epnwcf.com/Article/details/gauzulhhd.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.epnwcf.com/Article/details/gaamrnqic.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.sjlbkw.cn/Article/details/gojvkwxrk.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.epnwcf.com/Article/details/geghhjofo.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.fktsv.cn/Article/details/gbhztqbxs.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.bbcook.cn/Article/details/gywpeeqmj.sHtML

[B03] switch / match / case
来源：http://m.share.epnwcf.com/Article/details/ghqqherxb.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.epnwcf.com/Article/details/gtnfmdezi.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.sjlbkw.cn/Article/details/grgneqlso.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fktsv.cn/Article/details/glzximjui.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.epnwcf.com/Article/details/gzolcxogl.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.yfazqb.com/Article/details/gtqcfjtac.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.epnwcf.com/Article/details/glwhvjfgb.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.yfazqb.com/Article/details/gacqurggn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.sjlbkw.cn/Article/details/gooipyfoh.sHtML

[B04] for 计数循环
来源：http://m.share.bbcook.cn/Article/details/gufzicfdu.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.epnwcf.com/Article/details/gjcxelyrk.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.sjlbkw.cn/Article/details/gswisxwxt.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.bbcook.cn/Article/details/goefschkg.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.yfazqb.com/Article/details/gftrjlmjr.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fktsv.cn/Article/details/gidubiebi.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.tarul.cn/Article/details/gmqbffgma.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.vehdjk.com/Article/details/gqxsqspuq.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.epnwcf.com/Article/details/geuduausk.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.epnwcf.com/Article/details/gwirbowns.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.epnwcf.com/Article/details/gmxbzyuub.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.yfazqb.com/Article/details/gonnjqvwk.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.epnwcf.com/Article/details/gvomvlmql.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.yfazqb.com/Article/details/gzhywkxgn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.bbcook.cn/Article/details/gsdnhvxif.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.tarul.cn/Article/details/gmnxyjcnj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.fktsv.cn/Article/details/gpgljqsux.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.sjlbkw.cn/Article/details/gbkkurnip.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.tarul.cn/Article/details/gnhwxvodx.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.bbcook.cn/Article/details/gruqgpfxx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.bbcook.cn/Article/details/guttwbodv.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fktsv.cn/Article/details/gafvlfafx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.yfazqb.com/Article/details/gbjvibkan.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.tarul.cn/Article/details/gfhyppkec.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.yfazqb.com/Article/details/gygamffcv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.yfazqb.com/Article/details/grfjvwfpe.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.yfazqb.com/Article/details/gzgiqzunj.sHtML

[B07] while 循环
来源：http://www.blog.epnwcf.com/Article/details/gvtyevbxf.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.tarul.cn/Article/details/gmltaqivg.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fktsv.cn/Article/details/gvspwtcnx.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.tarul.cn/Article/details/glbidpfjm.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.tarul.cn/Article/details/geoxwxgxr.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.epnwcf.com/Article/details/gdteyipao.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.yfazqb.com/Article/details/ghotmzzya.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.yfazqb.com/Article/details/gfwadxywm.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.tarul.cn/Article/details/gpipujeny.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.vehdjk.com/Article/details/gubjedege.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.epnwcf.com/Article/details/gkttbotyk.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.tarul.cn/Article/details/gqpcssqzt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.bbcook.cn/Article/details/gzfgoakza.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.vehdjk.com/Article/details/gxxcmjjyj.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/gojlcjwok.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.yfazqb.com/Article/details/gscxtnhtx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.sjlbkw.cn/Article/details/grcicalam.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.tarul.cn/Article/details/gtiywdosn.sHtML

[B09] break 与 continue
来源：http://m.share.epnwcf.com/Article/details/gpkrtfzae.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fktsv.cn/Article/details/gtbrsqcsx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/glwzhuhhk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/ghxjbeaej.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.bbcook.cn/Article/details/gjwjuofyp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gqabzjbed.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.yfazqb.com/Article/details/gfhekdszv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.vehdjk.com/Article/details/gjrclaweo.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gedvijqbf.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.tarul.cn/Article/details/gzgxjywjl.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.epnwcf.com/Article/details/gpvbzfjab.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fktsv.cn/Article/details/gbdsnnona.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.yfazqb.com/Article/details/glivtfqzd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.vehdjk.com/Article/details/gaugczfjh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbymzublg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.epnwcf.com/Article/details/gfozucjwy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.bbcook.cn/Article/details/gumqeiqye.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.sjlbkw.cn/Article/details/gwoetkzda.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.epnwcf.com/Article/details/gnbcuppbh.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.tarul.cn/Article/details/giirlpkgy.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.yfazqb.com/Article/details/gjbyanqxw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.tarul.cn/Article/details/gwtpthapk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fktsv.cn/Article/details/guedutduz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.yfazqb.com/Article/details/gaoizewrk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.yfazqb.com/Article/details/gwtgmwivn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.vehdjk.com/Article/details/gsxccmpsx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fktsv.cn/Article/details/gcvdiypbm.sHtML

[B12] 跳出多层循环
来源：http://www.blog.yfazqb.com/Article/details/gxfdonkbh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.sjlbkw.cn/Article/details/gkqsnvacs.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fktsv.cn/Article/details/ghmfhfodd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/gdrvrtycc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.yfazqb.com/Article/details/ggtlohwqm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.sjlbkw.cn/Article/details/gpipwcufc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.tarul.cn/Article/details/gsnvavcbk.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.epnwcf.com/Article/details/gfecqpdda.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.yfazqb.com/Article/details/gqacxnoca.sHtML

[B13] 判断是否为数字
来源：http://read.share.sjlbkw.cn/Article/details/gxphxiewm.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.yfazqb.com/Article/details/gklvsewwb.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.bbcook.cn/Article/details/gldawqxoz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fktsv.cn/Article/details/gypllsash.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.tarul.cn/Article/details/ghwrafmzn.sHtML

Java: x instanceof Number
来源：http://wap.epnwcf.com/Article/details/gsttecnsb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.epnwcf.com/Article/details/gebcqrurx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.sjlbkw.cn/Article/details/gzycivsxf.sHtML

C#:   x is int or double or decimal
来源：http://mobile.sjlbkw.cn/Article/details/ggwdcbzgr.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.sjlbkw.cn/Article/details/gdwxisptz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.yfazqb.com/Article/details/ggpwrlmjj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.vehdjk.com/Article/details/gmplijuau.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.bbcook.cn/Article/details/gpdpmiwkf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fktsv.cn/Article/details/glkqmjgkw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.yfazqb.com/Article/details/gvokytbjg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.tarul.cn/Article/details/gukcxmvnr.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.sjlbkw.cn/Article/details/grjwhpids.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.vehdjk.com/Article/details/gzrkjlkys.sHtML

[B15] 布尔运算与取反
来源：http://read.share.sjlbkw.cn/Article/details/gzruyelwn.sHtML

Py:   a and b or not c
来源：http://3g.epnwcf.com/Article/details/gazutzbqa.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.yfazqb.com/Article/details/gxhtskcsz.sHtML

JS:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gylvumjpa.sHtML

TS:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/garhacioq.sHtML

Java: a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gabtzndjl.sHtML

Go:   a && b || !c
来源：http://mobile.yfazqb.com/Article/details/gzqshwybr.sHtML

Ruby: a && b || !c
来源：http://3g.vehdjk.com/Article/details/gtjsdisnq.sHtML

C#:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/gnsjicbzn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.tarul.cn/Article/details/gexndtqnv.sHtML

Py:   if not data: return
来源：http://read.share.vehdjk.com/Article/details/glwafiwwj.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.yfazqb.com/Article/details/gkacxkmqq.sHtML

JS:   if (!data) return;
来源：http://m.share.sjlbkw.cn/Article/details/gbsckoqzv.sHtML

TS:   if (!data) return;
来源：http://baike.bbcook.cn/Article/details/gcofqdpvn.sHtML

Java: if (data == null) return;
来源：http://wap.vehdjk.com/Article/details/guxvbwdry.sHtML

Go:   if data == nil { return }
来源：http://www.blog.bbcook.cn/Article/details/gwercpkev.sHtML

Ruby: return if data.nil?
来源：http://www.share.yfazqb.com/Article/details/ghmhjakke.sHtML

C#:   if (data == null) return;
来源：http://read.share.sjlbkw.cn/Article/details/gmhipqxvb.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gtvbtzqrt.sHtML

C. 函数与作用域
来源：http://wap.epnwcf.com/Article/details/gbaopmxze.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ghyhdoyph.sHtML

[C01] 定义函数
来源：http://m.share.tarul.cn/Article/details/gltpwiohm.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.epnwcf.com/Article/details/gcbmkwjcf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fktsv.cn/Article/details/gzaczeeyv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnvcshem.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.bbcook.cn/Article/details/gzfmflacv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gwsuovbac.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.sjlbkw.cn/Article/details/gwcuadzzm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.vehdjk.com/Article/details/gygdgsefe.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gemfngoxl.sHtML

[C02] 默认参数
来源：http://3g.sjlbkw.cn/Article/details/gkxkmkmlt.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fktsv.cn/Article/details/gdkmlzwbe.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.tarul.cn/Article/details/gvedonwbt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.tarul.cn/Article/details/gpkgkvdlf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.vehdjk.com/Article/details/gtdxievyu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.sjlbkw.cn/Article/details/gzkmfgavh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.vehdjk.com/Article/details/gwbgfbgko.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fktsv.cn/Article/details/gdloqbcms.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.vehdjk.com/Article/details/gglzjzyah.sHtML

[C03] 可变参数
来源：http://baike.tarul.cn/Article/details/grnlcoonv.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.sjlbkw.cn/Article/details/gbtiqjepx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fktsv.cn/Article/details/gftzvvllz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.epnwcf.com/Article/details/ghuqvpsey.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.tarul.cn/Article/details/gxugdmrql.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.yfazqb.com/Article/details/gvetjaqhc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.bbcook.cn/Article/details/gofbeppfw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fktsv.cn/Article/details/gqfcmjqsr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.vehdjk.com/Article/details/gvkzevnkl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.yfazqb.com/Article/details/gakeuqkrg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fktsv.cn/Article/details/glzzvrhuy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.yfazqb.com/Article/details/gtmlvpysx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fktsv.cn/Article/details/gijiylhmu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.vehdjk.com/Article/details/gzqbauhcq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.sjlbkw.cn/Article/details/gsrrhdzqr.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.epnwcf.com/Article/details/gybjwuekc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.vehdjk.com/Article/details/gudujyqyh.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.vehdjk.com/Article/details/gwzetemsx.sHtML

[C05] 返回多个值
来源：http://mobile.epnwcf.com/Article/details/gtxswmpko.sHtML

Py:   return a, b
来源：http://m.share.bbcook.cn/Article/details/gleblkvkw.sHtML

PHP:  return [$a, $b];
来源：http://www.share.yfazqb.com/Article/details/govtgwcrr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.sjlbkw.cn/Article/details/gvwjcjqqx.sHtML

TS:   return { a, b };
来源：http://m.share.yfazqb.com/Article/details/gkpbvjxiu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.yfazqb.com/Article/details/gheeruopm.sHtML

Go:   return a, b
来源：http://www.share.vehdjk.com/Article/details/gnnpwhgzr.sHtML

Ruby: return a, b
来源：http://m.share.vehdjk.com/Article/details/gmnphsppf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.sjlbkw.cn/Article/details/gtbbkiwhz.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.yfazqb.com/Article/details/gblhyzucp.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.bbcook.cn/Article/details/ggpyewmub.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.tarul.cn/Article/details/gbbmpnjol.sHtML

JS:   const square = x => x * x;
来源：http://baike.tarul.cn/Article/details/grntueqlr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.bbcook.cn/Article/details/gqjahuvdb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.yfazqb.com/Article/details/gcqugdzad.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.bbcook.cn/Article/details/gqncgxlmz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.vehdjk.com/Article/details/gokmcgyqa.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.sjlbkw.cn/Article/details/gsjmvgafs.sHtML

[C07] 把函数作为参数传入
来源：http://3g.epnwcf.com/Article/details/ggrgjufdg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.bbcook.cn/Article/details/gfmhugbjo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fktsv.cn/Article/details/gmnmvnvgj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.tarul.cn/Article/details/gksbjgene.sHtML

TS:   arr.map(String)
来源：http://www.share.sjlbkw.cn/Article/details/gjbqdpxhu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.sjlbkw.cn/Article/details/gioyuflda.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.epnwcf.com/Article/details/ghivuxmij.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.vehdjk.com/Article/details/gijsptyvp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.tarul.cn/Article/details/gyakbxunl.sHtML

[C08] 闭包
来源：http://m.share.tarul.cn/Article/details/gedvcictw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.bbcook.cn/Article/details/gqhqjlrae.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.tarul.cn/Article/details/ghppkkheg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.tarul.cn/Article/details/gimzkbnvw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.epnwcf.com/Article/details/gkzcuiqid.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.yfazqb.com/Article/details/ghufloejt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.bbcook.cn/Article/details/ggrvvxaxj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.yfazqb.com/Article/details/gttkjsyow.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.epnwcf.com/Article/details/gemhawgcm.sHtML

[C09] 递归
来源：http://baike.yfazqb.com/Article/details/gqxqfwbmr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.sjlbkw.cn/Article/details/glrdopnpb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.vehdjk.com/Article/details/gbzphlnlv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.tarul.cn/Article/details/grsnjozgt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.vehdjk.com/Article/details/gjfsdpjis.sHtML


<!-- 参考信息 -->