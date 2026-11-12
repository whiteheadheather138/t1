代发 wailian999

Ruby: PI = 3.14159
来源：http://fgh.hammf.cn

C#:   const double PI = 3.14159;
来源：http://dib.xuetiantiany.cn

[A04] 判断变量类型
来源：http://vjv.tian-w.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://rao.aibaodan.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hfr.fengsongda.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://aca.gogol.net.cn

TS:   typeof x; x instanceof Date
来源：http://ity.fengsongda.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fmm.fengsongda.top

Go:   reflect.TypeOf(x).Name()
来源：http://uov.yongpay.top

Ruby: x.class; x.is_a?(Integer)
来源：http://sbz.uphjek.com

C#:   x.GetType().Name; x is int
来源：http://ave.jinyuanbaomall.cn

[A05] 整数除法与取模
来源：http://hwf.zhongyouzk.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vqm.jinqigufen.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://cuu.chenzaomai.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mnw.yangfankeji.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xqq.jianghu66.top

Java: 7 / 2; 7 % 2
来源：http://wif.shangyingyoupin.top

Go:   7 / 2; 7 % 2
来源：http://qqv.0kj1m.cn

Ruby: 7 / 2; 7 % 2
来源：http://yef.jinghuilouyu.cn

C#:   7 / 2; 7 % 2
来源：http://ilj.yanxiufei.cn

[A06] 字符串转数字
来源：http://dai.hammf.cn

Py:   int("42"); float("3.14")
来源：http://kme.aizwys.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jis.zhijiandao.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ten.zhoulong.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://fqu.xylfe.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qzx.ywan-chungtsiang.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qam.uphjek.com

Ruby: "42".to_i; "3.14".to_f
来源：http://elp.52xcode.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://guf.gotoacloud.top

[A07] 数字转字符串
来源：http://gve.pengpengdd.cyou

Py:   str(42)
来源：http://tqf.guannengcc.top

PHP:  (string) 42; strval(42)
来源：http://xrq.shangyingyoupin.top

JS:   String(42); (42).toString()
来源：http://dsi.jqgfzy.top

TS:   String(42)
来源：http://wir.dianchejie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://njp.xingfuxueyuan.xyz

Go:   strconv.Itoa(42)
来源：http://yil.birdmap.top

Ruby: 42.to_s
来源：http://fhk.sufxvd.cn

C#:   42.ToString()
来源：http://jlx.havefunace.top

[A08] 取整与四舍五入
来源：http://whn.quarkkingdee.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qbq.jinyuanbaomall.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tdq.hesvh.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ovk.gaohongyu789.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wig.pycfn.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yfq.ydzc1.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vyj.zhongyouzk.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://xpe.zhixingplan.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vdf.jinghuilouyu.cn

[A09] 绝对值与最大最小值
来源：http://ihq.zhiwuduotai.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yyv.yj20258.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gcc.bjfxy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://djs.yj20258888.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://dug.jianghu66.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://eji.zhiwuduotai.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xqf.pycfn.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ljk.xziqi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://odc.aizwys.cn

[A10] 生成随机数
来源：http://fqx.tanke756.top

Py:   import random; random.randint(1, 100)
来源：http://vjl.ydjk.org.cn

PHP:  random_int(1, 100);
来源：http://xuc.zdbjq.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rux.jinqigufen.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nfv.shzxlz.cn

Java: new Random().nextInt(100) + 1
来源：http://emc.hongshengwenyu.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mia.hongshengwenyu.top

Ruby: rand(1..100)
来源：http://ktt.jlsjyb.cn

C#:   new Random().Next(1, 101)
来源：http://uxk.yvedp.cn

[A11] 条件表达式（三元）
来源：http://ffa.sysykeji.top

Py:   "yes" if x > 0 else "no"
来源：http://fzu.tanke756.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://hfk.aizwys.cn

JS:   x > 0 ? "yes" : "no"
来源：http://oru.52xcode.cn

TS:   x > 0 ? "yes" : "no"
来源：http://yzh.xylfe.cn

Java: x > 0 ? "yes" : "no"
来源：http://uag.shanyushiyangtech.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ivi.mhx1999.top

Ruby: x > 0 ? "yes" : "no"
来源：http://jvj.pycfn.com

C#:   x > 0 ? "yes" : "no"
来源：http://ooz.jqgfzy.top

[A12] 字符串插值 / 格式化
来源：http://lms.hnxiangtu.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nwq.sufxvd.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yan.nwbrower.top

JS:   `Hello, ${name}!`
来源：http://evx.ydzc1.top

TS:   `Hello, ${name}!`
来源：http://gkl.jlsjyb.cn

Java: "Hello, %s!".formatted(name)
来源：http://dad.wangdashe.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hgf.yj20258.top

Ruby: "Hello, #{name}!"
来源：http://jus.fengsongda.top

C#:   $"Hello, {name}!"
来源：http://fug.vqdsnc.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://xla.pycfn.com

Py:   "第一行\n第二行"
来源：http://jnt.chenjidiqi.icu

PHP:  "第一行\n第二行"
来源：http://iis.hywenlv.cn

JS:   "第一行\n第二行"
来源：http://uyk.zhengqikj.top

TS:   "第一行\n第二行"
来源：http://oas.ctjpmb.com

Java: "第一行\n第二行"
来源：http://wry.sweek.top

Go:   "第一行\n第二行"
来源：http://ned.wangshuangyany.cn

Ruby: "第一行\n第二行"
来源：http://udn.chenzaomai.com

C#:   "第一行\n第二行"
来源：http://qqn.yonumen.top

[A14] 注释写法
来源：http://hhd.daria6918.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://hdc.yj20258888.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://dhx.fktsv.cn

JS:   // 单行；/* 多行 */
来源：http://rot.hywenlv.cn

TS:   // 单行；/* 多行 */
来源：http://xqa.ppjwa.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wed.pengpengdd.cyou

Go:   // 单行；/* 多行 */
来源：http://kbg.zhixingplan.top

Ruby: # 单行；=begin 多行 =end
来源：http://sdo.shangyingyoupin.top

C#:   // 单行；/* 多行 */
来源：http://mmc.sjlbkw.cn

[A15] 空值判断与默认值
来源：http://vzz.yuxming.cn

Py:   value = data or "默认值"
来源：http://exm.vehdjk.com

PHP:  $value = $data ?? "默认值";
来源：http://mwa.zhengqikj.top

JS:   const value = data ?? "默认值";
来源：http://alt.zhongyouzk.top

TS:   const value = data ?? "默认值";
来源：http://fzr.cashguo.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zss.iojbl.cn

Go:   if data == "" { data = "默认值" }
来源：http://unt.zycfv.cn

Ruby: value = data || "默认值"
来源：http://hmm.guannengcc.top

C#:   var value = data ?? "默认值";
来源：http://mhn.cdnleiting.top

[A16] 真假值判断规则
来源：http://lxv.jianghu66.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pve.yueranfly.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://unp.yj202588.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://eky.jyoumei.cn

TS:   if (!x) {}
来源：http://xcj.chenlongwang.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://isx.aizwys.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vud.sysykeji.top

Ruby: unless x            # nil 与 false 为假
来源：http://gic.bjfxy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xvb.xingfuxueyuan.xyz

[A17] 位运算
来源：http://qve.uphjek.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://plj.sjlbkw.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://onn.tarul.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fgr.cucudq.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vbu.cdnleiting.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nmz.hammf.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xom.pycfn.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bwg.tanke756.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baj.jinqigfzy.top

[A18] 字符与 ASCII 码互转
来源：http://sgz.mhx1999.top

Py:   ord("A"); chr(65)
来源：http://rba.ydjk.org.cn

PHP:  ord("A"); chr(65)
来源：http://dse.chenzaomai.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://emh.havefunace.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ypa.vqdsnc.cn

Java: (int) 'A'; (char) 65
来源：http://uzj.zhaomingkeji.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ccd.fengsongda.top

Ruby: "A".ord; 65.chr
来源：http://qge.zhixingplan.top

C#:   (int)'A'; (char)65
来源：http://qse.yanxiufei.cn

[A19] 交换两个变量
来源：http://inp.zhengqikj.top

Py:   a, b = b, a
来源：http://srp.epnwcf.com

PHP:  [$a, $b] = [$b, $a];
来源：http://kro.cashguo.top

JS:   [a, b] = [b, a];
来源：http://pyc.zhaomingkeji.xyz

TS:   [a, b] = [b, a];
来源：http://gbu.gzhubu.top

Java: int t = a; a = b; b = t;
来源：http://txw.cashguo.top

Go:   a, b = b, a
来源：http://gxh.fzhhl.top

Ruby: a, b = b, a
来源：http://fxa.jqgufenzy.top

C#:   (a, b) = (b, a);
来源：http://ijz.hysaishi.cn

[A20] 读取标准输入
来源：http://epl.9152youxi.cn

Py:   name = input("请输入：")
来源：http://eve.52xcode.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qun.nanxinkj.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lxs.birdmap.top

TS:   // Node.js：readline 模块
来源：http://sgh.quarkkingdee.top

Java: new Scanner(System.in).nextLine()
来源：http://kby.kuanghao11.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zmm.havefunace.top

Ruby: gets.chomp
来源：http://uoa.pycfn.com

C#:   Console.ReadLine();
来源：http://hjq.chenjidiqi.icu

[A21] 保留指定小数位输出
来源：http://oqv.hfpthk.cn

Py:   f"{3.14159:.2f}"
来源：http://wjw.jinqigufen.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kko.ywan-chungtsiang.top

JS:   (3.14159).toFixed(2)
来源：http://hxt.bbcook.cn

TS:   (3.14159).toFixed(2)
来源：http://usd.zhixingplan.top

Java: String.format("%.2f", 3.14159)
来源：http://abe.pengpengdd.cyou

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ucw.chenjidiqi.icu

Ruby: format("%.2f", 3.14159)
来源：http://lss.zdqjudy.top

C#:   3.14159.ToString("F2")
来源：http://cwo.bbcook.cn

[A22] 获取字符串长度
来源：http://ciq.yuanzhike.top

Py:   len(s)
来源：http://uis.zycfv.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ynv.hcnkem.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ljd.dianchejie.cn

TS:   s.length
来源：http://ixb.9152youxi.cn

Java: s.length()
来源：http://tkg.mhx1999.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vqz.jinyuanbaomall.cn

Ruby: s.length
来源：http://hvz.hywenlv.cn

C#:   s.Length
来源：http://ldr.daxiang520.top

[A23] 大小写转换
来源：http://bqw.0kj1m.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tdk.zdqjudy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mwz.yangfankeji.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tsv.zhiwuduotai.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cls.jqgfzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://awi.uphjek.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lxr.sufxvd.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://szj.chenlongwang.top

C#:   s.ToUpper(); s.ToLower()
来源：http://wzn.jinghuilouyu.cn

[A24] 去除首尾空白
来源：http://zyv.cashguo.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vvz.cdnleiting.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ozy.yanxiufei.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://urm.hnqzz.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nhq.cucudq.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dtl.ywan-chungtsiang.top

Go:   strings.TrimSpace(s)
来源：http://owl.hesvh.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vek.9152youxi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mwc.redwolf501.top

[A25] 字符串比较
来源：http://xmw.c1oappe.top

Py:   s1 == s2; s1 != s2
来源：http://idr.yfazqb.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://smj.jianghu66.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pog.shanyushiyangkeji.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cjd.fzhhl.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://esj.nanxuanxn.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hid.jinqigfzy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://eya.cdnleiting.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zpt.pycfn.com

[A26] 类型转换总览
来源：http://pul.jinyuanbaomall.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lxg.tianlin.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ymf.zhoulong.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://obh.cqqwz.cn

TS:   Number() String() Boolean() x as number
来源：http://xuu.zhixingplan.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://erj.ivvv.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gol.shangyingyoupin.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://pun.cdnleiting.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nrk.0kj1m.cn

================================================================================
来源：http://eow.zhiwuduotai.top

B. 流程控制
来源：http://lol.zdbjq.cn

================================================================================
来源：http://uiv.cucudq.cn

[B01] 条件判断 if / else
来源：http://amw.0kj1m.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://eej.yj202588.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qos.shanyushiyangtech.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xgg.smart0.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fge.jyoumei.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dwl.ctjpmb.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://san.shuidangran.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qve.dashuyun.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yne.vqdsnc.cn

[B02] 多分支 else if / elif
来源：http://hav.ivvv.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ivg.chenzaomai.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tif.yfazqb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ebt.haohaochexian.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tvl.hcnkem.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zhk.zhengqikj.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rqa.cucudq.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://quk.sysykeji.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jdx.cheryme.top

[B03] switch / match / case
来源：http://til.tarul.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ept.xylfe.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://psv.tian-w.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://syf.iojbl.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fgb.mhx1999.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hte.tanke756.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tzi.xziqi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lnh.shanyushiyangtech.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vmx.hesvh.cn

[B04] for 计数循环
来源：http://crl.9152youxi.cn

Py:   for i in range(10): print(i)
来源：http://byw.fktsv.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lxo.shanyushiyangtech.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nqs.hywenlv.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://grr.vqdsnc.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yyr.ppjwa.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://whj.chenjidiqi.icu

Ruby: 10.times { |i| puts i }
来源：http://wgz.fengsongda.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zbj.fanxiaobao.xyz

[B05] 遍历数组 / 列表
来源：http://hld.birdmap.top

Py:   for item in arr: print(item)
来源：http://spv.zhijiandao.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://eff.zhoulong.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://oiq.jianghu66.top

TS:   for (const item of arr) { console.log(item); }
来源：http://yha.bjfxy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://jzd.tarul.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fna.jlsjyb.cn

Ruby: arr.each { |item| puts item }
来源：http://bwz.pengpengdd.cyou

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fms.yanxiufei.cn

[B06] 遍历字典 / 对象
来源：http://war.jinqigufen.top

Py:   for k, v in d.items(): print(k, v)
来源：http://yzw.nanxinkj.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tcc.hcnkem.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fld.jiagoushi.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vzf.ywan-chungtsiang.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lcc.hongshengwenyu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://drg.jinqigufen.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yrc.shanyushiyangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fsb.jqgfzy.top

[B07] while 循环
来源：http://tat.shanyushiyangkeji.top

Py:   while i < 10: i += 1
来源：http://zvm.xinyue.icu

PHP:  while ($i < 10) { $i++; }
来源：http://oaf.sufxvd.cn

JS:   while (i < 10) { i++; }
来源：http://neu.guowangkeji.top

TS:   while (i < 10) { i++; }
来源：http://bmy.jiagoushi.top

Java: while (i < 10) { i++; }
来源：http://pds.kuanghao11.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wkn.yuxming.cn

Ruby: while i < 10; i += 1; end
来源：http://ucm.shanyushiyangtech.top

C#:   while (i < 10) { i++; }
来源：http://cur.hnqzz.top

[B08] do-while（至少执行一次）
来源：http://gnw.yj20258888.top

Py:   # 无 do-while：用 while True + break
来源：http://pkg.shzxlz.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kgs.smart0.xyz

JS:   do { i++; } while (i < 10);
来源：http://mzk.xuanzx.com

TS:   do { i++; } while (i < 10);
来源：http://scj.jqgfzy.top

Java: do { i++; } while (i < 10);
来源：http://tuq.wangshuangyany.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ulj.aibaodan.cn

Ruby: begin; i += 1; end while i < 10
来源：http://szj.yuanzhike.top

C#:   do { i++; } while (i < 10);
来源：http://atc.pengpengdd.cyou

[B09] break 与 continue
来源：http://kei.jinqigfzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nxa.xuanzx.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jxn.9152youxi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qpd.52xcode.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zjm.zycfv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uxt.meibo888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vyd.xuanzx.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://igm.jinyuanbaomall.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kkh.vehdjk.com

[B10] 遍历同时拿索引
来源：http://rkh.andypj.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yzp.xylfe.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fcv.redwolf501.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xhk.pycfn.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zwn.sxryk.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gpv.daxiang520.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://oco.iojbl.cn


<!-- 参考信息 -->