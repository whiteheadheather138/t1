代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.yfazqb.com/Article/details/ghyxaxodj.sHtML

[A07] 数字转字符串
来源：http://www.blog.bbcook.cn/Article/details/gqdkpbxaf.sHtML

Py:   str(42)
来源：http://www.blog.sjlbkw.cn/Article/details/gyhfftyfp.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.tarul.cn/Article/details/gnpxrttej.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.sjlbkw.cn/Article/details/gozsdzpre.sHtML

TS:   String(42)
来源：http://mobile.sjlbkw.cn/Article/details/gkrhyknxa.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.yfazqb.com/Article/details/gbfqusjsh.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpeyvmnip.sHtML

Ruby: 42.to_s
来源：http://mobile.fktsv.cn/Article/details/ggomzsapk.sHtML

C#:   42.ToString()
来源：http://baike.epnwcf.com/Article/details/glqonaypo.sHtML

[A08] 取整与四舍五入
来源：http://3g.yfazqb.com/Article/details/gflsqufae.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.bbcook.cn/Article/details/gvulonwjh.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.sjlbkw.cn/Article/details/gbzjlbkii.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fktsv.cn/Article/details/glmebtcqh.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.sjlbkw.cn/Article/details/gymfzfncl.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.tarul.cn/Article/details/gpkzixryl.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.bbcook.cn/Article/details/gjyyxxdnw.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.tarul.cn/Article/details/ggjtgwsla.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.sjlbkw.cn/Article/details/gpwtvhbgg.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.fktsv.cn/Article/details/gvbtsflzm.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.sjlbkw.cn/Article/details/gdnkimiou.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.epnwcf.com/Article/details/gihzjlgiu.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gsueznvbe.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.vehdjk.com/Article/details/ghccxqkhs.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.tarul.cn/Article/details/glwzgmels.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.yfazqb.com/Article/details/guekdqzyb.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.bbcook.cn/Article/details/gngmjzoce.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.epnwcf.com/Article/details/gglytupep.sHtML

[A10] 生成随机数
来源：http://www.m.share.fktsv.cn/Article/details/gtukratad.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.sjlbkw.cn/Article/details/gotvcsfol.sHtML

PHP:  random_int(1, 100);
来源：http://baike.epnwcf.com/Article/details/ghfrbdcxb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fktsv.cn/Article/details/gojvgubet.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.yfazqb.com/Article/details/gdedgjyxe.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.epnwcf.com/Article/details/gytkhdfrv.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.vehdjk.com/Article/details/gjlohnmtm.sHtML

Ruby: rand(1..100)
来源：http://m.share.yfazqb.com/Article/details/gqgdtdhov.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.bbcook.cn/Article/details/ghjrzkywy.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.sjlbkw.cn/Article/details/garawkcob.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.fktsv.cn/Article/details/gbmsgwqxy.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.bbcook.cn/Article/details/gwrfzhcmp.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.tarul.cn/Article/details/gzxvqqact.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.sjlbkw.cn/Article/details/gydyfgkbc.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.bbcook.cn/Article/details/gcgpjhbmu.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.sjlbkw.cn/Article/details/gjfkikpui.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.sjlbkw.cn/Article/details/guewrejch.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.tarul.cn/Article/details/gazjrwohn.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.vehdjk.com/Article/details/gnfwzkvob.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.sjlbkw.cn/Article/details/gzfxcinjw.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.fktsv.cn/Article/details/gjpfzyrdi.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.epnwcf.com/Article/details/graeeukcu.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.bbcook.cn/Article/details/grxqtfimy.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.bbcook.cn/Article/details/gzvuhupvl.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gsbaioxsp.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.tarul.cn/Article/details/gnwsnafpx.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.sjlbkw.cn/Article/details/gqkqehzgq.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.yfazqb.com/Article/details/ghfxqcazu.sHtML

Py:   "第一行\n第二行"
来源：http://baike.fktsv.cn/Article/details/gsviemozo.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.yfazqb.com/Article/details/gphjuqspl.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.epnwcf.com/Article/details/giupcvrva.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.epnwcf.com/Article/details/guydhrdfr.sHtML

Java: "第一行\n第二行"
来源：http://baike.epnwcf.com/Article/details/gpzkthnpm.sHtML

Go:   "第一行\n第二行"
来源：http://3g.epnwcf.com/Article/details/gdequqdkm.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.vehdjk.com/Article/details/gjtxtfuii.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.epnwcf.com/Article/details/gmfxratwa.sHtML

[A14] 注释写法
来源：http://3g.yfazqb.com/Article/details/gjiyqvpdi.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.tarul.cn/Article/details/gqbmbuugt.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.yfazqb.com/Article/details/geyjyzcmz.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.bbcook.cn/Article/details/gbojhfmwn.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.bbcook.cn/Article/details/gumelsmty.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.fktsv.cn/Article/details/glfnitddh.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.sjlbkw.cn/Article/details/guhfsjolr.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.tarul.cn/Article/details/ghczezodf.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.yfazqb.com/Article/details/gfjithfts.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.tarul.cn/Article/details/ghwxtpths.sHtML

Py:   value = data or "默认值"
来源：http://www.share.sjlbkw.cn/Article/details/ghbpbmtyk.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.bbcook.cn/Article/details/gbviicmve.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.tarul.cn/Article/details/gvlleaihj.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.fktsv.cn/Article/details/gvkadixmb.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.yfazqb.com/Article/details/gwneujmna.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.fktsv.cn/Article/details/gvkooegjb.sHtML

Ruby: value = data || "默认值"
来源：http://3g.fktsv.cn/Article/details/gzluortxp.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.fktsv.cn/Article/details/gbpwlfpzf.sHtML

[A16] 真假值判断规则
来源：http://blog.yfazqb.com/Article/details/gasouwula.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.sjlbkw.cn/Article/details/gpglvnxpd.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.epnwcf.com/Article/details/gzfumaqec.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.vehdjk.com/Article/details/gkgntxnmn.sHtML

TS:   if (!x) {}
来源：http://mobile.sjlbkw.cn/Article/details/gznaxminz.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.bbcook.cn/Article/details/gaxmrzzjk.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.bbcook.cn/Article/details/glrecjxkf.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.tarul.cn/Article/details/gsesgluka.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.vehdjk.com/Article/details/gifmloewk.sHtML

[A17] 位运算
来源：http://m.share.yfazqb.com/Article/details/gqjhwbefc.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.bbcook.cn/Article/details/ggmaczknj.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.tarul.cn/Article/details/guxfmoisu.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/guksyypnc.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.epnwcf.com/Article/details/gnwgxcems.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.sjlbkw.cn/Article/details/gcybbntvp.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.yfazqb.com/Article/details/gbopjuduu.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.vehdjk.com/Article/details/gyqrdjujt.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.bbcook.cn/Article/details/gucbstmyv.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.sjlbkw.cn/Article/details/gnazqfnhe.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.sjlbkw.cn/Article/details/gfdpriopp.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.vehdjk.com/Article/details/gkkhnhqgq.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.tarul.cn/Article/details/gtecsvspj.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.fktsv.cn/Article/details/ghvkqsepw.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.epnwcf.com/Article/details/gpxtaftxu.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.fktsv.cn/Article/details/gviiaorwv.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.bbcook.cn/Article/details/gyajeayei.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.vehdjk.com/Article/details/grmznaxpl.sHtML

[A19] 交换两个变量
来源：http://www.share.tarul.cn/Article/details/gaesepcny.sHtML

Py:   a, b = b, a
来源：http://www.share.yfazqb.com/Article/details/gfrvohvdu.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.vehdjk.com/Article/details/gcbpefenw.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.fktsv.cn/Article/details/ggzwieuxw.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.fktsv.cn/Article/details/ghnzvckkc.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.fktsv.cn/Article/details/gvqomkngs.sHtML

Go:   a, b = b, a
来源：http://3g.epnwcf.com/Article/details/gppsxvseb.sHtML

Ruby: a, b = b, a
来源：http://www.blog.bbcook.cn/Article/details/gvcscijvx.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.yfazqb.com/Article/details/gbyxxauiy.sHtML

[A20] 读取标准输入
来源：http://3g.tarul.cn/Article/details/gojkqixtn.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.vehdjk.com/Article/details/gegoeucww.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.sjlbkw.cn/Article/details/gvzjekamu.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.yfazqb.com/Article/details/goflrbjnd.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.tarul.cn/Article/details/gbdloidxf.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.bbcook.cn/Article/details/gdakdfdew.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.vehdjk.com/Article/details/gitrzygim.sHtML

Ruby: gets.chomp
来源：http://blog.bbcook.cn/Article/details/giaqocyen.sHtML

C#:   Console.ReadLine();
来源：http://baike.bbcook.cn/Article/details/guhhtbsie.sHtML

[A21] 保留指定小数位输出
来源：http://wap.sjlbkw.cn/Article/details/gaptijddz.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.fktsv.cn/Article/details/gljvqerlz.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.epnwcf.com/Article/details/glblikcnl.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.fktsv.cn/Article/details/gptsvfvjd.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.epnwcf.com/Article/details/gtrcivctf.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.epnwcf.com/Article/details/gvfzsddje.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.bbcook.cn/Article/details/grludatcn.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.yfazqb.com/Article/details/gfzlpbnyf.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.bbcook.cn/Article/details/gjcxodbof.sHtML

[A22] 获取字符串长度
来源：http://mobile.tarul.cn/Article/details/gmdnjmjjc.sHtML

Py:   len(s)
来源：http://www.share.sjlbkw.cn/Article/details/gmywywwtz.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.tarul.cn/Article/details/gnysiirke.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.yfazqb.com/Article/details/gujxbzdgh.sHtML

TS:   s.length
来源：http://www.blog.bbcook.cn/Article/details/gzavwcmto.sHtML

Java: s.length()
来源：http://3g.tarul.cn/Article/details/gurgqyrti.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.tarul.cn/Article/details/gxbhzkzym.sHtML

Ruby: s.length
来源：http://wap.epnwcf.com/Article/details/gcwcqiieu.sHtML

C#:   s.Length
来源：http://mobile.epnwcf.com/Article/details/gaatqyazg.sHtML

[A23] 大小写转换
来源：http://wap.yfazqb.com/Article/details/gyxggyjui.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.bbcook.cn/Article/details/ggsadnrfu.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.vehdjk.com/Article/details/gnhstpaca.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.epnwcf.com/Article/details/glgmondcg.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.epnwcf.com/Article/details/gefgzqbrx.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.sjlbkw.cn/Article/details/glzfxjiaa.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.yfazqb.com/Article/details/gyjxmoydj.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.fktsv.cn/Article/details/gnytzroks.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.tarul.cn/Article/details/ggjeirrtw.sHtML

[A24] 去除首尾空白
来源：http://3g.epnwcf.com/Article/details/gvabdabas.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.sjlbkw.cn/Article/details/gaculdpit.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.epnwcf.com/Article/details/gbbbrvvuc.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.tarul.cn/Article/details/geskqsarj.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.sjlbkw.cn/Article/details/gorztczig.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.vehdjk.com/Article/details/gezyixxjv.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gscnbqonc.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.epnwcf.com/Article/details/gfepqelik.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.bbcook.cn/Article/details/gndoolfrm.sHtML

[A25] 字符串比较
来源：http://m.share.fktsv.cn/Article/details/gfzzpoavb.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.bbcook.cn/Article/details/gklbswspg.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.tarul.cn/Article/details/gbazabqfy.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.bbcook.cn/Article/details/gkoobcmfp.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.bbcook.cn/Article/details/gwqbvkbfs.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.bbcook.cn/Article/details/gqfxwzfsf.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.fktsv.cn/Article/details/gqywlslfe.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.fktsv.cn/Article/details/gpitbkzzh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.bbcook.cn/Article/details/gttaeaafx.sHtML

[A26] 类型转换总览
来源：http://read.share.vehdjk.com/Article/details/gjsjbaqdb.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.vehdjk.com/Article/details/gektgbowi.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.yfazqb.com/Article/details/gmscoefbv.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.sjlbkw.cn/Article/details/gffbhbgrh.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.tarul.cn/Article/details/gllgloiyr.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.epnwcf.com/Article/details/ghfmfjpjh.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.epnwcf.com/Article/details/gkwtmujub.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.tarul.cn/Article/details/gzazliqgc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.vehdjk.com/Article/details/gqcpgdplv.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gknhlvcpp.sHtML

B. 流程控制
来源：http://www.share.vehdjk.com/Article/details/gkrcgixfv.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/ggbsydqzy.sHtML

[B01] 条件判断 if / else
来源：http://baike.fktsv.cn/Article/details/gefmlaulz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.yfazqb.com/Article/details/gmmmouqus.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.fktsv.cn/Article/details/gftibaeel.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.yfazqb.com/Article/details/gvwayjpmr.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.yfazqb.com/Article/details/grwxveslv.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.sjlbkw.cn/Article/details/ggrtkwpyr.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.tarul.cn/Article/details/gluqqozbk.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.tarul.cn/Article/details/gqerjepfx.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.bbcook.cn/Article/details/grzphkqfw.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.vehdjk.com/Article/details/grmepoteh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.yfazqb.com/Article/details/grjofiidv.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.tarul.cn/Article/details/gpzubjsyc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.epnwcf.com/Article/details/glkrlezyz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fktsv.cn/Article/details/gxghvswuq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.sjlbkw.cn/Article/details/gsttkgvaz.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfahizkc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.epnwcf.com/Article/details/glshwbrwy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.epnwcf.com/Article/details/gifxbehfl.sHtML

[B03] switch / match / case
来源：http://www.share.yfazqb.com/Article/details/gfntutlpe.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.epnwcf.com/Article/details/gubzbrznc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.fktsv.cn/Article/details/gfwutqgwz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.sjlbkw.cn/Article/details/gcgqovhlv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.epnwcf.com/Article/details/gvneqcgnw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.bbcook.cn/Article/details/glhprmrcq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fktsv.cn/Article/details/gxhujkddj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.bbcook.cn/Article/details/gtizpjzsz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.vehdjk.com/Article/details/gcfzcgeba.sHtML

[B04] for 计数循环
来源：http://read.share.fktsv.cn/Article/details/gokrswxfm.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.fktsv.cn/Article/details/gjzgbxqxu.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.vehdjk.com/Article/details/gqajdoybn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.yfazqb.com/Article/details/gvursfeym.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.tarul.cn/Article/details/ghrbfkuld.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.tarul.cn/Article/details/gqkalumom.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.fktsv.cn/Article/details/gpirbdfev.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.tarul.cn/Article/details/gkzhpktgl.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.epnwcf.com/Article/details/ghcelviie.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.vehdjk.com/Article/details/gwmrpekde.sHtML

Py:   for item in arr: print(item)
来源：http://baike.bbcook.cn/Article/details/gjavrgtjh.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.vehdjk.com/Article/details/gnmkyekcg.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.epnwcf.com/Article/details/gcttxwpek.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.tarul.cn/Article/details/gtlmdmqye.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.bbcook.cn/Article/details/gsnkkwyiq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.tarul.cn/Article/details/gccslfeut.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.fktsv.cn/Article/details/gdnspryba.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.yfazqb.com/Article/details/gzbzgaxif.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.sjlbkw.cn/Article/details/gjbwhmrxz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.vehdjk.com/Article/details/gdomskhmg.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.fktsv.cn/Article/details/gykqhtjrb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.bbcook.cn/Article/details/godfcdapj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.sjlbkw.cn/Article/details/gsduvnzaa.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.sjlbkw.cn/Article/details/gpbhlgqbz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.bbcook.cn/Article/details/gukhqawvc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.yfazqb.com/Article/details/ggwgmkydf.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.yfazqb.com/Article/details/gugzthulf.sHtML

[B07] while 循环
来源：http://www.m.share.fktsv.cn/Article/details/ghyucgunv.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.sjlbkw.cn/Article/details/gimbxzsyx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fktsv.cn/Article/details/gdsrygfxx.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.bbcook.cn/Article/details/gwlqywphw.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.tarul.cn/Article/details/gjzehdauu.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.fktsv.cn/Article/details/goexzbsep.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.tarul.cn/Article/details/gqylqspuw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gplmzudta.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.bbcook.cn/Article/details/gckkadjhm.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.sjlbkw.cn/Article/details/gkoqlelsg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.epnwcf.com/Article/details/ghknzyepu.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.tarul.cn/Article/details/gqeefanam.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fktsv.cn/Article/details/gwvobhqty.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.fktsv.cn/Article/details/gmrtavdnf.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.tarul.cn/Article/details/gsupvqjsl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.tarul.cn/Article/details/ghbyonozo.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.tarul.cn/Article/details/ggfreortq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.tarul.cn/Article/details/gkckkhqoe.sHtML

[B09] break 与 continue
来源：http://m.share.vehdjk.com/Article/details/geaurvcvr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.vehdjk.com/Article/details/gnprylmcc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.sjlbkw.cn/Article/details/gfikeflqy.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/gjvzrezan.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.yfazqb.com/Article/details/gviuassyk.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.epnwcf.com/Article/details/gttmxjvqs.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.sjlbkw.cn/Article/details/gcpbictqa.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.bbcook.cn/Article/details/gbrotfvkb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.vehdjk.com/Article/details/gauruolbj.sHtML

[B10] 遍历同时拿索引
来源：http://3g.bbcook.cn/Article/details/gxhohilwp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fktsv.cn/Article/details/gvjdpkouf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.bbcook.cn/Article/details/gqvpwpmiv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fktsv.cn/Article/details/giwalslbk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.yfazqb.com/Article/details/gsvzciper.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.yfazqb.com/Article/details/gfrkahykq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fktsv.cn/Article/details/gosrwhksu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.sjlbkw.cn/Article/details/gxxmcombb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.vehdjk.com/Article/details/gikgmaeqx.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fktsv.cn/Article/details/gqzkmknog.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.yfazqb.com/Article/details/gyshktxqf.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.yfazqb.com/Article/details/gegxnlbcx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.sjlbkw.cn/Article/details/gihhrzizg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.vehdjk.com/Article/details/gftaoczqy.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fktsv.cn/Article/details/gfewkynlv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.bbcook.cn/Article/details/gsiaqyeob.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.epnwcf.com/Article/details/gevccvptz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.sjlbkw.cn/Article/details/gvcuacegt.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gldglrcmz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.epnwcf.com/Article/details/gendmrlgp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.sjlbkw.cn/Article/details/ghyfkyhss.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.bbcook.cn/Article/details/gzhcwidbi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.bbcook.cn/Article/details/gbpculvwk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.vehdjk.com/Article/details/gvkjpsccl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.tarul.cn/Article/details/gyvzwaxwk.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.yfazqb.com/Article/details/gvtnxmroo.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.tarul.cn/Article/details/gwsxsivth.sHtML

[B13] 判断是否为数字
来源：http://www.share.vehdjk.com/Article/details/gevscuazy.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.tarul.cn/Article/details/gewdtkqfw.sHtML

PHP:  is_numeric($x)
来源：http://mobile.vehdjk.com/Article/details/gtguivmik.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.epnwcf.com/Article/details/gboiyyiun.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fktsv.cn/Article/details/gzcscckyr.sHtML

Java: x instanceof Number
来源：http://baike.yfazqb.com/Article/details/gbmgmpfre.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.epnwcf.com/Article/details/gvxjhhuee.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.epnwcf.com/Article/details/gttzddjec.sHtML


<!-- 参考信息 -->