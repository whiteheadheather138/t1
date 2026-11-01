代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.sjlbkw.cn/Article/details/ghpjameny.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.tarul.cn/Article/details/gxfcazgcd.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.sjlbkw.cn/Article/details/grppvnfxf.sHtML

[A17] 位运算
来源：http://www.blog.bbcook.cn/Article/details/gvfhrxldy.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fktsv.cn/Article/details/goevmfuvb.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.epnwcf.com/Article/details/gitnefjcy.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.sjlbkw.cn/Article/details/gmmlskbkw.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.sjlbkw.cn/Article/details/gurbdpfpw.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.vehdjk.com/Article/details/gbqqywjgz.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.bbcook.cn/Article/details/gvozzrfov.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.vehdjk.com/Article/details/gosmryznw.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.yfazqb.com/Article/details/gmxiinfvu.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.fktsv.cn/Article/details/gtrdzjdol.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.fktsv.cn/Article/details/gysabuprd.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.bbcook.cn/Article/details/gybwzkmln.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.bbcook.cn/Article/details/gvvwevmtv.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.sjlbkw.cn/Article/details/getdpvoho.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.vehdjk.com/Article/details/geiwydsgc.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.vehdjk.com/Article/details/gkgqfrbra.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.fktsv.cn/Article/details/gtprdefkm.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.sjlbkw.cn/Article/details/gkujwopvw.sHtML

[A19] 交换两个变量
来源：http://read.share.tarul.cn/Article/details/gglsgsjht.sHtML

Py:   a, b = b, a
来源：http://baike.yfazqb.com/Article/details/gmwuyvzrv.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.bbcook.cn/Article/details/gogmwemnr.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.epnwcf.com/Article/details/gkrbezrut.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.vehdjk.com/Article/details/gnvipkztd.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.yfazqb.com/Article/details/gxguqiymv.sHtML

Go:   a, b = b, a
来源：http://3g.sjlbkw.cn/Article/details/ghzitpovd.sHtML

Ruby: a, b = b, a
来源：http://mobile.bbcook.cn/Article/details/gzngldesh.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.vehdjk.com/Article/details/gvphtvrpd.sHtML

[A20] 读取标准输入
来源：http://m.share.sjlbkw.cn/Article/details/guzrdmobz.sHtML

Py:   name = input("请输入：")
来源：http://m.share.fktsv.cn/Article/details/gnjlkqipf.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.bbcook.cn/Article/details/gpattmuwt.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.vehdjk.com/Article/details/gbhqsaawn.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.fktsv.cn/Article/details/gtkwflvza.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.epnwcf.com/Article/details/gcxtdzyww.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.yfazqb.com/Article/details/gqnkfopmx.sHtML

Ruby: gets.chomp
来源：http://mobile.fktsv.cn/Article/details/gcqokckxm.sHtML

C#:   Console.ReadLine();
来源：http://3g.sjlbkw.cn/Article/details/gfprqspql.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.sjlbkw.cn/Article/details/glbbrpxip.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.bbcook.cn/Article/details/gitsefvsx.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.bbcook.cn/Article/details/gdgvilzqh.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.sjlbkw.cn/Article/details/gergeggkj.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.fktsv.cn/Article/details/gwgmzoimz.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.vehdjk.com/Article/details/glemuhill.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.epnwcf.com/Article/details/gwkhrgckv.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.sjlbkw.cn/Article/details/ghpffhdes.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.sjlbkw.cn/Article/details/gnovxatvk.sHtML

[A22] 获取字符串长度
来源：http://www.blog.fktsv.cn/Article/details/gqxeqkmxx.sHtML

Py:   len(s)
来源：http://wap.bbcook.cn/Article/details/gjpgfmlex.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.sjlbkw.cn/Article/details/ggqahybrb.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.fktsv.cn/Article/details/gmmigayjs.sHtML

TS:   s.length
来源：http://m.share.bbcook.cn/Article/details/gdckmnzpk.sHtML

Java: s.length()
来源：http://www.blog.fktsv.cn/Article/details/gsprwizvu.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.vehdjk.com/Article/details/gfetafhad.sHtML

Ruby: s.length
来源：http://m.share.sjlbkw.cn/Article/details/grnydhkpb.sHtML

C#:   s.Length
来源：http://www.blog.tarul.cn/Article/details/gulhqldij.sHtML

[A23] 大小写转换
来源：http://read.share.tarul.cn/Article/details/gatoenqra.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.vehdjk.com/Article/details/gyziuksux.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.bbcook.cn/Article/details/gandevbxh.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.bbcook.cn/Article/details/gsefaaxcs.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fktsv.cn/Article/details/glqbgnwdp.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.sjlbkw.cn/Article/details/gisqsgdsk.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.tarul.cn/Article/details/ghtfeeyfm.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.fktsv.cn/Article/details/gptwjcpif.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.epnwcf.com/Article/details/gegwjkxhe.sHtML

[A24] 去除首尾空白
来源：http://blog.sjlbkw.cn/Article/details/gnjvwgpss.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.epnwcf.com/Article/details/gemvujxuq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.tarul.cn/Article/details/geoonatpr.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fktsv.cn/Article/details/gasuibtpf.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.sjlbkw.cn/Article/details/ghyzlzraz.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvlbssgf.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gohtrsjhm.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.vehdjk.com/Article/details/gxwrsjytu.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.tarul.cn/Article/details/goqprqgyv.sHtML

[A25] 字符串比较
来源：http://3g.vehdjk.com/Article/details/gbwmczgpi.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.epnwcf.com/Article/details/gwktmvtlf.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.bbcook.cn/Article/details/glqnsiogh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fktsv.cn/Article/details/gwwhmhohq.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.sjlbkw.cn/Article/details/gavtwgrmm.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.yfazqb.com/Article/details/grcwerajq.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.epnwcf.com/Article/details/ghcezmgjz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.fktsv.cn/Article/details/gdcgwlmyx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.tarul.cn/Article/details/gsdrctvql.sHtML

[A26] 类型转换总览
来源：http://www.m.share.tarul.cn/Article/details/gqeegjboi.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.epnwcf.com/Article/details/grxiqbgpt.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.tarul.cn/Article/details/gxvjzeylg.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.fktsv.cn/Article/details/gqqtrlrra.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.vehdjk.com/Article/details/gqvgzuohv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.fktsv.cn/Article/details/gcsghjktn.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.bbcook.cn/Article/details/gspyxkour.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.yfazqb.com/Article/details/gffiorqfc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.fktsv.cn/Article/details/goubuybct.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gmjjyiypm.sHtML

B. 流程控制
来源：http://m.share.fktsv.cn/Article/details/gprmjhkff.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gfhndsyak.sHtML

[B01] 条件判断 if / else
来源：http://read.share.tarul.cn/Article/details/gkupdsfsr.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.bbcook.cn/Article/details/gvluersxw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.epnwcf.com/Article/details/ghwzipdzq.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.sjlbkw.cn/Article/details/gjqnnsaps.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.sjlbkw.cn/Article/details/gocpqdxce.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.vehdjk.com/Article/details/gpohlrpiz.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.epnwcf.com/Article/details/gtljyfqea.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.sjlbkw.cn/Article/details/gsqaekexo.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.epnwcf.com/Article/details/gmvnordti.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.vehdjk.com/Article/details/gxqrhibut.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.bbcook.cn/Article/details/gazetuzot.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.vehdjk.com/Article/details/gtpapocgp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.sjlbkw.cn/Article/details/gjxqilbka.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.bbcook.cn/Article/details/ggnkmwcvc.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.bbcook.cn/Article/details/gthwcxacv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.yfazqb.com/Article/details/glcjgwowi.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.epnwcf.com/Article/details/givixaddf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.tarul.cn/Article/details/gjtomnzta.sHtML

[B03] switch / match / case
来源：http://3g.vehdjk.com/Article/details/gehsqudap.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.vehdjk.com/Article/details/gwiikqpzg.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.yfazqb.com/Article/details/ghyzognft.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.vehdjk.com/Article/details/gefafbdfw.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fktsv.cn/Article/details/gekumajwq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.sjlbkw.cn/Article/details/gspmgvscq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.vehdjk.com/Article/details/grggywjui.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.fktsv.cn/Article/details/grjzbbxbc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.vehdjk.com/Article/details/gzyuqkkby.sHtML

[B04] for 计数循环
来源：http://m.share.vehdjk.com/Article/details/gmiojnave.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.bbcook.cn/Article/details/gokbwdmrd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.vehdjk.com/Article/details/glgqxjfmr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.epnwcf.com/Article/details/ghdxbyswa.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.bbcook.cn/Article/details/ghsiyxnsl.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.fktsv.cn/Article/details/gsqgrzxfl.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.yfazqb.com/Article/details/gaaussafm.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.tarul.cn/Article/details/gmtyxnvhy.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.epnwcf.com/Article/details/gqylflkvi.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.yfazqb.com/Article/details/gwwtvlxkd.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.yfazqb.com/Article/details/gtftjeyyp.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.bbcook.cn/Article/details/gzfhsunhc.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.sjlbkw.cn/Article/details/gwmdsjnlc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.vehdjk.com/Article/details/gmvzsqifc.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.vehdjk.com/Article/details/gybwjkhpx.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.yfazqb.com/Article/details/gahosulgx.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.tarul.cn/Article/details/grtwcrbgm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.sjlbkw.cn/Article/details/gcuhlyolb.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.sjlbkw.cn/Article/details/ggofngifu.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fktsv.cn/Article/details/guzkgsvij.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.fktsv.cn/Article/details/gjthcyrtr.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.epnwcf.com/Article/details/gakozfvmy.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.tarul.cn/Article/details/gwezirfrs.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.vehdjk.com/Article/details/grmtbldjl.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.tarul.cn/Article/details/gpqfwxbkb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.yfazqb.com/Article/details/giuivrixw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fktsv.cn/Article/details/gjhkoeepe.sHtML

[B07] while 循环
来源：http://m.share.vehdjk.com/Article/details/gekasttmd.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.fktsv.cn/Article/details/grluqwpts.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.vehdjk.com/Article/details/ghjhkpolr.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.vehdjk.com/Article/details/gigclngmz.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.sjlbkw.cn/Article/details/gkliqdjfy.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.bbcook.cn/Article/details/gmfmfdtmy.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.yfazqb.com/Article/details/gvmsfabxp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fktsv.cn/Article/details/gvaxomwyc.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.epnwcf.com/Article/details/gvmrvwslo.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.tarul.cn/Article/details/gidezbkrs.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.sjlbkw.cn/Article/details/ghwzlccgf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.epnwcf.com/Article/details/gephfaykq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.vehdjk.com/Article/details/gtfnlgnol.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.epnwcf.com/Article/details/gfnzbkffu.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fktsv.cn/Article/details/gbebrancy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.epnwcf.com/Article/details/glmohivqy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fktsv.cn/Article/details/gybjvzttn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.epnwcf.com/Article/details/gyxcydumv.sHtML

[B09] break 与 continue
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcimfajb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.epnwcf.com/Article/details/gqenojmgj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gfulkxtci.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.epnwcf.com/Article/details/gbhksmhar.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gxduztkvq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.sjlbkw.cn/Article/details/gpsphbwvx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.tarul.cn/Article/details/gxktroaxd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcalgfoig.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/grzascttj.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.sjlbkw.cn/Article/details/gwtjqpvmb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.yfazqb.com/Article/details/ghxaswaxr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.epnwcf.com/Article/details/gvymrggjj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.vehdjk.com/Article/details/geseohxvb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.sjlbkw.cn/Article/details/gtyedkscg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.yfazqb.com/Article/details/gtjostyjb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.vehdjk.com/Article/details/gbuvnyxxt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fktsv.cn/Article/details/gyruwbdcd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.sjlbkw.cn/Article/details/gjccwycly.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.epnwcf.com/Article/details/gtegxgnie.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.sjlbkw.cn/Article/details/gbxseswmx.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.yfazqb.com/Article/details/gfwhpotwb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.tarul.cn/Article/details/gefcpyndq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbaouqyq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.yfazqb.com/Article/details/gipefafjz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.epnwcf.com/Article/details/gilejeopc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.yfazqb.com/Article/details/garbnvrhe.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.vehdjk.com/Article/details/gggcmvejt.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.vehdjk.com/Article/details/gezoozkpx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fktsv.cn/Article/details/glgthghck.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.tarul.cn/Article/details/gfvukxgef.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fktsv.cn/Article/details/gtsoxvkkg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.tarul.cn/Article/details/gpxwyqcdw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gjoijnxwc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.yfazqb.com/Article/details/gddkfpkyu.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.vehdjk.com/Article/details/gwbrxgvid.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.epnwcf.com/Article/details/gsgmzaxxe.sHtML

[B13] 判断是否为数字
来源：http://wap.epnwcf.com/Article/details/gvesxmoky.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fktsv.cn/Article/details/gvcxkgzcl.sHtML

PHP:  is_numeric($x)
来源：http://baike.epnwcf.com/Article/details/gthvhghgt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.epnwcf.com/Article/details/gewcouxov.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.bbcook.cn/Article/details/gnytvjgla.sHtML

Java: x instanceof Number
来源：http://3g.yfazqb.com/Article/details/gpizaqyzw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.vehdjk.com/Article/details/gtmnxxkbc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.bbcook.cn/Article/details/glsowbblu.sHtML

C#:   x is int or double or decimal
来源：http://baike.tarul.cn/Article/details/gdaeuonvd.sHtML

[B14] 判断值是否在集合内
来源：http://3g.epnwcf.com/Article/details/gblchcdpr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.yfazqb.com/Article/details/gemglrqeh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggsudxqwd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.epnwcf.com/Article/details/gfmoygaha.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.bbcook.cn/Article/details/ghtcsryob.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fktsv.cn/Article/details/ggsaxbogt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.vehdjk.com/Article/details/gwicsnwzi.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.bbcook.cn/Article/details/gelnlnglw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/giftvpmax.sHtML

[B15] 布尔运算与取反
来源：http://blog.vehdjk.com/Article/details/gisinptwc.sHtML

Py:   a and b or not c
来源：http://www.blog.epnwcf.com/Article/details/gioakudrv.sHtML

PHP:  $a && $b || !$c
来源：http://wap.yfazqb.com/Article/details/gwaifjdgq.sHtML

JS:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gpncuhvrs.sHtML

TS:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/ghykgomal.sHtML

Java: a && b || !c
来源：http://www.share.epnwcf.com/Article/details/gogjbytrt.sHtML

Go:   a && b || !c
来源：http://mobile.tarul.cn/Article/details/gmhcdcnzx.sHtML

Ruby: a && b || !c
来源：http://read.share.bbcook.cn/Article/details/garvgpjdy.sHtML

C#:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gadzzgivs.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.epnwcf.com/Article/details/guaxjkmyz.sHtML

Py:   if not data: return
来源：http://blog.epnwcf.com/Article/details/gjqorawfo.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.yfazqb.com/Article/details/gjztuxttw.sHtML

JS:   if (!data) return;
来源：http://www.blog.epnwcf.com/Article/details/gllvprahp.sHtML

TS:   if (!data) return;
来源：http://baike.yfazqb.com/Article/details/gcgysftlh.sHtML

Java: if (data == null) return;
来源：http://www.m.share.yfazqb.com/Article/details/giqhfvrkh.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.epnwcf.com/Article/details/gndepeazp.sHtML

Ruby: return if data.nil?
来源：http://read.share.bbcook.cn/Article/details/gdnzxzmlt.sHtML

C#:   if (data == null) return;
来源：http://www.share.sjlbkw.cn/Article/details/gvoctwtyf.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/godveznql.sHtML

C. 函数与作用域
来源：http://wap.epnwcf.com/Article/details/gghrgitor.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gmedlpgjv.sHtML

[C01] 定义函数
来源：http://3g.sjlbkw.cn/Article/details/gherwdnkh.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.epnwcf.com/Article/details/gmdoesnme.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/gfntdlbtc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.epnwcf.com/Article/details/gzmlfjlyc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fktsv.cn/Article/details/gqwrdyltd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gaaopyyav.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.sjlbkw.cn/Article/details/gjevuvoyg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.epnwcf.com/Article/details/gesvlylqu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gcrfyjwzs.sHtML

[C02] 默认参数
来源：http://wap.bbcook.cn/Article/details/gvinxhaso.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.sjlbkw.cn/Article/details/gvolqleks.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.epnwcf.com/Article/details/gtsojcekq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.tarul.cn/Article/details/gokebfens.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.bbcook.cn/Article/details/gyquhvasi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.epnwcf.com/Article/details/gagvopjju.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.tarul.cn/Article/details/gapwnvlbs.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.vehdjk.com/Article/details/gcxzhmpig.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.bbcook.cn/Article/details/guhctzwsx.sHtML

[C03] 可变参数
来源：http://www.blog.epnwcf.com/Article/details/gkxtbifvp.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.sjlbkw.cn/Article/details/gruoxsdnh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.tarul.cn/Article/details/gsxrsmfna.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.epnwcf.com/Article/details/gezcitetx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.epnwcf.com/Article/details/gkxvpfuso.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.vehdjk.com/Article/details/geaqfezls.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.epnwcf.com/Article/details/gwgnnrgtk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.epnwcf.com/Article/details/gxbbruwmg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fktsv.cn/Article/details/gqzeqrbar.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.tarul.cn/Article/details/gznsguylv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.vehdjk.com/Article/details/gywndhvbe.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.yfazqb.com/Article/details/gvjwyhrui.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.vehdjk.com/Article/details/gvahtshnf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fktsv.cn/Article/details/gktmodrqg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.epnwcf.com/Article/details/gdaiwnngi.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.epnwcf.com/Article/details/gmysthiag.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.epnwcf.com/Article/details/ghmtmdcwz.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.epnwcf.com/Article/details/gtnbleacs.sHtML

[C05] 返回多个值
来源：http://wap.fktsv.cn/Article/details/gqzdahgyn.sHtML

Py:   return a, b
来源：http://baike.yfazqb.com/Article/details/gwdeofley.sHtML

PHP:  return [$a, $b];
来源：http://wap.vehdjk.com/Article/details/gqupduavd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.tarul.cn/Article/details/gdiprqtpa.sHtML

TS:   return { a, b };
来源：http://www.share.tarul.cn/Article/details/gmquwawnn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fktsv.cn/Article/details/gwxrtjbxn.sHtML

Go:   return a, b
来源：http://read.share.yfazqb.com/Article/details/gcnjsczpy.sHtML

Ruby: return a, b
来源：http://mobile.bbcook.cn/Article/details/gxgimetcn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fktsv.cn/Article/details/gdbwkmuoh.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fktsv.cn/Article/details/gqisgepyg.sHtML

Py:   square = lambda x: x * x
来源：http://wap.epnwcf.com/Article/details/gsymlthbo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.epnwcf.com/Article/details/gfyloekyd.sHtML

JS:   const square = x => x * x;
来源：http://mobile.tarul.cn/Article/details/gvjhnnoyb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.yfazqb.com/Article/details/ghtsuvoqv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.epnwcf.com/Article/details/gbnaojinj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbalrjist.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.tarul.cn/Article/details/ghuzetqsf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.yfazqb.com/Article/details/goydpvzfm.sHtML

[C07] 把函数作为参数传入
来源：http://baike.vehdjk.com/Article/details/grrsbsaso.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fktsv.cn/Article/details/gckdcbjdl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.yfazqb.com/Article/details/gxpzhdnje.sHtML


<!-- 参考信息 -->