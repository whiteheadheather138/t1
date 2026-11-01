代发 wailian999

JS:   [a, b] = [b, a];
来源：http://3g.vehdjk.com/Article/details/ghdgkqkcu.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.fktsv.cn/Article/details/gsqsyfywd.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.bbcook.cn/Article/details/ggfbfprxt.sHtML

Go:   a, b = b, a
来源：http://www.blog.sjlbkw.cn/Article/details/gqimtilfh.sHtML

Ruby: a, b = b, a
来源：http://mobile.bbcook.cn/Article/details/geextfbot.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.vehdjk.com/Article/details/gbyxkrcnz.sHtML

[A20] 读取标准输入
来源：http://www.share.tarul.cn/Article/details/guiyhztwm.sHtML

Py:   name = input("请输入：")
来源：http://blog.bbcook.cn/Article/details/gcnuawqfn.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.epnwcf.com/Article/details/gdwzzoycn.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.sjlbkw.cn/Article/details/gdrsegmtn.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.fktsv.cn/Article/details/gccntjqfy.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.fktsv.cn/Article/details/gnwiyakst.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.fktsv.cn/Article/details/gqgjrrkxc.sHtML

Ruby: gets.chomp
来源：http://read.share.sjlbkw.cn/Article/details/gubuhsazf.sHtML

C#:   Console.ReadLine();
来源：http://read.share.epnwcf.com/Article/details/gdorsypax.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.sjlbkw.cn/Article/details/gvdcnferb.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.yfazqb.com/Article/details/gvhtztuqu.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.fktsv.cn/Article/details/gnnyreoof.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.yfazqb.com/Article/details/gflxbtrei.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.bbcook.cn/Article/details/ggehdcqmq.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.sjlbkw.cn/Article/details/gmtnedjae.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.epnwcf.com/Article/details/gpwoknbzs.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.bbcook.cn/Article/details/ganmviivc.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.tarul.cn/Article/details/ghtynfvof.sHtML

[A22] 获取字符串长度
来源：http://blog.fktsv.cn/Article/details/gkbbpckdg.sHtML

Py:   len(s)
来源：http://blog.bbcook.cn/Article/details/gabtjhosu.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.sjlbkw.cn/Article/details/gpmjwfnbk.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.yfazqb.com/Article/details/gxalbflge.sHtML

TS:   s.length
来源：http://blog.yfazqb.com/Article/details/gsattvfie.sHtML

Java: s.length()
来源：http://wap.sjlbkw.cn/Article/details/gkbphcbig.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.bbcook.cn/Article/details/gzgolinls.sHtML

Ruby: s.length
来源：http://wap.epnwcf.com/Article/details/gdxnsdxpb.sHtML

C#:   s.Length
来源：http://read.share.vehdjk.com/Article/details/ghatsfhqi.sHtML

[A23] 大小写转换
来源：http://www.m.share.vehdjk.com/Article/details/gsnwwpkqu.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.sjlbkw.cn/Article/details/glycnyoov.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.vehdjk.com/Article/details/gahkelgqf.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fktsv.cn/Article/details/gcrzwnfpq.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.epnwcf.com/Article/details/gieyxwujz.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.fktsv.cn/Article/details/gjbkcksxb.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.sjlbkw.cn/Article/details/gbkufsjkl.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.tarul.cn/Article/details/glpaewbzr.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.epnwcf.com/Article/details/gpwgefibc.sHtML

[A24] 去除首尾空白
来源：http://www.share.vehdjk.com/Article/details/gdnfgvakl.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.bbcook.cn/Article/details/gohiizzwq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.yfazqb.com/Article/details/gykvgoppi.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.vehdjk.com/Article/details/gztcthtsu.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.sjlbkw.cn/Article/details/gkpdtnfec.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.sjlbkw.cn/Article/details/gjodwlgmf.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.epnwcf.com/Article/details/gxxkqoxgz.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.bbcook.cn/Article/details/gvqlhaqjt.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.bbcook.cn/Article/details/gpvcbtgbu.sHtML

[A25] 字符串比较
来源：http://mobile.epnwcf.com/Article/details/gvkvbednh.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.sjlbkw.cn/Article/details/gnuuxfuxv.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.tarul.cn/Article/details/gqllhjscg.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.vehdjk.com/Article/details/gvuehdnuz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.tarul.cn/Article/details/gcglbfrtv.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.tarul.cn/Article/details/gvxtrgfef.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.epnwcf.com/Article/details/gqyvoalmo.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.yfazqb.com/Article/details/gvoajblxl.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.sjlbkw.cn/Article/details/gfttdzjub.sHtML

[A26] 类型转换总览
来源：http://www.m.share.yfazqb.com/Article/details/goaoibkvz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.bbcook.cn/Article/details/gkglabrgv.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.bbcook.cn/Article/details/gzvsgixaq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.tarul.cn/Article/details/gukgdvetw.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.epnwcf.com/Article/details/ghrqqtqlw.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.vehdjk.com/Article/details/gqbtlnsal.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.sjlbkw.cn/Article/details/gmjevpggb.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.epnwcf.com/Article/details/gmbfhogwh.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.epnwcf.com/Article/details/gcrlvfgjm.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gqqmewmoe.sHtML

B. 流程控制
来源：http://www.blog.bbcook.cn/Article/details/glxwtmbaw.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gurtdlodz.sHtML

[B01] 条件判断 if / else
来源：http://www.share.yfazqb.com/Article/details/gnkkmmhwt.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.fktsv.cn/Article/details/gisjuubch.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.fktsv.cn/Article/details/gxrfmbxzz.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlrnhvne.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.vehdjk.com/Article/details/gwcjqverf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.vehdjk.com/Article/details/gtsktckje.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.tarul.cn/Article/details/gqwdqebka.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.yfazqb.com/Article/details/gwjndogxp.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.bbcook.cn/Article/details/gtmojxbzq.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.vehdjk.com/Article/details/gniznmgpj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.epnwcf.com/Article/details/gztckcaqf.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.epnwcf.com/Article/details/gpzrkjhgu.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.epnwcf.com/Article/details/gikzjlrsq.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.vehdjk.com/Article/details/gpqlzsned.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.epnwcf.com/Article/details/geioiixnv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.sjlbkw.cn/Article/details/gbjqqelcb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.yfazqb.com/Article/details/gxvdgoonu.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fktsv.cn/Article/details/gpdhhbent.sHtML

[B03] switch / match / case
来源：http://read.share.vehdjk.com/Article/details/gcxmqlpkn.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.vehdjk.com/Article/details/gnussnoci.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/ggqfdggmz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.epnwcf.com/Article/details/ghmscrolu.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.epnwcf.com/Article/details/gzuvpxwfg.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/ghpfivlim.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.vehdjk.com/Article/details/ggydtjwkk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.epnwcf.com/Article/details/gvmqodlpl.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.yfazqb.com/Article/details/gfqqltmjs.sHtML

[B04] for 计数循环
来源：http://read.share.epnwcf.com/Article/details/gwcnnaaxu.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.tarul.cn/Article/details/gkdaecwts.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.fktsv.cn/Article/details/galjnqdzi.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.yfazqb.com/Article/details/glngzgoav.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.tarul.cn/Article/details/gbhkqmbcw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fktsv.cn/Article/details/gwoqmjtfj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.bbcook.cn/Article/details/gicpedcpl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.vehdjk.com/Article/details/gvdrsmuqd.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.vehdjk.com/Article/details/gciolbfyu.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gpgttjnkw.sHtML

Py:   for item in arr: print(item)
来源：http://3g.vehdjk.com/Article/details/gpmqlyyek.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.epnwcf.com/Article/details/gczuhkjel.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gipohobhc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.vehdjk.com/Article/details/ghyyqsnam.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.bbcook.cn/Article/details/gxgsduqpo.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.sjlbkw.cn/Article/details/guofmdeci.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.fktsv.cn/Article/details/grmblyiif.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.yfazqb.com/Article/details/gpnbtbbji.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.fktsv.cn/Article/details/gzgrjybfs.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.yfazqb.com/Article/details/gyjshjumk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.vehdjk.com/Article/details/gczthrldy.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.yfazqb.com/Article/details/gqxylczwh.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fktsv.cn/Article/details/gwqiyamjl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.vehdjk.com/Article/details/gigwhveek.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.yfazqb.com/Article/details/gkgfdpwqn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.bbcook.cn/Article/details/gpzmuiwxh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.bbcook.cn/Article/details/glbxlawkp.sHtML

[B07] while 循环
来源：http://wap.epnwcf.com/Article/details/gjgmiyiss.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.yfazqb.com/Article/details/gpkxrlyoy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.yfazqb.com/Article/details/gxbigvmak.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gfwoagbnw.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/glahuqgqa.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.vehdjk.com/Article/details/ggddqhqlz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.vehdjk.com/Article/details/gbflzhmgx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.tarul.cn/Article/details/gfufuupsi.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.tarul.cn/Article/details/gzxdgqgum.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.bbcook.cn/Article/details/gfwxpvpbh.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.epnwcf.com/Article/details/gluuczogz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.tarul.cn/Article/details/gjwveppsu.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fktsv.cn/Article/details/gdqaanwuy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.bbcook.cn/Article/details/guzblwfyc.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/gsqnkluta.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.vehdjk.com/Article/details/gxetpgvaq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.vehdjk.com/Article/details/gdtaagriw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.epnwcf.com/Article/details/gnnjnygfa.sHtML

[B09] break 与 continue
来源：http://m.share.tarul.cn/Article/details/gjupnuzoz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.epnwcf.com/Article/details/gyjcfokzb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gmglkdtcb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fktsv.cn/Article/details/gjcqhwera.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gqachsdyc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/ghtubjret.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.bbcook.cn/Article/details/grgtskeln.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fktsv.cn/Article/details/gsptkcdhh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gjwotnrgf.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fktsv.cn/Article/details/gdcugssjk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.yfazqb.com/Article/details/gljevmvss.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.epnwcf.com/Article/details/gtewonfgv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.sjlbkw.cn/Article/details/gjznglzkb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.sjlbkw.cn/Article/details/gaiewpppx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.epnwcf.com/Article/details/ggruuznxz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.vehdjk.com/Article/details/gcfopifnl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fktsv.cn/Article/details/gqnlwcube.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.sjlbkw.cn/Article/details/gispbymxs.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fktsv.cn/Article/details/gwtyymutf.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.sjlbkw.cn/Article/details/gzxrebrkk.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gltwwfduo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.bbcook.cn/Article/details/gdcyoleck.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.vehdjk.com/Article/details/gqfgluagv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fktsv.cn/Article/details/gucqarqrj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.bbcook.cn/Article/details/gfminvtuw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fktsv.cn/Article/details/gdvjnulno.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.tarul.cn/Article/details/gajomndyv.sHtML

[B12] 跳出多层循环
来源：http://read.share.fktsv.cn/Article/details/grthjtpms.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fktsv.cn/Article/details/gxmjbxwpa.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.tarul.cn/Article/details/gkcyszngu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/gkeueocwb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fktsv.cn/Article/details/gdehfvbae.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fktsv.cn/Article/details/gvmirnnyg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fktsv.cn/Article/details/ghddfyivl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.tarul.cn/Article/details/gyqisuefh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fktsv.cn/Article/details/gqdgnvhwq.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.tarul.cn/Article/details/gdmjpofks.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.tarul.cn/Article/details/gcmqohpdy.sHtML

PHP:  is_numeric($x)
来源：http://blog.fktsv.cn/Article/details/gjuerlteq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.epnwcf.com/Article/details/gcsmlnpnq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fktsv.cn/Article/details/ginyegcmh.sHtML

Java: x instanceof Number
来源：http://mobile.yfazqb.com/Article/details/gvtztxgie.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.sjlbkw.cn/Article/details/gkvfkvxkr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.sjlbkw.cn/Article/details/gbrgeblae.sHtML

C#:   x is int or double or decimal
来源：http://mobile.epnwcf.com/Article/details/gduedffoz.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.epnwcf.com/Article/details/gmagemkjm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.vehdjk.com/Article/details/gnwbwfsyz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.vehdjk.com/Article/details/gyymzzzew.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fktsv.cn/Article/details/gftzeqrtc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/gweqcqenl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.yfazqb.com/Article/details/gracaguqu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.sjlbkw.cn/Article/details/gbditiqri.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fktsv.cn/Article/details/gemmjukvx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.vehdjk.com/Article/details/gasqwdaln.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.sjlbkw.cn/Article/details/giytmskkc.sHtML

Py:   a and b or not c
来源：http://www.m.share.bbcook.cn/Article/details/gvvqlmybs.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fktsv.cn/Article/details/gcfmlhyzn.sHtML

JS:   a && b || !c
来源：http://baike.bbcook.cn/Article/details/gzqbepyjr.sHtML

TS:   a && b || !c
来源：http://wap.vehdjk.com/Article/details/goxcarxrm.sHtML

Java: a && b || !c
来源：http://wap.vehdjk.com/Article/details/gkpcabrkh.sHtML

Go:   a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gstkorjcg.sHtML

Ruby: a && b || !c
来源：http://read.share.tarul.cn/Article/details/gjdlqcmpl.sHtML

C#:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gslytitzi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.epnwcf.com/Article/details/gynyxqbor.sHtML

Py:   if not data: return
来源：http://blog.vehdjk.com/Article/details/gbaaymhoz.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.sjlbkw.cn/Article/details/gjhjmlkbr.sHtML

JS:   if (!data) return;
来源：http://www.share.vehdjk.com/Article/details/glwlnvsae.sHtML

TS:   if (!data) return;
来源：http://mobile.sjlbkw.cn/Article/details/gqipggqug.sHtML

Java: if (data == null) return;
来源：http://m.share.tarul.cn/Article/details/geoxuvknt.sHtML

Go:   if data == nil { return }
来源：http://read.share.vehdjk.com/Article/details/grvgfuhnb.sHtML

Ruby: return if data.nil?
来源：http://3g.vehdjk.com/Article/details/gjbfpxevd.sHtML

C#:   if (data == null) return;
来源：http://blog.epnwcf.com/Article/details/gyowbjdzf.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gutpgmbdc.sHtML

C. 函数与作用域
来源：http://baike.vehdjk.com/Article/details/gipprqduu.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gxavptgrd.sHtML

[C01] 定义函数
来源：http://mobile.epnwcf.com/Article/details/gmpibeksa.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.vehdjk.com/Article/details/gdbxsobwy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/glzptwyrr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gfzqwzmmd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gnkcknyku.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.tarul.cn/Article/details/gygroupmh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.sjlbkw.cn/Article/details/gzmmhopdp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.sjlbkw.cn/Article/details/guwuovfxe.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gyocpghfv.sHtML

[C02] 默认参数
来源：http://blog.bbcook.cn/Article/details/gyhbglsdb.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.tarul.cn/Article/details/gqjrqsujk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.tarul.cn/Article/details/gkfvbfhne.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fktsv.cn/Article/details/gkilqtykv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fktsv.cn/Article/details/ghyatzbhc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.sjlbkw.cn/Article/details/gekdbtpbf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.sjlbkw.cn/Article/details/gfhqarzbo.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.epnwcf.com/Article/details/gjzjdojjy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.sjlbkw.cn/Article/details/gvjauircb.sHtML

[C03] 可变参数
来源：http://www.blog.sjlbkw.cn/Article/details/gyihxpkyo.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.sjlbkw.cn/Article/details/gnhxtwags.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fktsv.cn/Article/details/gwfglumcz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fktsv.cn/Article/details/gmgostflu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.epnwcf.com/Article/details/gxtytzdnr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.bbcook.cn/Article/details/gxmahlzgk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.sjlbkw.cn/Article/details/gkxpzzkxh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.vehdjk.com/Article/details/gtxocrjtf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.sjlbkw.cn/Article/details/ggvkllgcg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.bbcook.cn/Article/details/gbzirwhvd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.vehdjk.com/Article/details/giwzatpgd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.vehdjk.com/Article/details/gawitwljd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fktsv.cn/Article/details/gfhraeqzz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fktsv.cn/Article/details/ghmryjksk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.epnwcf.com/Article/details/gxnqetllj.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.yfazqb.com/Article/details/gbbegqhcb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.yfazqb.com/Article/details/gaocmhshx.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.yfazqb.com/Article/details/ggbmftvpd.sHtML

[C05] 返回多个值
来源：http://baike.yfazqb.com/Article/details/girninhjd.sHtML

Py:   return a, b
来源：http://www.m.share.vehdjk.com/Article/details/gosbtncrg.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fktsv.cn/Article/details/glmpxhhht.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.vehdjk.com/Article/details/grpkoboce.sHtML

TS:   return { a, b };
来源：http://m.share.fktsv.cn/Article/details/gzstsoriy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.yfazqb.com/Article/details/gekyvurme.sHtML

Go:   return a, b
来源：http://m.share.fktsv.cn/Article/details/ghcpdkgva.sHtML

Ruby: return a, b
来源：http://3g.yfazqb.com/Article/details/gemileovp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.epnwcf.com/Article/details/gkobqbyar.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.vehdjk.com/Article/details/gwaipwlkv.sHtML

Py:   square = lambda x: x * x
来源：http://blog.bbcook.cn/Article/details/gwvocrzgt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.yfazqb.com/Article/details/ggdvcpvua.sHtML

JS:   const square = x => x * x;
来源：http://blog.yfazqb.com/Article/details/grrfruiqi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.tarul.cn/Article/details/gcwmjyhwt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.yfazqb.com/Article/details/gvwdusuix.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.yfazqb.com/Article/details/ggemeuldw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.sjlbkw.cn/Article/details/ghbtgoxki.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.epnwcf.com/Article/details/gtqctebdi.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fktsv.cn/Article/details/gflunybkc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.yfazqb.com/Article/details/gdkrfepbn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fktsv.cn/Article/details/gvsbtgyka.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.bbcook.cn/Article/details/gklivejly.sHtML

TS:   arr.map(String)
来源：http://baike.sjlbkw.cn/Article/details/gligorowv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.tarul.cn/Article/details/gdmbrxlgg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.epnwcf.com/Article/details/gydqnpuce.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.tarul.cn/Article/details/gcvffhirx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.tarul.cn/Article/details/gxqklkfwv.sHtML

[C08] 闭包
来源：http://mobile.epnwcf.com/Article/details/glvwgzkzz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.bbcook.cn/Article/details/gwkixlmtm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.tarul.cn/Article/details/ghsbgccas.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.sjlbkw.cn/Article/details/girzlpnlp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fktsv.cn/Article/details/gbtxroduu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.vehdjk.com/Article/details/goswvrytf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.tarul.cn/Article/details/gkvsfzbkf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.vehdjk.com/Article/details/gesstzmjc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.epnwcf.com/Article/details/ggzaajskw.sHtML

[C09] 递归
来源：http://www.blog.fktsv.cn/Article/details/gwbzgqptt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fktsv.cn/Article/details/giwrecbqe.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.sjlbkw.cn/Article/details/gessesbuq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.vehdjk.com/Article/details/gkretyqwj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.vehdjk.com/Article/details/gzzsmuohw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.bbcook.cn/Article/details/gegcbiiye.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.bbcook.cn/Article/details/gcqsqjcfx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.sjlbkw.cn/Article/details/gdzertfqj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.vehdjk.com/Article/details/gznnyyqxp.sHtML


<!-- 参考信息 -->