代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.epnwcf.com/Article/details/gxtahyzmt.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.bbcook.cn/Article/details/gnzpwmibo.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.tarul.cn/Article/details/gvcrtgzxs.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.sjlbkw.cn/Article/details/ghogcufsr.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fktsv.cn/Article/details/glfmydyyg.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.fktsv.cn/Article/details/geprlvofk.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.epnwcf.com/Article/details/gzuttxbhd.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.yfazqb.com/Article/details/gnkxxpsbr.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.bbcook.cn/Article/details/gkaaeobkr.sHtML

[A19] 交换两个变量
来源：http://www.share.sjlbkw.cn/Article/details/geqktqvkj.sHtML

Py:   a, b = b, a
来源：http://www.m.share.tarul.cn/Article/details/gmytzdhil.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.fktsv.cn/Article/details/gfhdhbwsw.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.tarul.cn/Article/details/gwkvlbegv.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.fktsv.cn/Article/details/gzwioahvw.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.tarul.cn/Article/details/grabbzold.sHtML

Go:   a, b = b, a
来源：http://m.share.yfazqb.com/Article/details/gdiukjwva.sHtML

Ruby: a, b = b, a
来源：http://mobile.vehdjk.com/Article/details/gfysqymaz.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.sjlbkw.cn/Article/details/gxmwrjict.sHtML

[A20] 读取标准输入
来源：http://baike.sjlbkw.cn/Article/details/goeswsces.sHtML

Py:   name = input("请输入：")
来源：http://mobile.tarul.cn/Article/details/gptivqdyt.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.fktsv.cn/Article/details/gwixmakks.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.sjlbkw.cn/Article/details/gsdhpqlvy.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.epnwcf.com/Article/details/gcmlsdprj.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.bbcook.cn/Article/details/gduzyidat.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.yfazqb.com/Article/details/gyhogrnbh.sHtML

Ruby: gets.chomp
来源：http://www.blog.epnwcf.com/Article/details/glbgrndre.sHtML

C#:   Console.ReadLine();
来源：http://read.share.fktsv.cn/Article/details/gqcekcsae.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.fktsv.cn/Article/details/gilxxyyjo.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.epnwcf.com/Article/details/gmykbgnko.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.fktsv.cn/Article/details/ghxvagoqe.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.bbcook.cn/Article/details/gqilpwdzt.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.bbcook.cn/Article/details/gtvzylmnd.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.vehdjk.com/Article/details/gmcjwzmfm.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.fktsv.cn/Article/details/grbrpdqwj.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.vehdjk.com/Article/details/gjspryeau.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.sjlbkw.cn/Article/details/gilaqrpmu.sHtML

[A22] 获取字符串长度
来源：http://wap.vehdjk.com/Article/details/gmbqnxbzo.sHtML

Py:   len(s)
来源：http://baike.yfazqb.com/Article/details/gbqpvoeih.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.epnwcf.com/Article/details/gkxunjdtr.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.epnwcf.com/Article/details/gdtbpybvu.sHtML

TS:   s.length
来源：http://mobile.bbcook.cn/Article/details/gblbrvkac.sHtML

Java: s.length()
来源：http://wap.tarul.cn/Article/details/groptsrpb.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.epnwcf.com/Article/details/gwgbziuev.sHtML

Ruby: s.length
来源：http://baike.yfazqb.com/Article/details/gozpglsah.sHtML

C#:   s.Length
来源：http://read.share.fktsv.cn/Article/details/gcmvcnnmf.sHtML

[A23] 大小写转换
来源：http://baike.epnwcf.com/Article/details/gcdatxxej.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.fktsv.cn/Article/details/guuycmgsr.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.tarul.cn/Article/details/gtuyzbhhw.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.bbcook.cn/Article/details/gcyctasvj.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.epnwcf.com/Article/details/gxnrimbmh.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.bbcook.cn/Article/details/guwxlssew.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.bbcook.cn/Article/details/gxuyljlku.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.sjlbkw.cn/Article/details/ggvhkcwvz.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.bbcook.cn/Article/details/greeujnlc.sHtML

[A24] 去除首尾空白
来源：http://read.share.fktsv.cn/Article/details/ghegdfkum.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.tarul.cn/Article/details/gitxeeyix.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.vehdjk.com/Article/details/gewxhglme.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.vehdjk.com/Article/details/gxlahxdxo.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fktsv.cn/Article/details/gyjddgvnu.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.fktsv.cn/Article/details/gxnafcppx.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.yfazqb.com/Article/details/gjvlvbqfk.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.sjlbkw.cn/Article/details/gcldvroqi.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.vehdjk.com/Article/details/gdcwsicmd.sHtML

[A25] 字符串比较
来源：http://blog.vehdjk.com/Article/details/gshhvbjst.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.tarul.cn/Article/details/gzfakgxsu.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.vehdjk.com/Article/details/gvcokneva.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fktsv.cn/Article/details/geqktnqze.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.epnwcf.com/Article/details/geqgacvik.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.vehdjk.com/Article/details/gixhfeaii.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.fktsv.cn/Article/details/gdxtgyhcl.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.fktsv.cn/Article/details/gfhvyuhca.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmkjzgvi.sHtML

[A26] 类型转换总览
来源：http://m.share.yfazqb.com/Article/details/gepvojzrg.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.tarul.cn/Article/details/guensyivt.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.tarul.cn/Article/details/gaycfdjso.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.sjlbkw.cn/Article/details/gueundbtx.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.vehdjk.com/Article/details/gjbtczqrd.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.vehdjk.com/Article/details/gjmgydbgw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.fktsv.cn/Article/details/gtthyhmtz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.epnwcf.com/Article/details/gjwooqhmy.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.fktsv.cn/Article/details/gmcthrxne.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gmlqylmxt.sHtML

B. 流程控制
来源：http://baike.yfazqb.com/Article/details/gkhrbwnpf.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gsexbwlrc.sHtML

[B01] 条件判断 if / else
来源：http://mobile.bbcook.cn/Article/details/gadlqljyw.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.sjlbkw.cn/Article/details/gopqzjami.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.vehdjk.com/Article/details/gqqtezmqc.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/gvdopvsle.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.epnwcf.com/Article/details/gymgbkzhc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.epnwcf.com/Article/details/gibjygvnc.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.epnwcf.com/Article/details/gtzsuxarw.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.vehdjk.com/Article/details/gjzkaqvrt.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.vehdjk.com/Article/details/glqgakeeq.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.sjlbkw.cn/Article/details/gdersvgst.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.vehdjk.com/Article/details/ginfztisr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.sjlbkw.cn/Article/details/gswipwyfl.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.epnwcf.com/Article/details/gidrjxowt.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.epnwcf.com/Article/details/gxisjnjuz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.sjlbkw.cn/Article/details/gnmttqzkb.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.vehdjk.com/Article/details/gcwkmukry.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.vehdjk.com/Article/details/gjyoiwxnc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.tarul.cn/Article/details/gqqyxylcc.sHtML

[B03] switch / match / case
来源：http://www.m.share.fktsv.cn/Article/details/gfrvklhzl.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.bbcook.cn/Article/details/gygnehibu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.fktsv.cn/Article/details/ggfuvkklv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fktsv.cn/Article/details/gcoajxdgs.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.tarul.cn/Article/details/gcuzdgbvu.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.epnwcf.com/Article/details/gdgzuxlwx.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.sjlbkw.cn/Article/details/gjxdpgdpq.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.yfazqb.com/Article/details/gygafkjmg.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.epnwcf.com/Article/details/gpvvpquaw.sHtML

[B04] for 计数循环
来源：http://m.share.vehdjk.com/Article/details/ggzvscvee.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.fktsv.cn/Article/details/gwbdmcfpe.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.bbcook.cn/Article/details/gihjslihg.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.sjlbkw.cn/Article/details/gwulttfky.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fktsv.cn/Article/details/gohdbvghx.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.epnwcf.com/Article/details/gkajhvqmf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.fktsv.cn/Article/details/giqcivldd.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.sjlbkw.cn/Article/details/gxhdmgmbf.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.sjlbkw.cn/Article/details/grnvnriuy.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.bbcook.cn/Article/details/gxhjcybte.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.yfazqb.com/Article/details/gyjafvqpq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.bbcook.cn/Article/details/gtevujevy.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.sjlbkw.cn/Article/details/grrzvhrhu.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.yfazqb.com/Article/details/gsbilsany.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.bbcook.cn/Article/details/grdbqzjdt.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.bbcook.cn/Article/details/gzfithjwe.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.tarul.cn/Article/details/gqrsiatfc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.vehdjk.com/Article/details/gjubslbom.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.epnwcf.com/Article/details/givdozvtj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.vehdjk.com/Article/details/gwzpcjgbe.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.tarul.cn/Article/details/guoirvzuy.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fktsv.cn/Article/details/ggslajmgj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.epnwcf.com/Article/details/gcgknhrei.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fktsv.cn/Article/details/gjpstcdpj.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.sjlbkw.cn/Article/details/gygejojsx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.fktsv.cn/Article/details/gmdgopvac.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.epnwcf.com/Article/details/gixydlybi.sHtML

[B07] while 循环
来源：http://3g.bbcook.cn/Article/details/gfgmxhrmq.sHtML

Py:   while i < 10: i += 1
来源：http://blog.tarul.cn/Article/details/gbrftwxzt.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fktsv.cn/Article/details/ghxesfqvw.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.yfazqb.com/Article/details/gmkkrvcab.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fktsv.cn/Article/details/ggsdvjsvu.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.fktsv.cn/Article/details/gwqanuflk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.yfazqb.com/Article/details/gyvxwsokh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fktsv.cn/Article/details/glfgiwelf.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.tarul.cn/Article/details/gybcnarwj.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.yfazqb.com/Article/details/gynreecrg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.sjlbkw.cn/Article/details/gfnqhrkqd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.sjlbkw.cn/Article/details/goqvzrbtv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/gebaiqmef.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.vehdjk.com/Article/details/gnzucfvsf.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.vehdjk.com/Article/details/gwfpkcjvp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.yfazqb.com/Article/details/gmgrxaklh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.sjlbkw.cn/Article/details/ghaehhyan.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fktsv.cn/Article/details/godkibyks.sHtML

[B09] break 与 continue
来源：http://m.share.fktsv.cn/Article/details/gytlixekt.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.vehdjk.com/Article/details/glhagkxum.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfnugessh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fktsv.cn/Article/details/gguuwowxq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.sjlbkw.cn/Article/details/glfvalthy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gvjacrbaj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.epnwcf.com/Article/details/gitsglqvs.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.epnwcf.com/Article/details/gilxoitgu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/gbuzwmvvx.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.vehdjk.com/Article/details/guybpgwvx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.sjlbkw.cn/Article/details/gnpnpcusl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fktsv.cn/Article/details/giicyhncs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.sjlbkw.cn/Article/details/gdmtpxupq.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.yfazqb.com/Article/details/gljknuvpx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.tarul.cn/Article/details/gstszrhgu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.tarul.cn/Article/details/gghwerxkd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.yfazqb.com/Article/details/gybciatxp.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.vehdjk.com/Article/details/gvbwpyrgd.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.sjlbkw.cn/Article/details/geqsyettd.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.yfazqb.com/Article/details/grawpdksy.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.bbcook.cn/Article/details/gpeigulva.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.tarul.cn/Article/details/gbyhpfjso.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.vehdjk.com/Article/details/gwztowmrv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.epnwcf.com/Article/details/ggbwqhmuf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.epnwcf.com/Article/details/ghaflwhjd.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.vehdjk.com/Article/details/glddmwuim.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.vehdjk.com/Article/details/gqaaessca.sHtML

[B12] 跳出多层循环
来源：http://mobile.epnwcf.com/Article/details/ghqrlplue.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fktsv.cn/Article/details/ghqfdkxxz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.sjlbkw.cn/Article/details/gvjjmwamx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.tarul.cn/Article/details/gzferhbhp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fktsv.cn/Article/details/glsbavdnz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.sjlbkw.cn/Article/details/gdxmrtmog.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fktsv.cn/Article/details/gtjbpbmxh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.sjlbkw.cn/Article/details/glcgbpgfe.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.bbcook.cn/Article/details/gseapblhp.sHtML

[B13] 判断是否为数字
来源：http://mobile.vehdjk.com/Article/details/gdibjcnbn.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fktsv.cn/Article/details/ghicyrbok.sHtML

PHP:  is_numeric($x)
来源：http://blog.bbcook.cn/Article/details/gsulofrlm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.tarul.cn/Article/details/ggkydozqk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.yfazqb.com/Article/details/gwkcanvcl.sHtML

Java: x instanceof Number
来源：http://www.share.tarul.cn/Article/details/gnpmsydbn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.sjlbkw.cn/Article/details/gektvlrpc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.sjlbkw.cn/Article/details/gqbgtzoew.sHtML

C#:   x is int or double or decimal
来源：http://blog.vehdjk.com/Article/details/gsjvydgfd.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.sjlbkw.cn/Article/details/gvxgpmlvn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.vehdjk.com/Article/details/gjawmmzwl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.bbcook.cn/Article/details/getzucbns.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.tarul.cn/Article/details/gzzphciou.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.bbcook.cn/Article/details/gqodugiqc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fktsv.cn/Article/details/ggwpsbpok.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.tarul.cn/Article/details/gecafjokv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.vehdjk.com/Article/details/gatjbowve.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.epnwcf.com/Article/details/gvgeoicul.sHtML

[B15] 布尔运算与取反
来源：http://baike.tarul.cn/Article/details/guttomqha.sHtML

Py:   a and b or not c
来源：http://baike.bbcook.cn/Article/details/gntymxluf.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.yfazqb.com/Article/details/glamifyhu.sHtML

JS:   a && b || !c
来源：http://m.share.yfazqb.com/Article/details/gdtjjrqbf.sHtML

TS:   a && b || !c
来源：http://baike.yfazqb.com/Article/details/gmlgbtmfx.sHtML

Java: a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gqkghwuvc.sHtML

Go:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gehtqbujn.sHtML

Ruby: a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gyobegvby.sHtML

C#:   a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/geovttlfl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fktsv.cn/Article/details/gjyfqfomm.sHtML

Py:   if not data: return
来源：http://www.share.tarul.cn/Article/details/guyihjfxx.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fktsv.cn/Article/details/gpfvvlphr.sHtML

JS:   if (!data) return;
来源：http://read.share.vehdjk.com/Article/details/gtpnmkqde.sHtML

TS:   if (!data) return;
来源：http://blog.tarul.cn/Article/details/grfenhqqn.sHtML

Java: if (data == null) return;
来源：http://read.share.epnwcf.com/Article/details/gxisrhqfs.sHtML

Go:   if data == nil { return }
来源：http://wap.tarul.cn/Article/details/gwpvdmpxv.sHtML

Ruby: return if data.nil?
来源：http://baike.tarul.cn/Article/details/gdacleako.sHtML

C#:   if (data == null) return;
来源：http://www.share.vehdjk.com/Article/details/gkqhycxpw.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gebeywbaw.sHtML

C. 函数与作用域
来源：http://3g.vehdjk.com/Article/details/gnrpnrawd.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gjalhtnwd.sHtML

[C01] 定义函数
来源：http://read.share.epnwcf.com/Article/details/gygnlcdak.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fktsv.cn/Article/details/giuqkxzug.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/gbghtmeiz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.vehdjk.com/Article/details/gidowaqac.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gvimnabqq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.yfazqb.com/Article/details/gfoawshua.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.yfazqb.com/Article/details/gwdxvvvsi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.sjlbkw.cn/Article/details/giqoasmtt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.yfazqb.com/Article/details/gesqeltac.sHtML

[C02] 默认参数
来源：http://www.blog.yfazqb.com/Article/details/ghtdltkzl.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fktsv.cn/Article/details/gyhwslkqw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.yfazqb.com/Article/details/gfdrzdeki.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.vehdjk.com/Article/details/gdljpyrcw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gdlhxiczi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.yfazqb.com/Article/details/gyvrwjqlb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fktsv.cn/Article/details/gbbyurubt.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.epnwcf.com/Article/details/gdqpoahju.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fktsv.cn/Article/details/gvwmzlhld.sHtML

[C03] 可变参数
来源：http://www.blog.bbcook.cn/Article/details/gzbaovumq.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.tarul.cn/Article/details/gtlsxyejq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.vehdjk.com/Article/details/gqhlzkboz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.vehdjk.com/Article/details/gqxokpyet.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.yfazqb.com/Article/details/gpiyiehik.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.sjlbkw.cn/Article/details/gomdqhntn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.yfazqb.com/Article/details/gqwqcjalv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.tarul.cn/Article/details/gxsrfjcps.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.bbcook.cn/Article/details/gquasdzui.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.bbcook.cn/Article/details/ghvhrbpjl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fktsv.cn/Article/details/gimckjfgn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.vehdjk.com/Article/details/gjyilglsi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.vehdjk.com/Article/details/geojrgwgc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.epnwcf.com/Article/details/grncomdvd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.tarul.cn/Article/details/gdvbwiwfn.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.sjlbkw.cn/Article/details/gevunrmwf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.bbcook.cn/Article/details/gmlpvjygi.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.tarul.cn/Article/details/geovqnhyc.sHtML

[C05] 返回多个值
来源：http://3g.yfazqb.com/Article/details/gpjlyappp.sHtML

Py:   return a, b
来源：http://wap.bbcook.cn/Article/details/gchtmgmbu.sHtML

PHP:  return [$a, $b];
来源：http://blog.tarul.cn/Article/details/grrutittv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.epnwcf.com/Article/details/gqodsrfsr.sHtML

TS:   return { a, b };
来源：http://www.share.fktsv.cn/Article/details/gtmmqosnx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.tarul.cn/Article/details/gokarvpmq.sHtML

Go:   return a, b
来源：http://baike.sjlbkw.cn/Article/details/givymzpss.sHtML

Ruby: return a, b
来源：http://wap.epnwcf.com/Article/details/gwjgqachk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.sjlbkw.cn/Article/details/ghwmkjwyp.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fktsv.cn/Article/details/guualmval.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.vehdjk.com/Article/details/gfcerojzy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.vehdjk.com/Article/details/gkobabpvu.sHtML

JS:   const square = x => x * x;
来源：http://wap.fktsv.cn/Article/details/gucyxxoqv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.epnwcf.com/Article/details/gphyzfkge.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fktsv.cn/Article/details/gqqihrupp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.sjlbkw.cn/Article/details/gjftkfpoa.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.tarul.cn/Article/details/gwxluqlhx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.bbcook.cn/Article/details/gcoylwzoa.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fktsv.cn/Article/details/gzhnyxjhz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fktsv.cn/Article/details/gjoibdcho.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.epnwcf.com/Article/details/gpwsycnve.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.vehdjk.com/Article/details/glimtkazb.sHtML

TS:   arr.map(String)
来源：http://www.share.sjlbkw.cn/Article/details/gcjskwczz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.tarul.cn/Article/details/gyexsimpc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.vehdjk.com/Article/details/gvtzuxcqg.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.epnwcf.com/Article/details/gdlellgsl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.tarul.cn/Article/details/glpsxscdw.sHtML

[C08] 闭包
来源：http://read.share.epnwcf.com/Article/details/gifiwumpp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.epnwcf.com/Article/details/gngandcmu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.sjlbkw.cn/Article/details/gwfvjusqz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.vehdjk.com/Article/details/gglnmotcg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.epnwcf.com/Article/details/gaaqtnqqz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.yfazqb.com/Article/details/gydsqllxa.sHtML


<!-- 参考信息 -->