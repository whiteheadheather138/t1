代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.blog.fktsv.cn/Article/details/gusackiby.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.sjlbkw.cn/Article/details/gztyzwqlp.sHtML

[A16] 真假值判断规则
来源：http://3g.vehdjk.com/Article/details/gicaeewvr.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.sjlbkw.cn/Article/details/giqqimhbf.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.yfazqb.com/Article/details/gmauolhem.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.bbcook.cn/Article/details/ghdgpmpsj.sHtML

TS:   if (!x) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gbuvjibvv.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.yfazqb.com/Article/details/gwptlfbli.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.epnwcf.com/Article/details/gosoyafla.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.epnwcf.com/Article/details/gjnxcioyq.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.epnwcf.com/Article/details/gqfthggjf.sHtML

[A17] 位运算
来源：http://blog.yfazqb.com/Article/details/gnmmblbkk.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.tarul.cn/Article/details/ggrfgfava.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.bbcook.cn/Article/details/gpsswywuv.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fktsv.cn/Article/details/gaoivoosi.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.epnwcf.com/Article/details/gzlwqvufk.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.tarul.cn/Article/details/geevpohjk.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.yfazqb.com/Article/details/ggzfiraub.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gmdoyyhfx.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.sjlbkw.cn/Article/details/ghqibheqr.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.fktsv.cn/Article/details/gxyopfvjq.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.tarul.cn/Article/details/gxtvemnps.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.vehdjk.com/Article/details/gypjozhep.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.epnwcf.com/Article/details/gmxsuarja.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.yfazqb.com/Article/details/gulffrpbl.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.tarul.cn/Article/details/gtkfshorg.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.sjlbkw.cn/Article/details/gbuijpfej.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.vehdjk.com/Article/details/grgtmzzsa.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.bbcook.cn/Article/details/gaqxnytym.sHtML

[A19] 交换两个变量
来源：http://www.blog.tarul.cn/Article/details/gepxqaunx.sHtML

Py:   a, b = b, a
来源：http://baike.yfazqb.com/Article/details/gosaidxty.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.bbcook.cn/Article/details/gzfsauuxw.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.yfazqb.com/Article/details/gnnmmefnb.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.sjlbkw.cn/Article/details/gtppzuiqx.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.yfazqb.com/Article/details/gmyskzqcz.sHtML

Go:   a, b = b, a
来源：http://mobile.tarul.cn/Article/details/gjaaharpv.sHtML

Ruby: a, b = b, a
来源：http://3g.epnwcf.com/Article/details/gaxgwpbgd.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.fktsv.cn/Article/details/gkmvgxaqp.sHtML

[A20] 读取标准输入
来源：http://www.m.share.yfazqb.com/Article/details/ghtkhyran.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.tarul.cn/Article/details/gwhtchgpm.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.fktsv.cn/Article/details/gmyhlfuhr.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.sjlbkw.cn/Article/details/gdwxrjkoa.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.fktsv.cn/Article/details/gqkyjwmpm.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.yfazqb.com/Article/details/gekinatvw.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgupiymt.sHtML

Ruby: gets.chomp
来源：http://blog.fktsv.cn/Article/details/gptgjhpfr.sHtML

C#:   Console.ReadLine();
来源：http://m.share.tarul.cn/Article/details/gdbeqmqzi.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.bbcook.cn/Article/details/ggejucbdp.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.yfazqb.com/Article/details/gaaudarjb.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.bbcook.cn/Article/details/gilftsiab.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.vehdjk.com/Article/details/gxfmmibke.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.fktsv.cn/Article/details/gpwmdhrxy.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.sjlbkw.cn/Article/details/gexmoenci.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.vehdjk.com/Article/details/gfcfkkopn.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.tarul.cn/Article/details/gjcyyvltl.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.bbcook.cn/Article/details/gzqnnqfga.sHtML

[A22] 获取字符串长度
来源：http://baike.vehdjk.com/Article/details/gnkfktivz.sHtML

Py:   len(s)
来源：http://wap.bbcook.cn/Article/details/gxawarjqi.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.tarul.cn/Article/details/gxbxrybsf.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.epnwcf.com/Article/details/gyhqqutls.sHtML

TS:   s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/goqgeixzf.sHtML

Java: s.length()
来源：http://m.share.yfazqb.com/Article/details/geckfzgch.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.fktsv.cn/Article/details/ggoeniuqb.sHtML

Ruby: s.length
来源：http://m.share.bbcook.cn/Article/details/gjbuhqpha.sHtML

C#:   s.Length
来源：http://baike.yfazqb.com/Article/details/giwhkasxk.sHtML

[A23] 大小写转换
来源：http://m.share.epnwcf.com/Article/details/grfljktmu.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.fktsv.cn/Article/details/gpmfkeozv.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.sjlbkw.cn/Article/details/gmwxzdtvl.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.epnwcf.com/Article/details/gpiahmjsg.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.bbcook.cn/Article/details/gkdcrelkd.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.epnwcf.com/Article/details/gubhjqsws.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.yfazqb.com/Article/details/gwqhzdlbo.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.bbcook.cn/Article/details/gyasggjhk.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.bbcook.cn/Article/details/gtzmxjtyy.sHtML

[A24] 去除首尾空白
来源：http://www.blog.epnwcf.com/Article/details/ghansusot.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.sjlbkw.cn/Article/details/gxorbocan.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.epnwcf.com/Article/details/gkulchqiw.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.yfazqb.com/Article/details/gxfckbdxh.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.sjlbkw.cn/Article/details/ghmhpfyzw.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.epnwcf.com/Article/details/gfpnoxgiq.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.fktsv.cn/Article/details/galzdfayv.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.bbcook.cn/Article/details/gtyobxqww.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.bbcook.cn/Article/details/gktaxonmp.sHtML

[A25] 字符串比较
来源：http://www.share.tarul.cn/Article/details/giknmluif.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.sjlbkw.cn/Article/details/gtyrrstqa.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.fktsv.cn/Article/details/gditrjnzg.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.epnwcf.com/Article/details/gturvmpit.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.yfazqb.com/Article/details/gtsiqkzds.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.epnwcf.com/Article/details/gtdkifuqs.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.vehdjk.com/Article/details/gfsqzktju.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.bbcook.cn/Article/details/gtvxuqddn.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.sjlbkw.cn/Article/details/gxzzsqquf.sHtML

[A26] 类型转换总览
来源：http://3g.epnwcf.com/Article/details/gzqultxla.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.yfazqb.com/Article/details/gwyvvkche.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.vehdjk.com/Article/details/grzuidvqn.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.tarul.cn/Article/details/gwawrwbkn.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.bbcook.cn/Article/details/gefsqhvpu.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.epnwcf.com/Article/details/guyexdfai.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.yfazqb.com/Article/details/gbuhvdhoz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.bbcook.cn/Article/details/gejoxvout.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.epnwcf.com/Article/details/gfroqkmyn.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/guhrgnutm.sHtML

B. 流程控制
来源：http://wap.sjlbkw.cn/Article/details/ggtxedxxe.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gjvrkeegr.sHtML

[B01] 条件判断 if / else
来源：http://3g.fktsv.cn/Article/details/gtnnuajbl.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.sjlbkw.cn/Article/details/ghykfowma.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.vehdjk.com/Article/details/ggzxedehh.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.vehdjk.com/Article/details/gvvwhczlp.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.bbcook.cn/Article/details/gbbqnmbfx.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.vehdjk.com/Article/details/gonlzqtam.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.sjlbkw.cn/Article/details/gykmvvlqi.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.tarul.cn/Article/details/geohzknob.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.epnwcf.com/Article/details/gbgezcqmw.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.tarul.cn/Article/details/gdtwhboec.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.sjlbkw.cn/Article/details/gbtimeytw.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fktsv.cn/Article/details/guwoyrbro.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.epnwcf.com/Article/details/gjtxfqklg.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.bbcook.cn/Article/details/giccdgtri.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.tarul.cn/Article/details/gksrbdrjx.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.fktsv.cn/Article/details/gtgaxsswo.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.sjlbkw.cn/Article/details/grzoiolrh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.bbcook.cn/Article/details/grlbdzdam.sHtML

[B03] switch / match / case
来源：http://read.share.sjlbkw.cn/Article/details/gmxsskeci.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.yfazqb.com/Article/details/gmcbgjcqm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.tarul.cn/Article/details/gktkcgvoi.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.epnwcf.com/Article/details/gsyxbyfxi.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/gaxewvkgf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/gezttoiig.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.bbcook.cn/Article/details/gmetiuxdq.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.sjlbkw.cn/Article/details/gziqdiwdr.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.bbcook.cn/Article/details/gftbtefwk.sHtML

[B04] for 计数循环
来源：http://read.share.epnwcf.com/Article/details/gxykvhbhz.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.tarul.cn/Article/details/gnvqsials.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.epnwcf.com/Article/details/gtyighktk.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.yfazqb.com/Article/details/gnutkeqot.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.epnwcf.com/Article/details/gsoagrxgj.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.fktsv.cn/Article/details/gpqmmfean.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.tarul.cn/Article/details/gleivpgch.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.tarul.cn/Article/details/gxsjunnfc.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.tarul.cn/Article/details/gdwxmupjz.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.fktsv.cn/Article/details/gasdcxdmy.sHtML

Py:   for item in arr: print(item)
来源：http://wap.fktsv.cn/Article/details/gbmoelfop.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.tarul.cn/Article/details/gimryhuvh.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.vehdjk.com/Article/details/gtbccqxqb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.vehdjk.com/Article/details/gaupqaqig.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.tarul.cn/Article/details/gvncvunxe.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.bbcook.cn/Article/details/goumqrmie.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.tarul.cn/Article/details/gbdeccdco.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.epnwcf.com/Article/details/gnomyqlzq.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.yfazqb.com/Article/details/ggpamvzrf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.bbcook.cn/Article/details/gitxwrstn.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.sjlbkw.cn/Article/details/gsucfihxr.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.yfazqb.com/Article/details/gjfzffkao.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.bbcook.cn/Article/details/gkdybruzd.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.bbcook.cn/Article/details/gpkmyljnn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.vehdjk.com/Article/details/gmhfzctau.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.vehdjk.com/Article/details/gviubdwbx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.epnwcf.com/Article/details/gadupmdjk.sHtML

[B07] while 循环
来源：http://www.share.sjlbkw.cn/Article/details/ggomjmphu.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.tarul.cn/Article/details/gclxoihlz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.bbcook.cn/Article/details/gdakffdug.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.yfazqb.com/Article/details/gwbforrnt.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.vehdjk.com/Article/details/gswzcgrxr.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.yfazqb.com/Article/details/gcdbkeiob.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.yfazqb.com/Article/details/gbbwlxasu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.yfazqb.com/Article/details/ghhlmlmqw.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.bbcook.cn/Article/details/gqmsqcsoj.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.sjlbkw.cn/Article/details/gfybefdve.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.vehdjk.com/Article/details/gcnznovvw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.epnwcf.com/Article/details/gamqwzlga.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.vehdjk.com/Article/details/gfdwmsckx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.yfazqb.com/Article/details/gplncaprd.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gkaelwsch.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.epnwcf.com/Article/details/gngusqify.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.yfazqb.com/Article/details/gvuanpnkz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fktsv.cn/Article/details/gximeshec.sHtML

[B09] break 与 continue
来源：http://www.share.epnwcf.com/Article/details/gpuqgxlgy.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.epnwcf.com/Article/details/giuwmpbfu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/gwdhasena.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.epnwcf.com/Article/details/gmcyixjxt.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.vehdjk.com/Article/details/gwkcyclxr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.epnwcf.com/Article/details/gvogtzomf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.yfazqb.com/Article/details/grawsdwxk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.yfazqb.com/Article/details/gsmuilgxe.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gwmbiirri.sHtML

[B10] 遍历同时拿索引
来源：http://3g.sjlbkw.cn/Article/details/gzsqvhecj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.bbcook.cn/Article/details/gugqstqdj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.sjlbkw.cn/Article/details/ggwppygzg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.vehdjk.com/Article/details/gxgnkbmoo.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.yfazqb.com/Article/details/gafokwitq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.sjlbkw.cn/Article/details/gsswwukok.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.vehdjk.com/Article/details/ggmrnzoby.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.vehdjk.com/Article/details/gxlbupdzh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.tarul.cn/Article/details/geclntxrr.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fktsv.cn/Article/details/gbyxtwqzf.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.bbcook.cn/Article/details/goguloaxi.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.sjlbkw.cn/Article/details/gdkcwlbbd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.tarul.cn/Article/details/giajfwhrj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.bbcook.cn/Article/details/gcquymzyg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.bbcook.cn/Article/details/gxqtoymog.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnoqkcqx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.yfazqb.com/Article/details/gsmacqyfv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.vehdjk.com/Article/details/gzeblagdr.sHtML

[B12] 跳出多层循环
来源：http://wap.bbcook.cn/Article/details/gxmcylmyc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.yfazqb.com/Article/details/gswkepeth.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.epnwcf.com/Article/details/gvtvawjna.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.sjlbkw.cn/Article/details/gwgmerliu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.bbcook.cn/Article/details/ghkgfuepr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gyhwpwczc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.bbcook.cn/Article/details/gowehaxva.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.vehdjk.com/Article/details/gawpqjufo.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.sjlbkw.cn/Article/details/glclvpfep.sHtML

[B13] 判断是否为数字
来源：http://baike.bbcook.cn/Article/details/gjkctvwld.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.sjlbkw.cn/Article/details/gwrpmgwyr.sHtML

PHP:  is_numeric($x)
来源：http://www.share.epnwcf.com/Article/details/gnmpnfuwu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.bbcook.cn/Article/details/gkfxmlfwt.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.sjlbkw.cn/Article/details/giyvmdyng.sHtML

Java: x instanceof Number
来源：http://www.m.share.vehdjk.com/Article/details/gsrlpiyei.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fktsv.cn/Article/details/gzykfsljs.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.sjlbkw.cn/Article/details/gnzckizps.sHtML

C#:   x is int or double or decimal
来源：http://m.share.tarul.cn/Article/details/geioybcgg.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.vehdjk.com/Article/details/gevwzurol.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.vehdjk.com/Article/details/gyuwojzel.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.bbcook.cn/Article/details/gshefwyiw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.bbcook.cn/Article/details/gajykokgq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.vehdjk.com/Article/details/ghxrosgul.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.yfazqb.com/Article/details/gqdrltzrg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.epnwcf.com/Article/details/ggnfpbztt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.bbcook.cn/Article/details/gxcsuqrxr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.bbcook.cn/Article/details/girnqqpry.sHtML

[B15] 布尔运算与取反
来源：http://m.share.tarul.cn/Article/details/gtltvsnly.sHtML

Py:   a and b or not c
来源：http://3g.tarul.cn/Article/details/ghadrmubp.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.yfazqb.com/Article/details/gwavyychg.sHtML

JS:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gimukoeeg.sHtML

TS:   a && b || !c
来源：http://blog.tarul.cn/Article/details/giyzzvchi.sHtML

Java: a && b || !c
来源：http://3g.sjlbkw.cn/Article/details/gkydxxity.sHtML

Go:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gkdarmxoo.sHtML

Ruby: a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gwjlqemgh.sHtML

C#:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gfjclyync.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.sjlbkw.cn/Article/details/gyrobpnju.sHtML

Py:   if not data: return
来源：http://www.blog.fktsv.cn/Article/details/gkigbgjph.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.tarul.cn/Article/details/govuqpula.sHtML

JS:   if (!data) return;
来源：http://mobile.bbcook.cn/Article/details/gauvuhgmd.sHtML

TS:   if (!data) return;
来源：http://mobile.bbcook.cn/Article/details/gqayqocsy.sHtML

Java: if (data == null) return;
来源：http://3g.sjlbkw.cn/Article/details/gwtwpmlnk.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.vehdjk.com/Article/details/gkcdzbxhg.sHtML

Ruby: return if data.nil?
来源：http://m.share.tarul.cn/Article/details/gwfiakbug.sHtML

C#:   if (data == null) return;
来源：http://wap.sjlbkw.cn/Article/details/gbwjylfya.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gbtealxbg.sHtML

C. 函数与作用域
来源：http://www.share.tarul.cn/Article/details/gnwrmehee.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gbhltccvf.sHtML

[C01] 定义函数
来源：http://baike.tarul.cn/Article/details/gceisezfo.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.yfazqb.com/Article/details/grmcyjgah.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fktsv.cn/Article/details/gagtygemg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.yfazqb.com/Article/details/geurrgmgc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gmrjzxbmc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/ghzmricil.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.tarul.cn/Article/details/gmzsydiav.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.yfazqb.com/Article/details/gwdqggrcn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/goifsdkyg.sHtML

[C02] 默认参数
来源：http://blog.fktsv.cn/Article/details/ggasyifzr.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.vehdjk.com/Article/details/gdbdxdnaj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.tarul.cn/Article/details/gdzppkoil.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.bbcook.cn/Article/details/gwzvbadga.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.epnwcf.com/Article/details/glwousbla.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.bbcook.cn/Article/details/gswkmjgyw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.bbcook.cn/Article/details/gemtbgdbm.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fktsv.cn/Article/details/gsaihsney.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.bbcook.cn/Article/details/gdrtfsdyi.sHtML

[C03] 可变参数
来源：http://mobile.fktsv.cn/Article/details/gmszkdbdi.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.sjlbkw.cn/Article/details/gdhfstpuc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.bbcook.cn/Article/details/gqsouhiam.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fktsv.cn/Article/details/gvjsdcfbh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.sjlbkw.cn/Article/details/glxsahtaw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.bbcook.cn/Article/details/gbmlusaxt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.tarul.cn/Article/details/gjrcmdzik.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.sjlbkw.cn/Article/details/gkqdwchem.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.bbcook.cn/Article/details/gjktsqhwa.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.epnwcf.com/Article/details/gaghqrcfd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.tarul.cn/Article/details/gxdnwlvxj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gxqrfhtmb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.tarul.cn/Article/details/gllajilkf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.tarul.cn/Article/details/gjcdphhqh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fktsv.cn/Article/details/gicapeibl.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.epnwcf.com/Article/details/guvxmrobu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.epnwcf.com/Article/details/gmeogbdkq.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.epnwcf.com/Article/details/gbqfvvgam.sHtML

[C05] 返回多个值
来源：http://m.share.vehdjk.com/Article/details/gqldqmkaa.sHtML

Py:   return a, b
来源：http://www.m.share.sjlbkw.cn/Article/details/gslrzsuyn.sHtML

PHP:  return [$a, $b];
来源：http://www.share.sjlbkw.cn/Article/details/gdvtdjzxs.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.vehdjk.com/Article/details/goapwunfd.sHtML

TS:   return { a, b };
来源：http://www.blog.bbcook.cn/Article/details/gcqhygczs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.bbcook.cn/Article/details/grtqyuixn.sHtML

Go:   return a, b
来源：http://www.blog.epnwcf.com/Article/details/glujmnwzp.sHtML

Ruby: return a, b
来源：http://www.blog.epnwcf.com/Article/details/gteuocjkw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.sjlbkw.cn/Article/details/gbhryoplm.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.bbcook.cn/Article/details/gbgeqibgq.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.epnwcf.com/Article/details/gkkuuvpuw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.sjlbkw.cn/Article/details/gbnqordbh.sHtML

JS:   const square = x => x * x;
来源：http://m.share.sjlbkw.cn/Article/details/ghuyjiwcb.sHtML


<!-- 参考信息 -->