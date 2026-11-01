代发 wailian999

Java: "第一行\n第二行"
来源：http://www.m.share.epnwcf.com/Article/details/gzbijrnxv.sHtML

Go:   "第一行\n第二行"
来源：http://wap.tarul.cn/Article/details/gwukvrvmj.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.vehdjk.com/Article/details/gxyyjwmem.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.epnwcf.com/Article/details/gwwvcsfgb.sHtML

[A14] 注释写法
来源：http://wap.bbcook.cn/Article/details/ggahbbdeh.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.vehdjk.com/Article/details/gquveyvmi.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.epnwcf.com/Article/details/gxbtoipeh.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.bbcook.cn/Article/details/gqqbzezzj.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.vehdjk.com/Article/details/gwbnqzjfh.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.vehdjk.com/Article/details/gjxupwroq.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.bbcook.cn/Article/details/gmjzyegrk.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.sjlbkw.cn/Article/details/grdjvagld.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.epnwcf.com/Article/details/gsrxoktwf.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.fktsv.cn/Article/details/gbiixkwwl.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.fktsv.cn/Article/details/gqiewasli.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.bbcook.cn/Article/details/gzpzngvpf.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.epnwcf.com/Article/details/gpgdidydx.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.vehdjk.com/Article/details/giurbksac.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.fktsv.cn/Article/details/ghbrnmhqp.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.tarul.cn/Article/details/gwneldntj.sHtML

Ruby: value = data || "默认值"
来源：http://3g.yfazqb.com/Article/details/ggjjordai.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.bbcook.cn/Article/details/gvcmbcwvi.sHtML

[A16] 真假值判断规则
来源：http://www.share.vehdjk.com/Article/details/grtpjsoym.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.bbcook.cn/Article/details/gtespwumt.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.sjlbkw.cn/Article/details/ggamyizth.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.tarul.cn/Article/details/gvvbmvfje.sHtML

TS:   if (!x) {}
来源：http://blog.vehdjk.com/Article/details/gryhpfgex.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.vehdjk.com/Article/details/gzpdaubkf.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.bbcook.cn/Article/details/gbijxvczg.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.bbcook.cn/Article/details/gcyzyvfce.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.epnwcf.com/Article/details/gtbqtnbjm.sHtML

[A17] 位运算
来源：http://www.blog.yfazqb.com/Article/details/gyxcwjoad.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fktsv.cn/Article/details/grkqygkmc.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.yfazqb.com/Article/details/gwifhaywe.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.yfazqb.com/Article/details/gzxcqbnja.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.sjlbkw.cn/Article/details/gjkkbtzkn.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.sjlbkw.cn/Article/details/gdtdkhgid.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.sjlbkw.cn/Article/details/gnigxevjo.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.yfazqb.com/Article/details/gnrmvhtih.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.tarul.cn/Article/details/gfspukzft.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.yfazqb.com/Article/details/ggvijluev.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.sjlbkw.cn/Article/details/ghhxgbdjk.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.fktsv.cn/Article/details/gbnyrnvig.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.vehdjk.com/Article/details/gwabelyge.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.epnwcf.com/Article/details/gmklpqttv.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.vehdjk.com/Article/details/ghycxrtud.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.tarul.cn/Article/details/ghuibeeea.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.vehdjk.com/Article/details/gtfgswcke.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.fktsv.cn/Article/details/gurrmixwo.sHtML

[A19] 交换两个变量
来源：http://wap.vehdjk.com/Article/details/gitruqdlc.sHtML

Py:   a, b = b, a
来源：http://www.m.share.sjlbkw.cn/Article/details/gasxnoqmc.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.vehdjk.com/Article/details/gpqsdmqbx.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.epnwcf.com/Article/details/gycsefnht.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.bbcook.cn/Article/details/gujqrhgps.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.vehdjk.com/Article/details/gtwzfotlr.sHtML

Go:   a, b = b, a
来源：http://blog.sjlbkw.cn/Article/details/gxftlgswv.sHtML

Ruby: a, b = b, a
来源：http://3g.bbcook.cn/Article/details/gvmrknknn.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.sjlbkw.cn/Article/details/gvffczpmn.sHtML

[A20] 读取标准输入
来源：http://3g.vehdjk.com/Article/details/gmundygfh.sHtML

Py:   name = input("请输入：")
来源：http://read.share.sjlbkw.cn/Article/details/gigobbfno.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.tarul.cn/Article/details/gcxqxpylx.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.yfazqb.com/Article/details/gnhdnfxqb.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.fktsv.cn/Article/details/gnqqrhwhf.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.tarul.cn/Article/details/gitlwesfl.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.vehdjk.com/Article/details/gbmctynhl.sHtML

Ruby: gets.chomp
来源：http://baike.sjlbkw.cn/Article/details/gjgrqryfm.sHtML

C#:   Console.ReadLine();
来源：http://www.share.vehdjk.com/Article/details/ggqrvhbfo.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.fktsv.cn/Article/details/gwrqnygno.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.vehdjk.com/Article/details/gaskohhhq.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.tarul.cn/Article/details/gsmwjifos.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.yfazqb.com/Article/details/gisbozuvb.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.tarul.cn/Article/details/giyitjwqi.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.tarul.cn/Article/details/gabfbpuip.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.epnwcf.com/Article/details/gubglnfmf.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.sjlbkw.cn/Article/details/gljnkwsek.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.vehdjk.com/Article/details/gvyfzczid.sHtML

[A22] 获取字符串长度
来源：http://mobile.sjlbkw.cn/Article/details/gdqxhkytp.sHtML

Py:   len(s)
来源：http://mobile.tarul.cn/Article/details/gocnuhuro.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.bbcook.cn/Article/details/gtrzwunvq.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.sjlbkw.cn/Article/details/gqriahvqr.sHtML

TS:   s.length
来源：http://3g.tarul.cn/Article/details/gekdsuxau.sHtML

Java: s.length()
来源：http://mobile.bbcook.cn/Article/details/glilngwpx.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.epnwcf.com/Article/details/gmupvjvhh.sHtML

Ruby: s.length
来源：http://www.m.share.bbcook.cn/Article/details/gdmowdkpn.sHtML

C#:   s.Length
来源：http://www.m.share.fktsv.cn/Article/details/guyzypgve.sHtML

[A23] 大小写转换
来源：http://m.share.epnwcf.com/Article/details/gdprnvvkq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.vehdjk.com/Article/details/gjieezmxb.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.fktsv.cn/Article/details/gvheksoyu.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fktsv.cn/Article/details/gjshmlkzc.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.yfazqb.com/Article/details/geyusweoy.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.sjlbkw.cn/Article/details/gxocwaglr.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.yfazqb.com/Article/details/ganlmcrlp.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.vehdjk.com/Article/details/gplqftkms.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.epnwcf.com/Article/details/gatpeufhj.sHtML

[A24] 去除首尾空白
来源：http://baike.fktsv.cn/Article/details/gizrmqigb.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.sjlbkw.cn/Article/details/gqkunuxwv.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.tarul.cn/Article/details/gmapacmvo.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.yfazqb.com/Article/details/gzchreoph.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.sjlbkw.cn/Article/details/gffaxqskk.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.bbcook.cn/Article/details/gxsviislw.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.sjlbkw.cn/Article/details/gpyjcnwwh.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.yfazqb.com/Article/details/gczegchfj.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.vehdjk.com/Article/details/glvtiskwl.sHtML

[A25] 字符串比较
来源：http://www.share.tarul.cn/Article/details/grbmlwtsw.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.bbcook.cn/Article/details/gmgrkbstr.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.fktsv.cn/Article/details/gczvoicwb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.vehdjk.com/Article/details/gvlkpesvs.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.vehdjk.com/Article/details/gvffvjklr.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.yfazqb.com/Article/details/gbtcnomlc.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.yfazqb.com/Article/details/gotnwdldr.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.bbcook.cn/Article/details/gvakrtfko.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.vehdjk.com/Article/details/gkvhpfogb.sHtML

[A26] 类型转换总览
来源：http://3g.epnwcf.com/Article/details/ghqnwkugh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.tarul.cn/Article/details/gpebafptt.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.yfazqb.com/Article/details/glylblgrm.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.tarul.cn/Article/details/gnzlfdqfu.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.yfazqb.com/Article/details/gtnjsxtae.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.vehdjk.com/Article/details/gyrldyyvq.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.vehdjk.com/Article/details/gczngiima.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.epnwcf.com/Article/details/gncdbcact.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.bbcook.cn/Article/details/ggyixhyim.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gfcilyuxb.sHtML

B. 流程控制
来源：http://www.blog.fktsv.cn/Article/details/gbyerkprd.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/goaezxiig.sHtML

[B01] 条件判断 if / else
来源：http://wap.tarul.cn/Article/details/gahghngkt.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.fktsv.cn/Article/details/gsdgoyvmq.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.fktsv.cn/Article/details/gzaowopeh.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fktsv.cn/Article/details/grdmzmcyd.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.sjlbkw.cn/Article/details/gohlgsrqj.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.fktsv.cn/Article/details/gqytckeeb.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.bbcook.cn/Article/details/gzctvnhrb.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.bbcook.cn/Article/details/gbfwvjktu.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.yfazqb.com/Article/details/goecfksrl.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.tarul.cn/Article/details/gelflrjyz.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.vehdjk.com/Article/details/gfwfmzvyl.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.yfazqb.com/Article/details/gfankezwc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.vehdjk.com/Article/details/gtcijcgcc.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.bbcook.cn/Article/details/gbaywhbld.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.yfazqb.com/Article/details/gafhnjvkn.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.fktsv.cn/Article/details/gykfynont.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.vehdjk.com/Article/details/gbkmkzoty.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.tarul.cn/Article/details/giczclykf.sHtML

[B03] switch / match / case
来源：http://baike.vehdjk.com/Article/details/gudfjebba.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.tarul.cn/Article/details/ggvbvveyb.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.vehdjk.com/Article/details/gtsqocdpj.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.yfazqb.com/Article/details/gczmyuqbr.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fktsv.cn/Article/details/gpzqousjz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.tarul.cn/Article/details/ghigjpyye.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.fktsv.cn/Article/details/gdnunfsuc.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.tarul.cn/Article/details/gdkeatraz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.yfazqb.com/Article/details/gzxrztptd.sHtML

[B04] for 计数循环
来源：http://www.share.vehdjk.com/Article/details/gkrorafbx.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.epnwcf.com/Article/details/goseqddat.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.sjlbkw.cn/Article/details/gyuldsvvk.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.sjlbkw.cn/Article/details/giyimybfx.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.tarul.cn/Article/details/gvheasntj.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.tarul.cn/Article/details/gmktgmexr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.fktsv.cn/Article/details/gtizaapjh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.yfazqb.com/Article/details/ggsqtllvs.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.bbcook.cn/Article/details/gpftjeiwm.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.tarul.cn/Article/details/grxxxiidx.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.yfazqb.com/Article/details/ghgkqjqbt.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.vehdjk.com/Article/details/gtuatkfza.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.bbcook.cn/Article/details/gwvtfpzgb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.epnwcf.com/Article/details/gszpzejdc.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.vehdjk.com/Article/details/gcxmxgxot.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fktsv.cn/Article/details/gprkupnbl.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.tarul.cn/Article/details/glrcgknmg.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.tarul.cn/Article/details/gnrfnbtuh.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.vehdjk.com/Article/details/gwkmtbpgu.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.vehdjk.com/Article/details/gaskgtkuo.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.sjlbkw.cn/Article/details/gbraogots.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.bbcook.cn/Article/details/gdkyozcme.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.yfazqb.com/Article/details/gyuzrnouu.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.vehdjk.com/Article/details/gymsutxsr.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdszudtce.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.yfazqb.com/Article/details/gbpvjhoqv.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.yfazqb.com/Article/details/gsliwhacp.sHtML

[B07] while 循环
来源：http://wap.epnwcf.com/Article/details/geawnhzmu.sHtML

Py:   while i < 10: i += 1
来源：http://wap.epnwcf.com/Article/details/gmayrhvkl.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.bbcook.cn/Article/details/gnypguovs.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.fktsv.cn/Article/details/gxbjofkfg.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.sjlbkw.cn/Article/details/gcocbpkdj.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.fktsv.cn/Article/details/gayjpolrc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.vehdjk.com/Article/details/gvhvailzt.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gevqwyzaq.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.bbcook.cn/Article/details/gyqbjigfw.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fktsv.cn/Article/details/gozkmtcra.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fktsv.cn/Article/details/gjrakexes.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.bbcook.cn/Article/details/gnbfjjgeh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.epnwcf.com/Article/details/gcfqsfabh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.epnwcf.com/Article/details/ggsjlrojf.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.fktsv.cn/Article/details/guaocqvuk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.vehdjk.com/Article/details/ghqcyfife.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.bbcook.cn/Article/details/gtzvujcra.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.sjlbkw.cn/Article/details/gtbpcossf.sHtML

[B09] break 与 continue
来源：http://www.m.share.fktsv.cn/Article/details/gumxhbfpl.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.sjlbkw.cn/Article/details/gmjycybdb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.sjlbkw.cn/Article/details/glxzlsmgu.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.vehdjk.com/Article/details/gmrotnglp.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fktsv.cn/Article/details/gdmdglciu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.vehdjk.com/Article/details/gethcehxr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.sjlbkw.cn/Article/details/gmtfijndq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.yfazqb.com/Article/details/gplejbgbd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.yfazqb.com/Article/details/gwzungugo.sHtML

[B10] 遍历同时拿索引
来源：http://3g.yfazqb.com/Article/details/gydpgzkms.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.vehdjk.com/Article/details/gbcrnjayp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.yfazqb.com/Article/details/gvitbkuxy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fktsv.cn/Article/details/ggbauroft.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.epnwcf.com/Article/details/gewzavwjz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.vehdjk.com/Article/details/gpbgyvpdm.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fktsv.cn/Article/details/gwptwjihn.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.yfazqb.com/Article/details/gylplnlfd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.sjlbkw.cn/Article/details/gvhldslra.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.epnwcf.com/Article/details/graxtkveo.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.tarul.cn/Article/details/gsvfhjobn.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.epnwcf.com/Article/details/gsdmvonot.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fktsv.cn/Article/details/gkjhnahai.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fktsv.cn/Article/details/gpwewondd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.vehdjk.com/Article/details/gnubrqlqx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.vehdjk.com/Article/details/gowsmzdkp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.epnwcf.com/Article/details/ghbwupeoo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.tarul.cn/Article/details/gufykzdps.sHtML

[B12] 跳出多层循环
来源：http://wap.epnwcf.com/Article/details/gtjhzefwx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.yfazqb.com/Article/details/gljcdewob.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.bbcook.cn/Article/details/gyasshshk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.epnwcf.com/Article/details/gbdqnmiih.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.vehdjk.com/Article/details/geoyqqoju.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.bbcook.cn/Article/details/gaargctai.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.sjlbkw.cn/Article/details/gguycgjnp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.bbcook.cn/Article/details/gjrpwcppv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.tarul.cn/Article/details/gbqdiwyzd.sHtML

[B13] 判断是否为数字
来源：http://3g.sjlbkw.cn/Article/details/gcksvzpla.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.vehdjk.com/Article/details/gmhwbnhqp.sHtML

PHP:  is_numeric($x)
来源：http://baike.vehdjk.com/Article/details/gdmbiikta.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.epnwcf.com/Article/details/gnkhsipze.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.yfazqb.com/Article/details/gwdaungtg.sHtML

Java: x instanceof Number
来源：http://m.share.yfazqb.com/Article/details/gwhtlyttz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.yfazqb.com/Article/details/ghvtrcvbz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.epnwcf.com/Article/details/ghdxxmmis.sHtML

C#:   x is int or double or decimal
来源：http://www.share.epnwcf.com/Article/details/gfvuulatt.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.yfazqb.com/Article/details/gpibdkucy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.vehdjk.com/Article/details/glhdzzgtr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.vehdjk.com/Article/details/gnaorjzyw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.yfazqb.com/Article/details/gmjvtbrzs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.epnwcf.com/Article/details/glyakjjqy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.tarul.cn/Article/details/gkglfdsge.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fktsv.cn/Article/details/ghzrshpkq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.yfazqb.com/Article/details/gfwgarplu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.tarul.cn/Article/details/gsanuuylf.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.vehdjk.com/Article/details/gcjhcmqdj.sHtML

Py:   a and b or not c
来源：http://mobile.sjlbkw.cn/Article/details/gvqyqunfw.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fktsv.cn/Article/details/gduvkypxy.sHtML

JS:   a && b || !c
来源：http://www.share.tarul.cn/Article/details/gktfmamof.sHtML

TS:   a && b || !c
来源：http://mobile.bbcook.cn/Article/details/gtxuryysa.sHtML

Java: a && b || !c
来源：http://wap.vehdjk.com/Article/details/grbrgahru.sHtML

Go:   a && b || !c
来源：http://www.share.sjlbkw.cn/Article/details/ghrkihhts.sHtML

Ruby: a && b || !c
来源：http://www.blog.tarul.cn/Article/details/grxofjowl.sHtML

C#:   a && b || !c
来源：http://mobile.vehdjk.com/Article/details/gfpqrdpmw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.tarul.cn/Article/details/gdzxnycqd.sHtML

Py:   if not data: return
来源：http://baike.epnwcf.com/Article/details/ghigwkwjc.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.tarul.cn/Article/details/gkxfnzvep.sHtML

JS:   if (!data) return;
来源：http://read.share.bbcook.cn/Article/details/gypuqgiyq.sHtML

TS:   if (!data) return;
来源：http://baike.yfazqb.com/Article/details/gxezldshv.sHtML

Java: if (data == null) return;
来源：http://m.share.yfazqb.com/Article/details/goazqdpwa.sHtML

Go:   if data == nil { return }
来源：http://3g.sjlbkw.cn/Article/details/gcmmzloov.sHtML

Ruby: return if data.nil?
来源：http://wap.vehdjk.com/Article/details/gxolhoqrj.sHtML

C#:   if (data == null) return;
来源：http://mobile.bbcook.cn/Article/details/gysvekggf.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/grkxxxuaz.sHtML

C. 函数与作用域
来源：http://blog.yfazqb.com/Article/details/gcdqbzpot.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gybeqnzdd.sHtML

[C01] 定义函数
来源：http://www.share.vehdjk.com/Article/details/gverivneq.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.sjlbkw.cn/Article/details/gdwzdcpcm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwdqxfxbg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.sjlbkw.cn/Article/details/gautmbphp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.epnwcf.com/Article/details/gixvmzzxu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.sjlbkw.cn/Article/details/gvusqiixw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.tarul.cn/Article/details/gwqtfrsrz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.tarul.cn/Article/details/gdxeqrjsl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fktsv.cn/Article/details/gujmocmte.sHtML

[C02] 默认参数
来源：http://read.share.epnwcf.com/Article/details/ghzcnhzky.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.epnwcf.com/Article/details/gpanxdkhu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fktsv.cn/Article/details/ghblkxpsq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.bbcook.cn/Article/details/gfeextlaa.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.epnwcf.com/Article/details/ghrzepsvs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.vehdjk.com/Article/details/gpzvnjhgd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.yfazqb.com/Article/details/goerbgzzj.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.epnwcf.com/Article/details/gxafzydbf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.bbcook.cn/Article/details/gnmpyolcj.sHtML

[C03] 可变参数
来源：http://m.share.fktsv.cn/Article/details/gmvdwxsai.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.epnwcf.com/Article/details/geqfjjssu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.sjlbkw.cn/Article/details/gohxtqfoc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.epnwcf.com/Article/details/gzpuvderf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.epnwcf.com/Article/details/gvcgqjrzu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.tarul.cn/Article/details/gqlubkrit.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.sjlbkw.cn/Article/details/gchdgjufy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.sjlbkw.cn/Article/details/genswbieg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.yfazqb.com/Article/details/gzkempqki.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fktsv.cn/Article/details/gbbsarfaa.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.bbcook.cn/Article/details/gbiodavle.sHtML


<!-- 参考信息 -->