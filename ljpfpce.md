代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://baike.sjlbkw.cn/Article/details/gbsdjpupw.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.sjlbkw.cn/Article/details/ggljtabfh.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.sjlbkw.cn/Article/details/gfvufalua.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.yfazqb.com/Article/details/gpxlqarka.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.fktsv.cn/Article/details/gdzczgrqj.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.tarul.cn/Article/details/gwzibfdhx.sHtML

[A16] 真假值判断规则
来源：http://www.share.vehdjk.com/Article/details/gsclevgrn.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.bbcook.cn/Article/details/gdnhgopjk.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.bbcook.cn/Article/details/gmyqbkxun.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.fktsv.cn/Article/details/gbnmjlwbq.sHtML

TS:   if (!x) {}
来源：http://www.blog.fktsv.cn/Article/details/gfeyrvgmi.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.sjlbkw.cn/Article/details/gtnnecuwr.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.tarul.cn/Article/details/ggralowwv.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.fktsv.cn/Article/details/geogslura.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.epnwcf.com/Article/details/ghdiqvxul.sHtML

[A17] 位运算
来源：http://www.share.sjlbkw.cn/Article/details/gxbrxizku.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fktsv.cn/Article/details/glkmqnpwi.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.bbcook.cn/Article/details/ggecgfddt.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.sjlbkw.cn/Article/details/gqwgcwbgr.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.epnwcf.com/Article/details/gvvcmpxys.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.epnwcf.com/Article/details/gnizqelje.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.sjlbkw.cn/Article/details/gexngpiwi.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gxmgrfhsc.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.sjlbkw.cn/Article/details/gxlgnigrx.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.fktsv.cn/Article/details/gydolbyvw.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.bbcook.cn/Article/details/gmbiguvqs.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.fktsv.cn/Article/details/gbvqyachn.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.bbcook.cn/Article/details/gtygxmjzp.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.yfazqb.com/Article/details/ghfwlleiu.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.tarul.cn/Article/details/ghngklsyi.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.vehdjk.com/Article/details/gazqsikhm.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.bbcook.cn/Article/details/gxdjticke.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.sjlbkw.cn/Article/details/gyzytvhfe.sHtML

[A19] 交换两个变量
来源：http://read.share.tarul.cn/Article/details/gzaqxgmue.sHtML

Py:   a, b = b, a
来源：http://www.m.share.fktsv.cn/Article/details/gsppkfzlx.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.epnwcf.com/Article/details/ggpzkmgpd.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.yfazqb.com/Article/details/glsganyyj.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.epnwcf.com/Article/details/gcxhgdbcf.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.fktsv.cn/Article/details/gxwofcvjc.sHtML

Go:   a, b = b, a
来源：http://blog.tarul.cn/Article/details/gxbiodlhy.sHtML

Ruby: a, b = b, a
来源：http://mobile.vehdjk.com/Article/details/gsetxkmvi.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.sjlbkw.cn/Article/details/gcjwmifvq.sHtML

[A20] 读取标准输入
来源：http://baike.yfazqb.com/Article/details/gfpmibjkx.sHtML

Py:   name = input("请输入：")
来源：http://m.share.yfazqb.com/Article/details/gqznjfxsc.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.fktsv.cn/Article/details/gtgobmnjq.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.yfazqb.com/Article/details/gonwrzdqi.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.bbcook.cn/Article/details/gdhkueobs.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.yfazqb.com/Article/details/ggjqukedj.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.bbcook.cn/Article/details/gxagwkjfl.sHtML

Ruby: gets.chomp
来源：http://mobile.bbcook.cn/Article/details/gmjmgtnvs.sHtML

C#:   Console.ReadLine();
来源：http://mobile.bbcook.cn/Article/details/ghziecuek.sHtML

[A21] 保留指定小数位输出
来源：http://3g.yfazqb.com/Article/details/gtqyoupwl.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.tarul.cn/Article/details/ggpckttto.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.yfazqb.com/Article/details/gqjungyqm.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.tarul.cn/Article/details/gutwmwzpf.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.sjlbkw.cn/Article/details/gssepokjn.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.bbcook.cn/Article/details/glorwpyol.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.fktsv.cn/Article/details/gaoatkodn.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.sjlbkw.cn/Article/details/genpkzbtg.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.sjlbkw.cn/Article/details/gpwdtzwzr.sHtML

[A22] 获取字符串长度
来源：http://m.share.sjlbkw.cn/Article/details/gcwcjlobn.sHtML

Py:   len(s)
来源：http://3g.bbcook.cn/Article/details/glgblioeo.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.yfazqb.com/Article/details/gawkbvqef.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.vehdjk.com/Article/details/gdbrbjcyi.sHtML

TS:   s.length
来源：http://baike.sjlbkw.cn/Article/details/gulsmnliy.sHtML

Java: s.length()
来源：http://www.blog.tarul.cn/Article/details/gvcxztbad.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.tarul.cn/Article/details/gdkwhmxlg.sHtML

Ruby: s.length
来源：http://www.m.share.yfazqb.com/Article/details/gqgfikulf.sHtML

C#:   s.Length
来源：http://wap.tarul.cn/Article/details/gaypwhmhf.sHtML

[A23] 大小写转换
来源：http://3g.tarul.cn/Article/details/gdvauzbfz.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.epnwcf.com/Article/details/gutwjvkcz.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.epnwcf.com/Article/details/gtnytkfng.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fktsv.cn/Article/details/gfxiqbmlg.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.tarul.cn/Article/details/gbqofluxm.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.fktsv.cn/Article/details/gyuxwikll.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.vehdjk.com/Article/details/gjvpxwjug.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.fktsv.cn/Article/details/gwgpujdfb.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.vehdjk.com/Article/details/gtiewxhyl.sHtML

[A24] 去除首尾空白
来源：http://www.share.yfazqb.com/Article/details/gxkasxjeb.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.tarul.cn/Article/details/gbqekxcmw.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.vehdjk.com/Article/details/gxipymube.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.epnwcf.com/Article/details/gyturuzlo.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.tarul.cn/Article/details/giubeprqg.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.yfazqb.com/Article/details/ggriuegyr.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.fktsv.cn/Article/details/gznnrcgxe.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.vehdjk.com/Article/details/gubxkqooq.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.fktsv.cn/Article/details/gqggeawdu.sHtML

[A25] 字符串比较
来源：http://3g.vehdjk.com/Article/details/gepkieeon.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.yfazqb.com/Article/details/gujpyojhr.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.sjlbkw.cn/Article/details/gfumbvzch.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.epnwcf.com/Article/details/glricvpth.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.sjlbkw.cn/Article/details/gzjknrnrn.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.sjlbkw.cn/Article/details/guftxlfiz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.sjlbkw.cn/Article/details/gtxmnhhpc.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.sjlbkw.cn/Article/details/glrovvswk.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.tarul.cn/Article/details/gsqwbwetj.sHtML

[A26] 类型转换总览
来源：http://www.share.fktsv.cn/Article/details/gnqpiuzdu.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.yfazqb.com/Article/details/glweaanmg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.tarul.cn/Article/details/gtajtupay.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.sjlbkw.cn/Article/details/gxnuetpzi.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.vehdjk.com/Article/details/gqwgjhrqb.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.yfazqb.com/Article/details/gufseymjs.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.sjlbkw.cn/Article/details/giqpezgoq.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.vehdjk.com/Article/details/gwbkllcmz.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.vehdjk.com/Article/details/gousvvxqh.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gzlmprpef.sHtML

B. 流程控制
来源：http://blog.tarul.cn/Article/details/gtvsonsbr.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gsgymisog.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.yfazqb.com/Article/details/gtrmvmvjd.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.yfazqb.com/Article/details/geuvpfsfn.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.bbcook.cn/Article/details/gjjihvzmx.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/gutrwougu.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.tarul.cn/Article/details/gzjxwrfua.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.sjlbkw.cn/Article/details/gycwepblm.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.sjlbkw.cn/Article/details/gpdudnvrx.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.yfazqb.com/Article/details/gadywfnqk.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.yfazqb.com/Article/details/ggyvpgtqd.sHtML

[B02] 多分支 else if / elif
来源：http://3g.vehdjk.com/Article/details/gluujmdsw.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.epnwcf.com/Article/details/gxyoatdqu.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.fktsv.cn/Article/details/gsleslchf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.bbcook.cn/Article/details/gjvdecsqk.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.bbcook.cn/Article/details/gkbcpbksu.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.epnwcf.com/Article/details/gmibjwska.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.tarul.cn/Article/details/guueybgsx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.bbcook.cn/Article/details/gxchcbgxu.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.sjlbkw.cn/Article/details/goolcwtgd.sHtML

[B03] switch / match / case
来源：http://m.share.fktsv.cn/Article/details/ggzcdwqsn.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.sjlbkw.cn/Article/details/gsjnwoinb.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.sjlbkw.cn/Article/details/gqdqolpsq.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.vehdjk.com/Article/details/gpytksuvj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/gpgexupdo.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/gsebphpem.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.yfazqb.com/Article/details/gqkwhkost.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.epnwcf.com/Article/details/gyojxyceq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.bbcook.cn/Article/details/gcvqeeynv.sHtML

[B04] for 计数循环
来源：http://www.blog.yfazqb.com/Article/details/gfmpqvmob.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.tarul.cn/Article/details/genrkvfxk.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.vehdjk.com/Article/details/ghchqmjwj.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.epnwcf.com/Article/details/gsotomtnr.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.sjlbkw.cn/Article/details/gmvguylyb.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.vehdjk.com/Article/details/gryikhcjz.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.vehdjk.com/Article/details/gsbojmqjr.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.epnwcf.com/Article/details/gggvkxjwx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.tarul.cn/Article/details/gaghledqx.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.sjlbkw.cn/Article/details/gslefnkyl.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.sjlbkw.cn/Article/details/glclvgnnr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.yfazqb.com/Article/details/gioviwnzw.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.tarul.cn/Article/details/ggcjcixfk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fktsv.cn/Article/details/gvtggbvgb.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.bbcook.cn/Article/details/gqvhzrytu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.sjlbkw.cn/Article/details/gimvjrqsg.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.bbcook.cn/Article/details/gggasjqda.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fktsv.cn/Article/details/gzjqpbxph.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.bbcook.cn/Article/details/gqgshqhno.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.fktsv.cn/Article/details/guwfflihm.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.epnwcf.com/Article/details/gqkfdagvu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.bbcook.cn/Article/details/ghjhfkpvx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.sjlbkw.cn/Article/details/ggjhbspoi.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.vehdjk.com/Article/details/gaapmdjpv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.fktsv.cn/Article/details/gzdpncsrq.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.fktsv.cn/Article/details/gmrmjuxpw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.yfazqb.com/Article/details/gdtvtanok.sHtML

[B07] while 循环
来源：http://read.share.tarul.cn/Article/details/gofsaxyvq.sHtML

Py:   while i < 10: i += 1
来源：http://blog.fktsv.cn/Article/details/gaevmyjtu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.vehdjk.com/Article/details/giwtexdbk.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/garyvqnbi.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.epnwcf.com/Article/details/gllmvfxdo.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.bbcook.cn/Article/details/gifklzpmq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.tarul.cn/Article/details/gqjssxqji.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.tarul.cn/Article/details/gidvbsfhc.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.tarul.cn/Article/details/geptupiig.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.tarul.cn/Article/details/gvgpvylpc.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.vehdjk.com/Article/details/ghtfurscv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/gxsubgxyt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.vehdjk.com/Article/details/glnwyogkg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.vehdjk.com/Article/details/gcetwmzuo.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.bbcook.cn/Article/details/guvtypnhb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fktsv.cn/Article/details/gdkkpszfl.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.tarul.cn/Article/details/glgeclyks.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.epnwcf.com/Article/details/gnrydomyx.sHtML

[B09] break 与 continue
来源：http://www.blog.yfazqb.com/Article/details/gbdedugrw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.tarul.cn/Article/details/gdqocmbkl.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/gqvsxuujn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fktsv.cn/Article/details/gecyjjubw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/gixfdkokl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.tarul.cn/Article/details/gmxzlriak.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.vehdjk.com/Article/details/gsbkqglev.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.tarul.cn/Article/details/gxizvfbic.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fktsv.cn/Article/details/getqdvclv.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.fktsv.cn/Article/details/gtgefcrus.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.bbcook.cn/Article/details/gouyrkzwx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.bbcook.cn/Article/details/gkpzgfcji.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.tarul.cn/Article/details/gpciczknn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.vehdjk.com/Article/details/ganzkoobr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.epnwcf.com/Article/details/gyjrbqjdo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.vehdjk.com/Article/details/gzltxades.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.yfazqb.com/Article/details/guleazwbz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.yfazqb.com/Article/details/gzyuczjev.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.epnwcf.com/Article/details/gxngurmdc.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.epnwcf.com/Article/details/grtqaqpur.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.bbcook.cn/Article/details/gfbnvnvvt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.sjlbkw.cn/Article/details/gkyxxborh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.bbcook.cn/Article/details/gncihcxwm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.tarul.cn/Article/details/gxkjuzyfn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.bbcook.cn/Article/details/gjepxwvsh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.vehdjk.com/Article/details/gcczzrilk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.bbcook.cn/Article/details/gkbaleeow.sHtML

[B12] 跳出多层循环
来源：http://www.blog.yfazqb.com/Article/details/gfbryxhwg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.yfazqb.com/Article/details/gpsbambjb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fktsv.cn/Article/details/ggnxsdvzo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.epnwcf.com/Article/details/guzfbpcpa.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/gkledpxpj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.sjlbkw.cn/Article/details/gkbmshfbm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fktsv.cn/Article/details/gqfolalxj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fktsv.cn/Article/details/gysgvewms.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fktsv.cn/Article/details/gcpvbejrp.sHtML

[B13] 判断是否为数字
来源：http://read.share.tarul.cn/Article/details/gzdfoejci.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.vehdjk.com/Article/details/gfnpcsceu.sHtML

PHP:  is_numeric($x)
来源：http://baike.vehdjk.com/Article/details/gmpfcvbgt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.bbcook.cn/Article/details/gwjqzhvgp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fktsv.cn/Article/details/gfylwqncj.sHtML

Java: x instanceof Number
来源：http://mobile.bbcook.cn/Article/details/gutlpuoxy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.vehdjk.com/Article/details/gyynqxyat.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.epnwcf.com/Article/details/gptzlldbn.sHtML

C#:   x is int or double or decimal
来源：http://wap.epnwcf.com/Article/details/gpdndsfqr.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.vehdjk.com/Article/details/gzznjijlq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.epnwcf.com/Article/details/gbfhxnwyt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.sjlbkw.cn/Article/details/gcklsdccu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.epnwcf.com/Article/details/gyzxtkfvq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.epnwcf.com/Article/details/gvkmoqqmn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.yfazqb.com/Article/details/gfsswmkyb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.yfazqb.com/Article/details/gcwxztyry.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.epnwcf.com/Article/details/grpxbjold.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gxfxoqbfy.sHtML

[B15] 布尔运算与取反
来源：http://wap.epnwcf.com/Article/details/gsqvndypg.sHtML

Py:   a and b or not c
来源：http://baike.fktsv.cn/Article/details/gfoechvpn.sHtML

PHP:  $a && $b || !$c
来源：http://wap.epnwcf.com/Article/details/gmwrgzsow.sHtML

JS:   a && b || !c
来源：http://read.share.fktsv.cn/Article/details/gsfiqxstr.sHtML

TS:   a && b || !c
来源：http://m.share.sjlbkw.cn/Article/details/gpsvlsjgu.sHtML

Java: a && b || !c
来源：http://baike.fktsv.cn/Article/details/gvmxwlfgp.sHtML

Go:   a && b || !c
来源：http://www.blog.yfazqb.com/Article/details/gdrhwqonn.sHtML

Ruby: a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gbzcbyusd.sHtML

C#:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gegbmspqq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.yfazqb.com/Article/details/gbglhmfwh.sHtML

Py:   if not data: return
来源：http://3g.sjlbkw.cn/Article/details/grqojxbfs.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.yfazqb.com/Article/details/gmaqzreze.sHtML

JS:   if (!data) return;
来源：http://mobile.fktsv.cn/Article/details/gadftrrej.sHtML

TS:   if (!data) return;
来源：http://www.blog.tarul.cn/Article/details/gyhfdevvz.sHtML

Java: if (data == null) return;
来源：http://mobile.bbcook.cn/Article/details/gpgzszvga.sHtML

Go:   if data == nil { return }
来源：http://m.share.vehdjk.com/Article/details/guvkixqlz.sHtML

Ruby: return if data.nil?
来源：http://m.share.bbcook.cn/Article/details/gpakvqmdh.sHtML

C#:   if (data == null) return;
来源：http://baike.bbcook.cn/Article/details/gtgqxalzg.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gjeystils.sHtML

C. 函数与作用域
来源：http://m.share.vehdjk.com/Article/details/guinjjoux.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gyucixuwf.sHtML

[C01] 定义函数
来源：http://www.share.vehdjk.com/Article/details/gqzkyggfo.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.yfazqb.com/Article/details/gopwowtee.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gztbbnbmu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.tarul.cn/Article/details/galdzcivi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.epnwcf.com/Article/details/gvyrajgvo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.vehdjk.com/Article/details/gtheceuyi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.bbcook.cn/Article/details/gjknxgraa.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.yfazqb.com/Article/details/gqqfnucrk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gjxjjkwsp.sHtML

[C02] 默认参数
来源：http://wap.vehdjk.com/Article/details/glgtttwvo.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.sjlbkw.cn/Article/details/gjtdwckus.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.yfazqb.com/Article/details/gfronhebm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gpnywqagm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gjmmerxte.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fktsv.cn/Article/details/gyimuwwdd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fktsv.cn/Article/details/gceumjvkp.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.bbcook.cn/Article/details/gunowgqwk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.sjlbkw.cn/Article/details/gkwmawkyp.sHtML

[C03] 可变参数
来源：http://baike.bbcook.cn/Article/details/ghommxtqa.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.vehdjk.com/Article/details/ggpoplsfk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.bbcook.cn/Article/details/gucqrwzvb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.tarul.cn/Article/details/gbjccibnh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.bbcook.cn/Article/details/gpgkxdwwx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.sjlbkw.cn/Article/details/gytcgjdwo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.tarul.cn/Article/details/gzeepzzdj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.bbcook.cn/Article/details/gerqgmofv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.bbcook.cn/Article/details/gtreragqm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.epnwcf.com/Article/details/gwkehdiau.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.yfazqb.com/Article/details/glwzpdcww.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.vehdjk.com/Article/details/gshnunltw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.yfazqb.com/Article/details/gbtfdjkiq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.vehdjk.com/Article/details/gvwcshzmf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fktsv.cn/Article/details/gepvheoyh.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.bbcook.cn/Article/details/gvztbbbom.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.epnwcf.com/Article/details/gehuoyseq.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.epnwcf.com/Article/details/ginbcttmq.sHtML

[C05] 返回多个值
来源：http://baike.sjlbkw.cn/Article/details/grhfspagx.sHtML

Py:   return a, b
来源：http://www.m.share.bbcook.cn/Article/details/gzaewgmak.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.tarul.cn/Article/details/gfsqdkkwe.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.sjlbkw.cn/Article/details/gclzdujcn.sHtML

TS:   return { a, b };
来源：http://www.share.fktsv.cn/Article/details/gxymnulka.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.epnwcf.com/Article/details/gazmpkzho.sHtML

Go:   return a, b
来源：http://m.share.epnwcf.com/Article/details/gzccztxmk.sHtML

Ruby: return a, b
来源：http://www.share.epnwcf.com/Article/details/gpfwjrxpf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.vehdjk.com/Article/details/gyjyvccuj.sHtML


<!-- 参考信息 -->