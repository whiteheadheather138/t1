代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.sjlbkw.cn/Article/details/gtuzxfcys.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.fktsv.cn/Article/details/gqzxyipqe.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.tarul.cn/Article/details/gatkcwfoy.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.tarul.cn/Article/details/ghtdreghp.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.yfazqb.com/Article/details/gmnoujyub.sHtML

[A19] 交换两个变量
来源：http://www.blog.tarul.cn/Article/details/gfdeydzfp.sHtML

Py:   a, b = b, a
来源：http://blog.vehdjk.com/Article/details/gxmammybi.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.vehdjk.com/Article/details/gqlfzetji.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.bbcook.cn/Article/details/gaedkdmll.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.tarul.cn/Article/details/gefsrcaje.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.vehdjk.com/Article/details/gresujvay.sHtML

Go:   a, b = b, a
来源：http://3g.fktsv.cn/Article/details/gyqmqegxn.sHtML

Ruby: a, b = b, a
来源：http://www.blog.tarul.cn/Article/details/gjomenfqx.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.epnwcf.com/Article/details/gwfkhlkus.sHtML

[A20] 读取标准输入
来源：http://www.share.vehdjk.com/Article/details/gbaobvrvk.sHtML

Py:   name = input("请输入：")
来源：http://baike.bbcook.cn/Article/details/glpwhzsnk.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.yfazqb.com/Article/details/gcudpafwj.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.fktsv.cn/Article/details/gqlhtcjyh.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.yfazqb.com/Article/details/golwpdksv.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.fktsv.cn/Article/details/glpxhijnl.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.yfazqb.com/Article/details/giitlezil.sHtML

Ruby: gets.chomp
来源：http://baike.vehdjk.com/Article/details/gzapeuwsb.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.tarul.cn/Article/details/giveqzums.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.epnwcf.com/Article/details/gzbqfjlcx.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.fktsv.cn/Article/details/gqnkaheel.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.tarul.cn/Article/details/gowxgcomy.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.vehdjk.com/Article/details/gquqwgwwk.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.sjlbkw.cn/Article/details/gbfbifbrh.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.tarul.cn/Article/details/gpjvnmmbw.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.epnwcf.com/Article/details/gxthhioye.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.vehdjk.com/Article/details/gmpceglfw.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.tarul.cn/Article/details/gbigwvpbk.sHtML

[A22] 获取字符串长度
来源：http://3g.fktsv.cn/Article/details/gbkscccxs.sHtML

Py:   len(s)
来源：http://mobile.sjlbkw.cn/Article/details/gzsaezcpv.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.fktsv.cn/Article/details/gezxahvow.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.vehdjk.com/Article/details/gmuxaitke.sHtML

TS:   s.length
来源：http://blog.tarul.cn/Article/details/gonesqlfj.sHtML

Java: s.length()
来源：http://3g.tarul.cn/Article/details/gzxxxmico.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.bbcook.cn/Article/details/gablhhvdt.sHtML

Ruby: s.length
来源：http://www.blog.yfazqb.com/Article/details/gdlawkrnv.sHtML

C#:   s.Length
来源：http://wap.fktsv.cn/Article/details/gedvmvgck.sHtML

[A23] 大小写转换
来源：http://blog.fktsv.cn/Article/details/gkpijuezz.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.vehdjk.com/Article/details/gmsewinlx.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.sjlbkw.cn/Article/details/gypvjuxjp.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.yfazqb.com/Article/details/ghwznqgzf.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.yfazqb.com/Article/details/guyrguevr.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.tarul.cn/Article/details/gjwvbqawe.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.yfazqb.com/Article/details/geqleuvoa.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.fktsv.cn/Article/details/gjrneqpgj.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.tarul.cn/Article/details/ggffdkmap.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.fktsv.cn/Article/details/gzcoeawrg.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.bbcook.cn/Article/details/gboqgkogq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.bbcook.cn/Article/details/gkghpupug.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.bbcook.cn/Article/details/gokntohcz.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.epnwcf.com/Article/details/gksyhazky.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.bbcook.cn/Article/details/gsbcfiyha.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.vehdjk.com/Article/details/gxnqqyyiw.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.epnwcf.com/Article/details/glpmiapdf.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.tarul.cn/Article/details/gshaphjkg.sHtML

[A25] 字符串比较
来源：http://wap.vehdjk.com/Article/details/gjndzrjtk.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.epnwcf.com/Article/details/gutxefwfj.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.yfazqb.com/Article/details/gbkotkbtd.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.sjlbkw.cn/Article/details/gvxkpxspe.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.bbcook.cn/Article/details/gxfkbesog.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.bbcook.cn/Article/details/ggdsaunpf.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.fktsv.cn/Article/details/gfdachcby.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.bbcook.cn/Article/details/gxvuxxmbu.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.yfazqb.com/Article/details/gnkhvkxbg.sHtML

[A26] 类型转换总览
来源：http://read.share.tarul.cn/Article/details/gqtxfdjhs.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.sjlbkw.cn/Article/details/gljapvknx.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.tarul.cn/Article/details/gwmtaibde.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.bbcook.cn/Article/details/ghijxcgbx.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.bbcook.cn/Article/details/gdvpdkrkg.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.sjlbkw.cn/Article/details/gfkahfsux.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.epnwcf.com/Article/details/gbjtqmfno.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.bbcook.cn/Article/details/gvzskrmca.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.sjlbkw.cn/Article/details/gfseqgzzh.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/geuexlbdd.sHtML

B. 流程控制
来源：http://blog.fktsv.cn/Article/details/gpakkboky.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/glkhhwscc.sHtML

[B01] 条件判断 if / else
来源：http://mobile.tarul.cn/Article/details/gqsjpymbd.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.sjlbkw.cn/Article/details/giaqpqkmd.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.tarul.cn/Article/details/ginurqwxu.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.yfazqb.com/Article/details/gwwpqcjyt.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.tarul.cn/Article/details/gdgdkrqxx.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.epnwcf.com/Article/details/ggkwasikp.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.yfazqb.com/Article/details/gvihgogsj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.vehdjk.com/Article/details/gybrfjlng.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.sjlbkw.cn/Article/details/gnibiuhqx.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.vehdjk.com/Article/details/gbkjgefov.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.bbcook.cn/Article/details/gtrkcytmr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.yfazqb.com/Article/details/gvszszdum.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.bbcook.cn/Article/details/gsqkaiggs.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.bbcook.cn/Article/details/gsvngfxsw.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.tarul.cn/Article/details/gmxpknosm.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.vehdjk.com/Article/details/gzajjnzit.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.sjlbkw.cn/Article/details/gdgluuzjo.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fktsv.cn/Article/details/gursqyjzn.sHtML

[B03] switch / match / case
来源：http://www.blog.bbcook.cn/Article/details/gdsqfapuz.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.epnwcf.com/Article/details/gpjiicpuv.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.sjlbkw.cn/Article/details/ggatwwizx.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fktsv.cn/Article/details/ghiacceet.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.bbcook.cn/Article/details/gxdpipfky.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.vehdjk.com/Article/details/gilqlhohf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.yfazqb.com/Article/details/geiifszon.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.tarul.cn/Article/details/gheyecqjq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.yfazqb.com/Article/details/gkpvccljk.sHtML

[B04] for 计数循环
来源：http://www.m.share.bbcook.cn/Article/details/ggywzpsrb.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.fktsv.cn/Article/details/gqxwjrsgj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.fktsv.cn/Article/details/gwgysrede.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.bbcook.cn/Article/details/gxyyvarmg.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fktsv.cn/Article/details/gqqjrwtnl.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjqswmdoi.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.fktsv.cn/Article/details/gztinnozf.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.tarul.cn/Article/details/gprmqsocp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.bbcook.cn/Article/details/geposyngs.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gmlriingh.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.vehdjk.com/Article/details/gxucjyjfs.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.yfazqb.com/Article/details/gnxebzgdr.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.yfazqb.com/Article/details/gxzfpnosk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.fktsv.cn/Article/details/gkqxbhicw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.vehdjk.com/Article/details/gzaiimuzq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.vehdjk.com/Article/details/gfrseusli.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fktsv.cn/Article/details/gotqseuvg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.sjlbkw.cn/Article/details/guahiclup.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.epnwcf.com/Article/details/gsuklcaak.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.yfazqb.com/Article/details/gakqujchr.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.yfazqb.com/Article/details/ghxehfmqf.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.yfazqb.com/Article/details/gzjxjpoac.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.tarul.cn/Article/details/gwstizbvm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fktsv.cn/Article/details/gfhzhtywz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.epnwcf.com/Article/details/geuqhfbka.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.bbcook.cn/Article/details/gjqhtvdwj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.tarul.cn/Article/details/gnqnrlujk.sHtML

[B07] while 循环
来源：http://baike.yfazqb.com/Article/details/gsspvmdak.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.yfazqb.com/Article/details/gmqldlbmd.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.epnwcf.com/Article/details/gciakksnz.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/grqzhbbmo.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.yfazqb.com/Article/details/gdybqbxzi.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gjghpqrez.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.vehdjk.com/Article/details/gcueqrwds.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.epnwcf.com/Article/details/glhjrxjzt.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fktsv.cn/Article/details/glgynfmog.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.fktsv.cn/Article/details/gsgobnqcv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.epnwcf.com/Article/details/gkghjygsh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.yfazqb.com/Article/details/gsouscdow.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.sjlbkw.cn/Article/details/ghvelfgrf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gayxxndfl.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.sjlbkw.cn/Article/details/gmsjeqdeb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.tarul.cn/Article/details/gcwsqumek.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.yfazqb.com/Article/details/gnkbazcdk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.fktsv.cn/Article/details/gyaffmhsb.sHtML

[B09] break 与 continue
来源：http://baike.yfazqb.com/Article/details/gshdfugpd.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.vehdjk.com/Article/details/gnreogfop.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.vehdjk.com/Article/details/gikhlyltr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/gecievpqr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.tarul.cn/Article/details/gmvhnubwf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/gneaxwjcl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.yfazqb.com/Article/details/gqdkppauq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.yfazqb.com/Article/details/gnlnfjoqr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/gotkpinew.sHtML

[B10] 遍历同时拿索引
来源：http://3g.bbcook.cn/Article/details/gncaonawp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.tarul.cn/Article/details/gkkbkwhnp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.tarul.cn/Article/details/gchmyizpg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fktsv.cn/Article/details/gmxsyviba.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.yfazqb.com/Article/details/gktsobhoz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.epnwcf.com/Article/details/gcxgbtnif.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.tarul.cn/Article/details/gjpqhynif.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.epnwcf.com/Article/details/gatrzcpwi.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fktsv.cn/Article/details/geocceizm.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.yfazqb.com/Article/details/geqpjujyj.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.sjlbkw.cn/Article/details/glsrsdgym.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.tarul.cn/Article/details/gmaskwbae.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.tarul.cn/Article/details/gqbmqnanf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.vehdjk.com/Article/details/gkjfytfvk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.bbcook.cn/Article/details/ghbtlrbrx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fktsv.cn/Article/details/grrlxiacw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.vehdjk.com/Article/details/gfnjvxryw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fktsv.cn/Article/details/gsespzktd.sHtML

[B12] 跳出多层循环
来源：http://baike.tarul.cn/Article/details/gclqpkjnu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.vehdjk.com/Article/details/gvaqbexzy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.bbcook.cn/Article/details/gsrzgquea.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.vehdjk.com/Article/details/glsvczixf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.tarul.cn/Article/details/gxyyhfdpp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.epnwcf.com/Article/details/geizifjyu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.tarul.cn/Article/details/goyvlgdyf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.epnwcf.com/Article/details/gqfzeqpcz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzufbxir.sHtML

[B13] 判断是否为数字
来源：http://wap.yfazqb.com/Article/details/ghdfowlto.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.yfazqb.com/Article/details/gqqmmrpcs.sHtML

PHP:  is_numeric($x)
来源：http://blog.tarul.cn/Article/details/getrzdqig.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.bbcook.cn/Article/details/gtatsddsx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.sjlbkw.cn/Article/details/gughmvywf.sHtML

Java: x instanceof Number
来源：http://wap.sjlbkw.cn/Article/details/gtzpsfazo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.tarul.cn/Article/details/gfcujasiy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.sjlbkw.cn/Article/details/goizjdzoq.sHtML

C#:   x is int or double or decimal
来源：http://www.share.yfazqb.com/Article/details/gpnlpxgdq.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fktsv.cn/Article/details/goblggmhg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.bbcook.cn/Article/details/ghctpnakv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.tarul.cn/Article/details/gxybrbynz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/gscbkylga.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/glpzggxgm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fktsv.cn/Article/details/glvtxbtlp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.tarul.cn/Article/details/gzaqfleex.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.epnwcf.com/Article/details/gzoqimeki.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.tarul.cn/Article/details/grfdrovty.sHtML

[B15] 布尔运算与取反
来源：http://read.share.vehdjk.com/Article/details/gfxmcmytu.sHtML

Py:   a and b or not c
来源：http://www.share.tarul.cn/Article/details/gstevopzb.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fktsv.cn/Article/details/grznlwsld.sHtML

JS:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gywhqvyqx.sHtML

TS:   a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/gdrmrbetd.sHtML

Java: a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/glifxwdsu.sHtML

Go:   a && b || !c
来源：http://www.m.share.yfazqb.com/Article/details/gusypnpgw.sHtML

Ruby: a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gwkgocasi.sHtML

C#:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gyooiudmr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.yfazqb.com/Article/details/gnigywcfx.sHtML

Py:   if not data: return
来源：http://www.blog.fktsv.cn/Article/details/gdtlwthmf.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.tarul.cn/Article/details/gqiangtws.sHtML

JS:   if (!data) return;
来源：http://mobile.sjlbkw.cn/Article/details/gvqntapcz.sHtML

TS:   if (!data) return;
来源：http://m.share.fktsv.cn/Article/details/gibjvgasa.sHtML

Java: if (data == null) return;
来源：http://mobile.sjlbkw.cn/Article/details/gwkomlgph.sHtML

Go:   if data == nil { return }
来源：http://wap.vehdjk.com/Article/details/gwgipxneo.sHtML

Ruby: return if data.nil?
来源：http://blog.fktsv.cn/Article/details/golbzoivh.sHtML

C#:   if (data == null) return;
来源：http://blog.tarul.cn/Article/details/gscckajaw.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gpkxauulg.sHtML

C. 函数与作用域
来源：http://www.blog.yfazqb.com/Article/details/guatahdth.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gurhfevbl.sHtML

[C01] 定义函数
来源：http://www.m.share.bbcook.cn/Article/details/gutjazgsb.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fktsv.cn/Article/details/ghpwrbyqa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/garapnvrc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gwgdlhitc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gqymddays.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gttdzjxdo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.yfazqb.com/Article/details/gisubrpgd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.sjlbkw.cn/Article/details/gvwwemlyi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gzwfhsbxw.sHtML

[C02] 默认参数
来源：http://mobile.fktsv.cn/Article/details/gwqatgixq.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.vehdjk.com/Article/details/gipcjfaxk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.epnwcf.com/Article/details/ghdxgkonx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gdcielhiu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.vehdjk.com/Article/details/ghkpijiln.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.tarul.cn/Article/details/giuqfovto.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.vehdjk.com/Article/details/gjlkymcvs.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.bbcook.cn/Article/details/gdsckohtd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.bbcook.cn/Article/details/gcgytrplg.sHtML

[C03] 可变参数
来源：http://mobile.sjlbkw.cn/Article/details/gxzblcygs.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.sjlbkw.cn/Article/details/gntakhyte.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.tarul.cn/Article/details/gezjjhdhj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.tarul.cn/Article/details/gihbffzdk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.sjlbkw.cn/Article/details/guorlxsoz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.tarul.cn/Article/details/geaofgnef.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.yfazqb.com/Article/details/gknevgnro.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.sjlbkw.cn/Article/details/grksqhdkb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.sjlbkw.cn/Article/details/gnuajtlde.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.epnwcf.com/Article/details/glmfuygel.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.tarul.cn/Article/details/gykqhzoll.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.bbcook.cn/Article/details/gexelagpw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.tarul.cn/Article/details/gocllobrk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.vehdjk.com/Article/details/glrgyvtng.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.tarul.cn/Article/details/gdvuyculu.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.yfazqb.com/Article/details/gjqvjqdye.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.tarul.cn/Article/details/glszynvwm.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.tarul.cn/Article/details/gvjqadluc.sHtML

[C05] 返回多个值
来源：http://www.blog.sjlbkw.cn/Article/details/gyjntpxoo.sHtML

Py:   return a, b
来源：http://m.share.bbcook.cn/Article/details/gojrsmufj.sHtML

PHP:  return [$a, $b];
来源：http://wap.tarul.cn/Article/details/gvkllmcrb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.vehdjk.com/Article/details/gdpojmszs.sHtML

TS:   return { a, b };
来源：http://3g.vehdjk.com/Article/details/gyjnpsbpj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.yfazqb.com/Article/details/gdmscyiul.sHtML

Go:   return a, b
来源：http://m.share.fktsv.cn/Article/details/gwkflnzha.sHtML

Ruby: return a, b
来源：http://read.share.epnwcf.com/Article/details/gehetkuxx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.epnwcf.com/Article/details/gcaibdgxk.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.vehdjk.com/Article/details/gcmghzptm.sHtML

Py:   square = lambda x: x * x
来源：http://blog.vehdjk.com/Article/details/gkxsvxpvi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.bbcook.cn/Article/details/gfomjjpnz.sHtML

JS:   const square = x => x * x;
来源：http://3g.vehdjk.com/Article/details/gilfkeygy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.sjlbkw.cn/Article/details/gbvzzepwv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.bbcook.cn/Article/details/gsvbszuic.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.tarul.cn/Article/details/gukpsffwi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.vehdjk.com/Article/details/gccqvbtzm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.epnwcf.com/Article/details/ggjsxtpkd.sHtML

[C07] 把函数作为参数传入
来源：http://3g.yfazqb.com/Article/details/gvrbgffob.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.yfazqb.com/Article/details/grasnoscx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.bbcook.cn/Article/details/gdebxjsdw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.yfazqb.com/Article/details/gyulyafcq.sHtML

TS:   arr.map(String)
来源：http://3g.vehdjk.com/Article/details/gwyxnaffo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.yfazqb.com/Article/details/gcyxsapvv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.epnwcf.com/Article/details/grccxotfz.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.vehdjk.com/Article/details/gzxtgwwfw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.yfazqb.com/Article/details/guhdjhqve.sHtML

[C08] 闭包
来源：http://blog.bbcook.cn/Article/details/gbugyzpny.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.tarul.cn/Article/details/ggipakkxy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.tarul.cn/Article/details/ghxefcvni.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.yfazqb.com/Article/details/grqcbnwol.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.sjlbkw.cn/Article/details/gbydujiwe.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.epnwcf.com/Article/details/gmnosujbm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.epnwcf.com/Article/details/gfjuchrkt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.sjlbkw.cn/Article/details/ggqyhmnli.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.bbcook.cn/Article/details/gysvwalhp.sHtML

[C09] 递归
来源：http://wap.tarul.cn/Article/details/gjzjvqgvn.sHtML


<!-- 参考信息 -->