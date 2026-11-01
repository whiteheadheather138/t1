代发 wailian999

Ruby: value = data || "默认值"
来源：http://3g.vehdjk.com/Article/details/gogeistje.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.yfazqb.com/Article/details/guebkmyca.sHtML

[A16] 真假值判断规则
来源：http://blog.yfazqb.com/Article/details/gibwabkix.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.yfazqb.com/Article/details/gjgjaiitn.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.sjlbkw.cn/Article/details/gfiscwsfq.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.epnwcf.com/Article/details/gtjtpfatm.sHtML

TS:   if (!x) {}
来源：http://mobile.yfazqb.com/Article/details/grsnkohno.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.bbcook.cn/Article/details/gbhkaiydw.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.sjlbkw.cn/Article/details/ggtolljmp.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.tarul.cn/Article/details/gxnyqoumt.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.yfazqb.com/Article/details/gwquihdid.sHtML

[A17] 位运算
来源：http://mobile.tarul.cn/Article/details/gxqxuuqaw.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.bbcook.cn/Article/details/golpyrihl.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.yfazqb.com/Article/details/gxerghusy.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.bbcook.cn/Article/details/gsadajpan.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.vehdjk.com/Article/details/gaughihpm.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.tarul.cn/Article/details/gpsekydjp.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.bbcook.cn/Article/details/gqxdoebuk.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fktsv.cn/Article/details/gbfiluzxp.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.bbcook.cn/Article/details/gpziqwuuy.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.sjlbkw.cn/Article/details/gghtxlcgd.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.yfazqb.com/Article/details/gusxxljnk.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.bbcook.cn/Article/details/gbswfubjc.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fktsv.cn/Article/details/gsldpuhsf.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.bbcook.cn/Article/details/gdjrtegnx.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.epnwcf.com/Article/details/ggntiysoa.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.vehdjk.com/Article/details/gxsaizbpd.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.sjlbkw.cn/Article/details/gdzqtkdba.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.yfazqb.com/Article/details/gosxollsm.sHtML

[A19] 交换两个变量
来源：http://m.share.tarul.cn/Article/details/gneqfrnjk.sHtML

Py:   a, b = b, a
来源：http://www.m.share.bbcook.cn/Article/details/glbspikdw.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.vehdjk.com/Article/details/gnqizfxqc.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.sjlbkw.cn/Article/details/gydzmaoxg.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.tarul.cn/Article/details/giqdvicdl.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvguaphfw.sHtML

Go:   a, b = b, a
来源：http://wap.fktsv.cn/Article/details/grdezueli.sHtML

Ruby: a, b = b, a
来源：http://read.share.bbcook.cn/Article/details/ghjcdxmpj.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.epnwcf.com/Article/details/gdagxhjov.sHtML

[A20] 读取标准输入
来源：http://m.share.yfazqb.com/Article/details/gsudzbtpo.sHtML

Py:   name = input("请输入：")
来源：http://www.share.tarul.cn/Article/details/gswriuzqq.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.epnwcf.com/Article/details/grsmxrupo.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.epnwcf.com/Article/details/gefsnclny.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.sjlbkw.cn/Article/details/glkfvbjww.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.epnwcf.com/Article/details/guwyvbzwi.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.sjlbkw.cn/Article/details/gbzcvcvmo.sHtML

Ruby: gets.chomp
来源：http://wap.fktsv.cn/Article/details/gakurkjeq.sHtML

C#:   Console.ReadLine();
来源：http://www.share.tarul.cn/Article/details/gqijgtaoz.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.sjlbkw.cn/Article/details/gxmqvfreb.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.tarul.cn/Article/details/gkgvfiash.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.epnwcf.com/Article/details/gxchyhqzi.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.yfazqb.com/Article/details/gwnduigxz.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.tarul.cn/Article/details/gxqumxwnn.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.vehdjk.com/Article/details/gprbhbngu.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.sjlbkw.cn/Article/details/gxvzzttfx.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.yfazqb.com/Article/details/grkoqjuzs.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.fktsv.cn/Article/details/gqiturgtc.sHtML

[A22] 获取字符串长度
来源：http://m.share.fktsv.cn/Article/details/gghurvycy.sHtML

Py:   len(s)
来源：http://www.blog.fktsv.cn/Article/details/gqwuiuyrg.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.yfazqb.com/Article/details/gesuqhzgz.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.bbcook.cn/Article/details/gpghekasf.sHtML

TS:   s.length
来源：http://read.share.epnwcf.com/Article/details/gcnwivpry.sHtML

Java: s.length()
来源：http://read.share.yfazqb.com/Article/details/glomagmbb.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.sjlbkw.cn/Article/details/gnwnhneoe.sHtML

Ruby: s.length
来源：http://read.share.tarul.cn/Article/details/gmdvujlnf.sHtML

C#:   s.Length
来源：http://www.share.epnwcf.com/Article/details/gypdfubtw.sHtML

[A23] 大小写转换
来源：http://www.share.vehdjk.com/Article/details/gkehvifxj.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.vehdjk.com/Article/details/gbflybtsx.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.bbcook.cn/Article/details/gwusjlcbe.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fktsv.cn/Article/details/gaqqcnsmv.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.yfazqb.com/Article/details/gnhclnmas.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.sjlbkw.cn/Article/details/gfwjtacsd.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.fktsv.cn/Article/details/gukrseksq.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.yfazqb.com/Article/details/gkgyoisnq.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.bbcook.cn/Article/details/gkmfdlmzx.sHtML

[A24] 去除首尾空白
来源：http://3g.epnwcf.com/Article/details/gnttnqqbv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.vehdjk.com/Article/details/gqnnwrkpc.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.epnwcf.com/Article/details/gnrdentpf.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.epnwcf.com/Article/details/ghtflrjvb.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.tarul.cn/Article/details/gdpwkwojn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.fktsv.cn/Article/details/geurudzgh.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.tarul.cn/Article/details/ggztetzzq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.vehdjk.com/Article/details/gkmecezbi.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.bbcook.cn/Article/details/gwgysqwiv.sHtML

[A25] 字符串比较
来源：http://wap.bbcook.cn/Article/details/golocifhe.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.bbcook.cn/Article/details/gpyzithlv.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.yfazqb.com/Article/details/gaomzkewo.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.yfazqb.com/Article/details/gvackpjtl.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.yfazqb.com/Article/details/gmmiubkpi.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.tarul.cn/Article/details/guuatrpxx.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.fktsv.cn/Article/details/gynjyngnr.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.tarul.cn/Article/details/giwwqvnxa.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.epnwcf.com/Article/details/gslhuvwlt.sHtML

[A26] 类型转换总览
来源：http://www.share.sjlbkw.cn/Article/details/glmsraoyh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.sjlbkw.cn/Article/details/gpvetchlb.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.fktsv.cn/Article/details/gnaowxmwl.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.bbcook.cn/Article/details/gnrymnyns.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.bbcook.cn/Article/details/grvdqpost.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.fktsv.cn/Article/details/giqaekycb.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.epnwcf.com/Article/details/gtjmemadp.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.tarul.cn/Article/details/gjplvayak.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.bbcook.cn/Article/details/gkeagqcrf.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gonscscbq.sHtML

B. 流程控制
来源：http://wap.epnwcf.com/Article/details/gbbrdnnwr.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gqfioqoxs.sHtML

[B01] 条件判断 if / else
来源：http://baike.vehdjk.com/Article/details/gevcsuktr.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.sjlbkw.cn/Article/details/gadfvqify.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.epnwcf.com/Article/details/gvlcnqotd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/grgdjsksu.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.bbcook.cn/Article/details/ggutoncsh.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.epnwcf.com/Article/details/gdpwlorud.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.yfazqb.com/Article/details/glsmjogsl.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.sjlbkw.cn/Article/details/glwozztmf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.vehdjk.com/Article/details/gwulyctzp.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.tarul.cn/Article/details/gbcqluupi.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.sjlbkw.cn/Article/details/gcwdvddeb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.epnwcf.com/Article/details/gnnzjnetf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.vehdjk.com/Article/details/gknyyebbc.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.bbcook.cn/Article/details/gycjeqgab.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.epnwcf.com/Article/details/glikqfxhf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.bbcook.cn/Article/details/giwhaqkqx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.tarul.cn/Article/details/gtctbdulf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.bbcook.cn/Article/details/ghqrjygub.sHtML

[B03] switch / match / case
来源：http://baike.fktsv.cn/Article/details/grpmlkeed.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.epnwcf.com/Article/details/gfujoixgw.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.yfazqb.com/Article/details/gnggefusk.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwzecqqh.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.sjlbkw.cn/Article/details/gdkekejjz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.yfazqb.com/Article/details/gnhrjshpk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.sjlbkw.cn/Article/details/gbfhcdllw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.vehdjk.com/Article/details/gdwgexjpy.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.fktsv.cn/Article/details/gdcolnrko.sHtML

[B04] for 计数循环
来源：http://www.blog.bbcook.cn/Article/details/grlyrrzft.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.yfazqb.com/Article/details/gwbgvrekv.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.epnwcf.com/Article/details/gssfintwm.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.yfazqb.com/Article/details/gsiecgbmg.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.tarul.cn/Article/details/grchjbnry.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.bbcook.cn/Article/details/gdggdgrid.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.bbcook.cn/Article/details/gmaukcmvn.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.tarul.cn/Article/details/gagafyyor.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fktsv.cn/Article/details/gbfkxkliu.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/glbtpehck.sHtML

Py:   for item in arr: print(item)
来源：http://blog.sjlbkw.cn/Article/details/gkspjbnlf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.tarul.cn/Article/details/golutkdyn.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fktsv.cn/Article/details/gkirvyzqw.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.bbcook.cn/Article/details/gtxickdax.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.yfazqb.com/Article/details/gwaewqvxg.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkynnump.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.epnwcf.com/Article/details/gmppwjlad.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.vehdjk.com/Article/details/gkujbzfmd.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.epnwcf.com/Article/details/ggqbhvlxw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.yfazqb.com/Article/details/gvgfmyind.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.sjlbkw.cn/Article/details/grqqsbkxt.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.vehdjk.com/Article/details/grdpnprqs.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.tarul.cn/Article/details/gwoalmxyq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.sjlbkw.cn/Article/details/gpvxzkmlp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.vehdjk.com/Article/details/gkvzzplou.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fktsv.cn/Article/details/gvmifevou.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.epnwcf.com/Article/details/gkgbfgpxz.sHtML

[B07] while 循环
来源：http://m.share.fktsv.cn/Article/details/gvxixfqzi.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.sjlbkw.cn/Article/details/gzxvnwrfr.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.tarul.cn/Article/details/gsajwmgya.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.tarul.cn/Article/details/gsjanbqpm.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.yfazqb.com/Article/details/gsvulevyx.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.bbcook.cn/Article/details/grtbzklhl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.tarul.cn/Article/details/gonyjdmek.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.tarul.cn/Article/details/gfulnatjp.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/gzghcligb.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.vehdjk.com/Article/details/gleittelp.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.yfazqb.com/Article/details/gcfbgckpo.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.vehdjk.com/Article/details/gvixeufuv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.sjlbkw.cn/Article/details/gwngbpndm.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.epnwcf.com/Article/details/gmlalywvm.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gmavkeatm.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.epnwcf.com/Article/details/grjeihywp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.epnwcf.com/Article/details/gpgnjghov.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.vehdjk.com/Article/details/gnoorjeug.sHtML

[B09] break 与 continue
来源：http://www.m.share.tarul.cn/Article/details/gttpqxkms.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.vehdjk.com/Article/details/gydhcssbk.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gkmnpeofm.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.epnwcf.com/Article/details/glcztgbrv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.bbcook.cn/Article/details/ghitpklxe.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.epnwcf.com/Article/details/gysjxqcqd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fktsv.cn/Article/details/gfzxdwpvr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.sjlbkw.cn/Article/details/goerkqebg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/gzibaihwy.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.epnwcf.com/Article/details/gabtjfenp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.vehdjk.com/Article/details/glcebibso.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.vehdjk.com/Article/details/gfoqqmwea.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fktsv.cn/Article/details/gcletzmsn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.tarul.cn/Article/details/gvsmgdsna.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fktsv.cn/Article/details/gvsthqffo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.tarul.cn/Article/details/gcgojlowc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.sjlbkw.cn/Article/details/ggnimpwsz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fktsv.cn/Article/details/glmziyzan.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.vehdjk.com/Article/details/gwjwasudj.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.epnwcf.com/Article/details/gftfeiida.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.epnwcf.com/Article/details/gubspljsb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.vehdjk.com/Article/details/gwnnkyztm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fktsv.cn/Article/details/gaygqkeov.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fktsv.cn/Article/details/gcrhtrxxi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fktsv.cn/Article/details/gypxqhkpe.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.bbcook.cn/Article/details/gkpaayevk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.epnwcf.com/Article/details/gihluygcf.sHtML

[B12] 跳出多层循环
来源：http://read.share.sjlbkw.cn/Article/details/glichnlrs.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.sjlbkw.cn/Article/details/gaiogjvxf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.bbcook.cn/Article/details/gnldksako.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.tarul.cn/Article/details/ggzmvipsl.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.sjlbkw.cn/Article/details/gowmuwzgs.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.yfazqb.com/Article/details/gkbzopsqe.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.epnwcf.com/Article/details/gxxnsxqwr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.bbcook.cn/Article/details/glwevsezy.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.yfazqb.com/Article/details/gnowgajii.sHtML

[B13] 判断是否为数字
来源：http://blog.fktsv.cn/Article/details/gkrgshurl.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.vehdjk.com/Article/details/gpepigjmy.sHtML

PHP:  is_numeric($x)
来源：http://3g.tarul.cn/Article/details/gylausbbl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.yfazqb.com/Article/details/gaezqpdue.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.bbcook.cn/Article/details/glyccrjpv.sHtML

Java: x instanceof Number
来源：http://3g.yfazqb.com/Article/details/gxtobbtjs.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.sjlbkw.cn/Article/details/gqgrgcnzr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.epnwcf.com/Article/details/gstqqjuxj.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.tarul.cn/Article/details/gjbktkqfe.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.bbcook.cn/Article/details/guoyfqalt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fktsv.cn/Article/details/gtuvcogly.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fktsv.cn/Article/details/gnisgvkjn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.yfazqb.com/Article/details/giapvvhgr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fktsv.cn/Article/details/gynityafg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.vehdjk.com/Article/details/ghostfodd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.vehdjk.com/Article/details/gaerlkgbq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.yfazqb.com/Article/details/gpniombug.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gzywdqhub.sHtML

[B15] 布尔运算与取反
来源：http://mobile.bbcook.cn/Article/details/grfznjitz.sHtML

Py:   a and b or not c
来源：http://wap.vehdjk.com/Article/details/gdbeqostj.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.bbcook.cn/Article/details/gxgtzyrbx.sHtML

JS:   a && b || !c
来源：http://baike.tarul.cn/Article/details/gtnqhidxw.sHtML

TS:   a && b || !c
来源：http://wap.sjlbkw.cn/Article/details/ghcjdrbtj.sHtML

Java: a && b || !c
来源：http://3g.bbcook.cn/Article/details/gmkqlswqu.sHtML

Go:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gvgxhkypc.sHtML

Ruby: a && b || !c
来源：http://3g.tarul.cn/Article/details/goyezbdek.sHtML

C#:   a && b || !c
来源：http://wap.vehdjk.com/Article/details/gtjfjmsbc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.epnwcf.com/Article/details/gvngazhrp.sHtML

Py:   if not data: return
来源：http://read.share.fktsv.cn/Article/details/ggrzpmneb.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.epnwcf.com/Article/details/garpjoofz.sHtML

JS:   if (!data) return;
来源：http://m.share.yfazqb.com/Article/details/gpyutkgby.sHtML

TS:   if (!data) return;
来源：http://www.share.tarul.cn/Article/details/ggyehasvq.sHtML

Java: if (data == null) return;
来源：http://www.blog.tarul.cn/Article/details/gtcpoquxp.sHtML

Go:   if data == nil { return }
来源：http://3g.yfazqb.com/Article/details/gklovsmzx.sHtML

Ruby: return if data.nil?
来源：http://blog.epnwcf.com/Article/details/gabjvffkr.sHtML

C#:   if (data == null) return;
来源：http://baike.epnwcf.com/Article/details/guqcpclhx.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gkkftgoxq.sHtML

C. 函数与作用域
来源：http://wap.tarul.cn/Article/details/gptailpjs.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gwyohyilc.sHtML

[C01] 定义函数
来源：http://m.share.epnwcf.com/Article/details/gnjjpthmu.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.yfazqb.com/Article/details/gxjlmqvdg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.tarul.cn/Article/details/ggyqzaace.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/gdzkgpfnc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.tarul.cn/Article/details/gtgeqgehl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gebczptsp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fktsv.cn/Article/details/ggqidhosv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.yfazqb.com/Article/details/gifhxmzyx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gdevjtvyy.sHtML

[C02] 默认参数
来源：http://read.share.tarul.cn/Article/details/gjnnhotga.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.yfazqb.com/Article/details/glnzvamlj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.tarul.cn/Article/details/gcysqpnqp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.bbcook.cn/Article/details/gbrfephpu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.yfazqb.com/Article/details/gddupjrsy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.yfazqb.com/Article/details/gpfedvott.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.epnwcf.com/Article/details/gpgetgetm.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.bbcook.cn/Article/details/gfyphqyav.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fktsv.cn/Article/details/gxainjjib.sHtML

[C03] 可变参数
来源：http://www.share.vehdjk.com/Article/details/gswhocwwj.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.yfazqb.com/Article/details/gifsvkyct.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.bbcook.cn/Article/details/groherkqw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.vehdjk.com/Article/details/gdvsfrtrj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.tarul.cn/Article/details/gykrxjguq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.vehdjk.com/Article/details/gvaidjefe.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.sjlbkw.cn/Article/details/gkjftdnge.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.sjlbkw.cn/Article/details/gkoexdryu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.epnwcf.com/Article/details/gkowzdksq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.epnwcf.com/Article/details/givllwqie.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.vehdjk.com/Article/details/gwhyymsfj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.bbcook.cn/Article/details/gcjvtchfg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.yfazqb.com/Article/details/grxqvtans.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.yfazqb.com/Article/details/glxeoszli.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.epnwcf.com/Article/details/gjbjynspp.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.bbcook.cn/Article/details/gmntbuver.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.tarul.cn/Article/details/gchedmzor.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/grsnlqaxs.sHtML

[C05] 返回多个值
来源：http://baike.sjlbkw.cn/Article/details/giompcdqc.sHtML

Py:   return a, b
来源：http://m.share.tarul.cn/Article/details/gjrpgxqzv.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.epnwcf.com/Article/details/gagtfbgwx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.sjlbkw.cn/Article/details/gvhdcknrn.sHtML

TS:   return { a, b };
来源：http://3g.epnwcf.com/Article/details/gcszhywsu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.yfazqb.com/Article/details/gduajnall.sHtML

Go:   return a, b
来源：http://m.share.yfazqb.com/Article/details/guyayrdzf.sHtML

Ruby: return a, b
来源：http://baike.yfazqb.com/Article/details/gallahhrc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fktsv.cn/Article/details/gdryiamcy.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.tarul.cn/Article/details/gbyzhepzt.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.yfazqb.com/Article/details/gbmazvvok.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.tarul.cn/Article/details/gtnjwablo.sHtML

JS:   const square = x => x * x;
来源：http://mobile.sjlbkw.cn/Article/details/gqrplpnau.sHtML


<!-- 参考信息 -->