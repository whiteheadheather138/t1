代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fktsv.cn/Article/details/ghimvklkv.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.fktsv.cn/Article/details/gtjzaposq.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.epnwcf.com/Article/details/gpdaikoqr.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.tarul.cn/Article/details/gghfhosrk.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.epnwcf.com/Article/details/grxmlfbin.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.fktsv.cn/Article/details/grilmlido.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.vehdjk.com/Article/details/gcuwojrba.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.yfazqb.com/Article/details/ghppizaov.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.tarul.cn/Article/details/gupkmoumy.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.bbcook.cn/Article/details/ghnpkigek.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.sjlbkw.cn/Article/details/gbdhyskhl.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.tarul.cn/Article/details/gepxbxqwe.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.vehdjk.com/Article/details/gvtquamab.sHtML

[A19] 交换两个变量
来源：http://www.blog.yfazqb.com/Article/details/gdqrkicih.sHtML

Py:   a, b = b, a
来源：http://m.share.yfazqb.com/Article/details/gheqbjnqk.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.tarul.cn/Article/details/grkvfucal.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.tarul.cn/Article/details/gbwralyey.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.yfazqb.com/Article/details/gekwfspbc.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.tarul.cn/Article/details/gulfzvszw.sHtML

Go:   a, b = b, a
来源：http://baike.epnwcf.com/Article/details/gdponcvry.sHtML

Ruby: a, b = b, a
来源：http://baike.fktsv.cn/Article/details/gzvqydoqw.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.yfazqb.com/Article/details/gnvcefihn.sHtML

[A20] 读取标准输入
来源：http://wap.sjlbkw.cn/Article/details/gdohjclmv.sHtML

Py:   name = input("请输入：")
来源：http://blog.yfazqb.com/Article/details/gwgwkwwal.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.fktsv.cn/Article/details/gebgnocme.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.vehdjk.com/Article/details/glzgqcgwo.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.fktsv.cn/Article/details/gsyoxzadf.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.bbcook.cn/Article/details/garfggqzu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.yfazqb.com/Article/details/gjjvekwwy.sHtML

Ruby: gets.chomp
来源：http://mobile.sjlbkw.cn/Article/details/ghzosczop.sHtML

C#:   Console.ReadLine();
来源：http://baike.fktsv.cn/Article/details/gklwlmymg.sHtML

[A21] 保留指定小数位输出
来源：http://wap.epnwcf.com/Article/details/gihwoyxsa.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.sjlbkw.cn/Article/details/gdeynyfqt.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.epnwcf.com/Article/details/gwiexalsd.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.epnwcf.com/Article/details/gxnuoggtf.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.vehdjk.com/Article/details/gptdkrfjw.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.epnwcf.com/Article/details/gbtjxdnuf.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.vehdjk.com/Article/details/gmndshsfj.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.tarul.cn/Article/details/gffszsqyf.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.epnwcf.com/Article/details/ggfyrbljr.sHtML

[A22] 获取字符串长度
来源：http://www.blog.yfazqb.com/Article/details/gwskguucw.sHtML

Py:   len(s)
来源：http://read.share.yfazqb.com/Article/details/gvkyfzjlu.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.bbcook.cn/Article/details/gmuvssxib.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.fktsv.cn/Article/details/gyjagzwvb.sHtML

TS:   s.length
来源：http://www.share.yfazqb.com/Article/details/gtmcwlpwg.sHtML

Java: s.length()
来源：http://www.blog.tarul.cn/Article/details/gdkabnkdi.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.epnwcf.com/Article/details/ghcfvkqfl.sHtML

Ruby: s.length
来源：http://www.blog.epnwcf.com/Article/details/gnmatzflc.sHtML

C#:   s.Length
来源：http://3g.vehdjk.com/Article/details/gnxbxcdcu.sHtML

[A23] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/gsjefuyvp.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.bbcook.cn/Article/details/gizrseeln.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.yfazqb.com/Article/details/gttbklqhu.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.epnwcf.com/Article/details/gwgtjgqar.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.yfazqb.com/Article/details/gducgxjje.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.tarul.cn/Article/details/gxkdotwpf.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.tarul.cn/Article/details/gdqowlsmc.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.yfazqb.com/Article/details/gwandpuhm.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.fktsv.cn/Article/details/gvpujjkpd.sHtML

[A24] 去除首尾空白
来源：http://baike.sjlbkw.cn/Article/details/gbazqevvl.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.epnwcf.com/Article/details/gplclxmcg.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.epnwcf.com/Article/details/gefcwxmos.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.tarul.cn/Article/details/gwszvvtod.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.sjlbkw.cn/Article/details/gwaqudlcx.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.sjlbkw.cn/Article/details/gpcfhlorh.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.yfazqb.com/Article/details/gjplwfogs.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.vehdjk.com/Article/details/gtdxzftfu.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.vehdjk.com/Article/details/ggouhtsoo.sHtML

[A25] 字符串比较
来源：http://m.share.vehdjk.com/Article/details/gkhzxrlhw.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.fktsv.cn/Article/details/ghmsfekpj.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.epnwcf.com/Article/details/gbaqpfufv.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.bbcook.cn/Article/details/gpvvvuora.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.sjlbkw.cn/Article/details/gxvqzcnnk.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.yfazqb.com/Article/details/gtmmmzrqm.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.tarul.cn/Article/details/gumfrpsck.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.bbcook.cn/Article/details/gepijwzfg.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.bbcook.cn/Article/details/grsdeawhl.sHtML

[A26] 类型转换总览
来源：http://baike.fktsv.cn/Article/details/gbrhwnxxt.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.sjlbkw.cn/Article/details/gtilppbhp.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.epnwcf.com/Article/details/gcfbzguep.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.sjlbkw.cn/Article/details/gfsbdlnrl.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.bbcook.cn/Article/details/gznljuunr.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.epnwcf.com/Article/details/gebcijgrn.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.yfazqb.com/Article/details/gnfwgnhoq.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.yfazqb.com/Article/details/godgsdgdo.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.vehdjk.com/Article/details/gxrotafdk.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/ggfyszwfo.sHtML

B. 流程控制
来源：http://baike.bbcook.cn/Article/details/gtgcorbbe.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gfvhomvat.sHtML

[B01] 条件判断 if / else
来源：http://www.share.sjlbkw.cn/Article/details/gzfcbhuld.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.tarul.cn/Article/details/gwrixbdnm.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.yfazqb.com/Article/details/gpstreuzt.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.epnwcf.com/Article/details/gysaouznf.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.tarul.cn/Article/details/gppsxrcgc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.sjlbkw.cn/Article/details/gpwautikz.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.vehdjk.com/Article/details/geutqueyj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.bbcook.cn/Article/details/gwvcvqnic.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.tarul.cn/Article/details/gnctiasbo.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.vehdjk.com/Article/details/geibhmgwm.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.epnwcf.com/Article/details/gqhnvtxor.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.vehdjk.com/Article/details/gfddopuwx.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.bbcook.cn/Article/details/gsheddtjr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.bbcook.cn/Article/details/gawkthenq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.yfazqb.com/Article/details/gfktrmbdl.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.sjlbkw.cn/Article/details/ggyvyloav.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.bbcook.cn/Article/details/gjsmfevcu.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.tarul.cn/Article/details/gqavbiqcm.sHtML

[B03] switch / match / case
来源：http://www.m.share.bbcook.cn/Article/details/gmfhbqspe.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.tarul.cn/Article/details/girmkdlzz.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.yfazqb.com/Article/details/gfhmyidek.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.bbcook.cn/Article/details/gnlxnzity.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.tarul.cn/Article/details/gjyvlklpm.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/gjyvrxsmn.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.tarul.cn/Article/details/gaqjspdcz.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.epnwcf.com/Article/details/gvztwtmsu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.bbcook.cn/Article/details/gomasgixe.sHtML

[B04] for 计数循环
来源：http://blog.tarul.cn/Article/details/grfbkhgoy.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.vehdjk.com/Article/details/ghizfbmgl.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.epnwcf.com/Article/details/gakfjvpba.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.vehdjk.com/Article/details/gioukolia.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.epnwcf.com/Article/details/gtasuesma.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.vehdjk.com/Article/details/gwauinlup.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.bbcook.cn/Article/details/gyyydgpxi.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.yfazqb.com/Article/details/ghnrlvprq.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.vehdjk.com/Article/details/gtrwavpxi.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.sjlbkw.cn/Article/details/gvipxellj.sHtML

Py:   for item in arr: print(item)
来源：http://3g.tarul.cn/Article/details/gujzsjcmm.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.tarul.cn/Article/details/gojyknthy.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fktsv.cn/Article/details/ghtrlreuh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.sjlbkw.cn/Article/details/ggtwlprxs.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.yfazqb.com/Article/details/gpiyarjwu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.epnwcf.com/Article/details/gnskixwek.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.bbcook.cn/Article/details/glftfvujq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.vehdjk.com/Article/details/guwxxhryo.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.bbcook.cn/Article/details/ganweobas.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.sjlbkw.cn/Article/details/grvkziodp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.sjlbkw.cn/Article/details/gyqivbqja.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.tarul.cn/Article/details/giiklevzg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.tarul.cn/Article/details/gkogssrdo.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.vehdjk.com/Article/details/gtjjrllke.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.tarul.cn/Article/details/gymtcfrpf.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.vehdjk.com/Article/details/gnudqkjid.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.yfazqb.com/Article/details/gyquqqqci.sHtML

[B07] while 循环
来源：http://blog.fktsv.cn/Article/details/gnjvnvcgx.sHtML

Py:   while i < 10: i += 1
来源：http://3g.epnwcf.com/Article/details/gltbadidn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.tarul.cn/Article/details/gjvrwqgli.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.epnwcf.com/Article/details/gbnukjarq.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/grmfhsbcn.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.bbcook.cn/Article/details/gsbhfogph.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.yfazqb.com/Article/details/gxxqjscts.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.vehdjk.com/Article/details/gfzkdsanj.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/gjoekcxfh.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.sjlbkw.cn/Article/details/gapmoszcl.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.sjlbkw.cn/Article/details/gjdkpjdnl.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.vehdjk.com/Article/details/gvhfcofaf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/ganypghha.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.bbcook.cn/Article/details/gwfkpbbhs.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.tarul.cn/Article/details/gbceykzwk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.epnwcf.com/Article/details/gkpiivjpt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fktsv.cn/Article/details/gdcwmixuc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/gosazgaoc.sHtML

[B09] break 与 continue
来源：http://wap.yfazqb.com/Article/details/gjnwgbdbw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.epnwcf.com/Article/details/gocigecnl.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/glppliamy.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/gwmuwvkky.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gzcmwwntl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/grhyeuygu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.tarul.cn/Article/details/gkngkbrig.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.yfazqb.com/Article/details/gkmmmabro.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/gaqryjnpw.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.bbcook.cn/Article/details/guwqnhaeq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.epnwcf.com/Article/details/gjercbxow.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.vehdjk.com/Article/details/gaycnyzjw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fktsv.cn/Article/details/gkshcvpja.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.yfazqb.com/Article/details/gzmkeccsf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fktsv.cn/Article/details/gmsiplwcu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.sjlbkw.cn/Article/details/gtvtylbgz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.yfazqb.com/Article/details/gigfqomma.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.epnwcf.com/Article/details/guphslsby.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fktsv.cn/Article/details/gdxsrnvfx.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.vehdjk.com/Article/details/gtaoewzat.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.sjlbkw.cn/Article/details/gcztevgvj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fktsv.cn/Article/details/glbehzcqe.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.sjlbkw.cn/Article/details/gtcljcpng.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gytxrcqao.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.epnwcf.com/Article/details/gzfyxhwmw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.yfazqb.com/Article/details/gdqsplqdh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.sjlbkw.cn/Article/details/gotmlejbg.sHtML

[B12] 跳出多层循环
来源：http://m.share.yfazqb.com/Article/details/gezachpkp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.tarul.cn/Article/details/gvdasryrx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.tarul.cn/Article/details/gcootcdyp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/gbtnszbsl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.yfazqb.com/Article/details/gnswecknv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/gqkygxcrz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fktsv.cn/Article/details/gtmxpypnf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.tarul.cn/Article/details/gxpllwxqa.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.sjlbkw.cn/Article/details/gaofmlqdy.sHtML

[B13] 判断是否为数字
来源：http://www.blog.vehdjk.com/Article/details/gnbekvusv.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.sjlbkw.cn/Article/details/gwdhedvna.sHtML

PHP:  is_numeric($x)
来源：http://wap.tarul.cn/Article/details/gczpcrpan.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.tarul.cn/Article/details/ggmfrlgwu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.yfazqb.com/Article/details/gcdyxobvd.sHtML

Java: x instanceof Number
来源：http://wap.vehdjk.com/Article/details/gtkjduhkp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.bbcook.cn/Article/details/gujttxoxk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.epnwcf.com/Article/details/gqucwtlwu.sHtML

C#:   x is int or double or decimal
来源：http://read.share.yfazqb.com/Article/details/gczrobzpu.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.bbcook.cn/Article/details/gsywvvrnm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fktsv.cn/Article/details/gljpbzfhc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.yfazqb.com/Article/details/gvpmdcrdy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/goyfsgcdz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.sjlbkw.cn/Article/details/gkulwofma.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.tarul.cn/Article/details/gtlythydk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.epnwcf.com/Article/details/gddwfnpkz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fktsv.cn/Article/details/gcmrhwqqu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.yfazqb.com/Article/details/gjjiyegjt.sHtML

[B15] 布尔运算与取反
来源：http://read.share.epnwcf.com/Article/details/gyuowrrrn.sHtML

Py:   a and b or not c
来源：http://www.blog.bbcook.cn/Article/details/ghdwrbjkr.sHtML

PHP:  $a && $b || !$c
来源：http://wap.bbcook.cn/Article/details/gudebpaxc.sHtML

JS:   a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/gkjjezlnm.sHtML

TS:   a && b || !c
来源：http://www.m.share.epnwcf.com/Article/details/gxpzxvgas.sHtML

Java: a && b || !c
来源：http://read.share.vehdjk.com/Article/details/ghtohctxh.sHtML

Go:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/gutvseway.sHtML

Ruby: a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gagbcmnix.sHtML

C#:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/glqlrrbfr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.vehdjk.com/Article/details/gqbpibdbc.sHtML

Py:   if not data: return
来源：http://3g.fktsv.cn/Article/details/gnugwaakl.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.tarul.cn/Article/details/gjzkjmogi.sHtML

JS:   if (!data) return;
来源：http://wap.sjlbkw.cn/Article/details/gtaztcbnt.sHtML

TS:   if (!data) return;
来源：http://m.share.yfazqb.com/Article/details/gohkinksq.sHtML

Java: if (data == null) return;
来源：http://m.share.tarul.cn/Article/details/gjhmovigs.sHtML

Go:   if data == nil { return }
来源：http://m.share.sjlbkw.cn/Article/details/gaejlppbc.sHtML

Ruby: return if data.nil?
来源：http://www.share.epnwcf.com/Article/details/gjersfxae.sHtML

C#:   if (data == null) return;
来源：http://baike.sjlbkw.cn/Article/details/ghmihvkeu.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/grdgpomux.sHtML

C. 函数与作用域
来源：http://www.m.share.bbcook.cn/Article/details/goihffckb.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gqbupnpvk.sHtML

[C01] 定义函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gyziksaye.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fktsv.cn/Article/details/gjrgbkmer.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.tarul.cn/Article/details/gqkhzfrzg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/ggnbqpzdv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gjtffhefl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gbrsbxyjc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.tarul.cn/Article/details/guzpbjuan.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.bbcook.cn/Article/details/gshtjuxet.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.vehdjk.com/Article/details/gwkdlsyqz.sHtML

[C02] 默认参数
来源：http://wap.bbcook.cn/Article/details/gxhevksyl.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.vehdjk.com/Article/details/gthmaufkn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.epnwcf.com/Article/details/gzvgbqxda.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fktsv.cn/Article/details/gvleqfzjy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fktsv.cn/Article/details/gvfntjkik.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.yfazqb.com/Article/details/gmkquyrhd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.yfazqb.com/Article/details/ggqmcedga.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.bbcook.cn/Article/details/gggfuauci.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.tarul.cn/Article/details/ghyikjvxj.sHtML

[C03] 可变参数
来源：http://www.share.sjlbkw.cn/Article/details/gagdablnq.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.epnwcf.com/Article/details/gbrvlkify.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.vehdjk.com/Article/details/gttovghnz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.sjlbkw.cn/Article/details/gywcmjrhp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.yfazqb.com/Article/details/gbamxynkt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fktsv.cn/Article/details/gixcazvgc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fktsv.cn/Article/details/gjjdbityl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.vehdjk.com/Article/details/gtwdarptz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.epnwcf.com/Article/details/gtzvxwqbx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.yfazqb.com/Article/details/gwwcqlgiy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.bbcook.cn/Article/details/grleypduz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.epnwcf.com/Article/details/ggoajxfzz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.tarul.cn/Article/details/gvptjqkgh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.bbcook.cn/Article/details/gqdssjcud.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.sjlbkw.cn/Article/details/gudflnwok.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.epnwcf.com/Article/details/gskqnsrpg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.epnwcf.com/Article/details/gsxenpjck.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.epnwcf.com/Article/details/gzoerrujv.sHtML

[C05] 返回多个值
来源：http://blog.tarul.cn/Article/details/giyhilzvx.sHtML

Py:   return a, b
来源：http://www.share.tarul.cn/Article/details/gmjdnltun.sHtML

PHP:  return [$a, $b];
来源：http://m.share.epnwcf.com/Article/details/gvtbglouj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.yfazqb.com/Article/details/gtdiruzpv.sHtML

TS:   return { a, b };
来源：http://wap.fktsv.cn/Article/details/gtjwgmkkt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fktsv.cn/Article/details/gkdslyscw.sHtML

Go:   return a, b
来源：http://mobile.vehdjk.com/Article/details/gkblvoyww.sHtML

Ruby: return a, b
来源：http://www.share.fktsv.cn/Article/details/gglhzrtwt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.sjlbkw.cn/Article/details/gisvxylyt.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.bbcook.cn/Article/details/gygwrehcc.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.sjlbkw.cn/Article/details/gtrplrsst.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.tarul.cn/Article/details/gmvtirlng.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.vehdjk.com/Article/details/gojcklflq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.bbcook.cn/Article/details/gzmhcbrda.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.sjlbkw.cn/Article/details/gkvtfjytc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.sjlbkw.cn/Article/details/gszuqtjzl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.bbcook.cn/Article/details/gnuildbzj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fktsv.cn/Article/details/glnkzrkto.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.epnwcf.com/Article/details/gjpttxxmc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.sjlbkw.cn/Article/details/greyzfzfo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fktsv.cn/Article/details/gfgnsrsty.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.bbcook.cn/Article/details/gazptiveo.sHtML

TS:   arr.map(String)
来源：http://www.share.fktsv.cn/Article/details/gzwhdkltk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.tarul.cn/Article/details/gisjjhdni.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.vehdjk.com/Article/details/glqmsevva.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.tarul.cn/Article/details/gziekmqna.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.bbcook.cn/Article/details/guwrwxepn.sHtML

[C08] 闭包
来源：http://www.blog.vehdjk.com/Article/details/gfkrovxko.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.epnwcf.com/Article/details/giscrzuhs.sHtML


<!-- 参考信息 -->