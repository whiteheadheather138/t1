代发 wailian999

Java: "第一行\n第二行"
来源：http://baike.fktsv.cn/Article/details/genfyzwyy.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.sjlbkw.cn/Article/details/grwgclglw.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.fktsv.cn/Article/details/gvuiclhcm.sHtML

C#:   "第一行\n第二行"
来源：http://baike.vehdjk.com/Article/details/gptdzktvz.sHtML

[A14] 注释写法
来源：http://mobile.yfazqb.com/Article/details/guiqmbpow.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.tarul.cn/Article/details/gdryhqvjs.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.sjlbkw.cn/Article/details/gbmavrrid.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.sjlbkw.cn/Article/details/gltesxvqa.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.yfazqb.com/Article/details/gqtufukfx.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.vehdjk.com/Article/details/gjvyqsosu.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.vehdjk.com/Article/details/glvgybrcu.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.sjlbkw.cn/Article/details/gzvrbsvgm.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.vehdjk.com/Article/details/gscgllwsu.sHtML

[A15] 空值判断与默认值
来源：http://m.share.sjlbkw.cn/Article/details/gvhnkajjd.sHtML

Py:   value = data or "默认值"
来源：http://mobile.epnwcf.com/Article/details/gxdrwrhax.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.epnwcf.com/Article/details/gwuroiaei.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.bbcook.cn/Article/details/gvekmwhew.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.sjlbkw.cn/Article/details/groimkerr.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.vehdjk.com/Article/details/gmqqmfmmk.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.sjlbkw.cn/Article/details/gqmiyfebm.sHtML

Ruby: value = data || "默认值"
来源：http://baike.fktsv.cn/Article/details/gddkjqgmy.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.tarul.cn/Article/details/gltfllxia.sHtML

[A16] 真假值判断规则
来源：http://read.share.bbcook.cn/Article/details/govlwfspd.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.fktsv.cn/Article/details/gjonctjyy.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.fktsv.cn/Article/details/gcyptcebv.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.tarul.cn/Article/details/gpgbyqcus.sHtML

TS:   if (!x) {}
来源：http://baike.bbcook.cn/Article/details/gjijkdpso.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.fktsv.cn/Article/details/gfflegalv.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.tarul.cn/Article/details/gqxnhdpjw.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.yfazqb.com/Article/details/geovecvsg.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.epnwcf.com/Article/details/gwxleceou.sHtML

[A17] 位运算
来源：http://www.blog.sjlbkw.cn/Article/details/gajvuaqov.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.bbcook.cn/Article/details/glerchtpn.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.fktsv.cn/Article/details/gourgqgdu.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.tarul.cn/Article/details/gkyinfwyy.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.fktsv.cn/Article/details/gkbhiaxwb.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.bbcook.cn/Article/details/gcqpcnqem.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.bbcook.cn/Article/details/gnniuouks.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.sjlbkw.cn/Article/details/gvpfzqseg.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fktsv.cn/Article/details/gjionarxf.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.yfazqb.com/Article/details/gqjnjunxn.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.epnwcf.com/Article/details/gkxatgcpw.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.sjlbkw.cn/Article/details/gkwgkproq.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fktsv.cn/Article/details/gxrzlownk.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.yfazqb.com/Article/details/gsrfqwgoa.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.tarul.cn/Article/details/gkvmgtkwu.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.tarul.cn/Article/details/gpnhusown.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.epnwcf.com/Article/details/gcpkgwxxp.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.fktsv.cn/Article/details/gcmqkgino.sHtML

[A19] 交换两个变量
来源：http://wap.epnwcf.com/Article/details/glodaynkb.sHtML

Py:   a, b = b, a
来源：http://wap.tarul.cn/Article/details/gjrcvvqru.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.tarul.cn/Article/details/grkewwddw.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.tarul.cn/Article/details/girohsbet.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.yfazqb.com/Article/details/gvophklnv.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.fktsv.cn/Article/details/gvnrpwyol.sHtML

Go:   a, b = b, a
来源：http://m.share.epnwcf.com/Article/details/gndxprsia.sHtML

Ruby: a, b = b, a
来源：http://blog.vehdjk.com/Article/details/gxkfxhqyp.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.fktsv.cn/Article/details/ghxcrooik.sHtML

[A20] 读取标准输入
来源：http://www.share.bbcook.cn/Article/details/gdvptjfiv.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.bbcook.cn/Article/details/gyrzqufht.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.bbcook.cn/Article/details/gycctlwdp.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.bbcook.cn/Article/details/gxlytxhiu.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.fktsv.cn/Article/details/gxbsayrxk.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.yfazqb.com/Article/details/gpbdardbj.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.bbcook.cn/Article/details/gcoqrhpfn.sHtML

Ruby: gets.chomp
来源：http://read.share.fktsv.cn/Article/details/ghxlnpjwv.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.epnwcf.com/Article/details/gktjrpmax.sHtML

[A21] 保留指定小数位输出
来源：http://blog.epnwcf.com/Article/details/gwvgbloxn.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.yfazqb.com/Article/details/gmkbqqqnx.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.epnwcf.com/Article/details/giymzomzh.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.epnwcf.com/Article/details/gwdvixdyh.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.epnwcf.com/Article/details/gckncglgx.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.bbcook.cn/Article/details/gdtlppiyw.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.yfazqb.com/Article/details/gfxbcuuoe.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.yfazqb.com/Article/details/gsnmocxhb.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.fktsv.cn/Article/details/ggdazweai.sHtML

[A22] 获取字符串长度
来源：http://blog.fktsv.cn/Article/details/gsmiqzdeg.sHtML

Py:   len(s)
来源：http://mobile.tarul.cn/Article/details/grlbmzgpj.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.tarul.cn/Article/details/gjcxkpcwy.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://m.share.epnwcf.com/Article/details/glmolnsvb.sHtML

TS:   s.length
来源：http://blog.vehdjk.com/Article/details/gzqogpiok.sHtML

Java: s.length()
来源：http://wap.bbcook.cn/Article/details/gwawcxwqb.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.share.fktsv.cn/Article/details/ggipclayz.sHtML

Ruby: s.length
来源：http://mobile.fktsv.cn/Article/details/gntyuqphm.sHtML

C#:   s.Length
来源：http://blog.tarul.cn/Article/details/gzccsends.sHtML

[A23] 大小写转换
来源：http://baike.bbcook.cn/Article/details/gzrpsutjp.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.fktsv.cn/Article/details/gwwdzrnqw.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.sjlbkw.cn/Article/details/grdugbptb.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.bbcook.cn/Article/details/gpnyccggp.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.sjlbkw.cn/Article/details/gdhxegzyi.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.yfazqb.com/Article/details/gxgvvduma.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.epnwcf.com/Article/details/guoqfqvao.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.epnwcf.com/Article/details/gztlujbia.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.tarul.cn/Article/details/gdmcqhkln.sHtML

[A24] 去除首尾空白
来源：http://baike.epnwcf.com/Article/details/gqogtaasa.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.yfazqb.com/Article/details/gbkjtkhnr.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.tarul.cn/Article/details/gefvtjylv.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.vehdjk.com/Article/details/gkxaenrdg.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fktsv.cn/Article/details/grbgmgttm.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.epnwcf.com/Article/details/gexrgmwrm.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.vehdjk.com/Article/details/gihnjyayz.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.bbcook.cn/Article/details/gvzwscgup.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.bbcook.cn/Article/details/gtbihmort.sHtML

[A25] 字符串比较
来源：http://read.share.epnwcf.com/Article/details/ghxxypbqa.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.sjlbkw.cn/Article/details/gmcrbskvl.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.bbcook.cn/Article/details/gqzyzyknl.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.epnwcf.com/Article/details/gubuwiuwu.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.tarul.cn/Article/details/gssuwglyk.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.fktsv.cn/Article/details/gmsytmvdc.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.bbcook.cn/Article/details/gexmydyfh.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.tarul.cn/Article/details/gxhjapehy.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.epnwcf.com/Article/details/gpaypncrq.sHtML

[A26] 类型转换总览
来源：http://blog.epnwcf.com/Article/details/gkqcbisni.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.sjlbkw.cn/Article/details/gqtbmfajj.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.bbcook.cn/Article/details/gmwppnvil.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.yfazqb.com/Article/details/gpuaxlxda.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.sjlbkw.cn/Article/details/gdmlhbrpk.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.epnwcf.com/Article/details/gtpcisxjo.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.bbcook.cn/Article/details/gdnzxrjov.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.bbcook.cn/Article/details/gwnaibrxx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.vehdjk.com/Article/details/glpbanpvh.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gglboamqu.sHtML

B. 流程控制
来源：http://m.share.tarul.cn/Article/details/ggihuczxx.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gvaxjiheq.sHtML

[B01] 条件判断 if / else
来源：http://baike.epnwcf.com/Article/details/guvbdcknm.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.yfazqb.com/Article/details/gejnpwzfm.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.fktsv.cn/Article/details/gcqwcowhj.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.tarul.cn/Article/details/geagqlrfb.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.bbcook.cn/Article/details/gsnqjibmu.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.epnwcf.com/Article/details/garjrhxpu.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.yfazqb.com/Article/details/gzaguqbtz.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.fktsv.cn/Article/details/gzbsuziyj.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.yfazqb.com/Article/details/gzpswlmvv.sHtML

[B02] 多分支 else if / elif
来源：http://blog.epnwcf.com/Article/details/grxpnxtcj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.sjlbkw.cn/Article/details/gzdeguhwy.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.tarul.cn/Article/details/gkxhwetow.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.bbcook.cn/Article/details/gxqhzwsji.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.vehdjk.com/Article/details/gzbtpccxm.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.tarul.cn/Article/details/gfhqiqyyc.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.sjlbkw.cn/Article/details/gpkomvnww.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.yfazqb.com/Article/details/gbdxnqamb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.vehdjk.com/Article/details/gvvudtmfs.sHtML

[B03] switch / match / case
来源：http://3g.sjlbkw.cn/Article/details/gijvadttz.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.vehdjk.com/Article/details/ggwdfissw.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.sjlbkw.cn/Article/details/gljiynzyr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.tarul.cn/Article/details/gomitkeym.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.epnwcf.com/Article/details/gtdnocote.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.tarul.cn/Article/details/grfzesxve.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.bbcook.cn/Article/details/gilgsoofb.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.tarul.cn/Article/details/gpdfhhhfs.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.bbcook.cn/Article/details/gbpytkumk.sHtML

[B04] for 计数循环
来源：http://mobile.fktsv.cn/Article/details/glxceraqe.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.bbcook.cn/Article/details/gmxptjaww.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.vehdjk.com/Article/details/gifdmxvyz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fktsv.cn/Article/details/gqqqyhhuo.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.epnwcf.com/Article/details/gpekafbdo.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.fktsv.cn/Article/details/gchurmess.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.bbcook.cn/Article/details/gfnyaxhcm.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.vehdjk.com/Article/details/gxbcluitp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.sjlbkw.cn/Article/details/gzgdpxkgy.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.tarul.cn/Article/details/grkrwlssy.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.sjlbkw.cn/Article/details/grtydxtmr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.sjlbkw.cn/Article/details/gbhjdjjmv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.bbcook.cn/Article/details/gchbykten.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.yfazqb.com/Article/details/gtajmragz.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.vehdjk.com/Article/details/gwxvvstnm.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.yfazqb.com/Article/details/giszyytwm.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.sjlbkw.cn/Article/details/gidexgrim.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.yfazqb.com/Article/details/gefisebdz.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.sjlbkw.cn/Article/details/gmstzyaor.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.vehdjk.com/Article/details/gwwbppwvf.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvyrhpbbs.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.tarul.cn/Article/details/gasgyfcuu.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.sjlbkw.cn/Article/details/grdkirikt.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fktsv.cn/Article/details/gxiyjdtfc.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.epnwcf.com/Article/details/gtpioyjwf.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.tarul.cn/Article/details/gfrnzufcw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.fktsv.cn/Article/details/gxkakdqtn.sHtML

[B07] while 循环
来源：http://m.share.tarul.cn/Article/details/gvlxnnyoe.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.sjlbkw.cn/Article/details/glbtvjohi.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.sjlbkw.cn/Article/details/gwvcqfxak.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.yfazqb.com/Article/details/gkmcsmtwa.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.yfazqb.com/Article/details/gyogqbjyc.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.fktsv.cn/Article/details/gldvbhdru.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.sjlbkw.cn/Article/details/gbthnezew.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.sjlbkw.cn/Article/details/ggnqyltzb.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.bbcook.cn/Article/details/gjfcsoawi.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.tarul.cn/Article/details/ggiwklhuj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.tarul.cn/Article/details/gwxgjefsj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.epnwcf.com/Article/details/gvbosxfai.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.tarul.cn/Article/details/ghodcnhwh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.vehdjk.com/Article/details/gezmcrvpn.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.sjlbkw.cn/Article/details/gtqgqzocd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.bbcook.cn/Article/details/gugadksnk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.sjlbkw.cn/Article/details/geisrfzqg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.epnwcf.com/Article/details/garupogbz.sHtML

[B09] break 与 continue
来源：http://www.blog.sjlbkw.cn/Article/details/gxsotvtiu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.bbcook.cn/Article/details/gvxjlvsyz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gkyxzvfbc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gsxtlylsh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.yfazqb.com/Article/details/gxefvtzax.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.bbcook.cn/Article/details/gicbtxgtu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fktsv.cn/Article/details/glfybuqkz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.vehdjk.com/Article/details/ggflfwtno.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.bbcook.cn/Article/details/gmxnsuxco.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.tarul.cn/Article/details/ggyxtjsbv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.sjlbkw.cn/Article/details/ghbdcxffr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fktsv.cn/Article/details/gaqfejnuj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.tarul.cn/Article/details/gfsonezcj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.epnwcf.com/Article/details/gsnkszrsg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.bbcook.cn/Article/details/goqnbbrjx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.tarul.cn/Article/details/gumycwued.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.vehdjk.com/Article/details/gszxlhrwa.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.tarul.cn/Article/details/gfsyijfsc.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.epnwcf.com/Article/details/gglgaoqon.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.sjlbkw.cn/Article/details/gktsmgnva.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.sjlbkw.cn/Article/details/gcnvseoyh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.yfazqb.com/Article/details/geimblmye.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.yfazqb.com/Article/details/gghqrzvwq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.yfazqb.com/Article/details/gqxfbgdpe.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.yfazqb.com/Article/details/gqlxhenju.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.yfazqb.com/Article/details/gajgoraln.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.vehdjk.com/Article/details/gbbubasml.sHtML

[B12] 跳出多层循环
来源：http://blog.yfazqb.com/Article/details/glosxxgvg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fktsv.cn/Article/details/ghorfxqdq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.epnwcf.com/Article/details/gvnmcerhr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.sjlbkw.cn/Article/details/gyipxheqm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.vehdjk.com/Article/details/gplgvrons.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.epnwcf.com/Article/details/gygxujhab.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.bbcook.cn/Article/details/gcfkevodo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.sjlbkw.cn/Article/details/gbehqyaze.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.epnwcf.com/Article/details/gykuliybk.sHtML

[B13] 判断是否为数字
来源：http://read.share.sjlbkw.cn/Article/details/gcuygqsky.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.yfazqb.com/Article/details/gjpygttuk.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.yfazqb.com/Article/details/gldhztrxs.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.epnwcf.com/Article/details/gtwpxpuza.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.epnwcf.com/Article/details/gstkaoywf.sHtML

Java: x instanceof Number
来源：http://3g.yfazqb.com/Article/details/gnziefvsl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.sjlbkw.cn/Article/details/gmrgkfmer.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.tarul.cn/Article/details/ggravavws.sHtML

C#:   x is int or double or decimal
来源：http://blog.vehdjk.com/Article/details/gtwegmqqv.sHtML

[B14] 判断值是否在集合内
来源：http://baike.sjlbkw.cn/Article/details/gfemjpgoz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fktsv.cn/Article/details/gwdaoicxz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.epnwcf.com/Article/details/grxnmcluc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.epnwcf.com/Article/details/gutpwzesl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.vehdjk.com/Article/details/gkohrlnur.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvavczejr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.yfazqb.com/Article/details/ghytefttx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.bbcook.cn/Article/details/gurbxpuyv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gitjpgcqa.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fktsv.cn/Article/details/ggxmwjtmr.sHtML

Py:   a and b or not c
来源：http://www.blog.epnwcf.com/Article/details/giavbgjay.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fktsv.cn/Article/details/ghswemerr.sHtML

JS:   a && b || !c
来源：http://3g.tarul.cn/Article/details/gspqtgmnl.sHtML

TS:   a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gsonvfaxv.sHtML

Java: a && b || !c
来源：http://3g.fktsv.cn/Article/details/gyfuuxlsj.sHtML

Go:   a && b || !c
来源：http://wap.vehdjk.com/Article/details/gatkqqtuw.sHtML

Ruby: a && b || !c
来源：http://www.blog.vehdjk.com/Article/details/gwrkqkvit.sHtML

C#:   a && b || !c
来源：http://wap.epnwcf.com/Article/details/gjjroxbja.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.bbcook.cn/Article/details/ggdfiyhto.sHtML

Py:   if not data: return
来源：http://mobile.tarul.cn/Article/details/gxsknmbid.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.tarul.cn/Article/details/gcdcftgcl.sHtML

JS:   if (!data) return;
来源：http://read.share.bbcook.cn/Article/details/gihlewngs.sHtML

TS:   if (!data) return;
来源：http://blog.tarul.cn/Article/details/gseaqslny.sHtML

Java: if (data == null) return;
来源：http://3g.bbcook.cn/Article/details/grbputcpd.sHtML

Go:   if data == nil { return }
来源：http://3g.bbcook.cn/Article/details/gaddlsill.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fktsv.cn/Article/details/gsycblape.sHtML

C#:   if (data == null) return;
来源：http://www.blog.bbcook.cn/Article/details/gmgikvisf.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/geqlaitgr.sHtML

C. 函数与作用域
来源：http://3g.fktsv.cn/Article/details/gcmasdzpv.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gjizrappx.sHtML

[C01] 定义函数
来源：http://m.share.tarul.cn/Article/details/gjnhmsixz.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fktsv.cn/Article/details/gvgiuhlat.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/gsictkevf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.vehdjk.com/Article/details/gjzxbqvqm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.yfazqb.com/Article/details/gkwsrylni.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fktsv.cn/Article/details/gxntqrplp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.tarul.cn/Article/details/gttdebbzw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.sjlbkw.cn/Article/details/gytfjrcfe.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.bbcook.cn/Article/details/gshxwqswq.sHtML

[C02] 默认参数
来源：http://baike.fktsv.cn/Article/details/ghnlwjgns.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.tarul.cn/Article/details/gtbailsee.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.bbcook.cn/Article/details/guzfqyawx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.epnwcf.com/Article/details/gtyanymhk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fktsv.cn/Article/details/gewpltxgv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.bbcook.cn/Article/details/gfjtuuccg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.bbcook.cn/Article/details/gvboareyu.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.epnwcf.com/Article/details/gmejhckru.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.tarul.cn/Article/details/glmcybphe.sHtML

[C03] 可变参数
来源：http://www.share.vehdjk.com/Article/details/gdtgezydh.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.yfazqb.com/Article/details/geqzbpedu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.tarul.cn/Article/details/gtohsfjxq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.yfazqb.com/Article/details/gjrkgjopf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.yfazqb.com/Article/details/guskzkihx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.yfazqb.com/Article/details/gqkhuuqrh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.sjlbkw.cn/Article/details/gxwamluvg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.sjlbkw.cn/Article/details/gcitpedwg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.vehdjk.com/Article/details/gkuvaidha.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.sjlbkw.cn/Article/details/getsnpbuc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.vehdjk.com/Article/details/gljpfyjve.sHtML


<!-- 参考信息 -->