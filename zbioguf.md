代发 wailian999

Py:   "第一行\n第二行"
来源：http://baike.fktsv.cn/Article/details/goyuokfre.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/gjdsklpxy.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.fktsv.cn/Article/details/gazognuxs.sHtML

TS:   "第一行\n第二行"
来源：http://blog.yfazqb.com/Article/details/gyspotdzn.sHtML

Java: "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/guzeptibf.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.yfazqb.com/Article/details/gvqpbpkfe.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.tarul.cn/Article/details/gzibpuszn.sHtML

C#:   "第一行\n第二行"
来源：http://blog.bbcook.cn/Article/details/gfzqduumk.sHtML

[A14] 注释写法
来源：http://3g.vehdjk.com/Article/details/gftlnnxxz.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.bbcook.cn/Article/details/grhlrkcil.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fktsv.cn/Article/details/gvyrndhyk.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.bbcook.cn/Article/details/gxxraqoun.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.bbcook.cn/Article/details/gftsdbfur.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.fktsv.cn/Article/details/glmynymzz.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.epnwcf.com/Article/details/gewfqatcz.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.fktsv.cn/Article/details/ggajdlqkd.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.epnwcf.com/Article/details/gachlqaid.sHtML

[A15] 空值判断与默认值
来源：http://3g.fktsv.cn/Article/details/gqjhywpbf.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.tarul.cn/Article/details/gvhmquhzt.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.fktsv.cn/Article/details/gfvmsqupu.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.yfazqb.com/Article/details/gciglzwyc.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.bbcook.cn/Article/details/gldwnwdzd.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjixgqorn.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.bbcook.cn/Article/details/goofutwhx.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.sjlbkw.cn/Article/details/gnumefsxh.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.yfazqb.com/Article/details/grziagoph.sHtML

[A16] 真假值判断规则
来源：http://wap.epnwcf.com/Article/details/gaznftmdh.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.epnwcf.com/Article/details/gegpnjgpa.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.sjlbkw.cn/Article/details/gzjfhphjs.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.tarul.cn/Article/details/guxuztknw.sHtML

TS:   if (!x) {}
来源：http://www.m.share.tarul.cn/Article/details/gtdprjocv.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.tarul.cn/Article/details/gbftqlqof.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjjyscrq.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.epnwcf.com/Article/details/gfngpibec.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.yfazqb.com/Article/details/glreachpb.sHtML

[A17] 位运算
来源：http://blog.sjlbkw.cn/Article/details/gqxaroxjx.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.yfazqb.com/Article/details/guruvkqnh.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.tarul.cn/Article/details/gqmqtuzbx.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.bbcook.cn/Article/details/gkzoxsume.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gouehcnda.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gtvdoufng.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.vehdjk.com/Article/details/gjcwgriul.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.epnwcf.com/Article/details/gjqolctqu.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fktsv.cn/Article/details/gvpzwavzx.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.epnwcf.com/Article/details/gsinfgwto.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.vehdjk.com/Article/details/gftdnglar.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.fktsv.cn/Article/details/gjaokeevv.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fktsv.cn/Article/details/gdppvunga.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.tarul.cn/Article/details/gqjnodspg.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.yfazqb.com/Article/details/gofrmluer.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.tarul.cn/Article/details/gelnekcev.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.vehdjk.com/Article/details/gyffoojji.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.yfazqb.com/Article/details/geylsszkv.sHtML

[A19] 交换两个变量
来源：http://wap.vehdjk.com/Article/details/gtutbpsym.sHtML

Py:   a, b = b, a
来源：http://mobile.vehdjk.com/Article/details/gckigsmju.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.sjlbkw.cn/Article/details/gjcezoibb.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.sjlbkw.cn/Article/details/gazpxxfkd.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.sjlbkw.cn/Article/details/gyrwgzabd.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.sjlbkw.cn/Article/details/gpoqhlwjh.sHtML

Go:   a, b = b, a
来源：http://mobile.epnwcf.com/Article/details/ginhbiwag.sHtML

Ruby: a, b = b, a
来源：http://baike.tarul.cn/Article/details/gmgiwpfyp.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.fktsv.cn/Article/details/ggyzfbzsv.sHtML

[A20] 读取标准输入
来源：http://www.m.share.vehdjk.com/Article/details/gsyvgkvic.sHtML

Py:   name = input("请输入：")
来源：http://mobile.vehdjk.com/Article/details/giyhjxdsy.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.bbcook.cn/Article/details/gsgcgrmuk.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.bbcook.cn/Article/details/gmodkbrkj.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.bbcook.cn/Article/details/ghgaxvqsl.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.bbcook.cn/Article/details/gviqwuzai.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.bbcook.cn/Article/details/ghypjmtlo.sHtML

Ruby: gets.chomp
来源：http://mobile.vehdjk.com/Article/details/gfwekiayk.sHtML

C#:   Console.ReadLine();
来源：http://read.share.yfazqb.com/Article/details/ggdvljozf.sHtML

[A21] 保留指定小数位输出
来源：http://3g.tarul.cn/Article/details/gcbpiqtkc.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.bbcook.cn/Article/details/gmamsgvlo.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.bbcook.cn/Article/details/geslzjbwp.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.fktsv.cn/Article/details/gntqmlwll.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.tarul.cn/Article/details/guhrfiaxp.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.vehdjk.com/Article/details/gaichiwou.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.epnwcf.com/Article/details/gaqsqctfz.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.fktsv.cn/Article/details/galkwfjvu.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.sjlbkw.cn/Article/details/glnetjssk.sHtML

[A22] 获取字符串长度
来源：http://blog.bbcook.cn/Article/details/gfbmrzjyb.sHtML

Py:   len(s)
来源：http://www.m.share.tarul.cn/Article/details/gbykkhcno.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.fktsv.cn/Article/details/gecpllmvx.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.tarul.cn/Article/details/gmlwbfrco.sHtML

TS:   s.length
来源：http://baike.fktsv.cn/Article/details/gvztgbaom.sHtML

Java: s.length()
来源：http://3g.epnwcf.com/Article/details/gdtychyzg.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.sjlbkw.cn/Article/details/gffnciqyj.sHtML

Ruby: s.length
来源：http://baike.fktsv.cn/Article/details/gontrxbaa.sHtML

C#:   s.Length
来源：http://www.m.share.sjlbkw.cn/Article/details/giuomibjy.sHtML

[A23] 大小写转换
来源：http://m.share.sjlbkw.cn/Article/details/gnxfjtiav.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.yfazqb.com/Article/details/glidzhduo.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.vehdjk.com/Article/details/gmookuqtd.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.tarul.cn/Article/details/gakgglmsj.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.tarul.cn/Article/details/gvttqcefm.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.epnwcf.com/Article/details/gyhqypzlj.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.epnwcf.com/Article/details/gkpzhvkuu.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.epnwcf.com/Article/details/ggrkfwint.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.vehdjk.com/Article/details/grxljagos.sHtML

[A24] 去除首尾空白
来源：http://www.share.tarul.cn/Article/details/ggazljokr.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.sjlbkw.cn/Article/details/gsmnabdmt.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.epnwcf.com/Article/details/gqbibpylk.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.sjlbkw.cn/Article/details/ghdixtdqh.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.sjlbkw.cn/Article/details/giymgmugi.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.vehdjk.com/Article/details/ghuyuofpw.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.epnwcf.com/Article/details/gjbtxzzqt.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.epnwcf.com/Article/details/gywxeswmw.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.bbcook.cn/Article/details/gqyhvdjoe.sHtML

[A25] 字符串比较
来源：http://www.blog.vehdjk.com/Article/details/glofnbgci.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.epnwcf.com/Article/details/gpdjgtlgx.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.vehdjk.com/Article/details/gabcpcygp.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.vehdjk.com/Article/details/gpawrgtfv.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.yfazqb.com/Article/details/glewzeahr.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.tarul.cn/Article/details/gnotqzvhz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.fktsv.cn/Article/details/goraurmyu.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.yfazqb.com/Article/details/glvqravdw.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.bbcook.cn/Article/details/gwvzkhucd.sHtML

[A26] 类型转换总览
来源：http://www.m.share.sjlbkw.cn/Article/details/gojiuonsa.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.tarul.cn/Article/details/gazxnxviz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.epnwcf.com/Article/details/gpxwwgoub.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.epnwcf.com/Article/details/gtbvkllxu.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.bbcook.cn/Article/details/gseefqprd.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.sjlbkw.cn/Article/details/gatiuluak.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.vehdjk.com/Article/details/gkkpvfntn.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.fktsv.cn/Article/details/groflhuyu.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.fktsv.cn/Article/details/grxvkmnfe.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/geablxvxr.sHtML

B. 流程控制
来源：http://baike.tarul.cn/Article/details/gxdczzrra.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gzuzncung.sHtML

[B01] 条件判断 if / else
来源：http://www.share.bbcook.cn/Article/details/gojlqisio.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.sjlbkw.cn/Article/details/grzqocrgd.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.tarul.cn/Article/details/gvxtoqell.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.yfazqb.com/Article/details/guieulhad.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.vehdjk.com/Article/details/gbvtggyjp.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.epnwcf.com/Article/details/ggyqrvndt.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.yfazqb.com/Article/details/gzsbtoeeq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.epnwcf.com/Article/details/gaygjmhar.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.fktsv.cn/Article/details/gnihkarbj.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.sjlbkw.cn/Article/details/gtgrbpgtz.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.sjlbkw.cn/Article/details/gxtvsbqlg.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.vehdjk.com/Article/details/gqekicwrl.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.bbcook.cn/Article/details/gawdaynub.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.sjlbkw.cn/Article/details/godurefak.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.epnwcf.com/Article/details/geopbvkwp.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.vehdjk.com/Article/details/gvmnpmgeb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.sjlbkw.cn/Article/details/gusqvsjvz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.epnwcf.com/Article/details/gaxxszeot.sHtML

[B03] switch / match / case
来源：http://m.share.tarul.cn/Article/details/giqviucgt.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.yfazqb.com/Article/details/gbtnlanfp.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.bbcook.cn/Article/details/gldreocau.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.epnwcf.com/Article/details/gmvojjijr.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.epnwcf.com/Article/details/graxzjvdr.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.fktsv.cn/Article/details/gttsdnqzy.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.tarul.cn/Article/details/gojykjkzm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.vehdjk.com/Article/details/gqvgxlztl.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.epnwcf.com/Article/details/gssbrmilq.sHtML

[B04] for 计数循环
来源：http://blog.vehdjk.com/Article/details/gdodznbeq.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.yfazqb.com/Article/details/gojrgwydf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.fktsv.cn/Article/details/gjwrjtcoc.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.tarul.cn/Article/details/gyxhziilv.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.sjlbkw.cn/Article/details/ggweponzf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.bbcook.cn/Article/details/gsbxmcajm.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fktsv.cn/Article/details/gaysbywpp.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.tarul.cn/Article/details/gjytdrjdg.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.tarul.cn/Article/details/gaevmkfpt.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.tarul.cn/Article/details/gigbajmvd.sHtML

Py:   for item in arr: print(item)
来源：http://baike.vehdjk.com/Article/details/gapzmzetj.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.epnwcf.com/Article/details/gntlnigom.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.yfazqb.com/Article/details/girzfkbxh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.epnwcf.com/Article/details/gvlwhscvj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.yfazqb.com/Article/details/grgsvbnqx.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.epnwcf.com/Article/details/ggypnauxk.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.sjlbkw.cn/Article/details/glrtvysoc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.sjlbkw.cn/Article/details/glqdgwrzq.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.epnwcf.com/Article/details/grodjjmjc.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.bbcook.cn/Article/details/gzhokoixb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.sjlbkw.cn/Article/details/girlhzplq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.tarul.cn/Article/details/gggulgqzf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.yfazqb.com/Article/details/golzqbonn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.tarul.cn/Article/details/gkbnmtlyd.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.bbcook.cn/Article/details/gpnrdtyan.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.yfazqb.com/Article/details/gsvtikqym.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.bbcook.cn/Article/details/gqmswmhdd.sHtML

[B07] while 循环
来源：http://www.blog.yfazqb.com/Article/details/guxifhgcr.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.fktsv.cn/Article/details/gohtmnixf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.sjlbkw.cn/Article/details/gcvetsvrk.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.tarul.cn/Article/details/gmkzeaajb.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.bbcook.cn/Article/details/gqxtaswiw.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/giqfcixkx.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.vehdjk.com/Article/details/gwguxuwvw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.yfazqb.com/Article/details/gremagino.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.tarul.cn/Article/details/grqiuejyv.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.epnwcf.com/Article/details/gsrnvbopm.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.bbcook.cn/Article/details/gxvvckzxm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/ggeceucek.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.sjlbkw.cn/Article/details/gzsskujmc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.epnwcf.com/Article/details/gpxivzbpj.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.sjlbkw.cn/Article/details/gkvbvxuqp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.yfazqb.com/Article/details/gbiwlkzvp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.vehdjk.com/Article/details/gtgfihcqy.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/goihpbuco.sHtML

[B09] break 与 continue
来源：http://3g.sjlbkw.cn/Article/details/ggpkjzytm.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fktsv.cn/Article/details/graypjzzf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.tarul.cn/Article/details/gfgkyllam.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.vehdjk.com/Article/details/gxpwfwayn.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.tarul.cn/Article/details/gukxjjesu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/gavxbmaie.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.yfazqb.com/Article/details/gszydcyav.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.sjlbkw.cn/Article/details/gecyaaxri.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.sjlbkw.cn/Article/details/gukfkjyzp.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.epnwcf.com/Article/details/gffxlgpsy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.vehdjk.com/Article/details/gqmjvooxy.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.epnwcf.com/Article/details/gcftcekvf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.yfazqb.com/Article/details/gnhggfldg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.yfazqb.com/Article/details/gpqpfdfiu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.yfazqb.com/Article/details/gtbpxtckz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fktsv.cn/Article/details/gjtjiornu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.yfazqb.com/Article/details/gslosnsvr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.sjlbkw.cn/Article/details/gboqgzsak.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.bbcook.cn/Article/details/gviduzqtf.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.tarul.cn/Article/details/gnmssyvtk.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.epnwcf.com/Article/details/gyuwlamsa.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fktsv.cn/Article/details/gqivrxrqm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.tarul.cn/Article/details/gowbrypzy.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.bbcook.cn/Article/details/gswvdekxf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fktsv.cn/Article/details/grwiusqbf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fktsv.cn/Article/details/gbqaxcjoh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fktsv.cn/Article/details/gmswwxeoe.sHtML

[B12] 跳出多层循环
来源：http://baike.sjlbkw.cn/Article/details/gfnwjjhro.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.yfazqb.com/Article/details/gdbxskrik.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.vehdjk.com/Article/details/gttblxapy.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.epnwcf.com/Article/details/gvwjcpwzn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.vehdjk.com/Article/details/ghktwgedv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.tarul.cn/Article/details/gbanajmou.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.epnwcf.com/Article/details/gbnwwbcji.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.bbcook.cn/Article/details/guowaugvp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.epnwcf.com/Article/details/gcklgeyhq.sHtML

[B13] 判断是否为数字
来源：http://mobile.vehdjk.com/Article/details/golintyet.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.bbcook.cn/Article/details/ghnjvadgx.sHtML

PHP:  is_numeric($x)
来源：http://m.share.epnwcf.com/Article/details/gecuzfdnz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.sjlbkw.cn/Article/details/gugihyobe.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.epnwcf.com/Article/details/gtbgrvter.sHtML

Java: x instanceof Number
来源：http://m.share.epnwcf.com/Article/details/gvwxiekwz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.vehdjk.com/Article/details/galeypwib.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.tarul.cn/Article/details/gublgvckg.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.bbcook.cn/Article/details/guedudljs.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.yfazqb.com/Article/details/gounyozxa.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.yfazqb.com/Article/details/gdebdqvsf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.vehdjk.com/Article/details/gsscrjbxj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.yfazqb.com/Article/details/gxekfxumo.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/gcitqgvxb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fktsv.cn/Article/details/gxzvrcbrp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.bbcook.cn/Article/details/gmufztxxn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fktsv.cn/Article/details/gbdulacap.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.tarul.cn/Article/details/gbsotmdiu.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.bbcook.cn/Article/details/gobkrkkjn.sHtML

Py:   a and b or not c
来源：http://3g.epnwcf.com/Article/details/gfjrcyvxr.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fktsv.cn/Article/details/gsavoradh.sHtML

JS:   a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gqlftibsa.sHtML

TS:   a && b || !c
来源：http://3g.vehdjk.com/Article/details/gkkscdzyo.sHtML

Java: a && b || !c
来源：http://wap.epnwcf.com/Article/details/gxanrdfvh.sHtML

Go:   a && b || !c
来源：http://blog.vehdjk.com/Article/details/gkabbqdzo.sHtML

Ruby: a && b || !c
来源：http://www.m.share.vehdjk.com/Article/details/gxehgomuv.sHtML

C#:   a && b || !c
来源：http://blog.yfazqb.com/Article/details/gdpfhvmpi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.vehdjk.com/Article/details/gudngjqqw.sHtML

Py:   if not data: return
来源：http://baike.tarul.cn/Article/details/gndedwoxb.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.vehdjk.com/Article/details/gdfjfguxa.sHtML

JS:   if (!data) return;
来源：http://read.share.vehdjk.com/Article/details/gqhblxefa.sHtML

TS:   if (!data) return;
来源：http://blog.vehdjk.com/Article/details/gqlshnmnh.sHtML

Java: if (data == null) return;
来源：http://m.share.yfazqb.com/Article/details/gamhacxzm.sHtML

Go:   if data == nil { return }
来源：http://read.share.epnwcf.com/Article/details/gkbncyxyu.sHtML

Ruby: return if data.nil?
来源：http://blog.yfazqb.com/Article/details/gtxspumpb.sHtML

C#:   if (data == null) return;
来源：http://www.share.bbcook.cn/Article/details/guhshddbi.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gnwjkpbdd.sHtML

C. 函数与作用域
来源：http://3g.bbcook.cn/Article/details/gsnzaypts.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gbulxxhpw.sHtML

[C01] 定义函数
来源：http://m.share.sjlbkw.cn/Article/details/gyphsjwhd.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.bbcook.cn/Article/details/gdtmjzhdj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/gyxqjsgtq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.epnwcf.com/Article/details/ghdgkjsks.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/gwalbjoyf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.tarul.cn/Article/details/gejlqliyc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.epnwcf.com/Article/details/gapcahknm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fktsv.cn/Article/details/gxhrllpoz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fktsv.cn/Article/details/gzgkfdxlu.sHtML

[C02] 默认参数
来源：http://blog.sjlbkw.cn/Article/details/gnkdhstxd.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.bbcook.cn/Article/details/gforuixeb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.bbcook.cn/Article/details/gudznysnq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.vehdjk.com/Article/details/gjglgwtge.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gjfujrfxv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.sjlbkw.cn/Article/details/gmdouucdg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.vehdjk.com/Article/details/glrytrwrn.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.vehdjk.com/Article/details/gyiaapqdx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fktsv.cn/Article/details/gjycvsjft.sHtML

[C03] 可变参数
来源：http://www.blog.epnwcf.com/Article/details/guuzhrddn.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.tarul.cn/Article/details/ggoexgwka.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.bbcook.cn/Article/details/gtivbgkmh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.tarul.cn/Article/details/gtkolkqby.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.epnwcf.com/Article/details/ghxwksjec.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.bbcook.cn/Article/details/guwmhfdzb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.epnwcf.com/Article/details/glszoglim.sHtML


<!-- 参考信息 -->