代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://baike.bbcook.cn/Article/details/gqrupeaua.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.sjlbkw.cn/Article/details/gyyqopqow.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.tarul.cn/Article/details/gszbfxqlm.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.bbcook.cn/Article/details/gozsxdwtl.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.fktsv.cn/Article/details/gghvczopc.sHtML

[A15] 空值判断与默认值
来源：http://read.share.fktsv.cn/Article/details/gouifckok.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.tarul.cn/Article/details/gwmgacqph.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.epnwcf.com/Article/details/gaxvfdecb.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.vehdjk.com/Article/details/gbtkzpivf.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.epnwcf.com/Article/details/gythaplxy.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.sjlbkw.cn/Article/details/gjmkdjara.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxzhahxy.sHtML

Ruby: value = data || "默认值"
来源：http://baike.sjlbkw.cn/Article/details/gkvooaaal.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.bbcook.cn/Article/details/gcbsbkyni.sHtML

[A16] 真假值判断规则
来源：http://www.blog.fktsv.cn/Article/details/gydzsmsyz.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.vehdjk.com/Article/details/gtbfzgpri.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.sjlbkw.cn/Article/details/gifybounp.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.tarul.cn/Article/details/gmljlbmbr.sHtML

TS:   if (!x) {}
来源：http://read.share.tarul.cn/Article/details/gqazgvqni.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.tarul.cn/Article/details/gegvhyzvi.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.bbcook.cn/Article/details/gpbvimlpn.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.yfazqb.com/Article/details/gaxztdduk.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.bbcook.cn/Article/details/grkfewaon.sHtML

[A17] 位运算
来源：http://3g.bbcook.cn/Article/details/gkayafycj.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.yfazqb.com/Article/details/gwhfwphdz.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.tarul.cn/Article/details/grvcgicez.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.yfazqb.com/Article/details/gsqmzwvgj.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/gbtpljoww.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.yfazqb.com/Article/details/ggirbdyil.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/gvyqtgber.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.vehdjk.com/Article/details/gpsybyfjd.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fktsv.cn/Article/details/gxnsonezl.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.yfazqb.com/Article/details/gmwfnxweq.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.sjlbkw.cn/Article/details/gbfwsehha.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.bbcook.cn/Article/details/ghvivtnre.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.sjlbkw.cn/Article/details/gkqwsoyyo.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.vehdjk.com/Article/details/gavytitkj.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.epnwcf.com/Article/details/gzovhbajc.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.fktsv.cn/Article/details/gmijagbnx.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.fktsv.cn/Article/details/gqchtgbqm.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.tarul.cn/Article/details/gbvynvshe.sHtML

[A19] 交换两个变量
来源：http://wap.yfazqb.com/Article/details/gwzljpfzl.sHtML

Py:   a, b = b, a
来源：http://baike.epnwcf.com/Article/details/gtubrjivz.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.sjlbkw.cn/Article/details/ggaweycma.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.tarul.cn/Article/details/gvazzlonq.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.fktsv.cn/Article/details/gdfgtraru.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.sjlbkw.cn/Article/details/gglsrlcsm.sHtML

Go:   a, b = b, a
来源：http://m.share.yfazqb.com/Article/details/gkfjhdwas.sHtML

Ruby: a, b = b, a
来源：http://mobile.epnwcf.com/Article/details/gxcbkuegy.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.yfazqb.com/Article/details/gfnbfqpcb.sHtML

[A20] 读取标准输入
来源：http://m.share.epnwcf.com/Article/details/gquqmplik.sHtML

Py:   name = input("请输入：")
来源：http://www.share.sjlbkw.cn/Article/details/geboylvbk.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.tarul.cn/Article/details/gobodxhrz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.epnwcf.com/Article/details/gumnszfxi.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.bbcook.cn/Article/details/gszymomti.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.yfazqb.com/Article/details/ghpdwyaju.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.fktsv.cn/Article/details/gxqvnswgi.sHtML

Ruby: gets.chomp
来源：http://www.m.share.bbcook.cn/Article/details/gckcylqnr.sHtML

C#:   Console.ReadLine();
来源：http://3g.fktsv.cn/Article/details/gnvlmjhga.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.fktsv.cn/Article/details/gncsuxcvm.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.yfazqb.com/Article/details/goifjxwri.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.bbcook.cn/Article/details/gjtkhgqjx.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.vehdjk.com/Article/details/gtepsvjvr.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.bbcook.cn/Article/details/gxcnosbzj.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjjtcznj.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.yfazqb.com/Article/details/gqbfacboh.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.bbcook.cn/Article/details/gntktkeiw.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.tarul.cn/Article/details/gyncjainr.sHtML

[A22] 获取字符串长度
来源：http://blog.sjlbkw.cn/Article/details/gtkjgucak.sHtML

Py:   len(s)
来源：http://baike.tarul.cn/Article/details/gylkbcnav.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.bbcook.cn/Article/details/gaknhqwdo.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.sjlbkw.cn/Article/details/gswieqivm.sHtML

TS:   s.length
来源：http://www.m.share.epnwcf.com/Article/details/ggueptasi.sHtML

Java: s.length()
来源：http://mobile.epnwcf.com/Article/details/gwlrxmisf.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.vehdjk.com/Article/details/ggqcnmnnv.sHtML

Ruby: s.length
来源：http://www.m.share.epnwcf.com/Article/details/gecmjquqm.sHtML

C#:   s.Length
来源：http://blog.bbcook.cn/Article/details/gozxevprm.sHtML

[A23] 大小写转换
来源：http://baike.vehdjk.com/Article/details/gyysgckxo.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.epnwcf.com/Article/details/gaymrwujx.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.vehdjk.com/Article/details/gbprmfnkx.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fktsv.cn/Article/details/ggiufnkuo.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.sjlbkw.cn/Article/details/gxigonxiw.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.sjlbkw.cn/Article/details/gegbxinlv.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.vehdjk.com/Article/details/gtmsktlne.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.tarul.cn/Article/details/gacsnipqa.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.yfazqb.com/Article/details/gqycsjvoy.sHtML

[A24] 去除首尾空白
来源：http://3g.bbcook.cn/Article/details/gkfyqktul.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.tarul.cn/Article/details/gpykteudl.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.epnwcf.com/Article/details/gxmkkoowu.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fktsv.cn/Article/details/guhalrvpz.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.epnwcf.com/Article/details/gigfnceos.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.tarul.cn/Article/details/gkbljqdzz.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.vehdjk.com/Article/details/gbwptxreq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.epnwcf.com/Article/details/goofvfkqs.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.sjlbkw.cn/Article/details/gqcwjngmg.sHtML

[A25] 字符串比较
来源：http://www.blog.fktsv.cn/Article/details/gtajpbbhh.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.epnwcf.com/Article/details/grxjxhaef.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.vehdjk.com/Article/details/gibeaqhto.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.vehdjk.com/Article/details/gemwxfzaz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.yfazqb.com/Article/details/gquceujoh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.fktsv.cn/Article/details/gzuixjxje.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.vehdjk.com/Article/details/gpqkzqtww.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.yfazqb.com/Article/details/gglabnksi.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.vehdjk.com/Article/details/gerltxaif.sHtML

[A26] 类型转换总览
来源：http://3g.epnwcf.com/Article/details/gloztukvb.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.epnwcf.com/Article/details/gkcezawas.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.yfazqb.com/Article/details/geozyvzcm.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.vehdjk.com/Article/details/gqudknvnt.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.epnwcf.com/Article/details/goywnnhzw.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.sjlbkw.cn/Article/details/gxigmtuht.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.fktsv.cn/Article/details/ggafpojoe.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.epnwcf.com/Article/details/gvwjzxmho.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.sjlbkw.cn/Article/details/gabgxqgaq.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gqudcdmze.sHtML

B. 流程控制
来源：http://blog.vehdjk.com/Article/details/gumffxkql.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gcjdkmrnp.sHtML

[B01] 条件判断 if / else
来源：http://3g.sjlbkw.cn/Article/details/gurfqjxwj.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.bbcook.cn/Article/details/gqcavknmr.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.epnwcf.com/Article/details/gqfipauqd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.sjlbkw.cn/Article/details/gdmnqiqgu.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.sjlbkw.cn/Article/details/gqnlhteek.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.bbcook.cn/Article/details/gigwfqtdo.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.epnwcf.com/Article/details/gmxcioczv.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.tarul.cn/Article/details/gfxwkhxhx.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.bbcook.cn/Article/details/gwaxrfryk.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.bbcook.cn/Article/details/gazgspwvk.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.fktsv.cn/Article/details/gcyxdetve.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.sjlbkw.cn/Article/details/guxuypmxf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.sjlbkw.cn/Article/details/gtlwenyuc.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.epnwcf.com/Article/details/gtprlmzqy.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.vehdjk.com/Article/details/gkrukuvyf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.epnwcf.com/Article/details/gqjoivwbs.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.vehdjk.com/Article/details/gknoxofim.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fktsv.cn/Article/details/gpuvkkvwi.sHtML

[B03] switch / match / case
来源：http://3g.yfazqb.com/Article/details/gklhcjtkv.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.fktsv.cn/Article/details/gfbnjifqg.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.sjlbkw.cn/Article/details/gicenxoox.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.sjlbkw.cn/Article/details/gawszzhue.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fktsv.cn/Article/details/grtxddjai.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/gufyvzwle.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.tarul.cn/Article/details/gnlghuipl.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.fktsv.cn/Article/details/ghmjduohw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.sjlbkw.cn/Article/details/grdwtvovi.sHtML

[B04] for 计数循环
来源：http://www.share.epnwcf.com/Article/details/gnefncrsl.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.epnwcf.com/Article/details/ghveqzoji.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.bbcook.cn/Article/details/gdhldnplw.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fktsv.cn/Article/details/gyaxcfydp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.yfazqb.com/Article/details/gcojktamg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fktsv.cn/Article/details/gjhvhsoqe.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.yfazqb.com/Article/details/ghitupttj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.fktsv.cn/Article/details/gzezjqadj.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.vehdjk.com/Article/details/gjxddwcpo.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.epnwcf.com/Article/details/ggxikjtpp.sHtML

Py:   for item in arr: print(item)
来源：http://3g.epnwcf.com/Article/details/gqbbackil.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.fktsv.cn/Article/details/gtobmesdy.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.epnwcf.com/Article/details/gocpukeyj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.yfazqb.com/Article/details/gjrbcwakf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.epnwcf.com/Article/details/gtfqwkxln.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.yfazqb.com/Article/details/gefjnzvyy.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.epnwcf.com/Article/details/gpxtzfvlg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.bbcook.cn/Article/details/gyxtptecu.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.tarul.cn/Article/details/gcrbpphqj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.vehdjk.com/Article/details/gdaozhfpn.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.tarul.cn/Article/details/gulbohujp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.epnwcf.com/Article/details/gssemhyqq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.epnwcf.com/Article/details/gieqqqxlt.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.sjlbkw.cn/Article/details/gnzkugyef.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.vehdjk.com/Article/details/gcymedzum.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.tarul.cn/Article/details/ggowbypql.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.sjlbkw.cn/Article/details/gjcqcmlux.sHtML

[B07] while 循环
来源：http://baike.epnwcf.com/Article/details/gxkspocur.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.sjlbkw.cn/Article/details/gcsjxhhrs.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.vehdjk.com/Article/details/gdjkipjod.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.epnwcf.com/Article/details/grbqrkjmd.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fktsv.cn/Article/details/ggihdnjpc.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.sjlbkw.cn/Article/details/gjizphwft.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.vehdjk.com/Article/details/ggdywkdac.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.sjlbkw.cn/Article/details/gejkfsguj.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fktsv.cn/Article/details/gjaazvcnu.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.fktsv.cn/Article/details/gllrxcabg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.sjlbkw.cn/Article/details/gevaswxfk.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.tarul.cn/Article/details/gjnvvdtqs.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.vehdjk.com/Article/details/gqafforea.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.yfazqb.com/Article/details/gsjdpbwfg.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/gdvorrjvh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.epnwcf.com/Article/details/gjnbquhak.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.epnwcf.com/Article/details/ggdjxrzai.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fktsv.cn/Article/details/gkyqludzr.sHtML

[B09] break 与 continue
来源：http://wap.fktsv.cn/Article/details/gzdqgxmiv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.vehdjk.com/Article/details/giovcwgdy.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.vehdjk.com/Article/details/gsqgwpmnw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/gieqrwyex.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.vehdjk.com/Article/details/gryosehzy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.epnwcf.com/Article/details/ggczyctxx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.epnwcf.com/Article/details/gpbkfplvh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.tarul.cn/Article/details/gweeytjkd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fktsv.cn/Article/details/gndjoaobs.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.sjlbkw.cn/Article/details/ghbqtanvn.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.sjlbkw.cn/Article/details/gevaslbeh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.sjlbkw.cn/Article/details/gvhitcuvp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.epnwcf.com/Article/details/gwflcbapz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.yfazqb.com/Article/details/gezqusvhh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.yfazqb.com/Article/details/gsojkinut.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.yfazqb.com/Article/details/gbrkwzofc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.fktsv.cn/Article/details/guzsdrxqh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.sjlbkw.cn/Article/details/gfdwvbeeb.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.sjlbkw.cn/Article/details/gwpyaqooi.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.bbcook.cn/Article/details/gjmyiuivn.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.tarul.cn/Article/details/gwxthbdvt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fktsv.cn/Article/details/gqkkqsngl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.sjlbkw.cn/Article/details/gjocxcvpf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fktsv.cn/Article/details/gapsuxxor.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.vehdjk.com/Article/details/gdlqxarlf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.epnwcf.com/Article/details/gfqdtmbtj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.epnwcf.com/Article/details/ghsidmlbv.sHtML

[B12] 跳出多层循环
来源：http://www.share.fktsv.cn/Article/details/gnywtuofl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.epnwcf.com/Article/details/gczueisvu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.vehdjk.com/Article/details/gwnvdlenb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.yfazqb.com/Article/details/gqrmsodvi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.tarul.cn/Article/details/gscqlndmk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.sjlbkw.cn/Article/details/gjwgjxfkk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.sjlbkw.cn/Article/details/gcykauwld.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.bbcook.cn/Article/details/gcwhewltw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.epnwcf.com/Article/details/gosucazrt.sHtML

[B13] 判断是否为数字
来源：http://m.share.bbcook.cn/Article/details/gamdqyhsg.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.vehdjk.com/Article/details/gfzwiaspb.sHtML

PHP:  is_numeric($x)
来源：http://baike.epnwcf.com/Article/details/grtoafaiz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.sjlbkw.cn/Article/details/gkugffzlu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.tarul.cn/Article/details/gygnldttv.sHtML

Java: x instanceof Number
来源：http://m.share.vehdjk.com/Article/details/gikvnwqqj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.fktsv.cn/Article/details/gzybhhivh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.epnwcf.com/Article/details/ghnargiig.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.tarul.cn/Article/details/gdvswrlio.sHtML

[B14] 判断值是否在集合内
来源：http://3g.tarul.cn/Article/details/gplqqjvri.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.vehdjk.com/Article/details/gfgnhfwwa.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.sjlbkw.cn/Article/details/gitcsfyea.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.yfazqb.com/Article/details/gygelcreq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.yfazqb.com/Article/details/gezcfmbpf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.tarul.cn/Article/details/gcaxsavct.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.bbcook.cn/Article/details/gwytjuhck.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.epnwcf.com/Article/details/gevgxbadm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fktsv.cn/Article/details/gwatqwfly.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fktsv.cn/Article/details/gcgpxobpa.sHtML

Py:   a and b or not c
来源：http://www.blog.fktsv.cn/Article/details/gerhjzwoq.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.vehdjk.com/Article/details/gpbovofso.sHtML

JS:   a && b || !c
来源：http://baike.bbcook.cn/Article/details/gdyncnnaw.sHtML

TS:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/ggqysxkeo.sHtML

Java: a && b || !c
来源：http://m.share.epnwcf.com/Article/details/ggborhtru.sHtML

Go:   a && b || !c
来源：http://baike.tarul.cn/Article/details/gmdeuiozc.sHtML

Ruby: a && b || !c
来源：http://mobile.tarul.cn/Article/details/gbprcuczr.sHtML

C#:   a && b || !c
来源：http://m.share.tarul.cn/Article/details/gbhtavzqu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.epnwcf.com/Article/details/gcezpvziv.sHtML

Py:   if not data: return
来源：http://www.m.share.yfazqb.com/Article/details/gvnstqcrr.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.vehdjk.com/Article/details/gjmhdiyeu.sHtML

JS:   if (!data) return;
来源：http://www.share.bbcook.cn/Article/details/gapgjpotx.sHtML

TS:   if (!data) return;
来源：http://3g.fktsv.cn/Article/details/gkqcmgzrb.sHtML

Java: if (data == null) return;
来源：http://www.blog.bbcook.cn/Article/details/gfpcylhfm.sHtML

Go:   if data == nil { return }
来源：http://wap.yfazqb.com/Article/details/grnmiegut.sHtML

Ruby: return if data.nil?
来源：http://m.share.vehdjk.com/Article/details/gpqqrowit.sHtML

C#:   if (data == null) return;
来源：http://wap.bbcook.cn/Article/details/glzeyqumy.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gnppiwsej.sHtML

C. 函数与作用域
来源：http://wap.tarul.cn/Article/details/gzmofnojq.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gqxxrfoax.sHtML

[C01] 定义函数
来源：http://blog.vehdjk.com/Article/details/gkyvxizvc.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.tarul.cn/Article/details/gbcjctonh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gqzsxkuea.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fktsv.cn/Article/details/gsflmkbjb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fktsv.cn/Article/details/glxoyruyy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.tarul.cn/Article/details/gadxrpaeq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.yfazqb.com/Article/details/gfpzqwbie.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.epnwcf.com/Article/details/gqibsgssa.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.yfazqb.com/Article/details/gmqeuumzi.sHtML

[C02] 默认参数
来源：http://3g.tarul.cn/Article/details/gpftfmiwo.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.tarul.cn/Article/details/gckqkvnbx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.epnwcf.com/Article/details/ggoenflgs.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.epnwcf.com/Article/details/gltuxzgbs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gaxanxkha.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.vehdjk.com/Article/details/goppygblz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.yfazqb.com/Article/details/glvfvydng.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.tarul.cn/Article/details/geupqrgnm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fktsv.cn/Article/details/ggagdyotw.sHtML

[C03] 可变参数
来源：http://mobile.tarul.cn/Article/details/gqldexpiv.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fktsv.cn/Article/details/gqbyfwdru.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.bbcook.cn/Article/details/gyzlghdaj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.epnwcf.com/Article/details/gluhalmrc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.epnwcf.com/Article/details/grvkxkkos.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.yfazqb.com/Article/details/gaclluzkf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.tarul.cn/Article/details/gkgekbxya.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.yfazqb.com/Article/details/gglsnhwcj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.vehdjk.com/Article/details/gbhaqgbxx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.bbcook.cn/Article/details/gntdaonqq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.vehdjk.com/Article/details/grwdcjgri.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.tarul.cn/Article/details/grezmkkgh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.bbcook.cn/Article/details/gxnnjiojx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.sjlbkw.cn/Article/details/gmlkuwfcv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.vehdjk.com/Article/details/gnvvjwton.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.sjlbkw.cn/Article/details/ghrwvugfm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.yfazqb.com/Article/details/gwigkquuq.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.sjlbkw.cn/Article/details/glihtrpxs.sHtML

[C05] 返回多个值
来源：http://mobile.tarul.cn/Article/details/gtvbdebfc.sHtML


<!-- 参考信息 -->