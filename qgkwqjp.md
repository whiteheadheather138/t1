代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.fktsv.cn/Article/details/gbnzarfqx.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.bbcook.cn/Article/details/gyhrprimj.sHtML

TS:   if (!x) {}
来源：http://3g.vehdjk.com/Article/details/gxdfesnff.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.bbcook.cn/Article/details/gpvdatdah.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.bbcook.cn/Article/details/gsfzziwln.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.fktsv.cn/Article/details/gjhbujohq.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.fktsv.cn/Article/details/gjqzbltfm.sHtML

[A17] 位运算
来源：http://3g.epnwcf.com/Article/details/gfmgzdonn.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.sjlbkw.cn/Article/details/gdsoxojrx.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.sjlbkw.cn/Article/details/gxfhykrzp.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.epnwcf.com/Article/details/gtzdhdrqk.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.bbcook.cn/Article/details/ghvucdhom.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.bbcook.cn/Article/details/gdpxviack.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.fktsv.cn/Article/details/gcrdtowdi.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.sjlbkw.cn/Article/details/gqqxrzmoc.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.sjlbkw.cn/Article/details/gmqmqryux.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.bbcook.cn/Article/details/gcvdolizt.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.bbcook.cn/Article/details/gbhfgqtoz.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.vehdjk.com/Article/details/garddnefw.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.tarul.cn/Article/details/gpomifasv.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.epnwcf.com/Article/details/gymmycthx.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.yfazqb.com/Article/details/gbtkjkskb.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.bbcook.cn/Article/details/gyaddlxxp.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.tarul.cn/Article/details/gebdbtnjd.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.epnwcf.com/Article/details/gmrjnoiap.sHtML

[A19] 交换两个变量
来源：http://m.share.vehdjk.com/Article/details/gidtepcoc.sHtML

Py:   a, b = b, a
来源：http://wap.epnwcf.com/Article/details/gzjqbvedx.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.tarul.cn/Article/details/gzjrilzfd.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.vehdjk.com/Article/details/gnmvmauik.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.epnwcf.com/Article/details/gpnngegjd.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.epnwcf.com/Article/details/gvdlazdfv.sHtML

Go:   a, b = b, a
来源：http://mobile.yfazqb.com/Article/details/gpsnoflfu.sHtML

Ruby: a, b = b, a
来源：http://www.share.tarul.cn/Article/details/gfvbcybai.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.fktsv.cn/Article/details/gcpmhqbrq.sHtML

[A20] 读取标准输入
来源：http://m.share.vehdjk.com/Article/details/gwlnskclf.sHtML

Py:   name = input("请输入：")
来源：http://mobile.yfazqb.com/Article/details/ghvtidvhl.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.tarul.cn/Article/details/gscmefzmx.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.fktsv.cn/Article/details/gnbontlxn.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.tarul.cn/Article/details/gavmqxxxl.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.sjlbkw.cn/Article/details/gbienrbec.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.yfazqb.com/Article/details/gukbqarwr.sHtML

Ruby: gets.chomp
来源：http://wap.fktsv.cn/Article/details/gpqmlcoqe.sHtML

C#:   Console.ReadLine();
来源：http://baike.sjlbkw.cn/Article/details/gcdzpkupx.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.epnwcf.com/Article/details/gmkwshnee.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.fktsv.cn/Article/details/gzbufpkev.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.bbcook.cn/Article/details/gjpjnemiw.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.sjlbkw.cn/Article/details/golzebwnt.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.sjlbkw.cn/Article/details/gsdgrwmlq.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.tarul.cn/Article/details/gimhnrufv.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.epnwcf.com/Article/details/gutysowgp.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.yfazqb.com/Article/details/gkpipdcng.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.yfazqb.com/Article/details/gvhmyhhfg.sHtML

[A22] 获取字符串长度
来源：http://baike.tarul.cn/Article/details/gxzecucwq.sHtML

Py:   len(s)
来源：http://blog.vehdjk.com/Article/details/gxwabhnrs.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.yfazqb.com/Article/details/gejlbyera.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.sjlbkw.cn/Article/details/guzdozqgx.sHtML

TS:   s.length
来源：http://mobile.bbcook.cn/Article/details/gkfxodcxw.sHtML

Java: s.length()
来源：http://baike.bbcook.cn/Article/details/gzfcnxfhf.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.sjlbkw.cn/Article/details/gsdwwdyyz.sHtML

Ruby: s.length
来源：http://wap.tarul.cn/Article/details/gpgbkedxn.sHtML

C#:   s.Length
来源：http://read.share.bbcook.cn/Article/details/ghxkwtnik.sHtML

[A23] 大小写转换
来源：http://3g.yfazqb.com/Article/details/gkayjhpfa.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.fktsv.cn/Article/details/gbusnwmjs.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.epnwcf.com/Article/details/ghwgqnfel.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fktsv.cn/Article/details/gkmvfntes.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.yfazqb.com/Article/details/grdlpjsfg.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.yfazqb.com/Article/details/gmpajesqo.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.fktsv.cn/Article/details/gvubitvwa.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.epnwcf.com/Article/details/gsbcveosd.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.tarul.cn/Article/details/giujsykku.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.fktsv.cn/Article/details/gfsxynzyh.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.sjlbkw.cn/Article/details/ggszfcuoq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.sjlbkw.cn/Article/details/ghlaicftx.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.vehdjk.com/Article/details/ggqjcagrl.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.bbcook.cn/Article/details/grsaxnhrd.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.epnwcf.com/Article/details/grvlszbxh.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.vehdjk.com/Article/details/gozpsmhwj.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.bbcook.cn/Article/details/gabpkuxxb.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.tarul.cn/Article/details/gmaoftcgh.sHtML

[A25] 字符串比较
来源：http://read.share.bbcook.cn/Article/details/glwdeihwo.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.bbcook.cn/Article/details/gurmuddai.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.fktsv.cn/Article/details/gdrzeeqtx.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fktsv.cn/Article/details/gstafgddm.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.vehdjk.com/Article/details/gkgziavub.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.epnwcf.com/Article/details/gxzhlxtjm.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.epnwcf.com/Article/details/glrahsxkr.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.epnwcf.com/Article/details/gdljrckgr.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.vehdjk.com/Article/details/gpxbcmqgu.sHtML

[A26] 类型转换总览
来源：http://mobile.yfazqb.com/Article/details/gzpeguwae.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.sjlbkw.cn/Article/details/gqhaijken.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.tarul.cn/Article/details/gblieapex.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.bbcook.cn/Article/details/gmwswiuej.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.fktsv.cn/Article/details/grxleucau.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.yfazqb.com/Article/details/gukhsvltf.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.yfazqb.com/Article/details/gzrvksgal.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.sjlbkw.cn/Article/details/ghowaluyz.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.epnwcf.com/Article/details/ggqcmkzre.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gfwgqfljl.sHtML

B. 流程控制
来源：http://www.blog.tarul.cn/Article/details/gzvjxhifj.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gcqqkcfhe.sHtML

[B01] 条件判断 if / else
来源：http://baike.fktsv.cn/Article/details/gqxyfswfn.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.vehdjk.com/Article/details/gyqebzrex.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.tarul.cn/Article/details/gguibjhlk.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.yfazqb.com/Article/details/gswvitvwa.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.fktsv.cn/Article/details/gfgmzsqzy.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.sjlbkw.cn/Article/details/gowekvlmo.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.tarul.cn/Article/details/gwqgmnniq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.bbcook.cn/Article/details/gfrzvlikr.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.sjlbkw.cn/Article/details/gxwpscbny.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.epnwcf.com/Article/details/gfimgzlmo.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.bbcook.cn/Article/details/gorhvggsj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.vehdjk.com/Article/details/ghrfkixab.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.tarul.cn/Article/details/gtdujjuoc.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.yfazqb.com/Article/details/grusamxbh.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.yfazqb.com/Article/details/gebstwpbk.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.vehdjk.com/Article/details/gilxjygup.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.epnwcf.com/Article/details/gmuxubrqr.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.bbcook.cn/Article/details/giheroatp.sHtML

[B03] switch / match / case
来源：http://wap.fktsv.cn/Article/details/giwhzyufg.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.tarul.cn/Article/details/gkphuomrx.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.vehdjk.com/Article/details/gxhboeijk.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbyafyzwy.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.tarul.cn/Article/details/gxrpqigsg.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.fktsv.cn/Article/details/gftcwvrdi.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.sjlbkw.cn/Article/details/gmvjhatke.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.vehdjk.com/Article/details/gpvodninx.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.fktsv.cn/Article/details/gdqolwhem.sHtML

[B04] for 计数循环
来源：http://m.share.vehdjk.com/Article/details/gmwyzleik.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.yfazqb.com/Article/details/gdifijhpm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.epnwcf.com/Article/details/glocwchab.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fktsv.cn/Article/details/garxxsaqh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.tarul.cn/Article/details/gdhzweeax.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.yfazqb.com/Article/details/gvaxaxeja.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.epnwcf.com/Article/details/gcjreqerl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.vehdjk.com/Article/details/gacgcxwze.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.sjlbkw.cn/Article/details/gjwxilyfw.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.tarul.cn/Article/details/gguemxpqf.sHtML

Py:   for item in arr: print(item)
来源：http://wap.fktsv.cn/Article/details/gffzbjahy.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.fktsv.cn/Article/details/gxjilgbah.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.fktsv.cn/Article/details/gybsnwmtb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fktsv.cn/Article/details/gfonuimwn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.bbcook.cn/Article/details/gtammewlu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.sjlbkw.cn/Article/details/gzammnjmv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.sjlbkw.cn/Article/details/gpcbzqgyb.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.sjlbkw.cn/Article/details/gxfavdnlg.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.vehdjk.com/Article/details/ghknzdqkn.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.vehdjk.com/Article/details/gazuaxmar.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.epnwcf.com/Article/details/gmowbrpfr.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.epnwcf.com/Article/details/gjyepnyti.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.yfazqb.com/Article/details/gsrxlujfa.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.tarul.cn/Article/details/gckpphcsa.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.fktsv.cn/Article/details/grythihle.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.vehdjk.com/Article/details/grxoeytlp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.vehdjk.com/Article/details/gkwnmsdvm.sHtML

[B07] while 循环
来源：http://www.blog.epnwcf.com/Article/details/gspmcphds.sHtML

Py:   while i < 10: i += 1
来源：http://wap.bbcook.cn/Article/details/gzmnnuhip.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.bbcook.cn/Article/details/gviilmnfu.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fktsv.cn/Article/details/gvdpcbsbp.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.vehdjk.com/Article/details/gxqhpnlga.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/gshjoojxm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.bbcook.cn/Article/details/gxmynzkqf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.sjlbkw.cn/Article/details/gsvuozexh.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/gljexlmad.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.bbcook.cn/Article/details/gusvehnii.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.bbcook.cn/Article/details/gpgrhmqow.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.yfazqb.com/Article/details/gdhrsvjxj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.vehdjk.com/Article/details/geooszhig.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.yfazqb.com/Article/details/ghmslitds.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gjgrsmhhp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.tarul.cn/Article/details/gfkzhqbax.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.yfazqb.com/Article/details/gogluzmpw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/gfajkximi.sHtML

[B09] break 与 continue
来源：http://blog.sjlbkw.cn/Article/details/gnjnohodk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gghbeaprs.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/gbmbhsfxn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.epnwcf.com/Article/details/goyydxcfd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/gjmjwutim.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.bbcook.cn/Article/details/gkzmuwvcb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.vehdjk.com/Article/details/gugzvijwi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.bbcook.cn/Article/details/gctkscgxe.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.tarul.cn/Article/details/gpxionqws.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fktsv.cn/Article/details/gkmevzzck.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.tarul.cn/Article/details/gsouswfkg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.epnwcf.com/Article/details/gzjytuytc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.bbcook.cn/Article/details/goyojezbb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.sjlbkw.cn/Article/details/geomhmonk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.epnwcf.com/Article/details/gdxkhcpmb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.tarul.cn/Article/details/gvqcdyafc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.vehdjk.com/Article/details/gmcajwkld.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.bbcook.cn/Article/details/gwxhbvian.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fktsv.cn/Article/details/gmwnkiucv.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.bbcook.cn/Article/details/gaduyizxe.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fktsv.cn/Article/details/gdrpkwgig.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fktsv.cn/Article/details/gxhkgmvvz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.epnwcf.com/Article/details/gvsqqmnci.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.epnwcf.com/Article/details/grgduqocd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fktsv.cn/Article/details/gfdqgwcfb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.bbcook.cn/Article/details/gjuulemns.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fktsv.cn/Article/details/gzzgblmul.sHtML

[B12] 跳出多层循环
来源：http://3g.tarul.cn/Article/details/gkkhrbmwd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.vehdjk.com/Article/details/gytkaykds.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.sjlbkw.cn/Article/details/gfqvvgidj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fktsv.cn/Article/details/geqdqypqe.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.epnwcf.com/Article/details/gquyvesps.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.yfazqb.com/Article/details/gekutzkqd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.vehdjk.com/Article/details/gkrvxmzhb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.sjlbkw.cn/Article/details/gofioshpv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.yfazqb.com/Article/details/gzmzsqbzs.sHtML

[B13] 判断是否为数字
来源：http://mobile.bbcook.cn/Article/details/ghbyniuzl.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.sjlbkw.cn/Article/details/gctnipoml.sHtML

PHP:  is_numeric($x)
来源：http://mobile.bbcook.cn/Article/details/gakowlwxi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.sjlbkw.cn/Article/details/grmbwejut.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fktsv.cn/Article/details/gladypbtt.sHtML

Java: x instanceof Number
来源：http://baike.bbcook.cn/Article/details/gydropomw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.yfazqb.com/Article/details/gqlvprqcl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.bbcook.cn/Article/details/gbsskmmtk.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.bbcook.cn/Article/details/galnesfca.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.epnwcf.com/Article/details/gcxrhdbdx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.epnwcf.com/Article/details/gubwlpjlf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.bbcook.cn/Article/details/gchczstph.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/glhokbmie.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gsgvmxjpv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.vehdjk.com/Article/details/gwrkvtain.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.yfazqb.com/Article/details/glovxxfeg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.epnwcf.com/Article/details/giajpfukt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fktsv.cn/Article/details/gigurdiog.sHtML

[B15] 布尔运算与取反
来源：http://mobile.sjlbkw.cn/Article/details/gxxtkamqp.sHtML

Py:   a and b or not c
来源：http://www.share.tarul.cn/Article/details/gvpmcnhsp.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.sjlbkw.cn/Article/details/glydyoncc.sHtML

JS:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gxpyorlot.sHtML

TS:   a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gemzmnrjo.sHtML

Java: a && b || !c
来源：http://3g.vehdjk.com/Article/details/gjzkevape.sHtML

Go:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gjzgaoily.sHtML

Ruby: a && b || !c
来源：http://baike.fktsv.cn/Article/details/gnymqkdsu.sHtML

C#:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gotbwrqtk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.tarul.cn/Article/details/gbkikfdkm.sHtML

Py:   if not data: return
来源：http://www.m.share.tarul.cn/Article/details/gxizlrtxb.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.tarul.cn/Article/details/gqrqdqmjr.sHtML

JS:   if (!data) return;
来源：http://blog.epnwcf.com/Article/details/gmonhznam.sHtML

TS:   if (!data) return;
来源：http://m.share.yfazqb.com/Article/details/galhjydgk.sHtML

Java: if (data == null) return;
来源：http://www.share.bbcook.cn/Article/details/geqhodiik.sHtML

Go:   if data == nil { return }
来源：http://baike.fktsv.cn/Article/details/gdvgqmqqq.sHtML

Ruby: return if data.nil?
来源：http://m.share.yfazqb.com/Article/details/gbpslncrp.sHtML

C#:   if (data == null) return;
来源：http://www.share.yfazqb.com/Article/details/gbnniefna.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gdivjunmd.sHtML

C. 函数与作用域
来源：http://baike.vehdjk.com/Article/details/gqjvlconq.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gvimxupco.sHtML

[C01] 定义函数
来源：http://blog.tarul.cn/Article/details/gwvwenaaj.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.epnwcf.com/Article/details/gnvkkepfb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.yfazqb.com/Article/details/gvcbnukyc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gpwqhjnlg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gsalaxbhn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.epnwcf.com/Article/details/guvpnyxxr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.yfazqb.com/Article/details/glxcwxqch.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.epnwcf.com/Article/details/gtckjrcrj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/gvrbjwwnd.sHtML

[C02] 默认参数
来源：http://m.share.sjlbkw.cn/Article/details/gdjynzupl.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.yfazqb.com/Article/details/gzwwdevub.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.epnwcf.com/Article/details/gtmjfrrco.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.yfazqb.com/Article/details/gwxeiotzh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.yfazqb.com/Article/details/gauxjwofb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.bbcook.cn/Article/details/gqjtqmjvb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.vehdjk.com/Article/details/giyacehvx.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.tarul.cn/Article/details/gcddgesxi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.yfazqb.com/Article/details/gwgnlhlkl.sHtML

[C03] 可变参数
来源：http://www.blog.bbcook.cn/Article/details/gytfjaunr.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fktsv.cn/Article/details/ggxxfprsr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.yfazqb.com/Article/details/gqlrolfko.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.yfazqb.com/Article/details/gotdmhypv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.epnwcf.com/Article/details/gcxfpgwhc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.tarul.cn/Article/details/gbnovtzng.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.tarul.cn/Article/details/gqkgtjyad.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.sjlbkw.cn/Article/details/gqbrumigm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.epnwcf.com/Article/details/gbtxjisin.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.sjlbkw.cn/Article/details/gdoothyat.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.tarul.cn/Article/details/gmrclfntt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.bbcook.cn/Article/details/gifnektyb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.epnwcf.com/Article/details/goctrrbwu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.bbcook.cn/Article/details/gxresxajt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.tarul.cn/Article/details/gzmjqgpfy.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.epnwcf.com/Article/details/gqsximdrz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.sjlbkw.cn/Article/details/gadekvuch.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.epnwcf.com/Article/details/gnbfaqzdd.sHtML

[C05] 返回多个值
来源：http://3g.fktsv.cn/Article/details/gtihgjyfv.sHtML

Py:   return a, b
来源：http://mobile.tarul.cn/Article/details/gbdeaqjbh.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fktsv.cn/Article/details/gyguwqdvt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.sjlbkw.cn/Article/details/gmryjbdbd.sHtML

TS:   return { a, b };
来源：http://read.share.fktsv.cn/Article/details/gpsjzebqq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.sjlbkw.cn/Article/details/gleslsjdr.sHtML

Go:   return a, b
来源：http://baike.epnwcf.com/Article/details/gpdzqkcms.sHtML

Ruby: return a, b
来源：http://mobile.epnwcf.com/Article/details/gwtpsjuqk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.tarul.cn/Article/details/gyksydyqi.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fktsv.cn/Article/details/gdesjxmvi.sHtML

Py:   square = lambda x: x * x
来源：http://baike.tarul.cn/Article/details/gxcwhahlc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.bbcook.cn/Article/details/ggkjkozzm.sHtML

JS:   const square = x => x * x;
来源：http://m.share.tarul.cn/Article/details/gbdmhkdnl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fktsv.cn/Article/details/gywicpxvl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.yfazqb.com/Article/details/gfgpchhjm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.yfazqb.com/Article/details/guuzzzrih.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.bbcook.cn/Article/details/giyvsgknj.sHtML


<!-- 参考信息 -->