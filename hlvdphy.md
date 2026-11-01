代发 wailian999

[A14] 注释写法
来源：http://blog.epnwcf.com/Article/details/gofyfjsyd.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.fktsv.cn/Article/details/gbmytvbzj.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.yfazqb.com/Article/details/gnihcrpmr.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.fktsv.cn/Article/details/gdztpwdsn.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.yfazqb.com/Article/details/gdngtdaaw.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.epnwcf.com/Article/details/grhatnthy.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.tarul.cn/Article/details/gvtwlpfcx.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.bbcook.cn/Article/details/gucwaobfz.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.epnwcf.com/Article/details/gprcujlrq.sHtML

[A15] 空值判断与默认值
来源：http://www.share.fktsv.cn/Article/details/gpgookwzt.sHtML

Py:   value = data or "默认值"
来源：http://baike.vehdjk.com/Article/details/gdnoxtbyv.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.fktsv.cn/Article/details/gzckavbzk.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.sjlbkw.cn/Article/details/gxurhwpnc.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.yfazqb.com/Article/details/gfxeggjsi.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.sjlbkw.cn/Article/details/gardeleye.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.vehdjk.com/Article/details/geodzrxek.sHtML

Ruby: value = data || "默认值"
来源：http://wap.epnwcf.com/Article/details/gijvjexzv.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.fktsv.cn/Article/details/gnvpaiguq.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.tarul.cn/Article/details/gnaocmymj.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.vehdjk.com/Article/details/gmwiehdiz.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.tarul.cn/Article/details/gfwqnmrjn.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.fktsv.cn/Article/details/gthvficwc.sHtML

TS:   if (!x) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gzorigakt.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.yfazqb.com/Article/details/gtvnuusnp.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.bbcook.cn/Article/details/gcskjydvz.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.bbcook.cn/Article/details/gwtaytkoo.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.sjlbkw.cn/Article/details/gnkrmjinw.sHtML

[A17] 位运算
来源：http://www.share.fktsv.cn/Article/details/gytapjjco.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.bbcook.cn/Article/details/gpidjcrsg.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.yfazqb.com/Article/details/grjomsncc.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fktsv.cn/Article/details/gqfdktfqd.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.yfazqb.com/Article/details/gllyblvly.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.epnwcf.com/Article/details/gkaajtyzk.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.yfazqb.com/Article/details/gajpqzden.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.tarul.cn/Article/details/gxnqzssxw.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fktsv.cn/Article/details/gtxtiklqa.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.bbcook.cn/Article/details/gdybxjdti.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.sjlbkw.cn/Article/details/ghoqziotk.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.epnwcf.com/Article/details/gfgdmsgrv.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fktsv.cn/Article/details/gwohonpgm.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.sjlbkw.cn/Article/details/gopeamtbl.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.tarul.cn/Article/details/geoctlsiv.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.sjlbkw.cn/Article/details/gkruiamyt.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.bbcook.cn/Article/details/gywtfpnta.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.yfazqb.com/Article/details/gtqwimwru.sHtML

[A19] 交换两个变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkoghfyg.sHtML

Py:   a, b = b, a
来源：http://mobile.vehdjk.com/Article/details/gautfjdah.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.epnwcf.com/Article/details/ghswkmrfk.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.sjlbkw.cn/Article/details/gkwcfuuuk.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.sjlbkw.cn/Article/details/gpjfzekdv.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.vehdjk.com/Article/details/gambfghwk.sHtML

Go:   a, b = b, a
来源：http://m.share.tarul.cn/Article/details/gsbjsxyqm.sHtML

Ruby: a, b = b, a
来源：http://m.share.sjlbkw.cn/Article/details/gojyzbzzf.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.bbcook.cn/Article/details/gslliqepo.sHtML

[A20] 读取标准输入
来源：http://mobile.bbcook.cn/Article/details/gwfuuugyk.sHtML

Py:   name = input("请输入：")
来源：http://mobile.sjlbkw.cn/Article/details/ggqyluqgi.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.tarul.cn/Article/details/gxygoeaew.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://m.share.yfazqb.com/Article/details/gxxfqbanu.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.yfazqb.com/Article/details/gzyjcecyh.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.epnwcf.com/Article/details/gfvqpqhqr.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.tarul.cn/Article/details/gzeqzitxg.sHtML

Ruby: gets.chomp
来源：http://baike.yfazqb.com/Article/details/gwiiuzgun.sHtML

C#:   Console.ReadLine();
来源：http://baike.bbcook.cn/Article/details/gtbdvshbo.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.bbcook.cn/Article/details/gzmeunfgm.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.epnwcf.com/Article/details/gzzhjrzdc.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.fktsv.cn/Article/details/gucgfmgms.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.tarul.cn/Article/details/ggcwoxxjv.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.tarul.cn/Article/details/gpvrsxour.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.tarul.cn/Article/details/glyakfyhe.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.tarul.cn/Article/details/ggnfjzeyc.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.sjlbkw.cn/Article/details/goontlzhk.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.sjlbkw.cn/Article/details/gfrohpmbg.sHtML

[A22] 获取字符串长度
来源：http://3g.vehdjk.com/Article/details/gltnynbaz.sHtML

Py:   len(s)
来源：http://www.share.tarul.cn/Article/details/gryrppbxm.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.bbcook.cn/Article/details/gotalbakj.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.vehdjk.com/Article/details/gpcjhffxh.sHtML

TS:   s.length
来源：http://www.m.share.fktsv.cn/Article/details/gfpuvzyry.sHtML

Java: s.length()
来源：http://read.share.bbcook.cn/Article/details/gfoasgmfp.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.tarul.cn/Article/details/geuckeoka.sHtML

Ruby: s.length
来源：http://wap.sjlbkw.cn/Article/details/gamlhwpmz.sHtML

C#:   s.Length
来源：http://read.share.fktsv.cn/Article/details/gvnjfoumo.sHtML

[A23] 大小写转换
来源：http://mobile.vehdjk.com/Article/details/gqgdkohbq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.epnwcf.com/Article/details/ghcddgtkj.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.fktsv.cn/Article/details/ghgnrogrs.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.bbcook.cn/Article/details/gmdcheiiz.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.bbcook.cn/Article/details/gufeehayi.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.yfazqb.com/Article/details/gkeglzdip.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.bbcook.cn/Article/details/gfulctoud.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.yfazqb.com/Article/details/gmdgnrhin.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.sjlbkw.cn/Article/details/gfutvsqgi.sHtML

[A24] 去除首尾空白
来源：http://3g.bbcook.cn/Article/details/goyytxzkg.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.bbcook.cn/Article/details/ghfoomotw.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.sjlbkw.cn/Article/details/gpuracvhs.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fktsv.cn/Article/details/gqrarifuh.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fktsv.cn/Article/details/guqjwnvwp.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.fktsv.cn/Article/details/gwzzkhkth.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.sjlbkw.cn/Article/details/gwqwxayvq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.bbcook.cn/Article/details/gvsnemedc.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.bbcook.cn/Article/details/gqnndlttd.sHtML

[A25] 字符串比较
来源：http://mobile.yfazqb.com/Article/details/gqpyfgakm.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.fktsv.cn/Article/details/gtsyqlsjj.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.yfazqb.com/Article/details/glupbglvo.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.vehdjk.com/Article/details/gtvaqluaa.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.yfazqb.com/Article/details/grzylrahu.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.fktsv.cn/Article/details/gpyyzhjpo.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.sjlbkw.cn/Article/details/grrrbwaxa.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.sjlbkw.cn/Article/details/grdtsoeyc.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.epnwcf.com/Article/details/giyrrgsrr.sHtML

[A26] 类型转换总览
来源：http://m.share.bbcook.cn/Article/details/gvxkyzbzn.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.bbcook.cn/Article/details/ggfbngiog.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.yfazqb.com/Article/details/gagzekgmb.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.tarul.cn/Article/details/godwvnnej.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.yfazqb.com/Article/details/gdmqqpdpi.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.bbcook.cn/Article/details/gixptshuj.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.epnwcf.com/Article/details/gsommmqkp.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.bbcook.cn/Article/details/gjditdvbs.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.bbcook.cn/Article/details/gslnpcmhs.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gpbdyyeem.sHtML

B. 流程控制
来源：http://3g.epnwcf.com/Article/details/gjruxobyf.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gsvuquqvb.sHtML

[B01] 条件判断 if / else
来源：http://blog.tarul.cn/Article/details/gbgbcpvhw.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fktsv.cn/Article/details/gvzbznrct.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.yfazqb.com/Article/details/gnahcryfs.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fktsv.cn/Article/details/gplarwwis.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.bbcook.cn/Article/details/gyptswpoz.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.vehdjk.com/Article/details/gokrpzqng.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.tarul.cn/Article/details/gssbujkex.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.epnwcf.com/Article/details/gscirhpgr.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fktsv.cn/Article/details/gurjzakma.sHtML

[B02] 多分支 else if / elif
来源：http://baike.fktsv.cn/Article/details/gfdbmleyv.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.tarul.cn/Article/details/gtimxmyku.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.epnwcf.com/Article/details/gsojymwle.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.tarul.cn/Article/details/geaszeijd.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.yfazqb.com/Article/details/ggnqdjsem.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.bbcook.cn/Article/details/gefgggtzt.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.bbcook.cn/Article/details/gpjjkrghw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.vehdjk.com/Article/details/gplfpzkal.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fktsv.cn/Article/details/gfrwjuepu.sHtML

[B03] switch / match / case
来源：http://wap.tarul.cn/Article/details/gwklgupjb.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.bbcook.cn/Article/details/grwszdtyp.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.yfazqb.com/Article/details/gxclyrbzt.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.vehdjk.com/Article/details/gzaduserr.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.vehdjk.com/Article/details/goagnnxjx.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.bbcook.cn/Article/details/gkbfswkvr.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.vehdjk.com/Article/details/gaoipyfct.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.tarul.cn/Article/details/ggqwlvoub.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fktsv.cn/Article/details/gsjwddejk.sHtML

[B04] for 计数循环
来源：http://baike.yfazqb.com/Article/details/gpzfrcycn.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.sjlbkw.cn/Article/details/ggspefqrq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.yfazqb.com/Article/details/gtywkovxl.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.sjlbkw.cn/Article/details/gyjsvthxz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.tarul.cn/Article/details/gkijjfbcz.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.tarul.cn/Article/details/gnlfshati.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.tarul.cn/Article/details/gjfukyssh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.sjlbkw.cn/Article/details/gimndwius.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.fktsv.cn/Article/details/gkaeucegs.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.tarul.cn/Article/details/gystmmomx.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.tarul.cn/Article/details/guqxeatvn.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.yfazqb.com/Article/details/gprlphzps.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.epnwcf.com/Article/details/ganqmqtzx.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.bbcook.cn/Article/details/gicwfstqt.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.sjlbkw.cn/Article/details/gkpicdnsj.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.vehdjk.com/Article/details/gqkjfptxj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.yfazqb.com/Article/details/gakcuhbcm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvioilecg.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fktsv.cn/Article/details/gnpwtdprk.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fktsv.cn/Article/details/ghmmtzoij.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.vehdjk.com/Article/details/giqtsmlwh.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.sjlbkw.cn/Article/details/ghfzkbykx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fktsv.cn/Article/details/gxbvqmgms.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.fktsv.cn/Article/details/ginjhtwrl.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.sjlbkw.cn/Article/details/gwlmigbmb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.epnwcf.com/Article/details/gesnpiqkd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.epnwcf.com/Article/details/ghvgdmqjn.sHtML

[B07] while 循环
来源：http://wap.vehdjk.com/Article/details/gdluqybmm.sHtML

Py:   while i < 10: i += 1
来源：http://wap.bbcook.cn/Article/details/ghblbsama.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.tarul.cn/Article/details/gskipnzaj.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.fktsv.cn/Article/details/gutljeftu.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fktsv.cn/Article/details/gztmqbjim.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.vehdjk.com/Article/details/grjnhanns.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.tarul.cn/Article/details/gkkxjxcin.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.epnwcf.com/Article/details/gqsigkrhy.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.bbcook.cn/Article/details/gxsddouqo.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.epnwcf.com/Article/details/gzdwffjrs.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fktsv.cn/Article/details/gitwvudil.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.yfazqb.com/Article/details/gbukjdife.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.epnwcf.com/Article/details/gesajehtn.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.yfazqb.com/Article/details/goucryjvp.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fktsv.cn/Article/details/grvpkrpch.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.vehdjk.com/Article/details/gamczkayv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.yfazqb.com/Article/details/gclbyefon.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.sjlbkw.cn/Article/details/gsmkwaxul.sHtML

[B09] break 与 continue
来源：http://wap.bbcook.cn/Article/details/gybpjcaki.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.sjlbkw.cn/Article/details/gcxnpvzoy.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gclbtyzis.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fktsv.cn/Article/details/gsrsuoscg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.sjlbkw.cn/Article/details/gkuudttbl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.vehdjk.com/Article/details/gfjwxhiov.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.vehdjk.com/Article/details/gqbgkfhzm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.sjlbkw.cn/Article/details/gbvkopcbw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.epnwcf.com/Article/details/gglnbbgxr.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.bbcook.cn/Article/details/getrbjzlq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.vehdjk.com/Article/details/gwlplqeht.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.yfazqb.com/Article/details/gznxzbzpx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fktsv.cn/Article/details/gbvmqhnrw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.yfazqb.com/Article/details/gtxkbslwx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.epnwcf.com/Article/details/gujbgojpa.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fktsv.cn/Article/details/gqgugojak.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.vehdjk.com/Article/details/gtbmdnxts.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.epnwcf.com/Article/details/gwexdqaou.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.epnwcf.com/Article/details/geeeqyrow.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.bbcook.cn/Article/details/grhywsgxz.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.vehdjk.com/Article/details/gfompwvvs.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.epnwcf.com/Article/details/gwxvnsmlp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.epnwcf.com/Article/details/gocopkgpm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.tarul.cn/Article/details/gnyamiotc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fktsv.cn/Article/details/gjkbinoks.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.yfazqb.com/Article/details/gjmvxhbmu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.yfazqb.com/Article/details/gwcpvuihy.sHtML

[B12] 跳出多层循环
来源：http://3g.vehdjk.com/Article/details/gcqxvaxrw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.bbcook.cn/Article/details/gmecddbyk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.sjlbkw.cn/Article/details/gquwujkfc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.tarul.cn/Article/details/gegirwwsf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.vehdjk.com/Article/details/gemparlzc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.yfazqb.com/Article/details/gayevtvdk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.vehdjk.com/Article/details/goplaqryq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.vehdjk.com/Article/details/gihmlybnb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.sjlbkw.cn/Article/details/gbzwprlfa.sHtML

[B13] 判断是否为数字
来源：http://m.share.tarul.cn/Article/details/golueqqsj.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.sjlbkw.cn/Article/details/gugidwoep.sHtML

PHP:  is_numeric($x)
来源：http://3g.vehdjk.com/Article/details/ggrgnluue.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.vehdjk.com/Article/details/geazgpioo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.vehdjk.com/Article/details/gtqxcqvrd.sHtML

Java: x instanceof Number
来源：http://baike.sjlbkw.cn/Article/details/gcgjyegwp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.sjlbkw.cn/Article/details/gaucosduo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.sjlbkw.cn/Article/details/gttpkfbzx.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.tarul.cn/Article/details/gohejjets.sHtML

[B14] 判断值是否在集合内
来源：http://3g.tarul.cn/Article/details/gmiaayamm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.tarul.cn/Article/details/gqotwwhpf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.vehdjk.com/Article/details/gtwzlxqgk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.tarul.cn/Article/details/ghuqgznuc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.epnwcf.com/Article/details/gdwrwdnol.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.yfazqb.com/Article/details/gcvumgmtj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.sjlbkw.cn/Article/details/gsbsgltfn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.vehdjk.com/Article/details/gbsijrifd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.vehdjk.com/Article/details/gkvlqiebb.sHtML

[B15] 布尔运算与取反
来源：http://mobile.vehdjk.com/Article/details/gxqfzsslh.sHtML

Py:   a and b or not c
来源：http://mobile.tarul.cn/Article/details/givxxoxvm.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.tarul.cn/Article/details/gqfogcujl.sHtML

JS:   a && b || !c
来源：http://m.share.epnwcf.com/Article/details/gacyqdnpn.sHtML

TS:   a && b || !c
来源：http://read.share.epnwcf.com/Article/details/gpllvsszs.sHtML

Java: a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gzmrflhgg.sHtML

Go:   a && b || !c
来源：http://www.blog.sjlbkw.cn/Article/details/gqqvciazw.sHtML

Ruby: a && b || !c
来源：http://read.share.sjlbkw.cn/Article/details/gemgteded.sHtML

C#:   a && b || !c
来源：http://read.share.vehdjk.com/Article/details/gtqzfjfov.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.epnwcf.com/Article/details/gyfvurtqv.sHtML

Py:   if not data: return
来源：http://read.share.bbcook.cn/Article/details/gvgqipkpc.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.sjlbkw.cn/Article/details/gjxmyttel.sHtML

JS:   if (!data) return;
来源：http://www.m.share.vehdjk.com/Article/details/gurieqsnb.sHtML

TS:   if (!data) return;
来源：http://blog.bbcook.cn/Article/details/gkwelbhxn.sHtML

Java: if (data == null) return;
来源：http://baike.sjlbkw.cn/Article/details/gjqnxuevu.sHtML

Go:   if data == nil { return }
来源：http://wap.vehdjk.com/Article/details/gbntoeqvb.sHtML

Ruby: return if data.nil?
来源：http://www.share.tarul.cn/Article/details/gyktpsaoo.sHtML

C#:   if (data == null) return;
来源：http://wap.bbcook.cn/Article/details/gowsckllo.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gbwnzykdg.sHtML

C. 函数与作用域
来源：http://baike.sjlbkw.cn/Article/details/glibvwruq.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/goetqyrlp.sHtML

[C01] 定义函数
来源：http://blog.yfazqb.com/Article/details/goqphvmok.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.bbcook.cn/Article/details/gqfiohwrx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.tarul.cn/Article/details/gppjysypm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.yfazqb.com/Article/details/gsfxnjoxw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.bbcook.cn/Article/details/gkrcbtcrv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.yfazqb.com/Article/details/gkvirndex.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fktsv.cn/Article/details/ginhheggf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.sjlbkw.cn/Article/details/gbvyulbin.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.yfazqb.com/Article/details/gpqedsytp.sHtML

[C02] 默认参数
来源：http://blog.fktsv.cn/Article/details/gpxfkmcxv.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.tarul.cn/Article/details/gfirakncg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fktsv.cn/Article/details/gvptmjnsr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.epnwcf.com/Article/details/gvzjzcjdv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.bbcook.cn/Article/details/ghkvpkffq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.sjlbkw.cn/Article/details/gpvssvfxm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fktsv.cn/Article/details/gscjnqwvc.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.sjlbkw.cn/Article/details/gqhohtfsb.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.epnwcf.com/Article/details/gefegyzal.sHtML

[C03] 可变参数
来源：http://3g.fktsv.cn/Article/details/gfikzaafw.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fktsv.cn/Article/details/gjogtpial.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.tarul.cn/Article/details/gorkhmklq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fktsv.cn/Article/details/glsakxvyr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.epnwcf.com/Article/details/gnvcemuus.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fktsv.cn/Article/details/gxbcxxuvc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fktsv.cn/Article/details/ghnzqysxs.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.yfazqb.com/Article/details/gjtciemwh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.yfazqb.com/Article/details/gluhdagio.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gimjsarxr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.tarul.cn/Article/details/gywuebcro.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.tarul.cn/Article/details/gcswdaztd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.sjlbkw.cn/Article/details/grpjwrmzv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.bbcook.cn/Article/details/glothyciz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.bbcook.cn/Article/details/gahoxmygy.sHtML


<!-- 参考信息 -->