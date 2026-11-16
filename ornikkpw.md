代发 wailian999

[A02] 变量声明与赋值
来源：http://zfk.sweek.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nri.aibaodan.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fdf.52xcode.cn

JS:   let name = "Alex"; const age = 20;
来源：http://pje.gzhubu.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fnh.hammf.cn

Java: String name = "Alex"; int age = 20;
来源：http://isx.gzhubu.top

Go:   name := "Alex"; age := 20
来源：http://cqm.mhx1999.top

Ruby: name = "Alex"; age = 20
来源：http://fwo.fktsv.cn

C#:   string name = "Alex"; int age = 20;
来源：http://kwu.yuanzhike.top

[A03] 常量定义
来源：http://lmx.yanxiufei.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://osq.vehdjk.com

PHP:  const PI = 3.14159;
来源：http://gmm.shanyushiyangtech.top

JS:   const PI = 3.14159;
来源：http://nzu.shanyushiyangkeji.top

TS:   const PI: number = 3.14159;
来源：http://lad.nwbrower.top

Java: static final double PI = 3.14159;
来源：http://efs.daria6918.cn

Go:   const PI = 3.14159
来源：http://qro.tarul.cn

Ruby: PI = 3.14159
来源：http://qzx.smart0.xyz

C#:   const double PI = 3.14159;
来源：http://ylr.wangdashe.top

[A04] 判断变量类型
来源：http://hoz.jlsjyb.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://duc.hnqzz.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jfp.chenlongwang.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bhy.shangyingyoupin.top

TS:   typeof x; x instanceof Date
来源：http://mwc.zhijiandao.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hda.ywan-chungtsiang.top

Go:   reflect.TypeOf(x).Name()
来源：http://rjp.kuanghao11.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://rbc.bjfxy.top

C#:   x.GetType().Name; x is int
来源：http://vkp.yongpay.top

[A05] 整数除法与取模
来源：http://fcs.ppjwa.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://iwf.sufxvd.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ylj.fktsv.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://oij.jianghu66.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mve.zdbjq.cn

Java: 7 / 2; 7 % 2
来源：http://oyd.hammf.cn

Go:   7 / 2; 7 % 2
来源：http://kzb.zhijiandao.cn

Ruby: 7 / 2; 7 % 2
来源：http://dfc.0kj1m.cn

C#:   7 / 2; 7 % 2
来源：http://nlu.zhijiandao.cn

[A06] 字符串转数字
来源：http://mlm.gaohongyu789.top

Py:   int("42"); float("3.14")
来源：http://dmu.zhengqikj.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nrw.wangdashe.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://guc.haohaochexian.top

TS:   parseInt("42", 10); Number("42")
来源：http://bll.ehwqpu.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zam.hnxiangtu.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mnh.gaohongyu789.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ytm.fzhhl.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ars.fzhhl.top

[A07] 数字转字符串
来源：http://tfn.hywenlv.cn

Py:   str(42)
来源：http://dgy.tianlin.xyz

PHP:  (string) 42; strval(42)
来源：http://lss.gotoacloud.top

JS:   String(42); (42).toString()
来源：http://hlb.yvedp.cn

TS:   String(42)
来源：http://bcq.mhx1999.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://gdv.pengpengdd.cyou

Go:   strconv.Itoa(42)
来源：http://iob.gaohongyu789.top

Ruby: 42.to_s
来源：http://nle.fktsv.cn

C#:   42.ToString()
来源：http://swh.hywenlv.cn

[A08] 取整与四舍五入
来源：http://ftn.zhaomingkeji.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ypc.guannengcc.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zsf.jinqigfzy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://oak.zdqjudy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tis.cheryme.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ccw.zhixingplan.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rdm.wangshuangyany.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://fwu.hysaishi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cfc.chenzaomai.com

[A09] 绝对值与最大最小值
来源：http://wei.snrcjt.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ekc.hongshengwenyu.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://aui.xinyue.icu

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bjp.hammf.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nhf.xinyue.icu

Java: Math.abs(-5); Math.max(1, 2)
来源：http://huj.ppjwa.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://sig.pengpengdd.cyou

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ztb.hnqzz.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tsm.svipenyu.cn

[A10] 生成随机数
来源：http://wze.jinqigufen.top

Py:   import random; random.randint(1, 100)
来源：http://qnt.wangshuangyany.cn

PHP:  random_int(1, 100);
来源：http://ide.cheryme.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://myz.sjlbkw.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ykj.birdmap.top

Java: new Random().nextInt(100) + 1
来源：http://gca.haohaochexian.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://psj.xuanzx.com

Ruby: rand(1..100)
来源：http://ggu.sysykeji.top

C#:   new Random().Next(1, 101)
来源：http://whe.hesvh.cn

[A11] 条件表达式（三元）
来源：http://jia.nanxuanxn.top

Py:   "yes" if x > 0 else "no"
来源：http://nyo.jinyuanbaomall.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://vdk.zhixingplan.top

JS:   x > 0 ? "yes" : "no"
来源：http://igh.smart0.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://dnw.ydzc1.top

Java: x > 0 ? "yes" : "no"
来源：http://zro.jqgfzy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://xcn.fzhhl.top

Ruby: x > 0 ? "yes" : "no"
来源：http://yif.yonumen.top

C#:   x > 0 ? "yes" : "no"
来源：http://rav.zhixingplan.top

[A12] 字符串插值 / 格式化
来源：http://qbw.gzhubu.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://utp.mhx1999.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://skf.yangfankeji.com

JS:   `Hello, ${name}!`
来源：http://zdz.nanxinkj.top

TS:   `Hello, ${name}!`
来源：http://imy.gogol.net.cn

Java: "Hello, %s!".formatted(name)
来源：http://zes.bbcook.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://txq.jinqigufen.top

Ruby: "Hello, #{name}!"
来源：http://sex.zhengqikj.top

C#:   $"Hello, {name}!"
来源：http://pwy.yvedp.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://cmt.cashguo.top

Py:   "第一行\n第二行"
来源：http://ljf.jlsjyb.cn

PHP:  "第一行\n第二行"
来源：http://ocn.ivvv.top

JS:   "第一行\n第二行"
来源：http://qvb.jlsjyb.cn

TS:   "第一行\n第二行"
来源：http://zkt.zhiwuduotai.top

Java: "第一行\n第二行"
来源：http://ytn.xylfe.cn

Go:   "第一行\n第二行"
来源：http://noc.yongpay.top

Ruby: "第一行\n第二行"
来源：http://dtb.vehdjk.com

C#:   "第一行\n第二行"
来源：http://nwn.cucudq.cn

[A14] 注释写法
来源：http://azn.shanyushiyangtech.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://xpw.cheryme.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://dqv.ehwqpu.com

JS:   // 单行；/* 多行 */
来源：http://mjd.chenlongwang.top

TS:   // 单行；/* 多行 */
来源：http://emr.chenlongwang.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lgi.chenlongwang.top

Go:   // 单行；/* 多行 */
来源：http://aoj.yonumen.top

Ruby: # 单行；=begin 多行 =end
来源：http://tuh.fehbvm.com

C#:   // 单行；/* 多行 */
来源：http://ttq.tian-w.cn

[A15] 空值判断与默认值
来源：http://yqy.hfpthk.cn

Py:   value = data or "默认值"
来源：http://kqd.pycfn.com

PHP:  $value = $data ?? "默认值";
来源：http://bra.zdqjudy.top

JS:   const value = data ?? "默认值";
来源：http://cda.dashuyun.cn

TS:   const value = data ?? "默认值";
来源：http://ssb.zhiwuduotai.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fke.xylfe.cn

Go:   if data == "" { data = "默认值" }
来源：http://nfr.sufxvd.cn

Ruby: value = data || "默认值"
来源：http://idj.smart0.xyz

C#:   var value = data ?? "默认值";
来源：http://pib.ivvv.top

[A16] 真假值判断规则
来源：http://cfp.zhengqikj.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xkx.guowangkeji.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mam.wangdashe.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ovy.gzhubu.top

TS:   if (!x) {}
来源：http://zwl.smart0.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://knj.feifeiyinyue.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pnj.pengpengdd.cyou

Ruby: unless x            # nil 与 false 为假
来源：http://fmp.fengsongda.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mvl.svipenyu.cn

[A17] 位运算
来源：http://cpt.yangfankeji.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gwl.dashuyun.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xco.tanke756.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pyw.yuxming.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ppv.cqqwz.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rac.jqgfzy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ccw.sweek.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://olf.zhijiandao.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ztg.vqdsnc.cn

[A18] 字符与 ASCII 码互转
来源：http://ioa.svipenyu.cn

Py:   ord("A"); chr(65)
来源：http://sey.dianchejie.cn

PHP:  ord("A"); chr(65)
来源：http://ypo.ivvv.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pte.yuxming.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://edw.jinyuanbaomall.cn

Java: (int) 'A'; (char) 65
来源：http://qye.jinghuilouyu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://klg.chenjidiqi.icu

Ruby: "A".ord; 65.chr
来源：http://alq.ydzc1.top

C#:   (int)'A'; (char)65
来源：http://sty.epnwcf.com

[A19] 交换两个变量
来源：http://eyl.shanyushiyangkeji.top

Py:   a, b = b, a
来源：http://dnl.aizwys.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://iho.daxiang520.top

JS:   [a, b] = [b, a];
来源：http://wsa.dashuyun.cn

TS:   [a, b] = [b, a];
来源：http://hxa.sysykeji.top

Java: int t = a; a = b; b = t;
来源：http://jso.sweek.top

Go:   a, b = b, a
来源：http://vxt.316326.xyz

Ruby: a, b = b, a
来源：http://zst.sxryk.cn

C#:   (a, b) = (b, a);
来源：http://zrs.ivvv.top

[A20] 读取标准输入
来源：http://qvs.cdnleiting.top

Py:   name = input("请输入：")
来源：http://ami.ehwqpu.com

PHP:  $name = trim(fgets(STDIN));
来源：http://xhj.yuxming.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gbn.hysaishi.cn

TS:   // Node.js：readline 模块
来源：http://ufw.guowangkeji.top

Java: new Scanner(System.in).nextLine()
来源：http://rgk.zhongyouzk.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cim.xingfuxueyuan.xyz

Ruby: gets.chomp
来源：http://fgd.cashguo.top

C#:   Console.ReadLine();
来源：http://yif.vehdjk.com

[A21] 保留指定小数位输出
来源：http://wjp.yongpay.top

Py:   f"{3.14159:.2f}"
来源：http://rcd.jyoumei.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fbm.guannengcc.top

JS:   (3.14159).toFixed(2)
来源：http://yyr.hnxiangtu.top

TS:   (3.14159).toFixed(2)
来源：http://oqe.hnqzz.top

Java: String.format("%.2f", 3.14159)
来源：http://eng.hongshengwenyu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hcx.zhixingplan.top

Ruby: format("%.2f", 3.14159)
来源：http://gos.pycfn.com

C#:   3.14159.ToString("F2")
来源：http://dul.hnqzz.top

[A22] 获取字符串长度
来源：http://ims.yvedp.cn

Py:   len(s)
来源：http://hrl.tanke756.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gia.yvedp.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fue.sjlbkw.cn

TS:   s.length
来源：http://ych.yonumen.top

Java: s.length()
来源：http://bhs.zdqjudy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lks.yangfankeji.com

Ruby: s.length
来源：http://agn.cdnleiting.top

C#:   s.Length
来源：http://zoh.guowangkeji.top

[A23] 大小写转换
来源：http://xqx.yonumen.top

Py:   s.upper(); s.lower(); s.title()
来源：http://jja.xuetiantiany.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kvu.gzhubu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kyu.xingfuxueyuan.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sxt.ppjwa.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dxg.yongpay.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rgg.shanyushiyangtech.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zor.chenzaomai.com

C#:   s.ToUpper(); s.ToLower()
来源：http://vnn.xuetiantiany.cn

[A24] 去除首尾空白
来源：http://hih.hywenlv.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rly.yj20258.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hvj.aizwys.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zic.cashguo.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wnj.gzhubu.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://abs.xuanzx.com

Go:   strings.TrimSpace(s)
来源：http://jnq.hnxiangtu.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://axo.yuanzhike.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ncb.ppjwa.cn

[A25] 字符串比较
来源：http://gbd.jinqigufen.top

Py:   s1 == s2; s1 != s2
来源：http://mfu.vehdjk.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://msq.tarul.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hlb.chenzaomai.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mzb.cqqwz.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sce.9152youxi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tyk.yuxming.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zej.tarul.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vdw.epnwcf.com

[A26] 类型转换总览
来源：http://mew.daria6918.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://eqr.sufxvd.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://opb.fktsv.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://inf.yfazqb.com

TS:   Number() String() Boolean() x as number
来源：http://lut.daxiang520.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kvl.epnwcf.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pqa.jqgfzy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://gma.yuanzhike.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pmw.jqgfzy.top

================================================================================
来源：http://wjk.tian-w.cn

B. 流程控制
来源：http://pkh.yj20258.top

================================================================================
来源：http://wht.zhoulong.xyz

[B01] 条件判断 if / else
来源：http://eka.ppjwa.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wro.hcnkem.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pah.ydzc1.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mms.xinyue.icu

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jkv.ehwqpu.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://vrb.tianlin.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tlj.bjfxy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://iar.zdqjudy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nkn.xuanzx.com

[B02] 多分支 else if / elif
来源：http://xpm.gzhubu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lgu.316326.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xib.sxryk.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qyc.jinqigfzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cwu.gzhubu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://alc.ybcxt.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://akv.zhijiandao.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vlr.feifeiyinyue.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xdg.snrcjt.cn

[B03] switch / match / case
来源：http://gut.nanxuanxn.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://etb.9152youxi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uvd.bjfxy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gft.chenjidiqi.icu

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ykk.vehdjk.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://smx.xingfuxueyuan.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xym.sufxvd.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zsc.zdbjq.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ndz.gotoacloud.top

[B04] for 计数循环
来源：http://oyd.vehdjk.com

Py:   for i in range(10): print(i)
来源：http://otf.fzhhl.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ggx.yongpay.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sks.yuxming.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jgc.feifeiyinyue.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wmd.andypj.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://szo.9152youxi.cn

Ruby: 10.times { |i| puts i }
来源：http://clf.hysaishi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uns.chenjidiqi.icu

[B05] 遍历数组 / 列表
来源：http://ajr.gotoacloud.top

Py:   for item in arr: print(item)
来源：http://uay.jqgfzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://spu.52xcode.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zcg.redwolf501.top

TS:   for (const item of arr) { console.log(item); }
来源：http://aeb.hfpthk.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kkf.jqgufenzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://slf.yuxming.cn

Ruby: arr.each { |item| puts item }
来源：http://ehm.cashguo.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sdh.xuetiantiany.cn

[B06] 遍历字典 / 对象
来源：http://rxf.yuanzhike.top

Py:   for k, v in d.items(): print(k, v)
来源：http://poe.gaohongyu789.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pnl.jinghuilouyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xma.bbcook.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kke.c1oappe.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xqt.tarul.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gpa.feifeiyinyue.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mlm.yuxming.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://adb.nwbrower.top

[B07] while 循环
来源：http://toh.xylfe.cn

Py:   while i < 10: i += 1
来源：http://irs.kuanghao11.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mdz.tianlin.xyz

JS:   while (i < 10) { i++; }
来源：http://cia.svipenyu.cn

TS:   while (i < 10) { i++; }
来源：http://lwn.chenjidiqi.icu

Java: while (i < 10) { i++; }
来源：http://nvs.yueranfly.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zut.jinyuanbaomall.cn

Ruby: while i < 10; i += 1; end
来源：http://drv.gotoacloud.top

C#:   while (i < 10) { i++; }
来源：http://mgl.chenlongwang.top

[B08] do-while（至少执行一次）
来源：http://jbq.feifeiyinyue.top

Py:   # 无 do-while：用 while True + break
来源：http://nsl.cucudq.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://tqx.zhoulong.xyz

JS:   do { i++; } while (i < 10);
来源：http://xww.hammf.cn

TS:   do { i++; } while (i < 10);
来源：http://spm.ywan-chungtsiang.top

Java: do { i++; } while (i < 10);
来源：http://stw.guannengcc.top

Go:   for { i++; if i >= 10 { break } }
来源：http://vuz.aibaodan.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ivi.iojbl.cn

C#:   do { i++; } while (i < 10);
来源：http://xfh.jlsjyb.cn


<!-- 参考信息 -->