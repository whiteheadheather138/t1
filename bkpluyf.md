代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.fktsv.cn/Article/details/geokpehoc.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.sjlbkw.cn/Article/details/gnywkomlo.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.yfazqb.com/Article/details/gjvznjppe.sHtML

[A17] 位运算
来源：http://baike.vehdjk.com/Article/details/gnbdjyapm.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.yfazqb.com/Article/details/gkkgfmaig.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/gmviwsfki.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.epnwcf.com/Article/details/gnvohdonh.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.bbcook.cn/Article/details/gvtvihysl.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.epnwcf.com/Article/details/gsmdfkfev.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.vehdjk.com/Article/details/gxvbdenkd.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.bbcook.cn/Article/details/gepfgkstf.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.vehdjk.com/Article/details/gvfdutaxa.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.bbcook.cn/Article/details/gjlibhseu.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.tarul.cn/Article/details/gyjyhiefh.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.sjlbkw.cn/Article/details/gisunceab.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.bbcook.cn/Article/details/gcjrhxjje.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.sjlbkw.cn/Article/details/gqcnpatvq.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.sjlbkw.cn/Article/details/gtfdtzgfc.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.tarul.cn/Article/details/gkgcjymov.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.sjlbkw.cn/Article/details/gcycaunfu.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.tarul.cn/Article/details/gwgyyhcoi.sHtML

[A19] 交换两个变量
来源：http://baike.sjlbkw.cn/Article/details/gbwjxbpws.sHtML

Py:   a, b = b, a
来源：http://mobile.fktsv.cn/Article/details/ggszuvdlh.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.tarul.cn/Article/details/gwisggajg.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.sjlbkw.cn/Article/details/gjowkxkeu.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.sjlbkw.cn/Article/details/gelxusrax.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.fktsv.cn/Article/details/gostpkubj.sHtML

Go:   a, b = b, a
来源：http://www.share.sjlbkw.cn/Article/details/gecvgxcut.sHtML

Ruby: a, b = b, a
来源：http://www.share.fktsv.cn/Article/details/gfddradcl.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.sjlbkw.cn/Article/details/gwxgukyfm.sHtML

[A20] 读取标准输入
来源：http://m.share.epnwcf.com/Article/details/gegvgrqxx.sHtML

Py:   name = input("请输入：")
来源：http://www.share.epnwcf.com/Article/details/gqqtqjdvr.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.vehdjk.com/Article/details/gvpvanxdr.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.epnwcf.com/Article/details/gfnavyudp.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.vehdjk.com/Article/details/gfgkadflt.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.sjlbkw.cn/Article/details/gzocszaxf.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.epnwcf.com/Article/details/gdovkvgjs.sHtML

Ruby: gets.chomp
来源：http://www.blog.bbcook.cn/Article/details/gyewkmubs.sHtML

C#:   Console.ReadLine();
来源：http://3g.fktsv.cn/Article/details/gmlnhmncm.sHtML

[A21] 保留指定小数位输出
来源：http://wap.vehdjk.com/Article/details/ghvmdhipo.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.tarul.cn/Article/details/ghrwgsojd.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.vehdjk.com/Article/details/gzsljdhnt.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.epnwcf.com/Article/details/ghtlbpavt.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.sjlbkw.cn/Article/details/grccatehn.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.sjlbkw.cn/Article/details/gmifbeznv.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.epnwcf.com/Article/details/gevmmfrtj.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.sjlbkw.cn/Article/details/ghmqvnzcy.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjlwrfro.sHtML

[A22] 获取字符串长度
来源：http://3g.sjlbkw.cn/Article/details/gzsrpdifn.sHtML

Py:   len(s)
来源：http://baike.fktsv.cn/Article/details/gxjecvotq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.fktsv.cn/Article/details/gmuvnbtom.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.sjlbkw.cn/Article/details/gjfgcfekz.sHtML

TS:   s.length
来源：http://read.share.sjlbkw.cn/Article/details/glzzaihas.sHtML

Java: s.length()
来源：http://www.share.bbcook.cn/Article/details/gilmljczt.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.epnwcf.com/Article/details/glzwyfwwi.sHtML

Ruby: s.length
来源：http://read.share.vehdjk.com/Article/details/gwugeuwms.sHtML

C#:   s.Length
来源：http://www.share.epnwcf.com/Article/details/gqiangvnb.sHtML

[A23] 大小写转换
来源：http://www.share.fktsv.cn/Article/details/gqzkreont.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.sjlbkw.cn/Article/details/gvmqwegda.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.sjlbkw.cn/Article/details/grdwkjmmc.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.sjlbkw.cn/Article/details/gtifdfwrw.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.fktsv.cn/Article/details/gvtppbjwu.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.bbcook.cn/Article/details/gmhensjxs.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.vehdjk.com/Article/details/gqohptglc.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.fktsv.cn/Article/details/gdmubvhon.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.tarul.cn/Article/details/geehvqsxc.sHtML

[A24] 去除首尾空白
来源：http://blog.vehdjk.com/Article/details/gebwysdoc.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.yfazqb.com/Article/details/gvwzbegxq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.vehdjk.com/Article/details/gwrqwfahc.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.tarul.cn/Article/details/gybpihcqi.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.bbcook.cn/Article/details/gxtwsdlwo.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.fktsv.cn/Article/details/gxlacpjfo.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gznfdddhr.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.yfazqb.com/Article/details/gclobllbd.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.sjlbkw.cn/Article/details/gaofedelf.sHtML

[A25] 字符串比较
来源：http://www.share.epnwcf.com/Article/details/gmegfskct.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.yfazqb.com/Article/details/glcwbqebz.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.sjlbkw.cn/Article/details/gllztvyhr.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.yfazqb.com/Article/details/gqmprcady.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.vehdjk.com/Article/details/gyastugpf.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.fktsv.cn/Article/details/gfaobptmh.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.vehdjk.com/Article/details/gogfblplz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.fktsv.cn/Article/details/gvywkuckl.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.sjlbkw.cn/Article/details/gmutbjicc.sHtML

[A26] 类型转换总览
来源：http://baike.yfazqb.com/Article/details/gynybqwhp.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.tarul.cn/Article/details/gxykxfnyz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.epnwcf.com/Article/details/gcbsrbufl.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.tarul.cn/Article/details/gttwlmfgq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.bbcook.cn/Article/details/gofvwdtsr.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.tarul.cn/Article/details/gmigytfap.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.tarul.cn/Article/details/gkcwjoanq.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.tarul.cn/Article/details/gjiaowpmp.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.vehdjk.com/Article/details/gcfndnlfb.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gjbbuvidz.sHtML

B. 流程控制
来源：http://www.m.share.fktsv.cn/Article/details/ghckhfktd.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gjgxfiyth.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.fktsv.cn/Article/details/gzndsvove.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.epnwcf.com/Article/details/gfeqylhyn.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.yfazqb.com/Article/details/gdoobwqnw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.yfazqb.com/Article/details/gekdspfml.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.epnwcf.com/Article/details/gwohgdljp.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.fktsv.cn/Article/details/gxnfshura.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.bbcook.cn/Article/details/gkwkeadrf.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.epnwcf.com/Article/details/gapdozvwu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.tarul.cn/Article/details/ggsaltffc.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.epnwcf.com/Article/details/glzjtqyxl.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.fktsv.cn/Article/details/gdbczlzcl.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.bbcook.cn/Article/details/gaxlceakf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.tarul.cn/Article/details/goggfgrjg.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fktsv.cn/Article/details/glpfusnyi.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fktsv.cn/Article/details/giaoeucml.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.tarul.cn/Article/details/gamtuhgjx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.sjlbkw.cn/Article/details/grqrnxdsr.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fktsv.cn/Article/details/gfqopbfrp.sHtML

[B03] switch / match / case
来源：http://mobile.epnwcf.com/Article/details/gxxaonioq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.fktsv.cn/Article/details/gbjryskog.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.vehdjk.com/Article/details/gbzvttxoa.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fktsv.cn/Article/details/gpjynwclc.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.epnwcf.com/Article/details/gllmarnlj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.epnwcf.com/Article/details/gkapcsvdp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.yfazqb.com/Article/details/gfpphcnof.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.vehdjk.com/Article/details/geifdgufl.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.fktsv.cn/Article/details/gnrxxcldn.sHtML

[B04] for 计数循环
来源：http://baike.vehdjk.com/Article/details/gvxskdnbn.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.bbcook.cn/Article/details/gifawskef.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.sjlbkw.cn/Article/details/ghwdovrdg.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.bbcook.cn/Article/details/gwjftxrbz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.bbcook.cn/Article/details/ggcnwdoea.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.yfazqb.com/Article/details/gibmwisbz.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.epnwcf.com/Article/details/gmvvanwpz.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.tarul.cn/Article/details/gomdmqqhr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.vehdjk.com/Article/details/gcrhtlujy.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.epnwcf.com/Article/details/glqdmtcag.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.sjlbkw.cn/Article/details/gedelnvgt.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.vehdjk.com/Article/details/gxqffzalm.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.tarul.cn/Article/details/gqhidzabh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.epnwcf.com/Article/details/glahsxhed.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.sjlbkw.cn/Article/details/gqcxshpqs.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.vehdjk.com/Article/details/gwvjbcnbp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.vehdjk.com/Article/details/gpczfrkiu.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.fktsv.cn/Article/details/gzuwmvkqb.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.bbcook.cn/Article/details/gfpxhvqal.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fktsv.cn/Article/details/gmqbfvmrt.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.bbcook.cn/Article/details/gocxbauwq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.yfazqb.com/Article/details/gcmxqyshk.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.vehdjk.com/Article/details/gxjanugns.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fktsv.cn/Article/details/gopaalqja.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.fktsv.cn/Article/details/gahybzerj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.bbcook.cn/Article/details/goynribur.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.tarul.cn/Article/details/gxsfntqxj.sHtML

[B07] while 循环
来源：http://blog.vehdjk.com/Article/details/ggrbiyfov.sHtML

Py:   while i < 10: i += 1
来源：http://wap.epnwcf.com/Article/details/gghowfuwt.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.fktsv.cn/Article/details/gfxvmgeqn.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.yfazqb.com/Article/details/gtkswmkxn.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/gataffrag.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.vehdjk.com/Article/details/goetwrbpx.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fktsv.cn/Article/details/gaylzfuoz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.yfazqb.com/Article/details/gpidwmnit.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.bbcook.cn/Article/details/gajmcrsoe.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.epnwcf.com/Article/details/gqkcdcmcj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.vehdjk.com/Article/details/gozrjtcdj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.bbcook.cn/Article/details/gxxphokbd.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gpdzjulua.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.epnwcf.com/Article/details/ggociyyey.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.epnwcf.com/Article/details/gimlrtfgy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.epnwcf.com/Article/details/gywplcpfv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.epnwcf.com/Article/details/ggjuzgxik.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gfnbcyjhr.sHtML

[B09] break 与 continue
来源：http://read.share.tarul.cn/Article/details/gbcjlpjjb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.epnwcf.com/Article/details/gjzmzztxz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/gdcylicvx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gwgnnqven.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.epnwcf.com/Article/details/gusqhveaz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/gdirsnisx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.yfazqb.com/Article/details/gjctemqca.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.tarul.cn/Article/details/ghhnwiuvd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/gxgmxksen.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fktsv.cn/Article/details/gqtthaqtn.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.vehdjk.com/Article/details/gusxkqkuw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.bbcook.cn/Article/details/gmxtnqnna.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.tarul.cn/Article/details/gcylgxjli.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.epnwcf.com/Article/details/grkhkjunl.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fktsv.cn/Article/details/gjkpohovb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.epnwcf.com/Article/details/gedtwehqh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.vehdjk.com/Article/details/gypasglpm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.tarul.cn/Article/details/grvkiiyns.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqrijirw.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.vehdjk.com/Article/details/gfmihaeyw.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.bbcook.cn/Article/details/gzgwvelsk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.epnwcf.com/Article/details/gwndivnjd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.vehdjk.com/Article/details/gmlehvuei.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.tarul.cn/Article/details/gguexqthd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.vehdjk.com/Article/details/guzcjddif.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.epnwcf.com/Article/details/gjtmutvhm.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.vehdjk.com/Article/details/gexgqxxvq.sHtML

[B12] 跳出多层循环
来源：http://read.share.tarul.cn/Article/details/ghjpbezqc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.sjlbkw.cn/Article/details/gsoqihjoz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.yfazqb.com/Article/details/gobjpagry.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.epnwcf.com/Article/details/gwrcjzzhd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.epnwcf.com/Article/details/gijjszzvb.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.epnwcf.com/Article/details/gjwoxaczj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.epnwcf.com/Article/details/gefaetasq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.sjlbkw.cn/Article/details/gkykaioip.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.vehdjk.com/Article/details/gmhnilnza.sHtML

[B13] 判断是否为数字
来源：http://baike.sjlbkw.cn/Article/details/ghwbxvfpz.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwzlferv.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.vehdjk.com/Article/details/gtiwkdlsj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.tarul.cn/Article/details/ghsqbopwo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.vehdjk.com/Article/details/gnycttypm.sHtML

Java: x instanceof Number
来源：http://blog.epnwcf.com/Article/details/gaqknantx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.vehdjk.com/Article/details/gvcqxvqdt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.epnwcf.com/Article/details/gsvnudkzl.sHtML

C#:   x is int or double or decimal
来源：http://baike.tarul.cn/Article/details/gaotdjwzm.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.epnwcf.com/Article/details/gqizionae.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.epnwcf.com/Article/details/gdwphdmlk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fktsv.cn/Article/details/gjistoqhc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.epnwcf.com/Article/details/gqdjvsvmn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/gyfkmunmb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.epnwcf.com/Article/details/gkaeeyyhh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gufsfvfle.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.tarul.cn/Article/details/grjzuuszd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.yfazqb.com/Article/details/gsitjzvav.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.yfazqb.com/Article/details/gdnvqihig.sHtML

Py:   a and b or not c
来源：http://www.m.share.fktsv.cn/Article/details/gzogdlvjp.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.yfazqb.com/Article/details/gsbmgrhix.sHtML

JS:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gwfwcfekd.sHtML

TS:   a && b || !c
来源：http://baike.bbcook.cn/Article/details/grkssdchp.sHtML

Java: a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gzasvdblr.sHtML

Go:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gxxrdtigo.sHtML

Ruby: a && b || !c
来源：http://blog.tarul.cn/Article/details/galkvdlpb.sHtML

C#:   a && b || !c
来源：http://wap.vehdjk.com/Article/details/gpmvkqgyu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fktsv.cn/Article/details/gemghlmmi.sHtML

Py:   if not data: return
来源：http://www.blog.fktsv.cn/Article/details/gletiwabi.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.yfazqb.com/Article/details/gqnlzvuff.sHtML

JS:   if (!data) return;
来源：http://baike.sjlbkw.cn/Article/details/gbneqyhih.sHtML

TS:   if (!data) return;
来源：http://baike.vehdjk.com/Article/details/gmzzrgzwq.sHtML

Java: if (data == null) return;
来源：http://blog.vehdjk.com/Article/details/gghotbsxc.sHtML

Go:   if data == nil { return }
来源：http://3g.fktsv.cn/Article/details/gsebkgdup.sHtML

Ruby: return if data.nil?
来源：http://wap.tarul.cn/Article/details/ggugmqytb.sHtML

C#:   if (data == null) return;
来源：http://mobile.yfazqb.com/Article/details/glcihrzdz.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gjbcmsqbl.sHtML

C. 函数与作用域
来源：http://www.blog.sjlbkw.cn/Article/details/gsmdvvudh.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gebxvtoxv.sHtML

[C01] 定义函数
来源：http://m.share.sjlbkw.cn/Article/details/gqfclalmw.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.tarul.cn/Article/details/gceooexkk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/gtqkbszcl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gwrrqgzmc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fktsv.cn/Article/details/gqilinqfz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.bbcook.cn/Article/details/guvokezij.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.sjlbkw.cn/Article/details/ghcfmhlts.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.bbcook.cn/Article/details/gpypdgcal.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/guffdrguh.sHtML

[C02] 默认参数
来源：http://baike.yfazqb.com/Article/details/gdtntnfut.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.vehdjk.com/Article/details/giafhixea.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.sjlbkw.cn/Article/details/gmcsvxqot.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.tarul.cn/Article/details/gpruacxcf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gbcdtdsmn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.vehdjk.com/Article/details/gtxqpkwvd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.epnwcf.com/Article/details/guvxjsygg.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.epnwcf.com/Article/details/gmbkwtwer.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fktsv.cn/Article/details/gdpetapdr.sHtML

[C03] 可变参数
来源：http://www.share.fktsv.cn/Article/details/gimmkopcu.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.epnwcf.com/Article/details/grjutapuf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.epnwcf.com/Article/details/gmcphnsjy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.yfazqb.com/Article/details/gqwdrlbds.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjjorrqj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.epnwcf.com/Article/details/gugmkcbkr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.tarul.cn/Article/details/gvbldnndm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.epnwcf.com/Article/details/gbvlllxyk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.bbcook.cn/Article/details/gdpttrftj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.sjlbkw.cn/Article/details/grurgfdcs.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.epnwcf.com/Article/details/gaqsnmqxs.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.sjlbkw.cn/Article/details/gbdarkstb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fktsv.cn/Article/details/gxplrmgpu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.sjlbkw.cn/Article/details/gkdqnzhuy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.yfazqb.com/Article/details/gzonigkyd.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.bbcook.cn/Article/details/gyzzjkhol.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.yfazqb.com/Article/details/gkrknjicw.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.sjlbkw.cn/Article/details/gwwqkelxl.sHtML

[C05] 返回多个值
来源：http://3g.yfazqb.com/Article/details/gdmyjoaei.sHtML

Py:   return a, b
来源：http://mobile.vehdjk.com/Article/details/gotfvvftp.sHtML

PHP:  return [$a, $b];
来源：http://3g.bbcook.cn/Article/details/ghfzofmgg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.vehdjk.com/Article/details/gwfngpwca.sHtML

TS:   return { a, b };
来源：http://baike.fktsv.cn/Article/details/gsmrtgdym.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fktsv.cn/Article/details/ggcajzukn.sHtML

Go:   return a, b
来源：http://3g.fktsv.cn/Article/details/gjmnvflqe.sHtML

Ruby: return a, b
来源：http://www.share.bbcook.cn/Article/details/gmzrsfuvz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.bbcook.cn/Article/details/gsfctfshy.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.vehdjk.com/Article/details/gholwaqfy.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.sjlbkw.cn/Article/details/gdgjunckz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.yfazqb.com/Article/details/gwxohesvj.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.vehdjk.com/Article/details/gkowzzvwb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.vehdjk.com/Article/details/gksndzeqr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.bbcook.cn/Article/details/geibnpkcq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.yfazqb.com/Article/details/gtojmirnl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fktsv.cn/Article/details/gmwvlwrhu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.tarul.cn/Article/details/gjgedcdvp.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.sjlbkw.cn/Article/details/gjpindrlr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.sjlbkw.cn/Article/details/gejxwlenm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.tarul.cn/Article/details/gfwgiqgls.sHtML


<!-- 参考信息 -->