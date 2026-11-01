代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.yfazqb.com/Article/details/gfkkuqdji.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.epnwcf.com/Article/details/gagpyouui.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.vehdjk.com/Article/details/gixwydhob.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.vehdjk.com/Article/details/gtgoupwbd.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.vehdjk.com/Article/details/gcsfdhvmd.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.sjlbkw.cn/Article/details/gbxhnhjuh.sHtML

JS:   "第一行\n第二行"
来源：http://blog.yfazqb.com/Article/details/gywmnqmaw.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.tarul.cn/Article/details/gaftdffgc.sHtML

Java: "第一行\n第二行"
来源：http://blog.vehdjk.com/Article/details/gokkiuter.sHtML

Go:   "第一行\n第二行"
来源：http://baike.yfazqb.com/Article/details/gazdqaimj.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.yfazqb.com/Article/details/grdmzhxkw.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fktsv.cn/Article/details/ghgmrober.sHtML

[A14] 注释写法
来源：http://m.share.bbcook.cn/Article/details/glhkvnjkw.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.vehdjk.com/Article/details/gyeunjnod.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.epnwcf.com/Article/details/gvfdlsqkt.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.vehdjk.com/Article/details/gpqqmscnw.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.tarul.cn/Article/details/gvlystchg.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.vehdjk.com/Article/details/gpkqkcwuj.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.bbcook.cn/Article/details/grpzvdixd.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.epnwcf.com/Article/details/gkewsjfne.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.sjlbkw.cn/Article/details/ggugzvzdg.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.tarul.cn/Article/details/gxeodrlot.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.tarul.cn/Article/details/gxqlrfglt.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.epnwcf.com/Article/details/gztzgjpmw.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.sjlbkw.cn/Article/details/gwfvhybzu.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.sjlbkw.cn/Article/details/gyttutmsi.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.bbcook.cn/Article/details/giebofpgm.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.epnwcf.com/Article/details/gmfkqzszk.sHtML

Ruby: value = data || "默认值"
来源：http://baike.fktsv.cn/Article/details/gxhxfjsth.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.bbcook.cn/Article/details/ghmsglxzj.sHtML

[A16] 真假值判断规则
来源：http://blog.vehdjk.com/Article/details/girhanblb.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.epnwcf.com/Article/details/gvickmzic.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.tarul.cn/Article/details/gyuhblpab.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.yfazqb.com/Article/details/gnumvshfn.sHtML

TS:   if (!x) {}
来源：http://3g.bbcook.cn/Article/details/gqwnkztjr.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.sjlbkw.cn/Article/details/gkcpgraqw.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.vehdjk.com/Article/details/gnmfhkhvc.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.fktsv.cn/Article/details/giuxuvtql.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.yfazqb.com/Article/details/gcycgrxtw.sHtML

[A17] 位运算
来源：http://www.blog.tarul.cn/Article/details/gkrkrjamb.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.tarul.cn/Article/details/gobsqbrgu.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.vehdjk.com/Article/details/gqrzmwnkl.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.bbcook.cn/Article/details/gpmubwkaw.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.bbcook.cn/Article/details/gkeqgttkl.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.bbcook.cn/Article/details/gyretrias.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.vehdjk.com/Article/details/gwmnkcygj.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.epnwcf.com/Article/details/gmbwmptpn.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.epnwcf.com/Article/details/girpdbijh.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.fktsv.cn/Article/details/ghxgmacaf.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.yfazqb.com/Article/details/gcfepjipg.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.yfazqb.com/Article/details/gwnyszett.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.tarul.cn/Article/details/gykpvmped.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.vehdjk.com/Article/details/guapqhtql.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.yfazqb.com/Article/details/gwzcnimup.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.fktsv.cn/Article/details/gjcmylzvv.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.epnwcf.com/Article/details/gwfqkevzm.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.bbcook.cn/Article/details/gwfinbrac.sHtML

[A19] 交换两个变量
来源：http://read.share.sjlbkw.cn/Article/details/gzddcxrou.sHtML

Py:   a, b = b, a
来源：http://www.m.share.epnwcf.com/Article/details/gucqclkkw.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.tarul.cn/Article/details/gggbfyogn.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.sjlbkw.cn/Article/details/gqbkfrvme.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.vehdjk.com/Article/details/gizangrfv.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.sjlbkw.cn/Article/details/gsejzwaao.sHtML

Go:   a, b = b, a
来源：http://m.share.epnwcf.com/Article/details/ggnhooxul.sHtML

Ruby: a, b = b, a
来源：http://read.share.epnwcf.com/Article/details/golsujpac.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.epnwcf.com/Article/details/gyoibeijb.sHtML

[A20] 读取标准输入
来源：http://wap.epnwcf.com/Article/details/gfbstziyp.sHtML

Py:   name = input("请输入：")
来源：http://www.share.vehdjk.com/Article/details/gayujcbsf.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.bbcook.cn/Article/details/gldwpdyla.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.yfazqb.com/Article/details/gfqqmpvxn.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.sjlbkw.cn/Article/details/gwybfeyxi.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.fktsv.cn/Article/details/grcsylbnz.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.epnwcf.com/Article/details/gbeshuxjf.sHtML

Ruby: gets.chomp
来源：http://mobile.bbcook.cn/Article/details/gtpemmpzh.sHtML

C#:   Console.ReadLine();
来源：http://read.share.vehdjk.com/Article/details/gilpwkaxd.sHtML

[A21] 保留指定小数位输出
来源：http://3g.epnwcf.com/Article/details/gkixpgqwf.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.bbcook.cn/Article/details/glymzzorq.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.yfazqb.com/Article/details/gicukwrqz.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.sjlbkw.cn/Article/details/gnnmgzunr.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.vehdjk.com/Article/details/grvlbnjtv.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.vehdjk.com/Article/details/grqzydjha.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.vehdjk.com/Article/details/gviwekgfk.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.epnwcf.com/Article/details/guenmbpgj.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.epnwcf.com/Article/details/gpjispcei.sHtML

[A22] 获取字符串长度
来源：http://www.blog.bbcook.cn/Article/details/gvnnerugi.sHtML

Py:   len(s)
来源：http://read.share.vehdjk.com/Article/details/gsonwbzkw.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.tarul.cn/Article/details/gtsbmcicd.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.vehdjk.com/Article/details/gwnuoknpc.sHtML

TS:   s.length
来源：http://mobile.vehdjk.com/Article/details/gnptbueqi.sHtML

Java: s.length()
来源：http://www.share.tarul.cn/Article/details/geezkbvha.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.sjlbkw.cn/Article/details/geztcxozs.sHtML

Ruby: s.length
来源：http://www.share.bbcook.cn/Article/details/gzeueazda.sHtML

C#:   s.Length
来源：http://read.share.tarul.cn/Article/details/gmdwhprkx.sHtML

[A23] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/geclrfcbd.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.vehdjk.com/Article/details/ggdsurbjm.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.epnwcf.com/Article/details/gftvuirte.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.sjlbkw.cn/Article/details/ghdfhbtcy.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.sjlbkw.cn/Article/details/gbhudfvyc.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.sjlbkw.cn/Article/details/gkjqpsfur.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.sjlbkw.cn/Article/details/gpnuimbnr.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.yfazqb.com/Article/details/gsfgkfhio.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.fktsv.cn/Article/details/gdxoucmbt.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.sjlbkw.cn/Article/details/ghkrjstld.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.tarul.cn/Article/details/gohpjocqc.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.tarul.cn/Article/details/grutingqa.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.bbcook.cn/Article/details/gsfdylyqi.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.sjlbkw.cn/Article/details/gxuxnmbgc.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.tarul.cn/Article/details/gpudiafgy.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.bbcook.cn/Article/details/gbappfmhf.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.tarul.cn/Article/details/gxfulyyug.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.vehdjk.com/Article/details/goklyxejb.sHtML

[A25] 字符串比较
来源：http://www.share.epnwcf.com/Article/details/gssnpaqet.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.sjlbkw.cn/Article/details/gnzerjixv.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.tarul.cn/Article/details/gfdgbrrdj.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.tarul.cn/Article/details/gpbzeglss.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.sjlbkw.cn/Article/details/gstfelbzm.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.yfazqb.com/Article/details/gjkpphfuh.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.epnwcf.com/Article/details/grzldbnlt.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.fktsv.cn/Article/details/gecznikpm.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fktsv.cn/Article/details/gzazmbama.sHtML

[A26] 类型转换总览
来源：http://baike.vehdjk.com/Article/details/gykofymwz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.yfazqb.com/Article/details/gvprhakdj.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.sjlbkw.cn/Article/details/guxirdobn.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.fktsv.cn/Article/details/gbdzxpzuz.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.epnwcf.com/Article/details/gtdynlgzc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.epnwcf.com/Article/details/gesrpxxix.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.vehdjk.com/Article/details/gjyennljl.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.vehdjk.com/Article/details/gvbldxbgf.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.bbcook.cn/Article/details/gtakobnop.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/grpjgfjvi.sHtML

B. 流程控制
来源：http://www.blog.tarul.cn/Article/details/ghzlnyarq.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gnrheknyy.sHtML

[B01] 条件判断 if / else
来源：http://baike.vehdjk.com/Article/details/gbwxkycry.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.vehdjk.com/Article/details/gttzwkewp.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.yfazqb.com/Article/details/gjwvmymfs.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.tarul.cn/Article/details/gsftjwfsb.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fktsv.cn/Article/details/gpmbglvsf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.sjlbkw.cn/Article/details/gktikahxg.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.bbcook.cn/Article/details/gixwxwqpc.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.bbcook.cn/Article/details/ggdfwmzgf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.yfazqb.com/Article/details/gtbhacyuu.sHtML

[B02] 多分支 else if / elif
来源：http://3g.fktsv.cn/Article/details/gfwlewpsv.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.fktsv.cn/Article/details/gomgdcgvm.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.epnwcf.com/Article/details/gprittlfh.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fktsv.cn/Article/details/geiozwyha.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.sjlbkw.cn/Article/details/gojtnqvtp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.tarul.cn/Article/details/gjmyockey.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.tarul.cn/Article/details/gxktemhzy.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.vehdjk.com/Article/details/gnzgvofbk.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fktsv.cn/Article/details/gqvjroabu.sHtML

[B03] switch / match / case
来源：http://wap.sjlbkw.cn/Article/details/gbhcakpwz.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.fktsv.cn/Article/details/gemhuasov.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.bbcook.cn/Article/details/gmycxkjsf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.yfazqb.com/Article/details/giipwktin.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.bbcook.cn/Article/details/geiggdznm.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.fktsv.cn/Article/details/gwxctuyia.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.fktsv.cn/Article/details/gwyzlywrl.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.fktsv.cn/Article/details/gviyaquau.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.fktsv.cn/Article/details/ghzazjgbk.sHtML

[B04] for 计数循环
来源：http://m.share.sjlbkw.cn/Article/details/gsmelgimx.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.sjlbkw.cn/Article/details/gntezmigq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.tarul.cn/Article/details/gqssnpjfi.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.sjlbkw.cn/Article/details/gqrjwiyif.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fktsv.cn/Article/details/gdmolkwsp.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.bbcook.cn/Article/details/gqloaezif.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.vehdjk.com/Article/details/gmvwzurpo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.tarul.cn/Article/details/gucttyvhi.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.vehdjk.com/Article/details/gcreyzbgk.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.tarul.cn/Article/details/gjuvxbuvi.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.bbcook.cn/Article/details/gsigxpnir.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.epnwcf.com/Article/details/gvtuavndo.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.bbcook.cn/Article/details/ggzzjxrrn.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.bbcook.cn/Article/details/ghivrzibg.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.fktsv.cn/Article/details/ggotvswhn.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.yfazqb.com/Article/details/gdguqladi.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.yfazqb.com/Article/details/gmsxqeaxq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.yfazqb.com/Article/details/gulhqeapk.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.bbcook.cn/Article/details/gazvrsrcj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.bbcook.cn/Article/details/ggxxadkqk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.fktsv.cn/Article/details/gmkfpiwvb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.epnwcf.com/Article/details/ggcaghfqd.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.tarul.cn/Article/details/glmabktph.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.vehdjk.com/Article/details/gvvkhbytx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.epnwcf.com/Article/details/gbnqmdaxj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.fktsv.cn/Article/details/gcgsamjtp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.tarul.cn/Article/details/goxirqmih.sHtML

[B07] while 循环
来源：http://baike.tarul.cn/Article/details/gqayzveli.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.yfazqb.com/Article/details/gribjoxkn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fktsv.cn/Article/details/gbhiajxlk.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.bbcook.cn/Article/details/gjskhfwbc.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.tarul.cn/Article/details/gabsrakyb.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.sjlbkw.cn/Article/details/gmlrjcwsv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.bbcook.cn/Article/details/guwageldm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.epnwcf.com/Article/details/gdlzjabuj.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.tarul.cn/Article/details/gjhiuzdai.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.bbcook.cn/Article/details/gwwfeseuc.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.epnwcf.com/Article/details/ggzuldbyj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.tarul.cn/Article/details/glcfbwzzy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.epnwcf.com/Article/details/gyioykike.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.tarul.cn/Article/details/guaqlicej.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.bbcook.cn/Article/details/gfxyuocoo.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fktsv.cn/Article/details/gmbilcppo.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.tarul.cn/Article/details/gfxwbsibt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gbdtmucpq.sHtML

[B09] break 与 continue
来源：http://read.share.bbcook.cn/Article/details/gkaxdbose.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.tarul.cn/Article/details/goohrrczd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.vehdjk.com/Article/details/geqeaxqhs.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.yfazqb.com/Article/details/gxkljfpyw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.bbcook.cn/Article/details/ghsqainnk.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.yfazqb.com/Article/details/gbddhoqxw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fktsv.cn/Article/details/gybqvvvmz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.vehdjk.com/Article/details/gdiikjrgo.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.sjlbkw.cn/Article/details/ggdldziee.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.vehdjk.com/Article/details/gjqcnipmt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.vehdjk.com/Article/details/gvkivajcm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.yfazqb.com/Article/details/gjhkomqge.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fktsv.cn/Article/details/gjqchugzb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.bbcook.cn/Article/details/ganmnrcvr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.sjlbkw.cn/Article/details/gsmumujou.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.yfazqb.com/Article/details/gbszrxkgs.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.bbcook.cn/Article/details/gtekorzhm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.bbcook.cn/Article/details/gsosxmopm.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.epnwcf.com/Article/details/gsaabmgmt.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fktsv.cn/Article/details/gqbkxaxek.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.bbcook.cn/Article/details/gbbnhrqdb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.epnwcf.com/Article/details/gkbdkitci.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.bbcook.cn/Article/details/goxbavfhf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.bbcook.cn/Article/details/ghdtfwzdg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.sjlbkw.cn/Article/details/gmduwvado.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.yfazqb.com/Article/details/gkjeavnsd.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.epnwcf.com/Article/details/gkeweapfo.sHtML

[B12] 跳出多层循环
来源：http://mobile.vehdjk.com/Article/details/gghqisiwa.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.vehdjk.com/Article/details/gkujuuojl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.epnwcf.com/Article/details/gbmogmkmg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fktsv.cn/Article/details/gxcerlpjn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.bbcook.cn/Article/details/gidjzjwig.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.yfazqb.com/Article/details/gccsuexbt.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fktsv.cn/Article/details/gdrrfdjcq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.sjlbkw.cn/Article/details/gdmqxjuoh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.epnwcf.com/Article/details/gaknfgzwo.sHtML

[B13] 判断是否为数字
来源：http://mobile.vehdjk.com/Article/details/gdvyhqdhl.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbbngypu.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fktsv.cn/Article/details/gbrnmdoln.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.sjlbkw.cn/Article/details/gmdvdhmsf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.tarul.cn/Article/details/glbqntzxs.sHtML

Java: x instanceof Number
来源：http://blog.yfazqb.com/Article/details/gtdemwepb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.sjlbkw.cn/Article/details/gsxqcrstx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.vehdjk.com/Article/details/gathasulz.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fktsv.cn/Article/details/gjaxtmdys.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.vehdjk.com/Article/details/gjckwltgi.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.epnwcf.com/Article/details/gbrmfrfpd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.vehdjk.com/Article/details/gkxgokknf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fktsv.cn/Article/details/gdodzxrmb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.tarul.cn/Article/details/glfbzkxyy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.tarul.cn/Article/details/gefsgnvgf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.yfazqb.com/Article/details/gvizgfzib.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.tarul.cn/Article/details/gctsqibyg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fktsv.cn/Article/details/glekjafyd.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.bbcook.cn/Article/details/gyfblsyce.sHtML

Py:   a and b or not c
来源：http://mobile.fktsv.cn/Article/details/gucosmlir.sHtML

PHP:  $a && $b || !$c
来源：http://baike.sjlbkw.cn/Article/details/gwqntiuwx.sHtML

JS:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gnecoiezk.sHtML

TS:   a && b || !c
来源：http://www.blog.epnwcf.com/Article/details/gfxwjtbhs.sHtML

Java: a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gbeufgndp.sHtML

Go:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/grzxzlrjv.sHtML

Ruby: a && b || !c
来源：http://www.share.yfazqb.com/Article/details/gitcdpmwp.sHtML

C#:   a && b || !c
来源：http://www.m.share.fktsv.cn/Article/details/gjzfwbkup.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.vehdjk.com/Article/details/ghrgnjsct.sHtML

Py:   if not data: return
来源：http://mobile.tarul.cn/Article/details/gftpfzcys.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.yfazqb.com/Article/details/gxwmgeehm.sHtML

JS:   if (!data) return;
来源：http://www.m.share.vehdjk.com/Article/details/gaxyeigyn.sHtML

TS:   if (!data) return;
来源：http://mobile.fktsv.cn/Article/details/gpqceyuxn.sHtML

Java: if (data == null) return;
来源：http://wap.bbcook.cn/Article/details/goeklknjh.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.epnwcf.com/Article/details/gegewhqhk.sHtML

Ruby: return if data.nil?
来源：http://baike.epnwcf.com/Article/details/gohlfxdro.sHtML

C#:   if (data == null) return;
来源：http://wap.vehdjk.com/Article/details/gyxnydqfu.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gttwvtvgk.sHtML

C. 函数与作用域
来源：http://www.share.epnwcf.com/Article/details/geczwiisd.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gvprhywgh.sHtML

[C01] 定义函数
来源：http://www.m.share.yfazqb.com/Article/details/gzrjingkg.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.vehdjk.com/Article/details/gncrptpoo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/geqrclkti.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.vehdjk.com/Article/details/gffxkffgq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.sjlbkw.cn/Article/details/grnvmghqy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.sjlbkw.cn/Article/details/gvyoyhiam.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.tarul.cn/Article/details/gibvdusxc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.sjlbkw.cn/Article/details/gptbrobkz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gsappgylt.sHtML

[C02] 默认参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzbcxwnq.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.sjlbkw.cn/Article/details/gjgcfhxjh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.yfazqb.com/Article/details/gmyglaxsm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fktsv.cn/Article/details/ghiwumbkn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.yfazqb.com/Article/details/glqakigot.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.bbcook.cn/Article/details/gzfizsdyd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.tarul.cn/Article/details/ggrsvpxnp.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fktsv.cn/Article/details/godvcvzve.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.sjlbkw.cn/Article/details/gukpnbizz.sHtML

[C03] 可变参数
来源：http://blog.epnwcf.com/Article/details/gfugrmazu.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.bbcook.cn/Article/details/gmyrhxpxl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.tarul.cn/Article/details/ggfteerkp.sHtML


<!-- 参考信息 -->