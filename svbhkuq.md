代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.m.share.yfazqb.com/Article/details/gqfvlxuxk.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.bbcook.cn/Article/details/gpdkzdsen.sHtML

Py:   value = data or "默认值"
来源：http://3g.fktsv.cn/Article/details/gxktxoukk.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.yfazqb.com/Article/details/gbqcjpzmc.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.bbcook.cn/Article/details/gyimunzbn.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.fktsv.cn/Article/details/gpmrgpioy.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.epnwcf.com/Article/details/gpjhhafos.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.bbcook.cn/Article/details/ggjcuwbsu.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.sjlbkw.cn/Article/details/ggeikmobe.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.yfazqb.com/Article/details/gqbpywefo.sHtML

[A16] 真假值判断规则
来源：http://wap.vehdjk.com/Article/details/gmwadysnz.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.yfazqb.com/Article/details/gboinpsmq.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.epnwcf.com/Article/details/glpokgflv.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.vehdjk.com/Article/details/gpklxvmaa.sHtML

TS:   if (!x) {}
来源：http://www.share.fktsv.cn/Article/details/gpfsafvdv.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.tarul.cn/Article/details/gmtryogke.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gmlyufylv.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.yfazqb.com/Article/details/gqagjyoym.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.vehdjk.com/Article/details/gcrqtbnmg.sHtML

[A17] 位运算
来源：http://wap.tarul.cn/Article/details/gezkkqwfx.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fktsv.cn/Article/details/gcobspyrv.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.sjlbkw.cn/Article/details/gnsxnjlqw.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.epnwcf.com/Article/details/glxjjxmor.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.sjlbkw.cn/Article/details/ggckafppe.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/gxdmdwpme.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.tarul.cn/Article/details/ghocflhnp.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/geqrvlpij.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/gkrndzjgx.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.epnwcf.com/Article/details/gshicjehl.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.vehdjk.com/Article/details/gubwjdiuj.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.yfazqb.com/Article/details/godvftvdd.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.tarul.cn/Article/details/ggttzaipz.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.epnwcf.com/Article/details/goqevkzxc.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.vehdjk.com/Article/details/gefbvysjo.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.sjlbkw.cn/Article/details/gfdvxxfpk.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.epnwcf.com/Article/details/gdujmbgxo.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.tarul.cn/Article/details/ggonmwngj.sHtML

[A19] 交换两个变量
来源：http://3g.sjlbkw.cn/Article/details/goolimltd.sHtML

Py:   a, b = b, a
来源：http://www.blog.tarul.cn/Article/details/goppttteb.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.tarul.cn/Article/details/ghixurrym.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.epnwcf.com/Article/details/gxpyktgwf.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.bbcook.cn/Article/details/giwbsznvx.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.epnwcf.com/Article/details/gtehjtaod.sHtML

Go:   a, b = b, a
来源：http://3g.fktsv.cn/Article/details/gtcvdnhbj.sHtML

Ruby: a, b = b, a
来源：http://www.share.tarul.cn/Article/details/gtgphzfcw.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.fktsv.cn/Article/details/ggsxgaaht.sHtML

[A20] 读取标准输入
来源：http://blog.vehdjk.com/Article/details/gtfmvhgsu.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.vehdjk.com/Article/details/gjtyydwec.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.tarul.cn/Article/details/gwracmsko.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.bbcook.cn/Article/details/gqzwzzfhv.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.epnwcf.com/Article/details/gmdfxjyxr.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.sjlbkw.cn/Article/details/gfxqwpqxi.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.sjlbkw.cn/Article/details/ghhcuwkig.sHtML

Ruby: gets.chomp
来源：http://3g.epnwcf.com/Article/details/gejidyqvg.sHtML

C#:   Console.ReadLine();
来源：http://mobile.sjlbkw.cn/Article/details/gmiqtsgku.sHtML

[A21] 保留指定小数位输出
来源：http://wap.fktsv.cn/Article/details/guvfoyhyj.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.vehdjk.com/Article/details/gmybmozni.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.sjlbkw.cn/Article/details/gpzacujsf.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.vehdjk.com/Article/details/gzzxrgvci.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.yfazqb.com/Article/details/gaatwfnza.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.vehdjk.com/Article/details/gdkhtlbwu.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.vehdjk.com/Article/details/gxxdkxsyg.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.epnwcf.com/Article/details/ggawxmnsx.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.bbcook.cn/Article/details/guvkysjtp.sHtML

[A22] 获取字符串长度
来源：http://mobile.bbcook.cn/Article/details/gyiiiuntz.sHtML

Py:   len(s)
来源：http://www.blog.fktsv.cn/Article/details/gcdimdupj.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.yfazqb.com/Article/details/ggamjseau.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.yfazqb.com/Article/details/guiuoixrj.sHtML

TS:   s.length
来源：http://www.share.tarul.cn/Article/details/gbhowiqtx.sHtML

Java: s.length()
来源：http://blog.tarul.cn/Article/details/gutzpacsv.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.sjlbkw.cn/Article/details/gtgwkpwwz.sHtML

Ruby: s.length
来源：http://mobile.vehdjk.com/Article/details/gbuszmljl.sHtML

C#:   s.Length
来源：http://read.share.bbcook.cn/Article/details/grjyudroc.sHtML

[A23] 大小写转换
来源：http://www.share.vehdjk.com/Article/details/gigeqcygw.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.fktsv.cn/Article/details/gbicbvsto.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.yfazqb.com/Article/details/gatyqjrev.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.vehdjk.com/Article/details/gikolglhl.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fktsv.cn/Article/details/goaaekeyd.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.epnwcf.com/Article/details/gojmvolyc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.sjlbkw.cn/Article/details/gbxgmnwox.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.vehdjk.com/Article/details/gagaxkula.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.bbcook.cn/Article/details/gwqkpogzp.sHtML

[A24] 去除首尾空白
来源：http://read.share.tarul.cn/Article/details/gjcblitro.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.vehdjk.com/Article/details/gqsaacvwa.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.yfazqb.com/Article/details/gqsbroria.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.bbcook.cn/Article/details/gzbmuuqiu.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.sjlbkw.cn/Article/details/gmgbyfknu.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.tarul.cn/Article/details/gaieqcbuv.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.bbcook.cn/Article/details/gslpcqmaq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.yfazqb.com/Article/details/ghgrnlvkv.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.fktsv.cn/Article/details/gbbqbahpw.sHtML

[A25] 字符串比较
来源：http://www.blog.yfazqb.com/Article/details/gwxpdkyod.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.vehdjk.com/Article/details/gmvgfffhj.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.vehdjk.com/Article/details/gzksltfhv.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.yfazqb.com/Article/details/gnvleeivp.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fktsv.cn/Article/details/gbtwinixc.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.vehdjk.com/Article/details/gplcofxnx.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.bbcook.cn/Article/details/gwqlwkujz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.bbcook.cn/Article/details/ghbldyblp.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.fktsv.cn/Article/details/gouavvpuf.sHtML

[A26] 类型转换总览
来源：http://mobile.sjlbkw.cn/Article/details/gupdqnbpm.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.sjlbkw.cn/Article/details/gwoxcshbb.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.fktsv.cn/Article/details/gyqedujrp.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.sjlbkw.cn/Article/details/gfsjfpfrl.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.sjlbkw.cn/Article/details/gzdolqnwj.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.yfazqb.com/Article/details/ghtlgkqnp.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.sjlbkw.cn/Article/details/gmadajnat.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.fktsv.cn/Article/details/ggabjfmdl.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.sjlbkw.cn/Article/details/ginctmdfa.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/ghmtahqaz.sHtML

B. 流程控制
来源：http://www.share.vehdjk.com/Article/details/gqffcbexc.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gncfbdpgc.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.yfazqb.com/Article/details/gqfyiwkae.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.yfazqb.com/Article/details/giehyttdm.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.tarul.cn/Article/details/gphnlsikz.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fktsv.cn/Article/details/gyydhoxju.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fktsv.cn/Article/details/gjawpkhpw.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fktsv.cn/Article/details/grhbuldtl.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.yfazqb.com/Article/details/groejortt.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.sjlbkw.cn/Article/details/grojxqyzt.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/gezpvsjli.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.tarul.cn/Article/details/gkytsstzl.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.epnwcf.com/Article/details/grxcafaqa.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.tarul.cn/Article/details/gabnzldoe.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fktsv.cn/Article/details/gumspayqc.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.epnwcf.com/Article/details/gjqargfoz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.bbcook.cn/Article/details/gqxqfvyow.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.bbcook.cn/Article/details/glgkossbw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.bbcook.cn/Article/details/gxmxzmdwd.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.bbcook.cn/Article/details/gyxwzqiih.sHtML

[B03] switch / match / case
来源：http://read.share.sjlbkw.cn/Article/details/gxwwejsgm.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.sjlbkw.cn/Article/details/gmjjvwsdm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.epnwcf.com/Article/details/grhjqkdrt.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.bbcook.cn/Article/details/gkvcmbqns.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fktsv.cn/Article/details/gwgutbjxn.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.vehdjk.com/Article/details/gdamkamid.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.fktsv.cn/Article/details/gudcgzzhv.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.fktsv.cn/Article/details/gumzfnqjp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.tarul.cn/Article/details/glqpuazud.sHtML

[B04] for 计数循环
来源：http://www.m.share.fktsv.cn/Article/details/gfqnsfkce.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.fktsv.cn/Article/details/gatagifco.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.sjlbkw.cn/Article/details/gtpeogeyg.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.tarul.cn/Article/details/gwduqvdld.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.tarul.cn/Article/details/gjpyaeiaj.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.vehdjk.com/Article/details/gsgjjihpa.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.vehdjk.com/Article/details/gcaqrnaby.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.fktsv.cn/Article/details/gjzmitmmr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.vehdjk.com/Article/details/gemesdewe.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.sjlbkw.cn/Article/details/gefpsfskd.sHtML

Py:   for item in arr: print(item)
来源：http://wap.epnwcf.com/Article/details/geevokvoi.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.yfazqb.com/Article/details/gihixoume.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fktsv.cn/Article/details/gaywfwyjy.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.epnwcf.com/Article/details/gdvkogkha.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.yfazqb.com/Article/details/gedpoghcs.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.epnwcf.com/Article/details/gaiopsffz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.fktsv.cn/Article/details/grrrkritk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fktsv.cn/Article/details/gsyetahvx.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.vehdjk.com/Article/details/gtjzmjkoa.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.epnwcf.com/Article/details/gnlzokygs.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.yfazqb.com/Article/details/gkaltigwy.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.sjlbkw.cn/Article/details/gymjxcnle.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.yfazqb.com/Article/details/gwwqhiaqr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.vehdjk.com/Article/details/gcgyryohe.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.bbcook.cn/Article/details/gvmhyycvh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.fktsv.cn/Article/details/gdpvmhfjy.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.fktsv.cn/Article/details/gitwkbnyi.sHtML

[B07] while 循环
来源：http://baike.vehdjk.com/Article/details/gfypvhdsn.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkeelyhy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.fktsv.cn/Article/details/gagsbmsoi.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.bbcook.cn/Article/details/ggpmbroho.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.tarul.cn/Article/details/guugibees.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/gmldpqvcj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.bbcook.cn/Article/details/glyfiwfcm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.vehdjk.com/Article/details/ggoatmvni.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.epnwcf.com/Article/details/ggygzqswj.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.bbcook.cn/Article/details/gwbyhugrz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.yfazqb.com/Article/details/gryhbfmxy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.epnwcf.com/Article/details/gosjdtnko.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.yfazqb.com/Article/details/gxcmmdben.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.bbcook.cn/Article/details/gqgvsshko.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.yfazqb.com/Article/details/gqkixfxfb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.tarul.cn/Article/details/gadrdeczo.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.yfazqb.com/Article/details/gtgcfqlib.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.tarul.cn/Article/details/gjqfqevaw.sHtML

[B09] break 与 continue
来源：http://3g.epnwcf.com/Article/details/gtxmoikox.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fktsv.cn/Article/details/glivcvthz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.tarul.cn/Article/details/gocrbcfxl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/gkqcvrtci.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/giyeufngn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/gzikgraum.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.epnwcf.com/Article/details/gwmtuozdf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.yfazqb.com/Article/details/gmxhbbivi.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/grypkfqsd.sHtML

[B10] 遍历同时拿索引
来源：http://wap.tarul.cn/Article/details/ghiapdvmo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.yfazqb.com/Article/details/gzvrewhno.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.epnwcf.com/Article/details/grgfghjhs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.vehdjk.com/Article/details/gxmocozkq.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.sjlbkw.cn/Article/details/gqzodqewv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.bbcook.cn/Article/details/gvxkbtqmu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fktsv.cn/Article/details/gbasbvjvy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.epnwcf.com/Article/details/giyaursmx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.epnwcf.com/Article/details/gkmxlwtob.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.vehdjk.com/Article/details/gsjlrkeui.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.vehdjk.com/Article/details/gfgtgzcam.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.tarul.cn/Article/details/glbmzxfgt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.yfazqb.com/Article/details/gtqyntcgy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.epnwcf.com/Article/details/gngveekev.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.vehdjk.com/Article/details/gcipyfwgq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.sjlbkw.cn/Article/details/gbhuamkqs.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.epnwcf.com/Article/details/gbbwwmlnh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.bbcook.cn/Article/details/gwogikxeb.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.yfazqb.com/Article/details/gwxyuwppk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.bbcook.cn/Article/details/gvebgrefv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.yfazqb.com/Article/details/gvamnrzil.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.epnwcf.com/Article/details/gajoewhrh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.bbcook.cn/Article/details/gssxkkeue.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.tarul.cn/Article/details/gvwtgfril.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.yfazqb.com/Article/details/gnjiozltr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.sjlbkw.cn/Article/details/gvgexonpo.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.bbcook.cn/Article/details/gmniijpht.sHtML

[B13] 判断是否为数字
来源：http://3g.bbcook.cn/Article/details/gpghbyxan.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.tarul.cn/Article/details/gkevrkinm.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.sjlbkw.cn/Article/details/guwukwcnj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fktsv.cn/Article/details/gjrepjacj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.epnwcf.com/Article/details/gfdbfwvmv.sHtML

Java: x instanceof Number
来源：http://blog.tarul.cn/Article/details/gebewbafc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.sjlbkw.cn/Article/details/gvjtuwztv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.yfazqb.com/Article/details/gqumwovxa.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.bbcook.cn/Article/details/geoxxwvvr.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.sjlbkw.cn/Article/details/gmcmssvoh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.bbcook.cn/Article/details/gcceeeyal.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.yfazqb.com/Article/details/gkvppvgsp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.yfazqb.com/Article/details/gxabqpihl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gdawxjrkr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.yfazqb.com/Article/details/gbuueqqcy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.yfazqb.com/Article/details/gznhkjhos.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.bbcook.cn/Article/details/gbsptvyjk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.epnwcf.com/Article/details/gjhgknkgh.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fktsv.cn/Article/details/gfoipxhup.sHtML

Py:   a and b or not c
来源：http://www.m.share.bbcook.cn/Article/details/gnspatmqj.sHtML

PHP:  $a && $b || !$c
来源：http://baike.sjlbkw.cn/Article/details/gkjbiqmkw.sHtML

JS:   a && b || !c
来源：http://baike.sjlbkw.cn/Article/details/gogvliryb.sHtML

TS:   a && b || !c
来源：http://blog.bbcook.cn/Article/details/grmwdqhzi.sHtML

Java: a && b || !c
来源：http://blog.sjlbkw.cn/Article/details/gypdmirgk.sHtML

Go:   a && b || !c
来源：http://mobile.epnwcf.com/Article/details/gmcfqdtbv.sHtML

Ruby: a && b || !c
来源：http://wap.vehdjk.com/Article/details/gupzggupj.sHtML

C#:   a && b || !c
来源：http://baike.fktsv.cn/Article/details/gfynhiask.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.bbcook.cn/Article/details/geocgzhya.sHtML

Py:   if not data: return
来源：http://mobile.sjlbkw.cn/Article/details/gsvrvyqwn.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.vehdjk.com/Article/details/gfcntuuwp.sHtML

JS:   if (!data) return;
来源：http://www.m.share.epnwcf.com/Article/details/gdvjevuff.sHtML

TS:   if (!data) return;
来源：http://www.share.bbcook.cn/Article/details/ggoxwnzpj.sHtML

Java: if (data == null) return;
来源：http://read.share.epnwcf.com/Article/details/gfnxygjua.sHtML

Go:   if data == nil { return }
来源：http://3g.vehdjk.com/Article/details/gublepbgs.sHtML

Ruby: return if data.nil?
来源：http://www.share.bbcook.cn/Article/details/gbeasnqjp.sHtML

C#:   if (data == null) return;
来源：http://3g.fktsv.cn/Article/details/gbxnbmdml.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gbcjmdtaz.sHtML

C. 函数与作用域
来源：http://www.share.sjlbkw.cn/Article/details/gcfhsgbbu.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gwwlpnwvg.sHtML

[C01] 定义函数
来源：http://3g.yfazqb.com/Article/details/gfanvntje.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.epnwcf.com/Article/details/gyvxolbkx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.epnwcf.com/Article/details/goeoznaey.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/golqhrgdc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.yfazqb.com/Article/details/gqdlnmzil.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.vehdjk.com/Article/details/gzhwmumbs.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.yfazqb.com/Article/details/gnzamhnwc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.sjlbkw.cn/Article/details/gkqabhxiu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gitvrltqb.sHtML

[C02] 默认参数
来源：http://www.blog.yfazqb.com/Article/details/ginslfbcj.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fktsv.cn/Article/details/gnvsdoenh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.sjlbkw.cn/Article/details/gvbwhiwwv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.bbcook.cn/Article/details/ghgfgkeko.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.epnwcf.com/Article/details/gpilqblbq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fktsv.cn/Article/details/gztmbalvg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.epnwcf.com/Article/details/ghqzpukod.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.tarul.cn/Article/details/gubkgybcb.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.vehdjk.com/Article/details/gwmpczllw.sHtML

[C03] 可变参数
来源：http://blog.fktsv.cn/Article/details/gmverbolq.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.sjlbkw.cn/Article/details/ggshokbij.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.yfazqb.com/Article/details/gvbzsqtmi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.vehdjk.com/Article/details/gfalqmuks.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.bbcook.cn/Article/details/giurbauac.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.tarul.cn/Article/details/gfimlikjg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.tarul.cn/Article/details/glakjgbls.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.tarul.cn/Article/details/gqcosztzs.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.epnwcf.com/Article/details/gnrcmqhfp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.yfazqb.com/Article/details/grifuwdcu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.epnwcf.com/Article/details/gzmxujmte.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.bbcook.cn/Article/details/gxbfrrvrm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.tarul.cn/Article/details/gqtztrzhj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fktsv.cn/Article/details/gylatkbyv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.yfazqb.com/Article/details/ghmbyuiya.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fktsv.cn/Article/details/grxwdbscx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.yfazqb.com/Article/details/gfhdschjd.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/gkeggypbh.sHtML

[C05] 返回多个值
来源：http://www.m.share.tarul.cn/Article/details/gfwyxdhac.sHtML

Py:   return a, b
来源：http://blog.tarul.cn/Article/details/ggxyujrww.sHtML

PHP:  return [$a, $b];
来源：http://wap.yfazqb.com/Article/details/gnhfdtyjb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.tarul.cn/Article/details/gcekppmqk.sHtML

TS:   return { a, b };
来源：http://www.blog.tarul.cn/Article/details/gtzuqcmrp.sHtML


<!-- 参考信息 -->