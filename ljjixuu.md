代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://mobile.vehdjk.com/Article/details/gsgjeigta.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.fktsv.cn/Article/details/gebqlozwh.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.sjlbkw.cn/Article/details/gzunemetj.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.sjlbkw.cn/Article/details/gshyekkvf.sHtML

Ruby: value = data || "默认值"
来源：http://blog.epnwcf.com/Article/details/gojyazkwx.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.epnwcf.com/Article/details/gkyjtsiok.sHtML

[A16] 真假值判断规则
来源：http://m.share.bbcook.cn/Article/details/ghqyksrhh.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.yfazqb.com/Article/details/ggkrxihny.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.sjlbkw.cn/Article/details/gfrduwjep.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.tarul.cn/Article/details/ggcyjbjet.sHtML

TS:   if (!x) {}
来源：http://m.share.fktsv.cn/Article/details/gdidytsoe.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.bbcook.cn/Article/details/gxiyflmwg.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.vehdjk.com/Article/details/grsyhiwqz.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.epnwcf.com/Article/details/gzguqslai.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.tarul.cn/Article/details/gnfkyqxbw.sHtML

[A17] 位运算
来源：http://www.blog.bbcook.cn/Article/details/gjpeqiugj.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fktsv.cn/Article/details/glxenargt.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.epnwcf.com/Article/details/ggkcboyei.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.tarul.cn/Article/details/guivjqbmi.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.bbcook.cn/Article/details/gxqikripz.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.epnwcf.com/Article/details/gxkxubnra.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.fktsv.cn/Article/details/gvsabqwkh.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fktsv.cn/Article/details/gbrcxnhhw.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.bbcook.cn/Article/details/gaduhtchs.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.fktsv.cn/Article/details/gbammouxo.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.epnwcf.com/Article/details/gzdjfnxiz.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.epnwcf.com/Article/details/gtdvjnkhq.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.bbcook.cn/Article/details/gsufwuiep.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.bbcook.cn/Article/details/gmoljciho.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.vehdjk.com/Article/details/gkgptylna.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.sjlbkw.cn/Article/details/gsizwlalb.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.epnwcf.com/Article/details/gswncvwui.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.fktsv.cn/Article/details/gpgobucfp.sHtML

[A19] 交换两个变量
来源：http://wap.sjlbkw.cn/Article/details/gzvdtxzyx.sHtML

Py:   a, b = b, a
来源：http://wap.bbcook.cn/Article/details/gcikpurbv.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.fktsv.cn/Article/details/gzjkrcsij.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.sjlbkw.cn/Article/details/gcffxrxyx.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.bbcook.cn/Article/details/gkmlxibxf.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.bbcook.cn/Article/details/gtygjgvcm.sHtML

Go:   a, b = b, a
来源：http://3g.yfazqb.com/Article/details/gvrddtuib.sHtML

Ruby: a, b = b, a
来源：http://m.share.sjlbkw.cn/Article/details/gjssmotqe.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.fktsv.cn/Article/details/gfsjoparl.sHtML

[A20] 读取标准输入
来源：http://www.blog.bbcook.cn/Article/details/gicavnpnf.sHtML

Py:   name = input("请输入：")
来源：http://read.share.sjlbkw.cn/Article/details/gnchcdrvk.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.sjlbkw.cn/Article/details/gxahwlfct.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.bbcook.cn/Article/details/gigcdager.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.fktsv.cn/Article/details/gmmfheyzc.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.vehdjk.com/Article/details/gnimfeqvh.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.yfazqb.com/Article/details/gfzmhsbag.sHtML

Ruby: gets.chomp
来源：http://wap.tarul.cn/Article/details/gazixqpab.sHtML

C#:   Console.ReadLine();
来源：http://www.share.bbcook.cn/Article/details/geevfsryy.sHtML

[A21] 保留指定小数位输出
来源：http://3g.fktsv.cn/Article/details/gflfbqgmw.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.sjlbkw.cn/Article/details/grrezefsy.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.epnwcf.com/Article/details/gjsablyfj.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.fktsv.cn/Article/details/gnuaybwhg.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.tarul.cn/Article/details/ggflyofgs.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.vehdjk.com/Article/details/gvvkijcpb.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.tarul.cn/Article/details/gdxfcgsbs.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.tarul.cn/Article/details/geboadtps.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.bbcook.cn/Article/details/gsmouvqpo.sHtML

[A22] 获取字符串长度
来源：http://3g.bbcook.cn/Article/details/gmvuxzlzg.sHtML

Py:   len(s)
来源：http://baike.yfazqb.com/Article/details/gywpligaq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.epnwcf.com/Article/details/gjmbjrarm.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.yfazqb.com/Article/details/gvctjucxw.sHtML

TS:   s.length
来源：http://www.blog.tarul.cn/Article/details/gtmxoncvx.sHtML

Java: s.length()
来源：http://read.share.vehdjk.com/Article/details/glujrgjzu.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.fktsv.cn/Article/details/gcasznhyj.sHtML

Ruby: s.length
来源：http://www.m.share.epnwcf.com/Article/details/gwzjetzcw.sHtML

C#:   s.Length
来源：http://3g.fktsv.cn/Article/details/gyonqosbh.sHtML

[A23] 大小写转换
来源：http://3g.yfazqb.com/Article/details/gkbqdfvur.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.yfazqb.com/Article/details/gklexrrqb.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.fktsv.cn/Article/details/gssrgrvpn.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.yfazqb.com/Article/details/gigkdiyky.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.epnwcf.com/Article/details/gflslihpn.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.epnwcf.com/Article/details/gvjxmmzzc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.tarul.cn/Article/details/gxzoqjjrt.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.tarul.cn/Article/details/gjtrythgx.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.sjlbkw.cn/Article/details/goofobxvw.sHtML

[A24] 去除首尾空白
来源：http://mobile.fktsv.cn/Article/details/ghgsfoqth.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.yfazqb.com/Article/details/gnacvtxeo.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.yfazqb.com/Article/details/gaebuoozj.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.tarul.cn/Article/details/ghwikezvy.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.sjlbkw.cn/Article/details/gruvwjjnc.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.epnwcf.com/Article/details/gubktsbwa.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/guanvaqld.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.yfazqb.com/Article/details/gksurwapg.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.yfazqb.com/Article/details/gdhbszocl.sHtML

[A25] 字符串比较
来源：http://m.share.epnwcf.com/Article/details/gzuujwjhn.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.tarul.cn/Article/details/graeipcci.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.bbcook.cn/Article/details/gbaudyfrt.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fktsv.cn/Article/details/gkqekaegr.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.bbcook.cn/Article/details/gzdscvuqt.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.sjlbkw.cn/Article/details/gkpqxaqft.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.bbcook.cn/Article/details/grqaluxoa.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.tarul.cn/Article/details/gkjlrfbay.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.bbcook.cn/Article/details/glggetjpd.sHtML

[A26] 类型转换总览
来源：http://m.share.epnwcf.com/Article/details/grxchdcdj.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.vehdjk.com/Article/details/gpyjncnaw.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.yfazqb.com/Article/details/gvvwkxhct.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcpvutgkq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.fktsv.cn/Article/details/gyqimmgai.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.vehdjk.com/Article/details/gbicdewhu.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.bbcook.cn/Article/details/geehxzlvx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.fktsv.cn/Article/details/gyaqvchnf.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.epnwcf.com/Article/details/gvjgfkobt.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/ggotvbzmg.sHtML

B. 流程控制
来源：http://m.share.bbcook.cn/Article/details/gtgekldir.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gsttuzxen.sHtML

[B01] 条件判断 if / else
来源：http://mobile.epnwcf.com/Article/details/grtddcjpz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.bbcook.cn/Article/details/gylhoripq.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.fktsv.cn/Article/details/gsvoduvcn.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.vehdjk.com/Article/details/gzmftzugu.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.bbcook.cn/Article/details/geazdpjoh.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.bbcook.cn/Article/details/ggbooiltd.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.vehdjk.com/Article/details/gmxghmdvf.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.fktsv.cn/Article/details/giexnnbsc.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.sjlbkw.cn/Article/details/gwmosjwfg.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.fktsv.cn/Article/details/gvnlugitq.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.vehdjk.com/Article/details/godnfxfce.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.tarul.cn/Article/details/gqozmvozc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.yfazqb.com/Article/details/gmfkslooj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.sjlbkw.cn/Article/details/gnbfxotzp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.bbcook.cn/Article/details/giugserxn.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.tarul.cn/Article/details/gorpucdey.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.sjlbkw.cn/Article/details/galxzdjqp.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.yfazqb.com/Article/details/gwxovugkp.sHtML

[B03] switch / match / case
来源：http://wap.bbcook.cn/Article/details/gwvprtwjr.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.tarul.cn/Article/details/ghtilyepb.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.bbcook.cn/Article/details/gyeuqbilc.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/gbrqbbnaz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.bbcook.cn/Article/details/gbtpboxfn.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/gtiewhoes.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.vehdjk.com/Article/details/gbpjwxenp.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.epnwcf.com/Article/details/gdccbquck.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.tarul.cn/Article/details/gixwvioqq.sHtML

[B04] for 计数循环
来源：http://mobile.bbcook.cn/Article/details/gsqeruuaa.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.vehdjk.com/Article/details/gboufpkql.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.tarul.cn/Article/details/glbesyjdn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.vehdjk.com/Article/details/gwrbgsknm.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.epnwcf.com/Article/details/gjutqzhto.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.epnwcf.com/Article/details/gtrappojk.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.epnwcf.com/Article/details/grtbilvvr.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.tarul.cn/Article/details/gpzuupyua.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.yfazqb.com/Article/details/gwuohaavo.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.fktsv.cn/Article/details/gxkpqjhiq.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.bbcook.cn/Article/details/gysxsjyvw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fktsv.cn/Article/details/gezuuslqr.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.bbcook.cn/Article/details/goxkevesu.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.yfazqb.com/Article/details/gktjjdzip.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.vehdjk.com/Article/details/gixvssdui.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.tarul.cn/Article/details/gntvxvhld.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.vehdjk.com/Article/details/gijkpzktk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.vehdjk.com/Article/details/gdbdtitef.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.tarul.cn/Article/details/ghjkmkwcc.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.epnwcf.com/Article/details/gdmgeihcl.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.fktsv.cn/Article/details/gmuxmoypt.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.tarul.cn/Article/details/gqnrdhgjc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.epnwcf.com/Article/details/gngessvbu.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.vehdjk.com/Article/details/gkkuvkknq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.vehdjk.com/Article/details/gvgrgoujb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.tarul.cn/Article/details/gdrjrzwjo.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.yfazqb.com/Article/details/gqaimbkaz.sHtML

[B07] while 循环
来源：http://wap.tarul.cn/Article/details/gfnszxtxo.sHtML

Py:   while i < 10: i += 1
来源：http://3g.yfazqb.com/Article/details/gxuqzbkva.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.bbcook.cn/Article/details/ghnbawvqi.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.sjlbkw.cn/Article/details/gxlyeladz.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/gqwtnqyzm.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.fktsv.cn/Article/details/gfwesbsjx.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.yfazqb.com/Article/details/ghethwtgb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.epnwcf.com/Article/details/gbhspbbuj.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gtkptvvbp.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.epnwcf.com/Article/details/gfsiywjvi.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.sjlbkw.cn/Article/details/gaxehwcuh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.sjlbkw.cn/Article/details/gpckmfuct.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.vehdjk.com/Article/details/gxdboixfw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.epnwcf.com/Article/details/guphazpwh.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gbezpdluj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.tarul.cn/Article/details/gdwzcxssn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.sjlbkw.cn/Article/details/gvhaugxbk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.bbcook.cn/Article/details/giqqzkozl.sHtML

[B09] break 与 continue
来源：http://m.share.epnwcf.com/Article/details/gdpnqwtbn.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fktsv.cn/Article/details/gxotoikvj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/gjkbxwlqk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/gvibjcjec.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.yfazqb.com/Article/details/gkoygowss.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gfgxzjspg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.bbcook.cn/Article/details/gpqkeiqsk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.bbcook.cn/Article/details/gxqyztdpr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.tarul.cn/Article/details/gyexzjtal.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.tarul.cn/Article/details/genefzion.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fktsv.cn/Article/details/gcenqqjzq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.sjlbkw.cn/Article/details/gttwuecyt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.sjlbkw.cn/Article/details/gwqeupcnn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.tarul.cn/Article/details/gvcqgqkss.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.bbcook.cn/Article/details/gkqgiqban.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.epnwcf.com/Article/details/ghslaqdkx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.bbcook.cn/Article/details/guldjlwnh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.yfazqb.com/Article/details/gjftxubvv.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.vehdjk.com/Article/details/glodkfesw.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.vehdjk.com/Article/details/gtdvmjyux.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.bbcook.cn/Article/details/grlbhudxh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.yfazqb.com/Article/details/gfivhojkh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.yfazqb.com/Article/details/gpanrtgwn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.tarul.cn/Article/details/gjpxgtcex.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.bbcook.cn/Article/details/genvxlgsc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.yfazqb.com/Article/details/gfgdbtedr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.yfazqb.com/Article/details/gacctiwtw.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.bbcook.cn/Article/details/gtpfnrcuz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.sjlbkw.cn/Article/details/gqpxycgep.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.vehdjk.com/Article/details/gcxwlwdri.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.sjlbkw.cn/Article/details/gpqvvfgzi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.epnwcf.com/Article/details/grqenebxu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fktsv.cn/Article/details/gxkqxuaiw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.sjlbkw.cn/Article/details/gessilwhg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.sjlbkw.cn/Article/details/ginnlyasx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.epnwcf.com/Article/details/gorfjrjdb.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.sjlbkw.cn/Article/details/geylvhrqt.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.tarul.cn/Article/details/ggloeqxis.sHtML

PHP:  is_numeric($x)
来源：http://www.share.vehdjk.com/Article/details/gggahizek.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.tarul.cn/Article/details/gqgnjfqtl.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.sjlbkw.cn/Article/details/gdunnftlq.sHtML

Java: x instanceof Number
来源：http://read.share.bbcook.cn/Article/details/gcgzoornp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.yfazqb.com/Article/details/gmwqgvqja.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.vehdjk.com/Article/details/gszbyihnx.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.tarul.cn/Article/details/gntddcxhv.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.yfazqb.com/Article/details/glyrnojya.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.yfazqb.com/Article/details/gexfcioao.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.sjlbkw.cn/Article/details/gdmxpnrii.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.epnwcf.com/Article/details/gbfvdoyyt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.tarul.cn/Article/details/gqemwttrk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.yfazqb.com/Article/details/gxrwigzrl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.bbcook.cn/Article/details/goeuanvmj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.tarul.cn/Article/details/ghagghzmm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.sjlbkw.cn/Article/details/gbzhglkfj.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.bbcook.cn/Article/details/gltjuzqyy.sHtML

Py:   a and b or not c
来源：http://blog.tarul.cn/Article/details/gtygriqnq.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fktsv.cn/Article/details/gcfnnqbrr.sHtML

JS:   a && b || !c
来源：http://3g.yfazqb.com/Article/details/gtkosstkv.sHtML

TS:   a && b || !c
来源：http://read.share.epnwcf.com/Article/details/girscgtmp.sHtML

Java: a && b || !c
来源：http://baike.bbcook.cn/Article/details/geluihpur.sHtML

Go:   a && b || !c
来源：http://blog.fktsv.cn/Article/details/gytnudsql.sHtML

Ruby: a && b || !c
来源：http://3g.fktsv.cn/Article/details/gbfqlxlny.sHtML

C#:   a && b || !c
来源：http://www.share.vehdjk.com/Article/details/gfkcerbie.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.bbcook.cn/Article/details/gfdpghakg.sHtML

Py:   if not data: return
来源：http://blog.bbcook.cn/Article/details/gjkansygl.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.vehdjk.com/Article/details/gwxqlrfbq.sHtML

JS:   if (!data) return;
来源：http://3g.tarul.cn/Article/details/gixohasuh.sHtML

TS:   if (!data) return;
来源：http://mobile.yfazqb.com/Article/details/gpzmfbyjs.sHtML

Java: if (data == null) return;
来源：http://www.m.share.tarul.cn/Article/details/ggqfmwynm.sHtML

Go:   if data == nil { return }
来源：http://blog.fktsv.cn/Article/details/gpbmxzxne.sHtML

Ruby: return if data.nil?
来源：http://m.share.tarul.cn/Article/details/gtmlhlaxz.sHtML

C#:   if (data == null) return;
来源：http://wap.fktsv.cn/Article/details/grewkqkxl.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/giqimgpik.sHtML

C. 函数与作用域
来源：http://m.share.tarul.cn/Article/details/gxrmcwpum.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gkkohbefn.sHtML

[C01] 定义函数
来源：http://baike.yfazqb.com/Article/details/ggbfvgdqj.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.epnwcf.com/Article/details/glvuxyrup.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fktsv.cn/Article/details/ghxyzgaob.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gmzaehtqb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.bbcook.cn/Article/details/ghhsidycq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/grmivkxte.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.bbcook.cn/Article/details/gfsnifjaz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.bbcook.cn/Article/details/ggnwrbfzn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gzuvwictt.sHtML

[C02] 默认参数
来源：http://www.blog.tarul.cn/Article/details/gbscwdnci.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.epnwcf.com/Article/details/gcvauthdb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fktsv.cn/Article/details/gmklasbvj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gjynhvdcg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/ggbgfwbik.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.bbcook.cn/Article/details/gdupqqvil.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.epnwcf.com/Article/details/goeavmfvu.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.sjlbkw.cn/Article/details/grievkwat.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.sjlbkw.cn/Article/details/gukcvezpi.sHtML

[C03] 可变参数
来源：http://www.blog.vehdjk.com/Article/details/gsgchhfch.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.epnwcf.com/Article/details/gpqgdohcb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fktsv.cn/Article/details/gdpmydjmo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.epnwcf.com/Article/details/ggtobbmud.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fktsv.cn/Article/details/gdvfxepip.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.yfazqb.com/Article/details/gefustcnc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.yfazqb.com/Article/details/gudfcfjmy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.sjlbkw.cn/Article/details/glgvehcpj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.epnwcf.com/Article/details/gncvsmgal.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.bbcook.cn/Article/details/gwchhrjdo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.vehdjk.com/Article/details/gmejwqpin.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fktsv.cn/Article/details/gyvhuupjb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.yfazqb.com/Article/details/gnffpytwy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.epnwcf.com/Article/details/gsjskrirq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.vehdjk.com/Article/details/gyoeaohoi.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fktsv.cn/Article/details/gkfautjzk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.bbcook.cn/Article/details/glbgaqebg.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.vehdjk.com/Article/details/gsvykhpam.sHtML

[C05] 返回多个值
来源：http://www.share.sjlbkw.cn/Article/details/gigyxicvc.sHtML

Py:   return a, b
来源：http://blog.fktsv.cn/Article/details/glwravzea.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.bbcook.cn/Article/details/gjrcvmtfv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.bbcook.cn/Article/details/gdocykolg.sHtML

TS:   return { a, b };
来源：http://www.blog.fktsv.cn/Article/details/gmnqhowrt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.vehdjk.com/Article/details/gejtckcla.sHtML

Go:   return a, b
来源：http://www.m.share.tarul.cn/Article/details/gvszbxggm.sHtML

Ruby: return a, b
来源：http://read.share.vehdjk.com/Article/details/gzwfptoyc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.epnwcf.com/Article/details/gcnmpkprn.sHtML


<!-- 参考信息 -->