代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.fktsv.cn/Article/details/goheyvtpe.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.fktsv.cn/Article/details/getfvnpyx.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.vehdjk.com/Article/details/gwpceaszv.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.yfazqb.com/Article/details/glgcnnggk.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.yfazqb.com/Article/details/gxbonlzho.sHtML

Ruby: gets.chomp
来源：http://3g.bbcook.cn/Article/details/gyiqnfpip.sHtML

C#:   Console.ReadLine();
来源：http://baike.bbcook.cn/Article/details/ggsdbqxfq.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.tarul.cn/Article/details/gkmkgwddp.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.epnwcf.com/Article/details/glsajwfhu.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.fktsv.cn/Article/details/gejvajzgi.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.vehdjk.com/Article/details/gtbcxrvzs.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.sjlbkw.cn/Article/details/gsvwxujjn.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.epnwcf.com/Article/details/gjhelrdrh.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.bbcook.cn/Article/details/gheddittz.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.fktsv.cn/Article/details/ggpdkqycl.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.yfazqb.com/Article/details/ghknvliyo.sHtML

[A22] 获取字符串长度
来源：http://www.share.epnwcf.com/Article/details/gyartcyyu.sHtML

Py:   len(s)
来源：http://3g.bbcook.cn/Article/details/gaxzrnjqq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.sjlbkw.cn/Article/details/gfqheolbc.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.yfazqb.com/Article/details/gjlqvwzhz.sHtML

TS:   s.length
来源：http://baike.vehdjk.com/Article/details/gxweyfsbl.sHtML

Java: s.length()
来源：http://wap.yfazqb.com/Article/details/gwddhxpib.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.bbcook.cn/Article/details/geettkcyb.sHtML

Ruby: s.length
来源：http://wap.sjlbkw.cn/Article/details/ghehaxcbn.sHtML

C#:   s.Length
来源：http://www.blog.epnwcf.com/Article/details/gnirxbwmt.sHtML

[A23] 大小写转换
来源：http://baike.sjlbkw.cn/Article/details/gyidntxlo.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.sjlbkw.cn/Article/details/gohtfhbue.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.epnwcf.com/Article/details/gczevlwzv.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.epnwcf.com/Article/details/gdzodgsfl.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.yfazqb.com/Article/details/gpeemarhf.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.tarul.cn/Article/details/ggsdmdeoy.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.sjlbkw.cn/Article/details/gwnfzaryb.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.epnwcf.com/Article/details/gyikwdzfa.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.yfazqb.com/Article/details/gtcmydnfc.sHtML

[A24] 去除首尾空白
来源：http://blog.fktsv.cn/Article/details/guyrutezt.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.epnwcf.com/Article/details/gcmehjuen.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.fktsv.cn/Article/details/glkqocryx.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fktsv.cn/Article/details/gxipkkcut.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.vehdjk.com/Article/details/gzdpkxbag.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.yfazqb.com/Article/details/gpohqyivw.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.fktsv.cn/Article/details/geouhzgyb.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.sjlbkw.cn/Article/details/gusoefhzr.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.bbcook.cn/Article/details/gccegwvyl.sHtML

[A25] 字符串比较
来源：http://www.share.fktsv.cn/Article/details/ghkazqbtz.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.vehdjk.com/Article/details/gwmesejsz.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.bbcook.cn/Article/details/gfzgumodr.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.yfazqb.com/Article/details/grhsapsjg.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fktsv.cn/Article/details/galmzlere.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.epnwcf.com/Article/details/gqencjbqk.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.yfazqb.com/Article/details/giazusmhj.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.bbcook.cn/Article/details/gjekpwdhc.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.bbcook.cn/Article/details/gaqvjafha.sHtML

[A26] 类型转换总览
来源：http://www.blog.yfazqb.com/Article/details/gndliqfnw.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.fktsv.cn/Article/details/gwndsddua.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.bbcook.cn/Article/details/gghayysgw.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.sjlbkw.cn/Article/details/gccpysksd.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.yfazqb.com/Article/details/grkiudruy.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.sjlbkw.cn/Article/details/gaivgjauc.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.epnwcf.com/Article/details/gusgfdrgy.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.yfazqb.com/Article/details/gsolcuhfv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.sjlbkw.cn/Article/details/gxatmuekj.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gepduoopt.sHtML

B. 流程控制
来源：http://www.m.share.fktsv.cn/Article/details/gypvstilx.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gnmhabrlo.sHtML

[B01] 条件判断 if / else
来源：http://wap.yfazqb.com/Article/details/gjybqqhmt.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.tarul.cn/Article/details/gxgvyfnxs.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.epnwcf.com/Article/details/gsefkriak.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.yfazqb.com/Article/details/gloymokvf.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.sjlbkw.cn/Article/details/gkfgqwzjx.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.vehdjk.com/Article/details/gnnyigyia.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.yfazqb.com/Article/details/ggmdiwdqb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.yfazqb.com/Article/details/gjznpujxu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.bbcook.cn/Article/details/gktlcxfpt.sHtML

[B02] 多分支 else if / elif
来源：http://3g.fktsv.cn/Article/details/gqrbwgmmc.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.epnwcf.com/Article/details/gfyhlghfm.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.tarul.cn/Article/details/grxqkpxwg.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.yfazqb.com/Article/details/gubsdicyc.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.sjlbkw.cn/Article/details/gccxiholc.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.bbcook.cn/Article/details/govgkkqqz.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.vehdjk.com/Article/details/guolsxvci.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.epnwcf.com/Article/details/gccucmcmh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.epnwcf.com/Article/details/ghvwdprek.sHtML

[B03] switch / match / case
来源：http://mobile.fktsv.cn/Article/details/gblnaumlt.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.epnwcf.com/Article/details/gnzstomfi.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.tarul.cn/Article/details/gmbgxfqoe.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.vehdjk.com/Article/details/gwtwjbrem.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.sjlbkw.cn/Article/details/gbqoqdxpj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.fktsv.cn/Article/details/gsedshtrq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.vehdjk.com/Article/details/gkilotldo.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.yfazqb.com/Article/details/gvvwhynqx.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.fktsv.cn/Article/details/ghatgojuf.sHtML

[B04] for 计数循环
来源：http://m.share.bbcook.cn/Article/details/guxxgopmy.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.fktsv.cn/Article/details/gndiguxpq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.bbcook.cn/Article/details/ggakfjxpz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.vehdjk.com/Article/details/gytjcprzk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.vehdjk.com/Article/details/gdlcphrcm.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.fktsv.cn/Article/details/gceqmsjpy.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.bbcook.cn/Article/details/ggepvrqbj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.tarul.cn/Article/details/gyfmctewe.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.yfazqb.com/Article/details/gvuczeczd.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.fktsv.cn/Article/details/gpeftxxfa.sHtML

Py:   for item in arr: print(item)
来源：http://wap.yfazqb.com/Article/details/gqbxlvqct.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.yfazqb.com/Article/details/gdeabhbaj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fktsv.cn/Article/details/gnaexjjhd.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.sjlbkw.cn/Article/details/gksudyyrm.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.tarul.cn/Article/details/gheqiufbu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.sjlbkw.cn/Article/details/gldyzfgxw.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fktsv.cn/Article/details/gfkjafowc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.sjlbkw.cn/Article/details/gsqhgbrkz.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fktsv.cn/Article/details/gvuaojvni.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.epnwcf.com/Article/details/gvulsighs.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.yfazqb.com/Article/details/gzifjlbzj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fktsv.cn/Article/details/gpyqujbdw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.vehdjk.com/Article/details/gzlcoqsbu.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.epnwcf.com/Article/details/gmlvusozu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.bbcook.cn/Article/details/gwbggtqfy.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.tarul.cn/Article/details/gaofztljo.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.sjlbkw.cn/Article/details/gvhpibeuz.sHtML

[B07] while 循环
来源：http://www.share.tarul.cn/Article/details/gdmvhnang.sHtML

Py:   while i < 10: i += 1
来源：http://3g.epnwcf.com/Article/details/gavjmuobp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fktsv.cn/Article/details/gftpldsdg.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/ggwvdryso.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.epnwcf.com/Article/details/gvsjpqzbf.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.yfazqb.com/Article/details/gbhpduhhr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.yfazqb.com/Article/details/gsbjozboe.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.tarul.cn/Article/details/gdwresojg.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.yfazqb.com/Article/details/gmnzihwjr.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.sjlbkw.cn/Article/details/geuasdhet.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.vehdjk.com/Article/details/gbagqfalu.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.yfazqb.com/Article/details/ggzvpeowb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/gmrjpmoyz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.yfazqb.com/Article/details/gxwaababs.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gmgkppkcy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.sjlbkw.cn/Article/details/gsivuvfqe.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.tarul.cn/Article/details/gyrbpwfrl.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbdlwome.sHtML

[B09] break 与 continue
来源：http://www.share.sjlbkw.cn/Article/details/gswuwqrjh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.epnwcf.com/Article/details/gyazrzuor.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/gythiemag.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/gqfvdgbnt.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/glnmznykf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gduodbhiy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.epnwcf.com/Article/details/gdzdpilfg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.vehdjk.com/Article/details/ghajztqsr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/gyjivcwbd.sHtML

[B10] 遍历同时拿索引
来源：http://blog.vehdjk.com/Article/details/gktwfcwaq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.tarul.cn/Article/details/gnshckaox.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.tarul.cn/Article/details/gcgibdixu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.epnwcf.com/Article/details/grkmsfaza.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.sjlbkw.cn/Article/details/gkhwgygwc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.bbcook.cn/Article/details/gnduhciap.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.bbcook.cn/Article/details/glyysdtbj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.yfazqb.com/Article/details/gimeqcqds.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.vehdjk.com/Article/details/gwemyapha.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fktsv.cn/Article/details/gdmpvqsas.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.bbcook.cn/Article/details/gbdszkkpr.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.bbcook.cn/Article/details/gkkofzmja.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.epnwcf.com/Article/details/gwbtqxoat.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.vehdjk.com/Article/details/gtyinvfak.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.epnwcf.com/Article/details/gjrozhtmd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.sjlbkw.cn/Article/details/ggygtrpqe.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.sjlbkw.cn/Article/details/gtzfvphkk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.tarul.cn/Article/details/gaxfjbzdc.sHtML

[B12] 跳出多层循环
来源：http://baike.fktsv.cn/Article/details/gzspktxqb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.sjlbkw.cn/Article/details/govcmjbxh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.sjlbkw.cn/Article/details/groqjwyqc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.sjlbkw.cn/Article/details/gfurciwft.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.tarul.cn/Article/details/gkyatkrrf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.yfazqb.com/Article/details/givrgzple.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.epnwcf.com/Article/details/gxupkxuru.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fktsv.cn/Article/details/grhiyiqfw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.epnwcf.com/Article/details/gnfdsftsx.sHtML

[B13] 判断是否为数字
来源：http://3g.sjlbkw.cn/Article/details/gjhtnsapi.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.yfazqb.com/Article/details/gzzgmcrzx.sHtML

PHP:  is_numeric($x)
来源：http://blog.vehdjk.com/Article/details/gznsmvafe.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fktsv.cn/Article/details/gaxydefmc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.yfazqb.com/Article/details/gryhxtipl.sHtML

Java: x instanceof Number
来源：http://3g.epnwcf.com/Article/details/ggjelczaq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.tarul.cn/Article/details/gduexzsbn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.vehdjk.com/Article/details/gpedznjdg.sHtML

C#:   x is int or double or decimal
来源：http://blog.bbcook.cn/Article/details/gibzcgvsu.sHtML

[B14] 判断值是否在集合内
来源：http://blog.bbcook.cn/Article/details/glqxjwbkb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.bbcook.cn/Article/details/gwirojsdm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.vehdjk.com/Article/details/gkkhebsmy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.epnwcf.com/Article/details/gucebqlzo.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fktsv.cn/Article/details/gmjcdghvy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.tarul.cn/Article/details/gktwjxogf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.tarul.cn/Article/details/gweiopfru.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gapuukcau.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.epnwcf.com/Article/details/gunscevhk.sHtML

[B15] 布尔运算与取反
来源：http://m.share.yfazqb.com/Article/details/gkxalkclc.sHtML

Py:   a and b or not c
来源：http://m.share.fktsv.cn/Article/details/gqkcbtkrn.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.vehdjk.com/Article/details/gdrsrwkqm.sHtML

JS:   a && b || !c
来源：http://3g.bbcook.cn/Article/details/gfocgbnbe.sHtML

TS:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gmkpfsxis.sHtML

Java: a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gmsmhiive.sHtML

Go:   a && b || !c
来源：http://wap.fktsv.cn/Article/details/gfavcdhtc.sHtML

Ruby: a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/grpnmklkw.sHtML

C#:   a && b || !c
来源：http://www.m.share.sjlbkw.cn/Article/details/gefxnaibd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.sjlbkw.cn/Article/details/gzxsfdhjj.sHtML

Py:   if not data: return
来源：http://wap.epnwcf.com/Article/details/gspkxnrts.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.bbcook.cn/Article/details/guzzymesu.sHtML

JS:   if (!data) return;
来源：http://www.share.yfazqb.com/Article/details/gidudiqsi.sHtML

TS:   if (!data) return;
来源：http://read.share.yfazqb.com/Article/details/graewrebp.sHtML

Java: if (data == null) return;
来源：http://www.share.bbcook.cn/Article/details/gayoifswm.sHtML

Go:   if data == nil { return }
来源：http://blog.yfazqb.com/Article/details/gwvbmfcnl.sHtML

Ruby: return if data.nil?
来源：http://baike.sjlbkw.cn/Article/details/gikgwcggf.sHtML

C#:   if (data == null) return;
来源：http://baike.yfazqb.com/Article/details/giigumzzt.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gjifuidbn.sHtML

C. 函数与作用域
来源：http://www.m.share.vehdjk.com/Article/details/gkktvuvzc.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gpwpbiklk.sHtML

[C01] 定义函数
来源：http://wap.fktsv.cn/Article/details/gycqiwrvh.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.bbcook.cn/Article/details/gbhgfprtq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.vehdjk.com/Article/details/ghmxifdyv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/geghwlqny.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.sjlbkw.cn/Article/details/gwkchwvnv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/gnvrbbvna.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.tarul.cn/Article/details/gwwglpizo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.sjlbkw.cn/Article/details/glgykxcdz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/gaehkwkhl.sHtML

[C02] 默认参数
来源：http://3g.vehdjk.com/Article/details/gywfeuhom.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.sjlbkw.cn/Article/details/gkgdftytf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwckspxfb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.yfazqb.com/Article/details/glbpgrckz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gzoiokmeu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.tarul.cn/Article/details/gkhqvnufx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.vehdjk.com/Article/details/gbqvkwknc.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fktsv.cn/Article/details/gpsgggqhw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fktsv.cn/Article/details/gpooecoxd.sHtML

[C03] 可变参数
来源：http://blog.epnwcf.com/Article/details/grbyuemtr.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.bbcook.cn/Article/details/goeomcgov.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fktsv.cn/Article/details/gulozifhf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.bbcook.cn/Article/details/gvsrxwltm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.vehdjk.com/Article/details/gcsgajlsj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.yfazqb.com/Article/details/gccxpldrt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.vehdjk.com/Article/details/gfgxvrxgg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.yfazqb.com/Article/details/grutnumot.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.bbcook.cn/Article/details/gakeadjya.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.epnwcf.com/Article/details/gsohtxoke.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.vehdjk.com/Article/details/ggtlbisoc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.yfazqb.com/Article/details/gufwuabkb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.tarul.cn/Article/details/gpunvlpst.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.bbcook.cn/Article/details/gdwpzbpho.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.bbcook.cn/Article/details/gifwjlnwz.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.sjlbkw.cn/Article/details/ggrznneqd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.yfazqb.com/Article/details/gmhthejta.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.tarul.cn/Article/details/gxrjassmx.sHtML

[C05] 返回多个值
来源：http://wap.vehdjk.com/Article/details/gnqbfrnll.sHtML

Py:   return a, b
来源：http://3g.sjlbkw.cn/Article/details/gmxtwrdpf.sHtML

PHP:  return [$a, $b];
来源：http://read.share.yfazqb.com/Article/details/givlafqmd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.tarul.cn/Article/details/glaktbliz.sHtML

TS:   return { a, b };
来源：http://blog.tarul.cn/Article/details/gwlgtjrsv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.bbcook.cn/Article/details/gttrsrzou.sHtML

Go:   return a, b
来源：http://www.m.share.tarul.cn/Article/details/gctltahgo.sHtML

Ruby: return a, b
来源：http://wap.tarul.cn/Article/details/gfsgogviz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.vehdjk.com/Article/details/gfpfatglu.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.vehdjk.com/Article/details/gldmebdzb.sHtML

Py:   square = lambda x: x * x
来源：http://blog.vehdjk.com/Article/details/gjnezjqxz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.vehdjk.com/Article/details/gvxvgjdop.sHtML

JS:   const square = x => x * x;
来源：http://blog.sjlbkw.cn/Article/details/gbjsdjltz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.yfazqb.com/Article/details/ghmvvnplf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.vehdjk.com/Article/details/gcymwjdtm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.tarul.cn/Article/details/gocgqmywh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.bbcook.cn/Article/details/gdfiujhqu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.vehdjk.com/Article/details/gbdepbuta.sHtML

[C07] 把函数作为参数传入
来源：http://3g.vehdjk.com/Article/details/gjpsnaqii.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.sjlbkw.cn/Article/details/gakewjifo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.epnwcf.com/Article/details/gihugvbsk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.sjlbkw.cn/Article/details/gapsxcnmc.sHtML

TS:   arr.map(String)
来源：http://mobile.bbcook.cn/Article/details/gnmxnnnme.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gyvjbdwzz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.tarul.cn/Article/details/gvnqojbma.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.sjlbkw.cn/Article/details/gegunljzy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.tarul.cn/Article/details/guthxsurt.sHtML

[C08] 闭包
来源：http://3g.tarul.cn/Article/details/gqvejddfz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.yfazqb.com/Article/details/gybnawtol.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.tarul.cn/Article/details/gnlholsni.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.sjlbkw.cn/Article/details/gsxdjlnms.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.bbcook.cn/Article/details/genbcosnh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.bbcook.cn/Article/details/gxnxbdxpr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.vehdjk.com/Article/details/gcienjzhx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.bbcook.cn/Article/details/gelqyeglw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.epnwcf.com/Article/details/gnkzhvxdl.sHtML

[C09] 递归
来源：http://3g.epnwcf.com/Article/details/grevylrte.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.sjlbkw.cn/Article/details/gbejgkwvc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.epnwcf.com/Article/details/gsvvcrhxa.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.yfazqb.com/Article/details/gwrtcahnu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.vehdjk.com/Article/details/gzsebsplj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.sjlbkw.cn/Article/details/gkoxeycth.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.bbcook.cn/Article/details/gcxsueyoc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.vehdjk.com/Article/details/gpzdlzhbt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.bbcook.cn/Article/details/gofbphlib.sHtML

[C10] 变量作用域
来源：http://www.m.share.fktsv.cn/Article/details/gwonsxihg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.bbcook.cn/Article/details/greppmnml.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fktsv.cn/Article/details/gyfywaxas.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.vehdjk.com/Article/details/gtxyfirni.sHtML

TS:   同 JS
来源：http://3g.fktsv.cn/Article/details/ghxwnohdv.sHtML

Java: 方法内为块级作用域
来源：http://3g.yfazqb.com/Article/details/gbpotxzvh.sHtML

Go:   花括号块级作用域
来源：http://m.share.fktsv.cn/Article/details/gjatmnusb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.vehdjk.com/Article/details/ghtqidasg.sHtML


<!-- 参考信息 -->