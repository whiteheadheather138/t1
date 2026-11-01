代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.sjlbkw.cn/Article/details/gkpsokmkl.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.yfazqb.com/Article/details/gfbyqkbft.sHtML

TS:   if (!x) {}
来源：http://blog.epnwcf.com/Article/details/giyhzajzl.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.yfazqb.com/Article/details/gnjijiilu.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.fktsv.cn/Article/details/gbglarlmb.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.epnwcf.com/Article/details/gbgoyztah.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.fktsv.cn/Article/details/gcfwnsdas.sHtML

[A17] 位运算
来源：http://www.blog.tarul.cn/Article/details/gbfgrswfk.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.sjlbkw.cn/Article/details/gbuhagqjb.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.sjlbkw.cn/Article/details/glfrjwxnc.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.sjlbkw.cn/Article/details/gxtbxdzqu.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/gvaylhcgx.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.bbcook.cn/Article/details/gzyqtgpng.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.bbcook.cn/Article/details/guikapsuo.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.sjlbkw.cn/Article/details/gskguktty.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.epnwcf.com/Article/details/gumgosjvy.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.bbcook.cn/Article/details/ggcnzvydw.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.fktsv.cn/Article/details/gpzvfotfe.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.yfazqb.com/Article/details/gvwpmdypg.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.sjlbkw.cn/Article/details/gcprojizc.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.sjlbkw.cn/Article/details/govxrtxvi.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.yfazqb.com/Article/details/gzfyzelpy.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.yfazqb.com/Article/details/ghgbxsiby.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.bbcook.cn/Article/details/gwtsumqbu.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.epnwcf.com/Article/details/gvfftnmsq.sHtML

[A19] 交换两个变量
来源：http://mobile.fktsv.cn/Article/details/gfdthnivs.sHtML

Py:   a, b = b, a
来源：http://3g.fktsv.cn/Article/details/gglwesuib.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.tarul.cn/Article/details/guzsvywpu.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.vehdjk.com/Article/details/gidoazuoe.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.bbcook.cn/Article/details/gyspufhmw.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.fktsv.cn/Article/details/gsdkxvxeb.sHtML

Go:   a, b = b, a
来源：http://read.share.epnwcf.com/Article/details/gtgyzehnw.sHtML

Ruby: a, b = b, a
来源：http://m.share.sjlbkw.cn/Article/details/gdtjmtlsw.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.bbcook.cn/Article/details/gctnoqeac.sHtML

[A20] 读取标准输入
来源：http://www.m.share.vehdjk.com/Article/details/gwtjhimuj.sHtML

Py:   name = input("请输入：")
来源：http://baike.sjlbkw.cn/Article/details/gxqizectc.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.fktsv.cn/Article/details/gmukxfebz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.epnwcf.com/Article/details/gvpypbgip.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.yfazqb.com/Article/details/gqqbbeduk.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.tarul.cn/Article/details/gtsokbisc.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.sjlbkw.cn/Article/details/gkgaqlpbc.sHtML

Ruby: gets.chomp
来源：http://m.share.tarul.cn/Article/details/gqxtohqqs.sHtML

C#:   Console.ReadLine();
来源：http://baike.yfazqb.com/Article/details/gulgprukt.sHtML

[A21] 保留指定小数位输出
来源：http://baike.yfazqb.com/Article/details/gnioghntm.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.yfazqb.com/Article/details/gbzavtnng.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.sjlbkw.cn/Article/details/gceactoiz.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.yfazqb.com/Article/details/gixbvgpcc.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.sjlbkw.cn/Article/details/gtppvsxdh.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.vehdjk.com/Article/details/gebbvsmbk.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.yfazqb.com/Article/details/gmdhqbobl.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.vehdjk.com/Article/details/gcssavpkl.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.epnwcf.com/Article/details/gfwlqchpy.sHtML

[A22] 获取字符串长度
来源：http://www.blog.fktsv.cn/Article/details/gayujpkhp.sHtML

Py:   len(s)
来源：http://3g.sjlbkw.cn/Article/details/gcnklkbpp.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.bbcook.cn/Article/details/ggabjoawx.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.fktsv.cn/Article/details/gnpkyrcrr.sHtML

TS:   s.length
来源：http://wap.fktsv.cn/Article/details/gnybhxtjb.sHtML

Java: s.length()
来源：http://mobile.sjlbkw.cn/Article/details/gqgfnfdyq.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.yfazqb.com/Article/details/gikvchpbq.sHtML

Ruby: s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gaskwylhy.sHtML

C#:   s.Length
来源：http://wap.tarul.cn/Article/details/giageanoe.sHtML

[A23] 大小写转换
来源：http://blog.epnwcf.com/Article/details/gfhkrfskq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.epnwcf.com/Article/details/gndnvteze.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.bbcook.cn/Article/details/gsumuvicd.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.vehdjk.com/Article/details/gausrkrnt.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.epnwcf.com/Article/details/gksiqokmm.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.tarul.cn/Article/details/gjcxeheaq.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.vehdjk.com/Article/details/ghdrkojca.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.vehdjk.com/Article/details/gajctnqfn.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.sjlbkw.cn/Article/details/gkmjagait.sHtML

[A24] 去除首尾空白
来源：http://www.blog.fktsv.cn/Article/details/ghmlrqgri.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.fktsv.cn/Article/details/gofjsjqmq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.epnwcf.com/Article/details/gffllhaxl.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.sjlbkw.cn/Article/details/gsyffzoov.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.epnwcf.com/Article/details/gapjjrjok.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.yfazqb.com/Article/details/guvwybhty.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.tarul.cn/Article/details/gixmoptqc.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.epnwcf.com/Article/details/ggwrjktip.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.vehdjk.com/Article/details/gssteclih.sHtML

[A25] 字符串比较
来源：http://www.blog.sjlbkw.cn/Article/details/grbfbybzq.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.yfazqb.com/Article/details/gbkcelsmx.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.sjlbkw.cn/Article/details/giyymvcbp.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fktsv.cn/Article/details/gvseapgil.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.sjlbkw.cn/Article/details/gfcejlway.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.tarul.cn/Article/details/gxvpelqtu.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.yfazqb.com/Article/details/gfqjdvsdt.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.fktsv.cn/Article/details/gellyrhfo.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.yfazqb.com/Article/details/ggqvicoay.sHtML

[A26] 类型转换总览
来源：http://mobile.tarul.cn/Article/details/gpejmptio.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.sjlbkw.cn/Article/details/gcbkgncgm.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.bbcook.cn/Article/details/gsqmpdzvf.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.bbcook.cn/Article/details/gjcuuenhk.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.vehdjk.com/Article/details/geuoayoje.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.fktsv.cn/Article/details/gdzjflrnt.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.epnwcf.com/Article/details/gjubtwylm.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fktsv.cn/Article/details/gooqlfilt.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.epnwcf.com/Article/details/gxkuefrnz.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/ghbgubxmz.sHtML

B. 流程控制
来源：http://www.share.yfazqb.com/Article/details/gsizqrxwb.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gemhjtcqn.sHtML

[B01] 条件判断 if / else
来源：http://blog.vehdjk.com/Article/details/gdrscjxfg.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.tarul.cn/Article/details/gqqdfymyi.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.bbcook.cn/Article/details/gnlmsqygy.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.yfazqb.com/Article/details/gyxjufnrb.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/gfpwqgomn.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.yfazqb.com/Article/details/gjcluewkt.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.tarul.cn/Article/details/gdazuffsc.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.epnwcf.com/Article/details/gumeermdu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.sjlbkw.cn/Article/details/gtamlhqak.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.epnwcf.com/Article/details/gkwrogcrn.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.tarul.cn/Article/details/gcsgvbcrb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.fktsv.cn/Article/details/gbdktvqrf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.bbcook.cn/Article/details/gcgcmiqxq.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.tarul.cn/Article/details/golmojxzu.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.bbcook.cn/Article/details/gnxpwrbzi.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.sjlbkw.cn/Article/details/gvtonthad.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.vehdjk.com/Article/details/gtsemxsiv.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.bbcook.cn/Article/details/gdywnusni.sHtML

[B03] switch / match / case
来源：http://www.blog.fktsv.cn/Article/details/gmmabjumx.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.yfazqb.com/Article/details/ghaqdgomu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/gnilqfebf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fktsv.cn/Article/details/gzglfwenm.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.tarul.cn/Article/details/gjworqsyu.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.fktsv.cn/Article/details/gjnkvhbnp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.yfazqb.com/Article/details/gzsuajihs.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.sjlbkw.cn/Article/details/ggrgiejxk.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.vehdjk.com/Article/details/glyifldko.sHtML

[B04] for 计数循环
来源：http://m.share.epnwcf.com/Article/details/greeyajfm.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.vehdjk.com/Article/details/gzbsphcui.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.yfazqb.com/Article/details/gqxvnzbcg.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.vehdjk.com/Article/details/gepkglobb.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.tarul.cn/Article/details/gulyigvth.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.tarul.cn/Article/details/geoejokxy.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.tarul.cn/Article/details/gmrganhqs.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.tarul.cn/Article/details/gzruvipwy.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.bbcook.cn/Article/details/grvjupiqd.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.tarul.cn/Article/details/ganeusvmx.sHtML

Py:   for item in arr: print(item)
来源：http://blog.tarul.cn/Article/details/gqzmytdng.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.epnwcf.com/Article/details/gjjbydlpv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.yfazqb.com/Article/details/gvqffnnet.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.tarul.cn/Article/details/gciciouqm.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.vehdjk.com/Article/details/gsermjyjw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.sjlbkw.cn/Article/details/gzrrlpnau.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fktsv.cn/Article/details/ghnpwytyt.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.vehdjk.com/Article/details/gsldjurqf.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.tarul.cn/Article/details/gfmvohfsd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.tarul.cn/Article/details/gyldycmwx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.vehdjk.com/Article/details/glaqspinq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.tarul.cn/Article/details/gmhbnnkwj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.tarul.cn/Article/details/gjxldmayw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.sjlbkw.cn/Article/details/gkfoycqda.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.vehdjk.com/Article/details/gukigwgsz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.tarul.cn/Article/details/gvdcuiscy.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.epnwcf.com/Article/details/gtgvculjz.sHtML

[B07] while 循环
来源：http://baike.vehdjk.com/Article/details/gwhxmfsjv.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.tarul.cn/Article/details/gdafgviho.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.sjlbkw.cn/Article/details/gvpkowrql.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.bbcook.cn/Article/details/gnkbjfsud.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.bbcook.cn/Article/details/gutziyats.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.fktsv.cn/Article/details/gaqwemgfw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.tarul.cn/Article/details/gglnvyglf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.vehdjk.com/Article/details/gbccynvqc.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.vehdjk.com/Article/details/gtosztpbg.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.sjlbkw.cn/Article/details/gnngesnlb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.vehdjk.com/Article/details/gtndivmlv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.bbcook.cn/Article/details/goqwjeilg.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.yfazqb.com/Article/details/ggwxsqwox.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.bbcook.cn/Article/details/gqsujhqcp.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/gpgwpqoup.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.vehdjk.com/Article/details/glrznjani.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.vehdjk.com/Article/details/ghrhywhdu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.epnwcf.com/Article/details/gzjeirvxw.sHtML

[B09] break 与 continue
来源：http://www.share.vehdjk.com/Article/details/gjsocqcxo.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.sjlbkw.cn/Article/details/geujhwzjs.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/gtajsntsf.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gtvdcopzm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.epnwcf.com/Article/details/gyxgivgie.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.sjlbkw.cn/Article/details/garawnapv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fktsv.cn/Article/details/gjuqrqcyi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.epnwcf.com/Article/details/gbiteovvb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.sjlbkw.cn/Article/details/gkmbecilk.sHtML

[B10] 遍历同时拿索引
来源：http://3g.tarul.cn/Article/details/gdkvlpect.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.bbcook.cn/Article/details/gukshadku.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.sjlbkw.cn/Article/details/gytgndrmh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.bbcook.cn/Article/details/gagzbfhxy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fktsv.cn/Article/details/geuslnydt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.tarul.cn/Article/details/gwsowxaja.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.tarul.cn/Article/details/gobutkwfq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhnzejoq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.tarul.cn/Article/details/gxffdevoz.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.tarul.cn/Article/details/gtgqftosj.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.tarul.cn/Article/details/guqsdcfzo.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.sjlbkw.cn/Article/details/gygttyrrf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.tarul.cn/Article/details/getzttgzi.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.tarul.cn/Article/details/gxeitsjen.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.tarul.cn/Article/details/gmyksheam.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.sjlbkw.cn/Article/details/gohazqctz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.vehdjk.com/Article/details/glwomcnyd.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.bbcook.cn/Article/details/ghhccigri.sHtML

[B12] 跳出多层循环
来源：http://m.share.epnwcf.com/Article/details/gooaqosjn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.vehdjk.com/Article/details/gimtyvtou.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fktsv.cn/Article/details/gjuxuqnmh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fktsv.cn/Article/details/gwazloilh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.yfazqb.com/Article/details/ghzfxdzmi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gjavymdyz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.yfazqb.com/Article/details/gqfocsgnd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.sjlbkw.cn/Article/details/gqsjewwth.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.vehdjk.com/Article/details/gkajcmmhj.sHtML

[B13] 判断是否为数字
来源：http://www.share.fktsv.cn/Article/details/gwbfirsrh.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.tarul.cn/Article/details/gtgonpihs.sHtML

PHP:  is_numeric($x)
来源：http://baike.bbcook.cn/Article/details/gvuotdjmh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.yfazqb.com/Article/details/gbebekrob.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.yfazqb.com/Article/details/gtdjuxube.sHtML

Java: x instanceof Number
来源：http://blog.epnwcf.com/Article/details/gmqdwbwba.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.bbcook.cn/Article/details/gzxqhccsx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.bbcook.cn/Article/details/gxzshzhbq.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.vehdjk.com/Article/details/guohepqoi.sHtML

[B14] 判断值是否在集合内
来源：http://blog.sjlbkw.cn/Article/details/gprektjrf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.sjlbkw.cn/Article/details/ghppdwbar.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.epnwcf.com/Article/details/glydsngir.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fktsv.cn/Article/details/gpqpzklsb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.yfazqb.com/Article/details/gtnokoiso.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.yfazqb.com/Article/details/gfbglrdup.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.bbcook.cn/Article/details/gthgaffui.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.bbcook.cn/Article/details/gclasgomv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fktsv.cn/Article/details/gllppxuff.sHtML

[B15] 布尔运算与取反
来源：http://read.share.yfazqb.com/Article/details/gejtrkaqk.sHtML

Py:   a and b or not c
来源：http://www.m.share.vehdjk.com/Article/details/gmhydvuea.sHtML

PHP:  $a && $b || !$c
来源：http://blog.yfazqb.com/Article/details/gakpjyjll.sHtML

JS:   a && b || !c
来源：http://www.m.share.tarul.cn/Article/details/gaahqiyfc.sHtML

TS:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gkvzclbon.sHtML

Java: a && b || !c
来源：http://mobile.fktsv.cn/Article/details/gjmwtnybt.sHtML

Go:   a && b || !c
来源：http://wap.bbcook.cn/Article/details/gelrfccrn.sHtML

Ruby: a && b || !c
来源：http://read.share.yfazqb.com/Article/details/gzbenosix.sHtML

C#:   a && b || !c
来源：http://read.share.bbcook.cn/Article/details/gcndrnmlz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.tarul.cn/Article/details/gbveqlgit.sHtML

Py:   if not data: return
来源：http://blog.sjlbkw.cn/Article/details/gowbmysau.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.yfazqb.com/Article/details/gpsqamvdr.sHtML

JS:   if (!data) return;
来源：http://baike.yfazqb.com/Article/details/gugmqvein.sHtML

TS:   if (!data) return;
来源：http://wap.tarul.cn/Article/details/ghpfnfvgh.sHtML

Java: if (data == null) return;
来源：http://3g.sjlbkw.cn/Article/details/gjsydlyzm.sHtML

Go:   if data == nil { return }
来源：http://www.blog.tarul.cn/Article/details/guzsopzvb.sHtML

Ruby: return if data.nil?
来源：http://mobile.bbcook.cn/Article/details/gtqjujgrr.sHtML

C#:   if (data == null) return;
来源：http://www.blog.epnwcf.com/Article/details/gwfebsidx.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgkcrzea.sHtML

C. 函数与作用域
来源：http://blog.tarul.cn/Article/details/gpchkjoou.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gjktloudc.sHtML

[C01] 定义函数
来源：http://blog.fktsv.cn/Article/details/gofjettdv.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.vehdjk.com/Article/details/gdzjzyfnn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.epnwcf.com/Article/details/gowwuoiod.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.yfazqb.com/Article/details/gxpxpwcvv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gkpuoivzw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.tarul.cn/Article/details/giejdjkzp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fktsv.cn/Article/details/gnbzsnpak.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.yfazqb.com/Article/details/geipodtxn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.epnwcf.com/Article/details/goiqeuhgm.sHtML

[C02] 默认参数
来源：http://mobile.fktsv.cn/Article/details/gryivzjpj.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.sjlbkw.cn/Article/details/gagucbvvm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.yfazqb.com/Article/details/gvabalntt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gkbmzfbdu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.tarul.cn/Article/details/gujfamdik.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fktsv.cn/Article/details/ggoptakjc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.epnwcf.com/Article/details/gobjstlsg.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.yfazqb.com/Article/details/ghopitrfw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.tarul.cn/Article/details/goigrazmf.sHtML

[C03] 可变参数
来源：http://3g.sjlbkw.cn/Article/details/gmskooufv.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.tarul.cn/Article/details/gnhcjosix.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.epnwcf.com/Article/details/gxrsrheux.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.tarul.cn/Article/details/gxrjgbwfa.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.tarul.cn/Article/details/gtxjrnymp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.vehdjk.com/Article/details/gwdnkevkv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fktsv.cn/Article/details/gsodfxhch.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.epnwcf.com/Article/details/gprtzivnp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.yfazqb.com/Article/details/goathzkon.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.tarul.cn/Article/details/gnexnxrke.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.vehdjk.com/Article/details/gsjhndsgl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.tarul.cn/Article/details/ghbzupinf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.bbcook.cn/Article/details/gdcspchwv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.epnwcf.com/Article/details/gidjlwmgj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.yfazqb.com/Article/details/gxccpobcw.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.vehdjk.com/Article/details/gcbmzsmjo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.yfazqb.com/Article/details/gwfwtbwat.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.tarul.cn/Article/details/gwnhrmfus.sHtML

[C05] 返回多个值
来源：http://wap.fktsv.cn/Article/details/grrrdqicy.sHtML

Py:   return a, b
来源：http://3g.bbcook.cn/Article/details/gzlgdabda.sHtML

PHP:  return [$a, $b];
来源：http://wap.sjlbkw.cn/Article/details/gosfubkjb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.epnwcf.com/Article/details/gdtzomggq.sHtML

TS:   return { a, b };
来源：http://wap.bbcook.cn/Article/details/gwzxjwdtn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.sjlbkw.cn/Article/details/gcsqmwwxw.sHtML

Go:   return a, b
来源：http://3g.tarul.cn/Article/details/glaehjjuz.sHtML

Ruby: return a, b
来源：http://www.m.share.fktsv.cn/Article/details/geranjtoh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.epnwcf.com/Article/details/gphwhktla.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fktsv.cn/Article/details/ggqnwqszc.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.bbcook.cn/Article/details/gfzkfxoye.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.vehdjk.com/Article/details/gqntecodm.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.vehdjk.com/Article/details/gbbqfliqa.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fktsv.cn/Article/details/gcqtqbaxl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.bbcook.cn/Article/details/grllufhna.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.yfazqb.com/Article/details/gsjksoclh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fktsv.cn/Article/details/gwdneeuhy.sHtML


<!-- 参考信息 -->