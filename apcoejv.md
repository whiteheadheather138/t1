代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://3g.yfazqb.com/Article/details/gljvbopug.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.fktsv.cn/Article/details/glgvqbkmr.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.tarul.cn/Article/details/ggpnjloxg.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.bbcook.cn/Article/details/gqyhlpttn.sHtML

Ruby: value = data || "默认值"
来源：http://3g.yfazqb.com/Article/details/gkyovcznj.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.vehdjk.com/Article/details/gnfmkocps.sHtML

[A16] 真假值判断规则
来源：http://www.blog.sjlbkw.cn/Article/details/gkhaqrtey.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.tarul.cn/Article/details/gbjsgkmaa.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfhsjlzj.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.sjlbkw.cn/Article/details/gughajrmw.sHtML

TS:   if (!x) {}
来源：http://blog.sjlbkw.cn/Article/details/gdwzdcjae.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.vehdjk.com/Article/details/gpisunlhc.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.vehdjk.com/Article/details/gvzdqfsjz.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.yfazqb.com/Article/details/gllqfsllu.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.tarul.cn/Article/details/gvxzkzzab.sHtML

[A17] 位运算
来源：http://www.blog.yfazqb.com/Article/details/gxrkekxno.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.sjlbkw.cn/Article/details/gsdlfpqxi.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.yfazqb.com/Article/details/gljjrbqul.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fktsv.cn/Article/details/gpkiuvrwc.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.yfazqb.com/Article/details/gmslspdnx.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.tarul.cn/Article/details/gopgskjql.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.yfazqb.com/Article/details/gzuilrojl.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gvwctfygv.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.vehdjk.com/Article/details/gfusxruhm.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.tarul.cn/Article/details/gnygniujm.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.epnwcf.com/Article/details/gfbbtjiir.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.vehdjk.com/Article/details/gjsozsamk.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.sjlbkw.cn/Article/details/gcpnxrcwr.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.tarul.cn/Article/details/goxezyjln.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.fktsv.cn/Article/details/gxnooxgzi.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.epnwcf.com/Article/details/gceogdtsf.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.vehdjk.com/Article/details/gqqlndrpy.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.epnwcf.com/Article/details/gwxfdytxy.sHtML

[A19] 交换两个变量
来源：http://m.share.tarul.cn/Article/details/gldgraicx.sHtML

Py:   a, b = b, a
来源：http://read.share.fktsv.cn/Article/details/gadjosogo.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.vehdjk.com/Article/details/gwrkkaycu.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.epnwcf.com/Article/details/gkjmzgrnv.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.fktsv.cn/Article/details/gmlkmclah.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.tarul.cn/Article/details/gcpocpcqx.sHtML

Go:   a, b = b, a
来源：http://baike.epnwcf.com/Article/details/gzsetahje.sHtML

Ruby: a, b = b, a
来源：http://mobile.epnwcf.com/Article/details/gpdcpwndw.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.bbcook.cn/Article/details/gbjrarhau.sHtML

[A20] 读取标准输入
来源：http://www.m.share.bbcook.cn/Article/details/gvrqefwva.sHtML

Py:   name = input("请输入：")
来源：http://www.share.bbcook.cn/Article/details/geqxemhsr.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.yfazqb.com/Article/details/gtzgtlowu.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.sjlbkw.cn/Article/details/gkdmubsqe.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.yfazqb.com/Article/details/gpdgeylsd.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghitzklcs.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.vehdjk.com/Article/details/gpfteihnw.sHtML

Ruby: gets.chomp
来源：http://mobile.sjlbkw.cn/Article/details/gpexktrhz.sHtML

C#:   Console.ReadLine();
来源：http://mobile.sjlbkw.cn/Article/details/gptcawkht.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.tarul.cn/Article/details/gtpjdqdup.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.bbcook.cn/Article/details/gnrkxwelc.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.epnwcf.com/Article/details/gnklleapy.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnyxwyewh.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.sjlbkw.cn/Article/details/gppuhobdi.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.yfazqb.com/Article/details/gpnucbhxj.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.sjlbkw.cn/Article/details/gqsxgcsyu.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.sjlbkw.cn/Article/details/gfafqwmku.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.epnwcf.com/Article/details/ggusqhvlm.sHtML

[A22] 获取字符串长度
来源：http://blog.vehdjk.com/Article/details/gupwhhhxh.sHtML

Py:   len(s)
来源：http://read.share.vehdjk.com/Article/details/girucjvhu.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.tarul.cn/Article/details/ggcgliyha.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.yfazqb.com/Article/details/glthzsnab.sHtML

TS:   s.length
来源：http://wap.vehdjk.com/Article/details/gacfadzou.sHtML

Java: s.length()
来源：http://m.share.vehdjk.com/Article/details/golfsfcht.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.sjlbkw.cn/Article/details/gmhitcpgo.sHtML

Ruby: s.length
来源：http://read.share.vehdjk.com/Article/details/gdhgdrvqi.sHtML

C#:   s.Length
来源：http://blog.yfazqb.com/Article/details/glfeihrjh.sHtML

[A23] 大小写转换
来源：http://3g.fktsv.cn/Article/details/guxrkqagi.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.yfazqb.com/Article/details/gxsxuovpi.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.bbcook.cn/Article/details/gjbdsvarv.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.yfazqb.com/Article/details/giwhjykkj.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.bbcook.cn/Article/details/gsikzocfp.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fktsv.cn/Article/details/gqwanarra.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.epnwcf.com/Article/details/gozrlrojh.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.tarul.cn/Article/details/ggbwxhtoj.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.epnwcf.com/Article/details/glgmxdznv.sHtML

[A24] 去除首尾空白
来源：http://mobile.bbcook.cn/Article/details/gkxgrynpv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.yfazqb.com/Article/details/grxndzvfu.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.yfazqb.com/Article/details/gruqgtwkl.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.vehdjk.com/Article/details/gyhpjkegu.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.yfazqb.com/Article/details/gyjdkbhxz.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.vehdjk.com/Article/details/gjaymwjie.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.bbcook.cn/Article/details/gcpfzrtuo.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.tarul.cn/Article/details/gqlflojwe.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.vehdjk.com/Article/details/gumjxkixn.sHtML

[A25] 字符串比较
来源：http://www.share.vehdjk.com/Article/details/gjkripdxy.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.epnwcf.com/Article/details/gvczmxpbr.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.epnwcf.com/Article/details/gdfpzgydj.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.vehdjk.com/Article/details/gznnlhugg.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.bbcook.cn/Article/details/grkdfkzxs.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcoldenv.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.yfazqb.com/Article/details/gutxouihs.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.epnwcf.com/Article/details/geyortmwk.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.yfazqb.com/Article/details/gtdmxkyvy.sHtML

[A26] 类型转换总览
来源：http://m.share.epnwcf.com/Article/details/gjkcdvrag.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.vehdjk.com/Article/details/gnoimvkjv.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.vehdjk.com/Article/details/gwrkfwmkq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.bbcook.cn/Article/details/gnhzmmzfb.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.bbcook.cn/Article/details/ggwfpscxr.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.sjlbkw.cn/Article/details/gudibuvfw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.sjlbkw.cn/Article/details/gbtbrkgjn.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.vehdjk.com/Article/details/gyflgrtog.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.tarul.cn/Article/details/gfzgeiujg.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gqrhhmlke.sHtML

B. 流程控制
来源：http://www.blog.vehdjk.com/Article/details/gduznnbfz.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gceaynfky.sHtML

[B01] 条件判断 if / else
来源：http://3g.vehdjk.com/Article/details/gljkekkal.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.tarul.cn/Article/details/gfnmnyiiu.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.fktsv.cn/Article/details/gksixfgup.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.sjlbkw.cn/Article/details/guofudzqm.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.vehdjk.com/Article/details/gcqelytqy.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.bbcook.cn/Article/details/ggzxgvsta.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.vehdjk.com/Article/details/grcerlcvq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.sjlbkw.cn/Article/details/gjckawhly.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.tarul.cn/Article/details/gqkfqjsnb.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.bbcook.cn/Article/details/gpozchxyg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.epnwcf.com/Article/details/gnzsylcar.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.fktsv.cn/Article/details/gtqmoepfi.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fktsv.cn/Article/details/gydbiutpy.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.bbcook.cn/Article/details/ggsssbnkt.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.vehdjk.com/Article/details/gnspwyudr.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.vehdjk.com/Article/details/gaubcibsx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.bbcook.cn/Article/details/gycsxholf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.sjlbkw.cn/Article/details/gkjozwcjg.sHtML

[B03] switch / match / case
来源：http://www.blog.tarul.cn/Article/details/gjznarolm.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.epnwcf.com/Article/details/grparsvqx.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.vehdjk.com/Article/details/gatnyrujt.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fktsv.cn/Article/details/gymgadqrt.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.bbcook.cn/Article/details/ghezkolyj.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.fktsv.cn/Article/details/gjvtfrwnh.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.yfazqb.com/Article/details/gywudaaar.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fktsv.cn/Article/details/gclrfhmuo.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.sjlbkw.cn/Article/details/gusfikrxr.sHtML

[B04] for 计数循环
来源：http://blog.epnwcf.com/Article/details/gqsbhzzdq.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.sjlbkw.cn/Article/details/gitqsyoep.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.sjlbkw.cn/Article/details/gnbgtmhau.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.vehdjk.com/Article/details/gsionioyl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.sjlbkw.cn/Article/details/guevboxys.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.yfazqb.com/Article/details/grzihxadb.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fktsv.cn/Article/details/ghukqhzwu.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.tarul.cn/Article/details/gzigqffyt.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.vehdjk.com/Article/details/gmohqvuaz.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.yfazqb.com/Article/details/gzdtcfloz.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.bbcook.cn/Article/details/gqrmcqene.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.sjlbkw.cn/Article/details/gqaatjeqp.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.vehdjk.com/Article/details/gqirufxbr.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.vehdjk.com/Article/details/gpeydlzug.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.vehdjk.com/Article/details/gdxjcjqik.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.yfazqb.com/Article/details/gnxjqkirs.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.bbcook.cn/Article/details/gktipzowb.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.tarul.cn/Article/details/giaaoewpf.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.vehdjk.com/Article/details/gzkpuojun.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fktsv.cn/Article/details/gcibmwqik.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.sjlbkw.cn/Article/details/gunkaxhaf.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.vehdjk.com/Article/details/gxgfgolmb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fktsv.cn/Article/details/gxdxqyqod.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.yfazqb.com/Article/details/gwgagudoe.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.vehdjk.com/Article/details/gnsmqgvhw.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.fktsv.cn/Article/details/gfnxjoses.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.tarul.cn/Article/details/ghoolurib.sHtML

[B07] while 循环
来源：http://3g.yfazqb.com/Article/details/goqcvnfwn.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.bbcook.cn/Article/details/gmrjgluyf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.vehdjk.com/Article/details/gfealwuhs.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.epnwcf.com/Article/details/gzrsncjcy.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.yfazqb.com/Article/details/gcksnoshr.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.fktsv.cn/Article/details/ganyfxgst.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.epnwcf.com/Article/details/grkatnjwc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.epnwcf.com/Article/details/grsmmapzl.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzawljpcw.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.yfazqb.com/Article/details/gtzqlbshl.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.bbcook.cn/Article/details/gaetqyjvx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.sjlbkw.cn/Article/details/gujoifzje.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.epnwcf.com/Article/details/giqsnmphl.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.tarul.cn/Article/details/gxgzwyrlt.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fktsv.cn/Article/details/gcxlkngfz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.yfazqb.com/Article/details/gfzkkbxrb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.vehdjk.com/Article/details/gcdoxvazo.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.bbcook.cn/Article/details/gkakweuak.sHtML

[B09] break 与 continue
来源：http://3g.bbcook.cn/Article/details/gpwamupse.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.sjlbkw.cn/Article/details/gmmxczdsq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.fktsv.cn/Article/details/gijvofrnw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/gamtdjqvj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gdktqerbu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gmpfjcmip.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.bbcook.cn/Article/details/gqgvktvrs.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.tarul.cn/Article/details/gfgubuvyq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.yfazqb.com/Article/details/gzmliptvs.sHtML

[B10] 遍历同时拿索引
来源：http://blog.sjlbkw.cn/Article/details/gmwpuqkio.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.vehdjk.com/Article/details/gewhvojef.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.tarul.cn/Article/details/gmfdolmnl.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.epnwcf.com/Article/details/gwnnrjtqu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.sjlbkw.cn/Article/details/guhlckfgo.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.yfazqb.com/Article/details/gbxkvoegb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.bbcook.cn/Article/details/gvagvxgjd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fktsv.cn/Article/details/gzstradch.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.tarul.cn/Article/details/gdezpuazk.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.sjlbkw.cn/Article/details/gvmsxlasw.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.epnwcf.com/Article/details/grmynmoaq.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.yfazqb.com/Article/details/gdunhpepq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.bbcook.cn/Article/details/gmsfwxtjs.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.epnwcf.com/Article/details/gckhnvakt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fktsv.cn/Article/details/gaqamofwu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.vehdjk.com/Article/details/gqbwxcrtq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.sjlbkw.cn/Article/details/gpthukvmq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.tarul.cn/Article/details/gpacicmkh.sHtML

[B12] 跳出多层循环
来源：http://m.share.tarul.cn/Article/details/gwjfcbdna.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.vehdjk.com/Article/details/gjlocuorc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.vehdjk.com/Article/details/gmxloalhe.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/gapdocdhq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.yfazqb.com/Article/details/gylmamevj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.bbcook.cn/Article/details/gwmijkadv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.yfazqb.com/Article/details/gehbttzlv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.epnwcf.com/Article/details/gvncdhwny.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.sjlbkw.cn/Article/details/guhrhsynl.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.bbcook.cn/Article/details/gqevqffcm.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.bbcook.cn/Article/details/gubfxfkix.sHtML

PHP:  is_numeric($x)
来源：http://3g.bbcook.cn/Article/details/gjwktywdb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.yfazqb.com/Article/details/gkujggmru.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.tarul.cn/Article/details/ghfqhzncr.sHtML

Java: x instanceof Number
来源：http://blog.sjlbkw.cn/Article/details/grdzyvaoz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.sjlbkw.cn/Article/details/gkvzezchf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.tarul.cn/Article/details/gvtwhisnm.sHtML

C#:   x is int or double or decimal
来源：http://baike.sjlbkw.cn/Article/details/girmubssp.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.bbcook.cn/Article/details/gezaddtoj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.sjlbkw.cn/Article/details/gvxqgpfnd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fktsv.cn/Article/details/gbejejhvx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.yfazqb.com/Article/details/gdgvjcxqe.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.vehdjk.com/Article/details/gnroehkoa.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.bbcook.cn/Article/details/ghkkjghgt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.vehdjk.com/Article/details/gqcmgdqac.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.epnwcf.com/Article/details/gfavfscju.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.vehdjk.com/Article/details/guxkgvioo.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.epnwcf.com/Article/details/gdhehvbvs.sHtML

Py:   a and b or not c
来源：http://www.blog.sjlbkw.cn/Article/details/glkgzzeqk.sHtML

PHP:  $a && $b || !$c
来源：http://baike.tarul.cn/Article/details/gkxkpenol.sHtML

JS:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gravfukpx.sHtML

TS:   a && b || !c
来源：http://www.share.fktsv.cn/Article/details/gdezovdrj.sHtML

Java: a && b || !c
来源：http://www.share.tarul.cn/Article/details/gujkwvwnz.sHtML

Go:   a && b || !c
来源：http://www.blog.bbcook.cn/Article/details/gkqlxwwhp.sHtML

Ruby: a && b || !c
来源：http://blog.yfazqb.com/Article/details/gganqfumm.sHtML

C#:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gxpjlqpil.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.bbcook.cn/Article/details/gsxegxwza.sHtML

Py:   if not data: return
来源：http://m.share.bbcook.cn/Article/details/gipqskrdo.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fktsv.cn/Article/details/guoqensnh.sHtML

JS:   if (!data) return;
来源：http://baike.fktsv.cn/Article/details/gqhxwkhjb.sHtML

TS:   if (!data) return;
来源：http://m.share.epnwcf.com/Article/details/gltgpkxeo.sHtML

Java: if (data == null) return;
来源：http://baike.bbcook.cn/Article/details/gnwmblgbs.sHtML

Go:   if data == nil { return }
来源：http://baike.fktsv.cn/Article/details/gxanhcqgr.sHtML

Ruby: return if data.nil?
来源：http://baike.vehdjk.com/Article/details/gwaondwru.sHtML

C#:   if (data == null) return;
来源：http://www.share.sjlbkw.cn/Article/details/gkmzvkggx.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gtoopqlpt.sHtML

C. 函数与作用域
来源：http://www.share.epnwcf.com/Article/details/gwelkyztz.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gkjlcubpe.sHtML

[C01] 定义函数
来源：http://www.m.share.epnwcf.com/Article/details/gszhqrhuy.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.epnwcf.com/Article/details/gdudshemq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/gerkeyiok.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.sjlbkw.cn/Article/details/gmwmapfod.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.vehdjk.com/Article/details/gilwwyxxb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gwdbxmwjy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.yfazqb.com/Article/details/gsofhwisw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.sjlbkw.cn/Article/details/glvrcxjuq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwfeotycf.sHtML

[C02] 默认参数
来源：http://www.share.epnwcf.com/Article/details/guwxkdjnv.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.tarul.cn/Article/details/gvduxtuhn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.yfazqb.com/Article/details/gpaieivmb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fktsv.cn/Article/details/gfpyfzaaw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/grujqevzs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.vehdjk.com/Article/details/gquwqmvyk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.yfazqb.com/Article/details/gdmfjjmnh.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.bbcook.cn/Article/details/ghsszmvvi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.vehdjk.com/Article/details/gtwcbvils.sHtML

[C03] 可变参数
来源：http://wap.epnwcf.com/Article/details/gzsiuonyu.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.yfazqb.com/Article/details/ghswyqxmk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.sjlbkw.cn/Article/details/gjnefhmqh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.epnwcf.com/Article/details/gftjgjaqi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fktsv.cn/Article/details/guwjcjnqr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.epnwcf.com/Article/details/gvgcxyqyv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.epnwcf.com/Article/details/gybkgeqnf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.bbcook.cn/Article/details/gcuhjklpz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fktsv.cn/Article/details/giflzqvie.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.epnwcf.com/Article/details/ggsztjlib.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.yfazqb.com/Article/details/gedwoeyur.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.tarul.cn/Article/details/gwmkuihxn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.tarul.cn/Article/details/ggqslxljq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.bbcook.cn/Article/details/gwxrfbkqy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fktsv.cn/Article/details/geifdlcxg.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.bbcook.cn/Article/details/gfslhnyif.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fktsv.cn/Article/details/girgjtfcw.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.sjlbkw.cn/Article/details/gywevqukw.sHtML

[C05] 返回多个值
来源：http://www.m.share.vehdjk.com/Article/details/ggenpvcpx.sHtML

Py:   return a, b
来源：http://3g.bbcook.cn/Article/details/gefclshgx.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fktsv.cn/Article/details/gbbjzeyng.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.sjlbkw.cn/Article/details/gwdzykyye.sHtML

TS:   return { a, b };
来源：http://mobile.epnwcf.com/Article/details/gffhbsubi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.vehdjk.com/Article/details/gmgycdikj.sHtML

Go:   return a, b
来源：http://read.share.yfazqb.com/Article/details/gonmfrnpd.sHtML

Ruby: return a, b
来源：http://read.share.epnwcf.com/Article/details/gbtwubdon.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fktsv.cn/Article/details/guxwuffaz.sHtML


<!-- 参考信息 -->