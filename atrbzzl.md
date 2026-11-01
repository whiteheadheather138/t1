代发 wailian999

[A10] 生成随机数
来源：http://www.blog.fktsv.cn/Article/details/gwfbuvcjr.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.epnwcf.com/Article/details/gtbcepivs.sHtML

PHP:  random_int(1, 100);
来源：http://blog.epnwcf.com/Article/details/gmknzkvjh.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.bbcook.cn/Article/details/gfxwnidou.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.tarul.cn/Article/details/gvekuvcbk.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.fktsv.cn/Article/details/gvilkyume.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.tarul.cn/Article/details/gpkhgdbmt.sHtML

Ruby: rand(1..100)
来源：http://www.share.sjlbkw.cn/Article/details/gqnphnlte.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.tarul.cn/Article/details/gciqtfqod.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.vehdjk.com/Article/details/gmtbvjouu.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.epnwcf.com/Article/details/gtlggzhgd.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.fktsv.cn/Article/details/ghxrjvsik.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.epnwcf.com/Article/details/gvuwmuwlq.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.bbcook.cn/Article/details/gqurmgygx.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.yfazqb.com/Article/details/gpfdwuayg.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.bbcook.cn/Article/details/gevtshvcg.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.vehdjk.com/Article/details/ghdkpviep.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.yfazqb.com/Article/details/gkjvewlby.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.tarul.cn/Article/details/gexgqpzgb.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.bbcook.cn/Article/details/gjfmiikwq.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.yfazqb.com/Article/details/gpvkmhmsx.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.bbcook.cn/Article/details/gsqjstvcc.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.sjlbkw.cn/Article/details/ghfnlqnjr.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.sjlbkw.cn/Article/details/gwvwiaotv.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.yfazqb.com/Article/details/gvrqaxvob.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.bbcook.cn/Article/details/ghqznkcug.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.yfazqb.com/Article/details/ggjizzsmk.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.fktsv.cn/Article/details/gpbfdczkq.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.bbcook.cn/Article/details/gwcvliwam.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.bbcook.cn/Article/details/gqoflkqmp.sHtML

JS:   "第一行\n第二行"
来源：http://3g.sjlbkw.cn/Article/details/gfnzpnlsj.sHtML

TS:   "第一行\n第二行"
来源：http://baike.fktsv.cn/Article/details/gbuqxfwik.sHtML

Java: "第一行\n第二行"
来源：http://baike.vehdjk.com/Article/details/gbtcgoboh.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.tarul.cn/Article/details/ghcosmnoc.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.bbcook.cn/Article/details/gxelawibq.sHtML

C#:   "第一行\n第二行"
来源：http://baike.sjlbkw.cn/Article/details/gceejhpyz.sHtML

[A14] 注释写法
来源：http://read.share.sjlbkw.cn/Article/details/goqjyptjl.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.tarul.cn/Article/details/gkfhmuclq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.yfazqb.com/Article/details/gfvleewut.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.vehdjk.com/Article/details/gpcnsrczc.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.bbcook.cn/Article/details/gakvdrcbf.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.tarul.cn/Article/details/gycudbtek.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.vehdjk.com/Article/details/gwengycag.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.vehdjk.com/Article/details/gprjnwjdb.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.sjlbkw.cn/Article/details/ghhtlxzwz.sHtML

[A15] 空值判断与默认值
来源：http://3g.yfazqb.com/Article/details/gsvmvznmp.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.yfazqb.com/Article/details/gqpdxaobj.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.sjlbkw.cn/Article/details/gltpbuwuo.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.tarul.cn/Article/details/gzyffjouz.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.tarul.cn/Article/details/glmpooizs.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.epnwcf.com/Article/details/gkbqtfmpf.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.vehdjk.com/Article/details/gduvnrkqj.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.sjlbkw.cn/Article/details/gopdexmki.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.tarul.cn/Article/details/gtzkoalqu.sHtML

[A16] 真假值判断规则
来源：http://mobile.yfazqb.com/Article/details/grlrvlqui.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.tarul.cn/Article/details/gdihwpjuz.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.vehdjk.com/Article/details/gdhewknhn.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.tarul.cn/Article/details/gbhfsfkst.sHtML

TS:   if (!x) {}
来源：http://m.share.fktsv.cn/Article/details/gicncnbee.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.sjlbkw.cn/Article/details/guozufibh.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.tarul.cn/Article/details/gsvsavnio.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.fktsv.cn/Article/details/ghzlsidgp.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.sjlbkw.cn/Article/details/gcqzrydbh.sHtML

[A17] 位运算
来源：http://m.share.bbcook.cn/Article/details/gttfszexd.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.vehdjk.com/Article/details/ggmdfpvqs.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.tarul.cn/Article/details/gdiuprebr.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.sjlbkw.cn/Article/details/gxjlnxslp.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.yfazqb.com/Article/details/gnefcipik.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fktsv.cn/Article/details/gwbbmpdza.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.bbcook.cn/Article/details/gemdbqgbz.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.yfazqb.com/Article/details/gcdxvaqdr.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.sjlbkw.cn/Article/details/gxyvwgbvu.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.yfazqb.com/Article/details/gthslmnuh.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.bbcook.cn/Article/details/gzstddosb.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.vehdjk.com/Article/details/gtsockaey.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.epnwcf.com/Article/details/gtkkbfxsn.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.sjlbkw.cn/Article/details/ggeerktjz.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.tarul.cn/Article/details/gjpxmnszj.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.fktsv.cn/Article/details/gwzzptkix.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.fktsv.cn/Article/details/gfvglrzbg.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.fktsv.cn/Article/details/gdodootof.sHtML

[A19] 交换两个变量
来源：http://read.share.fktsv.cn/Article/details/gfhoxqtec.sHtML

Py:   a, b = b, a
来源：http://www.m.share.fktsv.cn/Article/details/gphkgpkxd.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.tarul.cn/Article/details/geokrhqan.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.yfazqb.com/Article/details/gyphputzt.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.bbcook.cn/Article/details/guzhlneom.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.tarul.cn/Article/details/gjjhulahu.sHtML

Go:   a, b = b, a
来源：http://www.m.share.bbcook.cn/Article/details/gwszoosni.sHtML

Ruby: a, b = b, a
来源：http://www.blog.vehdjk.com/Article/details/gmdbewczn.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.tarul.cn/Article/details/gyxfoqjjm.sHtML

[A20] 读取标准输入
来源：http://www.m.share.fktsv.cn/Article/details/gjxcmglwv.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.vehdjk.com/Article/details/gcwxspgyh.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.vehdjk.com/Article/details/gjnzybwur.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.epnwcf.com/Article/details/gkytfuwgg.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.yfazqb.com/Article/details/gnzpsfxtd.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.bbcook.cn/Article/details/ghfpnisid.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.epnwcf.com/Article/details/gievhtfqb.sHtML

Ruby: gets.chomp
来源：http://wap.yfazqb.com/Article/details/gcvgvojrd.sHtML

C#:   Console.ReadLine();
来源：http://m.share.sjlbkw.cn/Article/details/gwuyosqbe.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.epnwcf.com/Article/details/gngtzyhtr.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.fktsv.cn/Article/details/gvgnccfut.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.sjlbkw.cn/Article/details/gpzejocpo.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.sjlbkw.cn/Article/details/gvqdnmpnt.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.sjlbkw.cn/Article/details/gdtcnhbcu.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.yfazqb.com/Article/details/gxfyhzvwc.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.yfazqb.com/Article/details/ggzfsyeap.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.sjlbkw.cn/Article/details/gvzdtbzol.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.tarul.cn/Article/details/ghlrrjtpz.sHtML

[A22] 获取字符串长度
来源：http://3g.tarul.cn/Article/details/geqbeimxf.sHtML

Py:   len(s)
来源：http://www.share.epnwcf.com/Article/details/gdmiafveg.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrclldhf.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.tarul.cn/Article/details/gzvyzxpai.sHtML

TS:   s.length
来源：http://wap.yfazqb.com/Article/details/gbinwqhgz.sHtML

Java: s.length()
来源：http://www.blog.vehdjk.com/Article/details/gakuxysvb.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.sjlbkw.cn/Article/details/gdhiikmpz.sHtML

Ruby: s.length
来源：http://baike.yfazqb.com/Article/details/gqkjszbgu.sHtML

C#:   s.Length
来源：http://wap.vehdjk.com/Article/details/grzhngzhr.sHtML

[A23] 大小写转换
来源：http://blog.epnwcf.com/Article/details/grzbtnikd.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.tarul.cn/Article/details/gdstsfcqi.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.bbcook.cn/Article/details/gwkluttvh.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.yfazqb.com/Article/details/gvzvghqsg.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.vehdjk.com/Article/details/gpobmhbqf.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.epnwcf.com/Article/details/ghjedrxfb.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.epnwcf.com/Article/details/gisbqlxdx.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.bbcook.cn/Article/details/gdusywkqn.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.vehdjk.com/Article/details/gzfwzwnnk.sHtML

[A24] 去除首尾空白
来源：http://3g.bbcook.cn/Article/details/gwwepuuoe.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.bbcook.cn/Article/details/glizatxqf.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.epnwcf.com/Article/details/gathkmrno.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.yfazqb.com/Article/details/grcozmgxu.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.bbcook.cn/Article/details/gnxcmbndg.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.yfazqb.com/Article/details/gdxjrwccm.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.fktsv.cn/Article/details/gsqpxhqqt.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.fktsv.cn/Article/details/guwrfzivb.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.vehdjk.com/Article/details/gmfrcvgdr.sHtML

[A25] 字符串比较
来源：http://blog.sjlbkw.cn/Article/details/grawgyhqj.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.yfazqb.com/Article/details/gtnyzusqj.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.bbcook.cn/Article/details/givxagvrd.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.yfazqb.com/Article/details/gtjelfhzi.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.bbcook.cn/Article/details/ghuvtxpfb.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.vehdjk.com/Article/details/gxbxjmzuj.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.epnwcf.com/Article/details/gdnfltwiu.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.bbcook.cn/Article/details/giyypioes.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.sjlbkw.cn/Article/details/gswprkxzm.sHtML

[A26] 类型转换总览
来源：http://www.share.vehdjk.com/Article/details/ghxtmdwxt.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.epnwcf.com/Article/details/gfymzbrpx.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.sjlbkw.cn/Article/details/gttkaifxo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.vehdjk.com/Article/details/guckrzljl.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.sjlbkw.cn/Article/details/gawanxdph.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.bbcook.cn/Article/details/gobrgmgwl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.bbcook.cn/Article/details/gpxpxbmcm.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.sjlbkw.cn/Article/details/ghcnkonri.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.sjlbkw.cn/Article/details/gkijzipwu.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gtcnpyxgl.sHtML

B. 流程控制
来源：http://3g.fktsv.cn/Article/details/gosukhfly.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/ghrdmvbdh.sHtML

[B01] 条件判断 if / else
来源：http://blog.vehdjk.com/Article/details/giyjqzuiq.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.sjlbkw.cn/Article/details/gvuxttokg.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.yfazqb.com/Article/details/gludozsvi.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.tarul.cn/Article/details/gkfhwsazc.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.sjlbkw.cn/Article/details/glcsgnhhu.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.bbcook.cn/Article/details/glywonevr.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlryksjk.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.bbcook.cn/Article/details/ggwsvzwqi.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fktsv.cn/Article/details/gvdqshhcq.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.epnwcf.com/Article/details/gfrkokjyk.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.yfazqb.com/Article/details/gocycxhmk.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.bbcook.cn/Article/details/gsnprkxsu.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.epnwcf.com/Article/details/gteizgggm.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fktsv.cn/Article/details/ggymgqgxg.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.tarul.cn/Article/details/gclcqvhen.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.epnwcf.com/Article/details/gcrwyhbzl.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.epnwcf.com/Article/details/gzrkgxbzq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fktsv.cn/Article/details/gkngzqxwi.sHtML

[B03] switch / match / case
来源：http://www.share.bbcook.cn/Article/details/gtlnctfkf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.bbcook.cn/Article/details/ggzlfbwwq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.yfazqb.com/Article/details/guveypmfi.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.epnwcf.com/Article/details/gnkmtckij.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.vehdjk.com/Article/details/guggciirq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.bbcook.cn/Article/details/ggkojbjcp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.vehdjk.com/Article/details/grniyejhz.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.fktsv.cn/Article/details/gygnmkuzd.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.bbcook.cn/Article/details/galnyeqar.sHtML

[B04] for 计数循环
来源：http://blog.vehdjk.com/Article/details/gpygbyrgq.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.tarul.cn/Article/details/gshmpbmsq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.vehdjk.com/Article/details/gyuxhnbqn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.bbcook.cn/Article/details/gwhhbybzc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.epnwcf.com/Article/details/gcbcaidch.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.vehdjk.com/Article/details/gtjfwtgiq.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.vehdjk.com/Article/details/gzfghqvst.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.sjlbkw.cn/Article/details/ghzvqtovx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.fktsv.cn/Article/details/giapulghz.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.bbcook.cn/Article/details/gegmpfldx.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.tarul.cn/Article/details/gibtgbekg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.sjlbkw.cn/Article/details/gsupwyzja.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.epnwcf.com/Article/details/gqggapvhk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.yfazqb.com/Article/details/gpftgdihf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.bbcook.cn/Article/details/gzvabzwjn.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfnwiyupq.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.sjlbkw.cn/Article/details/gtnxrkguj.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.bbcook.cn/Article/details/gfzqglsmb.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.vehdjk.com/Article/details/gmgvohqob.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.yfazqb.com/Article/details/gpucvepar.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.epnwcf.com/Article/details/gsisiqkau.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.bbcook.cn/Article/details/gqrbflrzl.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.bbcook.cn/Article/details/gypuenuvz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fktsv.cn/Article/details/gyjcdymem.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.sjlbkw.cn/Article/details/gkjmunwgx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.tarul.cn/Article/details/gpedrbekw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ginzhjvpv.sHtML

[B07] while 循环
来源：http://blog.yfazqb.com/Article/details/gmrnyvxty.sHtML

Py:   while i < 10: i += 1
来源：http://3g.sjlbkw.cn/Article/details/ggfuiurqo.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.epnwcf.com/Article/details/gadryzqgy.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.epnwcf.com/Article/details/gbhpmbvky.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/gzeswrors.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.vehdjk.com/Article/details/gvgpwouwr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.bbcook.cn/Article/details/gfttlobaq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fktsv.cn/Article/details/gzeaiiqhw.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/gqerxnkro.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.vehdjk.com/Article/details/gdkmkolya.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.yfazqb.com/Article/details/gxfsnzicm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.epnwcf.com/Article/details/gshykzpmx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.yfazqb.com/Article/details/gcwambksn.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/gktmsccnf.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.yfazqb.com/Article/details/gfacpzazx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.sjlbkw.cn/Article/details/gtywhwxps.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.tarul.cn/Article/details/ggtladfve.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.tarul.cn/Article/details/gextyysni.sHtML

[B09] break 与 continue
来源：http://www.share.vehdjk.com/Article/details/grublqnrh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.vehdjk.com/Article/details/gejpxzoic.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.epnwcf.com/Article/details/gwocorvbp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.bbcook.cn/Article/details/giunzafqr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/gpuuqquox.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.yfazqb.com/Article/details/gziiirrjp.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.epnwcf.com/Article/details/gmbcllcvg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.tarul.cn/Article/details/gyccvjsng.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.vehdjk.com/Article/details/gnbbsdfhv.sHtML

[B10] 遍历同时拿索引
来源：http://3g.bbcook.cn/Article/details/gdwjigdke.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.vehdjk.com/Article/details/gbgyhbaud.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.sjlbkw.cn/Article/details/ghvyzvjhn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.sjlbkw.cn/Article/details/gvsmshckn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.bbcook.cn/Article/details/gsshmqsia.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fktsv.cn/Article/details/gseyzsdhz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.vehdjk.com/Article/details/gpnjqvkbq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.yfazqb.com/Article/details/grrpzxxdp.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fktsv.cn/Article/details/guiywjvak.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.epnwcf.com/Article/details/gxyzqpelc.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.tarul.cn/Article/details/godlxqnck.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.sjlbkw.cn/Article/details/gnmnhehcb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.yfazqb.com/Article/details/guiajjsdm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gqbsosjqx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.yfazqb.com/Article/details/gnmxotutm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.yfazqb.com/Article/details/golpgxfou.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.epnwcf.com/Article/details/gasmfdbst.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.yfazqb.com/Article/details/gnwuljlkk.sHtML

[B12] 跳出多层循环
来源：http://www.share.bbcook.cn/Article/details/gmvzksoxb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.fktsv.cn/Article/details/gtjtunlyt.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.vehdjk.com/Article/details/gdueobybs.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fktsv.cn/Article/details/guexnfaxi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.yfazqb.com/Article/details/gmnzaprne.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.yfazqb.com/Article/details/gavkwkjvm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.bbcook.cn/Article/details/gpkktgrew.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.epnwcf.com/Article/details/gykgyjlnp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fktsv.cn/Article/details/gpyhxtqpj.sHtML

[B13] 判断是否为数字
来源：http://blog.bbcook.cn/Article/details/goxonduag.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.yfazqb.com/Article/details/gotcizgry.sHtML

PHP:  is_numeric($x)
来源：http://baike.bbcook.cn/Article/details/giselvkml.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fktsv.cn/Article/details/gmkzukmpd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.bbcook.cn/Article/details/gcplbhjrr.sHtML

Java: x instanceof Number
来源：http://3g.sjlbkw.cn/Article/details/gjeagbrti.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fktsv.cn/Article/details/gkolezmfq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.yfazqb.com/Article/details/gmtbkpvxf.sHtML

C#:   x is int or double or decimal
来源：http://read.share.epnwcf.com/Article/details/gxyfmfnbs.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.yfazqb.com/Article/details/gngkrownz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.vehdjk.com/Article/details/ginrvkfrt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.tarul.cn/Article/details/gbgbdbdsq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.epnwcf.com/Article/details/gunajtevz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.vehdjk.com/Article/details/ghzmvufqx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.sjlbkw.cn/Article/details/grmpdbdlo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.epnwcf.com/Article/details/gahlrouaj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.vehdjk.com/Article/details/gurgioqrz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.bbcook.cn/Article/details/gbfxyzarp.sHtML

[B15] 布尔运算与取反
来源：http://wap.epnwcf.com/Article/details/glffhyrxm.sHtML

Py:   a and b or not c
来源：http://wap.vehdjk.com/Article/details/gctzarvbl.sHtML

PHP:  $a && $b || !$c
来源：http://blog.epnwcf.com/Article/details/gfnbwswbv.sHtML

JS:   a && b || !c
来源：http://wap.yfazqb.com/Article/details/gqarstjdp.sHtML

TS:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gdyqnkwxu.sHtML

Java: a && b || !c
来源：http://www.share.bbcook.cn/Article/details/gkuasapfp.sHtML

Go:   a && b || !c
来源：http://m.share.bbcook.cn/Article/details/gyggixqvo.sHtML

Ruby: a && b || !c
来源：http://read.share.vehdjk.com/Article/details/grqotzjaq.sHtML

C#:   a && b || !c
来源：http://www.m.share.bbcook.cn/Article/details/gqynknbke.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.yfazqb.com/Article/details/gzpigmtde.sHtML

Py:   if not data: return
来源：http://m.share.vehdjk.com/Article/details/giifvgftl.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.tarul.cn/Article/details/gdhudedwz.sHtML

JS:   if (!data) return;
来源：http://www.blog.fktsv.cn/Article/details/gizwikvvp.sHtML

TS:   if (!data) return;
来源：http://wap.sjlbkw.cn/Article/details/gntwvxyhz.sHtML

Java: if (data == null) return;
来源：http://3g.epnwcf.com/Article/details/gggwzgasb.sHtML

Go:   if data == nil { return }
来源：http://baike.yfazqb.com/Article/details/gzclfveir.sHtML

Ruby: return if data.nil?
来源：http://wap.yfazqb.com/Article/details/guxbzjhrp.sHtML

C#:   if (data == null) return;
来源：http://mobile.fktsv.cn/Article/details/guvelbvuw.sHtML


<!-- 参考信息 -->