代发 wailian999

[A06] 字符串转数字
来源：http://byo.vehdjk.com

Py:   int("42"); float("3.14")
来源：http://mlq.birdmap.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yiv.uphjek.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://sek.nwbrower.top

TS:   parseInt("42", 10); Number("42")
来源：http://vfp.tian-w.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://end.vqdsnc.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pta.ctjpmb.com

Ruby: "42".to_i; "3.14".to_f
来源：http://qpv.0kj1m.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kqx.shanyushiyangkeji.top

[A07] 数字转字符串
来源：http://vlw.jinghuilouyu.cn

Py:   str(42)
来源：http://kya.fanxiaobao.xyz

PHP:  (string) 42; strval(42)
来源：http://epf.xingfuxueyuan.xyz

JS:   String(42); (42).toString()
来源：http://mfa.fktsv.cn

TS:   String(42)
来源：http://ldb.yfazqb.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://bkc.tanke756.top

Go:   strconv.Itoa(42)
来源：http://kag.zhijiandao.cn

Ruby: 42.to_s
来源：http://jzk.birdmap.top

C#:   42.ToString()
来源：http://xrr.yuanzhike.top

[A08] 取整与四舍五入
来源：http://zce.316326.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mce.cqqwz.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kfj.jqgufenzy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wea.jlsjyb.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://urp.zhiwuduotai.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kcl.gotoacloud.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ssq.ppjwa.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://rta.fktsv.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://exg.sufxvd.cn

[A09] 绝对值与最大最小值
来源：http://xgz.hesvh.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vgt.shangyingyoupin.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kax.shanyushiyangkeji.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hzk.fehbvm.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://otg.jlsjyb.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://erh.hammf.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://soh.nwbrower.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://icu.redwolf501.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vor.chenzaomai.com

[A10] 生成随机数
来源：http://pgx.uphjek.com

Py:   import random; random.randint(1, 100)
来源：http://adu.tianlin.xyz

PHP:  random_int(1, 100);
来源：http://lgu.fzhhl.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vwg.yfazqb.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cnl.ydjk.org.cn

Java: new Random().nextInt(100) + 1
来源：http://ofm.yongpay.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ecj.shanyushiyangkeji.top

Ruby: rand(1..100)
来源：http://dso.sufxvd.cn

C#:   new Random().Next(1, 101)
来源：http://pos.quarkkingdee.top

[A11] 条件表达式（三元）
来源：http://urb.quarkkingdee.top

Py:   "yes" if x > 0 else "no"
来源：http://gff.xinyue.icu

PHP:  $x > 0 ? "yes" : "no"
来源：http://tnd.redwolf501.top

JS:   x > 0 ? "yes" : "no"
来源：http://hun.feifeiyinyue.top

TS:   x > 0 ? "yes" : "no"
来源：http://fzy.316326.xyz

Java: x > 0 ? "yes" : "no"
来源：http://nke.hammf.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://sqo.jinyuanbaomall.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ywd.jinqigufen.top

C#:   x > 0 ? "yes" : "no"
来源：http://zbf.ctjpmb.com

[A12] 字符串插值 / 格式化
来源：http://vog.zycfv.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ybt.meibo888.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ths.kuanghao11.cn

JS:   `Hello, ${name}!`
来源：http://yli.zdbjq.cn

TS:   `Hello, ${name}!`
来源：http://bzh.jyoumei.cn

Java: "Hello, %s!".formatted(name)
来源：http://imp.yongpay.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://sap.vehdjk.com

Ruby: "Hello, #{name}!"
来源：http://dzv.hnqzz.top

C#:   $"Hello, {name}!"
来源：http://mpa.jinqigfzy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://rwm.xuanzx.com

Py:   "第一行\n第二行"
来源：http://qqt.feifeiyinyue.top

PHP:  "第一行\n第二行"
来源：http://ukp.cdnleiting.top

JS:   "第一行\n第二行"
来源：http://nqy.gzhubu.top

TS:   "第一行\n第二行"
来源：http://gmk.pengpengdd.cyou

Java: "第一行\n第二行"
来源：http://saj.zhiwuduotai.top

Go:   "第一行\n第二行"
来源：http://hju.yangfankeji.com

Ruby: "第一行\n第二行"
来源：http://dro.52xcode.cn

C#:   "第一行\n第二行"
来源：http://vnf.xylfe.cn

[A14] 注释写法
来源：http://oxl.snrcjt.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ncj.hnqzz.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://sfy.zhoulong.xyz

JS:   // 单行；/* 多行 */
来源：http://rdj.sjlbkw.cn

TS:   // 单行；/* 多行 */
来源：http://flv.gzhubu.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yxi.mhx1999.top

Go:   // 单行；/* 多行 */
来源：http://xcj.zhongyouzk.top

Ruby: # 单行；=begin 多行 =end
来源：http://nhu.cheryme.top

C#:   // 单行；/* 多行 */
来源：http://giy.shzxlz.cn

[A15] 空值判断与默认值
来源：http://mwl.zhiwuduotai.top

Py:   value = data or "默认值"
来源：http://hwp.yuanzhike.top

PHP:  $value = $data ?? "默认值";
来源：http://smr.hfpthk.cn

JS:   const value = data ?? "默认值";
来源：http://ada.jinqigfzy.top

TS:   const value = data ?? "默认值";
来源：http://xxa.zycfv.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cdx.gaohongyu789.top

Go:   if data == "" { data = "默认值" }
来源：http://qtm.shangyingyoupin.top

Ruby: value = data || "默认值"
来源：http://obm.fanxiaobao.xyz

C#:   var value = data ?? "默认值";
来源：http://tra.vqdsnc.cn

[A16] 真假值判断规则
来源：http://csb.bjfxy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ust.cheryme.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fcd.guowangkeji.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zox.0kj1m.cn

TS:   if (!x) {}
来源：http://phi.vehdjk.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ukz.uphjek.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wnw.bjfxy.top

Ruby: unless x            # nil 与 false 为假
来源：http://rip.daria6918.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://uiv.quarkkingdee.top

[A17] 位运算
来源：http://qkg.tian-w.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gcs.xinyue.icu

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jrt.jqgfzy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pmq.ywan-chungtsiang.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nvj.chenzaomai.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vbh.yvedp.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vgm.shanyushiyangtech.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://efv.tarul.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://svq.mhx1999.top

[A18] 字符与 ASCII 码互转
来源：http://zbo.zhiwuduotai.top

Py:   ord("A"); chr(65)
来源：http://uzy.zhengqikj.top

PHP:  ord("A"); chr(65)
来源：http://elr.chenzaomai.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://und.hcnkem.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bmc.fehbvm.com

Java: (int) 'A'; (char) 65
来源：http://hcd.hongshengwenyu.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rnj.vqdsnc.cn

Ruby: "A".ord; 65.chr
来源：http://uld.c1oappe.top

C#:   (int)'A'; (char)65
来源：http://xad.hongshengwenyu.top

[A19] 交换两个变量
来源：http://qdh.yanxiufei.cn

Py:   a, b = b, a
来源：http://kgf.xuetiantiany.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hhq.cheryme.top

JS:   [a, b] = [b, a];
来源：http://uaw.zhaomingkeji.xyz

TS:   [a, b] = [b, a];
来源：http://jhd.tian-w.cn

Java: int t = a; a = b; b = t;
来源：http://jtq.dianchejie.cn

Go:   a, b = b, a
来源：http://iqo.redwolf501.top

Ruby: a, b = b, a
来源：http://bnw.hesvh.cn

C#:   (a, b) = (b, a);
来源：http://kwp.bbcook.cn

[A20] 读取标准输入
来源：http://sui.yanxiufei.cn

Py:   name = input("请输入：")
来源：http://pir.yonumen.top

PHP:  $name = trim(fgets(STDIN));
来源：http://zdq.dianchejie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kay.epnwcf.com

TS:   // Node.js：readline 模块
来源：http://xcf.ybcxt.top

Java: new Scanner(System.in).nextLine()
来源：http://ood.fktsv.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ptc.wangshuangyany.cn

Ruby: gets.chomp
来源：http://nga.uphjek.com

C#:   Console.ReadLine();
来源：http://pzl.xylfe.cn

[A21] 保留指定小数位输出
来源：http://tkq.jinyuanbaomall.cn

Py:   f"{3.14159:.2f}"
来源：http://ebm.dashuyun.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wzt.yuanzhike.top

JS:   (3.14159).toFixed(2)
来源：http://nat.shanyushiyangkeji.top

TS:   (3.14159).toFixed(2)
来源：http://aos.chenlongwang.top

Java: String.format("%.2f", 3.14159)
来源：http://exn.jinqigfzy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://twn.shanyushiyangkeji.top

Ruby: format("%.2f", 3.14159)
来源：http://pkj.yangfankeji.com

C#:   3.14159.ToString("F2")
来源：http://syz.yfazqb.com

[A22] 获取字符串长度
来源：http://xhv.zdqjudy.top

Py:   len(s)
来源：http://rbd.zhengqikj.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bsp.fktsv.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jln.yuxming.cn

TS:   s.length
来源：http://jla.shuidangran.top

Java: s.length()
来源：http://jbr.jyoumei.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sxh.316326.xyz

Ruby: s.length
来源：http://src.316326.xyz

C#:   s.Length
来源：http://qjd.fengsongda.top

[A23] 大小写转换
来源：http://kwt.zdqjudy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://nup.xuanzx.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lyk.zhoulong.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mfp.yuanzhike.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xxm.sweek.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hfs.hnxiangtu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yug.hongshengwenyu.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nlb.fanxiaobao.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://qdg.feifeiyinyue.top

[A24] 去除首尾空白
来源：http://qee.sufxvd.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vmx.yj20258888.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ebw.guannengcc.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hci.yj20258888.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tvu.birdmap.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://spb.feifeiyinyue.top

Go:   strings.TrimSpace(s)
来源：http://lnx.xziqi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pmf.jianghu66.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://htb.cucudq.cn

[A25] 字符串比较
来源：http://vqh.kuanghao11.cn

Py:   s1 == s2; s1 != s2
来源：http://jfg.ivvv.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jhq.cqqwz.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fat.dianchejie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mje.jqgfzy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hba.xylfe.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cnu.shuidangran.top

Ruby: s1 == s2; s1 <=> s2
来源：http://vyn.chenjidiqi.icu

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kvn.tianlin.xyz

[A26] 类型转换总览
来源：http://jak.hnqzz.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rbc.ydjk.org.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://smv.ydjk.org.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rpw.guannengcc.top

TS:   Number() String() Boolean() x as number
来源：http://fwl.bjfxy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://drz.bjfxy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lgr.aibaodan.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jqn.yfazqb.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hrx.smart0.xyz

================================================================================
来源：http://twa.ybcxt.top

B. 流程控制
来源：http://rhh.aizwys.cn

================================================================================
来源：http://hrl.wangshuangyany.cn

[B01] 条件判断 if / else
来源：http://yug.gzhubu.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ocr.xuanzx.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bvp.xziqi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zhf.gzhubu.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oro.chenjidiqi.icu

Java: String r = x > 0 ? "正" : "非正";
来源：http://dby.hysaishi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nfl.hesvh.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xky.jiagoushi.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bip.jqgufenzy.top

[B02] 多分支 else if / elif
来源：http://ffy.jyoumei.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ebq.c1oappe.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yad.hnqzz.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jsd.fktsv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://smj.xziqi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dur.c1oappe.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cxr.xinyue.icu

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xtv.52xcode.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fee.meibo888.top

[B03] switch / match / case
来源：http://eed.zhengqikj.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lrq.hnxiangtu.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jeu.jinqigfzy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rny.zycfv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cqb.316326.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zwn.dianchejie.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://icd.jyoumei.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ayq.epnwcf.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wul.iojbl.cn

[B04] for 计数循环
来源：http://efw.sjlbkw.cn

Py:   for i in range(10): print(i)
来源：http://dzj.zhijiandao.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qsb.nwbrower.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ncm.nanxinkj.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tao.shzxlz.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ser.316326.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://csv.smart0.xyz

Ruby: 10.times { |i| puts i }
来源：http://ucj.nanxuanxn.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dgj.hywenlv.cn

[B05] 遍历数组 / 列表
来源：http://gur.xziqi.cn

Py:   for item in arr: print(item)
来源：http://sxw.gaohongyu789.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kov.chenzaomai.com

JS:   for (const item of arr) { console.log(item); }
来源：http://jle.shzxlz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://buo.hesvh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vrk.chenjidiqi.icu

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nfu.yvedp.cn

Ruby: arr.each { |item| puts item }
来源：http://tkr.fanxiaobao.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nly.zycfv.cn

[B06] 遍历字典 / 对象
来源：http://ygo.sysykeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://wzd.fanxiaobao.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wsa.jqgufenzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qof.ivvv.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ona.sufxvd.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mcz.hcnkem.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tnr.tian-w.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kgf.guowangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://txj.vqdsnc.cn

[B07] while 循环
来源：http://utk.yuanzhike.top

Py:   while i < 10: i += 1
来源：http://nyf.yuxming.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hif.ivvv.top

JS:   while (i < 10) { i++; }
来源：http://tqs.cqqwz.cn

TS:   while (i < 10) { i++; }
来源：http://qgc.hcnkem.com

Java: while (i < 10) { i++; }
来源：http://pgs.zhongyouzk.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mxv.daria6918.cn

Ruby: while i < 10; i += 1; end
来源：http://ori.dashuyun.cn

C#:   while (i < 10) { i++; }
来源：http://xly.iojbl.cn

[B08] do-while（至少执行一次）
来源：http://xzc.gaohongyu789.top

Py:   # 无 do-while：用 while True + break
来源：http://eyz.daria6918.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://eoa.nanxuanxn.top

JS:   do { i++; } while (i < 10);
来源：http://omk.jianghu66.top

TS:   do { i++; } while (i < 10);
来源：http://adc.0kj1m.cn

Java: do { i++; } while (i < 10);
来源：http://bys.vqdsnc.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wxv.tian-w.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rxv.zhiwuduotai.top

C#:   do { i++; } while (i < 10);
来源：http://ejb.gogol.net.cn

[B09] break 与 continue
来源：http://ewe.uphjek.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zxo.epnwcf.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nql.chenjidiqi.icu

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://frz.ppjwa.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ipy.fehbvm.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wsj.guannengcc.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://spt.bbcook.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://irf.jianghu66.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sng.tarul.cn

[B10] 遍历同时拿索引
来源：http://coj.aibaodan.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vdz.ehwqpu.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://igi.zhongyouzk.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bkw.sxryk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://apo.hammf.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dlk.zhengqikj.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oru.jlsjyb.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://krz.cheryme.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rsu.daxiang520.top

[B11] 生成数字序列 / 区间
来源：http://ftv.dashuyun.cn

Py:   list(range(0, 10, 2))
来源：http://ujn.hnqzz.top

PHP:  range(0, 10, 2);
来源：http://jxw.ctjpmb.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sru.shzxlz.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://opv.jiagoushi.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gdb.yongpay.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wce.ehwqpu.com

Ruby: (0...10).step(2).to_a
来源：http://nkd.zdqjudy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xzi.shanyushiyangtech.top

[B12] 跳出多层循环
来源：http://qok.zhengqikj.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://omi.xinyue.icu

PHP:  # 无标签：用 goto 或函数返回
来源：http://vpf.hnxiangtu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kak.xuetiantiany.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cww.zdbjq.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mho.feifeiyinyue.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hfw.uphjek.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sdo.cucudq.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ldv.ywan-chungtsiang.top


<!-- 参考信息 -->