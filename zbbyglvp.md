代发 wailian999

[A02] 变量声明与赋值
来源：http://eoa.zhixingplan.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jes.zhengqikj.top

PHP:  $name = "Alex"; $age = 20;
来源：http://khn.zdbjq.cn

JS:   let name = "Alex"; const age = 20;
来源：http://dra.wangshuangyany.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zbk.jinqigufen.top

Java: String name = "Alex"; int age = 20;
来源：http://qle.smart0.xyz

Go:   name := "Alex"; age := 20
来源：http://zyo.ehwqpu.com

Ruby: name = "Alex"; age = 20
来源：http://pyy.cqqwz.cn

C#:   string name = "Alex"; int age = 20;
来源：http://sks.sxryk.cn

[A03] 常量定义
来源：http://dxc.daria6918.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dqf.sxryk.cn

PHP:  const PI = 3.14159;
来源：http://zpt.yuanzhike.top

JS:   const PI = 3.14159;
来源：http://pjd.yj20258.top

TS:   const PI: number = 3.14159;
来源：http://shf.pycfn.com

Java: static final double PI = 3.14159;
来源：http://ukx.haohaochexian.top

Go:   const PI = 3.14159
来源：http://msg.fengsongda.top

Ruby: PI = 3.14159
来源：http://giu.mhx1999.top

C#:   const double PI = 3.14159;
来源：http://drn.yueranfly.top

[A04] 判断变量类型
来源：http://tot.daxiang520.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://jcf.vehdjk.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xsu.dashuyun.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xht.xingfuxueyuan.xyz

TS:   typeof x; x instanceof Date
来源：http://gel.andypj.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xpd.hysaishi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ukp.ppjwa.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yqj.zhoulong.xyz

C#:   x.GetType().Name; x is int
来源：http://vjs.shanyushiyangtech.top

[A05] 整数除法与取模
来源：http://niw.xuetiantiany.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rbm.52xcode.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://lco.yuxming.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://emg.nanxinkj.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kaa.yangfankeji.com

Java: 7 / 2; 7 % 2
来源：http://dkw.guowangkeji.top

Go:   7 / 2; 7 % 2
来源：http://esd.dianchejie.cn

Ruby: 7 / 2; 7 % 2
来源：http://gou.yuxming.cn

C#:   7 / 2; 7 % 2
来源：http://vpo.yuanzhike.top

[A06] 字符串转数字
来源：http://tgu.xylfe.cn

Py:   int("42"); float("3.14")
来源：http://xxl.fehbvm.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://naf.zhengqikj.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qyk.zycfv.cn

TS:   parseInt("42", 10); Number("42")
来源：http://gud.ywan-chungtsiang.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pfp.shzxlz.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://egz.andypj.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://tbw.guannengcc.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xlh.jianghu66.top

[A07] 数字转字符串
来源：http://ocj.chenzaomai.com

Py:   str(42)
来源：http://ksg.redwolf501.top

PHP:  (string) 42; strval(42)
来源：http://ggu.ppjwa.cn

JS:   String(42); (42).toString()
来源：http://xpt.dashuyun.cn

TS:   String(42)
来源：http://elk.xinyue.icu

Java: String.valueOf(42); Integer.toString(42)
来源：http://nxk.fktsv.cn

Go:   strconv.Itoa(42)
来源：http://dpa.0kj1m.cn

Ruby: 42.to_s
来源：http://fvq.jlsjyb.cn

C#:   42.ToString()
来源：http://hov.redwolf501.top

[A08] 取整与四舍五入
来源：http://bqb.birdmap.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://iaw.nanxinkj.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://upj.xingfuxueyuan.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wmj.fktsv.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://akp.hnqzz.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bte.yanxiufei.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tiy.sxryk.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://jei.nanxinkj.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ppn.9152youxi.cn

[A09] 绝对值与最大最小值
来源：http://obb.shangyingyoupin.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lfa.ydjk.org.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xhb.ctjpmb.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zyd.fengsongda.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vxe.sxryk.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dox.cucudq.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://puf.vqdsnc.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vte.cashguo.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ems.xylfe.cn

[A10] 生成随机数
来源：http://hog.guannengcc.top

Py:   import random; random.randint(1, 100)
来源：http://rjb.c1oappe.top

PHP:  random_int(1, 100);
来源：http://wuk.jinqigufen.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ikj.hesvh.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://oho.shangyingyoupin.top

Java: new Random().nextInt(100) + 1
来源：http://ccp.xylfe.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zvc.cucudq.cn

Ruby: rand(1..100)
来源：http://ila.sufxvd.cn

C#:   new Random().Next(1, 101)
来源：http://zcr.ywan-chungtsiang.top

[A11] 条件表达式（三元）
来源：http://oeq.jqgfzy.top

Py:   "yes" if x > 0 else "no"
来源：http://kvl.gzhubu.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://mkm.hesvh.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rbc.zycfv.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dqc.yj20258.top

Java: x > 0 ? "yes" : "no"
来源：http://xik.yongpay.top

Go:   // 无三元运算符，需用 if 语句
来源：http://qam.fanxiaobao.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://ldh.chenlongwang.top

C#:   x > 0 ? "yes" : "no"
来源：http://gyh.cdnleiting.top

[A12] 字符串插值 / 格式化
来源：http://yng.hnxiangtu.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://nfg.xziqi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rwz.shanyushiyangkeji.top

JS:   `Hello, ${name}!`
来源：http://glr.guannengcc.top

TS:   `Hello, ${name}!`
来源：http://uzu.nwbrower.top

Java: "Hello, %s!".formatted(name)
来源：http://qol.shzxlz.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vxd.vehdjk.com

Ruby: "Hello, #{name}!"
来源：http://tsu.yonumen.top

C#:   $"Hello, {name}!"
来源：http://ict.bjfxy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://oxq.fanxiaobao.xyz

Py:   "第一行\n第二行"
来源：http://pca.nwbrower.top

PHP:  "第一行\n第二行"
来源：http://viz.yueranfly.top

JS:   "第一行\n第二行"
来源：http://glf.jinqigfzy.top

TS:   "第一行\n第二行"
来源：http://qjb.9152youxi.cn

Java: "第一行\n第二行"
来源：http://dux.c1oappe.top

Go:   "第一行\n第二行"
来源：http://smb.yj20258888.top

Ruby: "第一行\n第二行"
来源：http://rzi.gzhubu.top

C#:   "第一行\n第二行"
来源：http://cqq.daxiang520.top

[A14] 注释写法
来源：http://dwi.chenlongwang.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://vxa.cdnleiting.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://dmb.zdqjudy.top

JS:   // 单行；/* 多行 */
来源：http://nrk.svipenyu.cn

TS:   // 单行；/* 多行 */
来源：http://dqc.daria6918.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nzw.hfpthk.cn

Go:   // 单行；/* 多行 */
来源：http://mbz.nanxinkj.top

Ruby: # 单行；=begin 多行 =end
来源：http://ybo.gotoacloud.top

C#:   // 单行；/* 多行 */
来源：http://asp.jinqigufen.top

[A15] 空值判断与默认值
来源：http://xei.zdbjq.cn

Py:   value = data or "默认值"
来源：http://aoe.bjfxy.top

PHP:  $value = $data ?? "默认值";
来源：http://gnf.cucudq.cn

JS:   const value = data ?? "默认值";
来源：http://oxo.shanyushiyangkeji.top

TS:   const value = data ?? "默认值";
来源：http://baa.zhixingplan.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hkn.jyoumei.cn

Go:   if data == "" { data = "默认值" }
来源：http://jhe.hnxiangtu.top

Ruby: value = data || "默认值"
来源：http://ojy.zhixingplan.top

C#:   var value = data ?? "默认值";
来源：http://elv.birdmap.top

[A16] 真假值判断规则
来源：http://bfe.aibaodan.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xyo.nanxuanxn.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ptf.hysaishi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lwp.hfpthk.cn

TS:   if (!x) {}
来源：http://ejt.zycfv.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://brc.hywenlv.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wzo.ehwqpu.com

Ruby: unless x            # nil 与 false 为假
来源：http://rqa.ppjwa.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yan.ywan-chungtsiang.top

[A17] 位运算
来源：http://fbd.pycfn.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://inm.52xcode.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mmz.jianghu66.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://etv.cdnleiting.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rgq.xuanzx.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://drd.ywan-chungtsiang.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mfi.hnxiangtu.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nik.svipenyu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gbh.shanyushiyangkeji.top

[A18] 字符与 ASCII 码互转
来源：http://vzq.jlsjyb.cn

Py:   ord("A"); chr(65)
来源：http://bls.zhixingplan.top

PHP:  ord("A"); chr(65)
来源：http://fbj.sjlbkw.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dvn.bbcook.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nai.feifeiyinyue.top

Java: (int) 'A'; (char) 65
来源：http://rto.gzhubu.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://joi.redwolf501.top

Ruby: "A".ord; 65.chr
来源：http://qkm.zhoulong.xyz

C#:   (int)'A'; (char)65
来源：http://kcs.0kj1m.cn

[A19] 交换两个变量
来源：http://pzg.hysaishi.cn

Py:   a, b = b, a
来源：http://pgf.feifeiyinyue.top

PHP:  [$a, $b] = [$b, $a];
来源：http://epb.smart0.xyz

JS:   [a, b] = [b, a];
来源：http://xnz.yongpay.top

TS:   [a, b] = [b, a];
来源：http://thf.fengsongda.top

Java: int t = a; a = b; b = t;
来源：http://yaw.uphjek.com

Go:   a, b = b, a
来源：http://spm.ppjwa.cn

Ruby: a, b = b, a
来源：http://hzm.yongpay.top

C#:   (a, b) = (b, a);
来源：http://mlw.sufxvd.cn

[A20] 读取标准输入
来源：http://fdg.pengpengdd.cyou

Py:   name = input("请输入：")
来源：http://ghn.c1oappe.top

PHP:  $name = trim(fgets(STDIN));
来源：http://qkm.dianchejie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vhj.gogol.net.cn

TS:   // Node.js：readline 模块
来源：http://tsi.ctjpmb.com

Java: new Scanner(System.in).nextLine()
来源：http://bfm.jqgufenzy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pln.nanxinkj.top

Ruby: gets.chomp
来源：http://fqh.chenzaomai.com

C#:   Console.ReadLine();
来源：http://osh.zhixingplan.top

[A21] 保留指定小数位输出
来源：http://ofc.pengpengdd.cyou

Py:   f"{3.14159:.2f}"
来源：http://ivq.shangyingyoupin.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hwn.jianghu66.top

JS:   (3.14159).toFixed(2)
来源：http://zqa.yongpay.top

TS:   (3.14159).toFixed(2)
来源：http://put.xylfe.cn

Java: String.format("%.2f", 3.14159)
来源：http://zyl.hnxiangtu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qhv.mhx1999.top

Ruby: format("%.2f", 3.14159)
来源：http://btf.dianchejie.cn

C#:   3.14159.ToString("F2")
来源：http://iey.shangyingyoupin.top

[A22] 获取字符串长度
来源：http://dmj.guannengcc.top

Py:   len(s)
来源：http://hwf.c1oappe.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fra.jyoumei.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ilr.xuanzx.com

TS:   s.length
来源：http://upk.shzxlz.cn

Java: s.length()
来源：http://zxi.birdmap.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kql.hywenlv.cn

Ruby: s.length
来源：http://smx.zycfv.cn

C#:   s.Length
来源：http://upt.gogol.net.cn

[A23] 大小写转换
来源：http://uzf.sufxvd.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ldb.tanke756.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nyr.hongshengwenyu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vrl.cashguo.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lgw.yj20258.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cko.dianchejie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://osf.birdmap.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xoq.pycfn.com

C#:   s.ToUpper(); s.ToLower()
来源：http://isv.vqdsnc.cn

[A24] 去除首尾空白
来源：http://zpa.gogol.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sqr.daria6918.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tvl.cdnleiting.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wkd.xziqi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dbn.zycfv.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nzy.yfazqb.com

Go:   strings.TrimSpace(s)
来源：http://jyf.zhixingplan.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://syc.tian-w.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baj.yj20258888.top

[A25] 字符串比较
来源：http://rzq.hesvh.cn

Py:   s1 == s2; s1 != s2
来源：http://asl.yj202588.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blo.xinyue.icu

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://exu.tarul.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jcs.jinqigfzy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jqj.yangfankeji.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lkv.9152youxi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qxq.ivvv.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://puf.zhixingplan.top

[A26] 类型转换总览
来源：http://cml.gzhubu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://byy.yj20258.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://itt.zhijiandao.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qpo.yuanzhike.top

TS:   Number() String() Boolean() x as number
来源：http://cuq.tianlin.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://web.quarkkingdee.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jmb.meibo888.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://zsx.tarul.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pyb.feifeiyinyue.top

================================================================================
来源：http://tke.ybcxt.top

B. 流程控制
来源：http://qgx.chenjidiqi.icu

================================================================================
来源：http://cbn.jinqigfzy.top

[B01] 条件判断 if / else
来源：http://rxd.ydjk.org.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://txu.quarkkingdee.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kpc.cucudq.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wad.hfpthk.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ypq.dianchejie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rqd.jinyuanbaomall.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xpz.guowangkeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ugm.ybcxt.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mbt.svipenyu.cn

[B02] 多分支 else if / elif
来源：http://rgj.zhaomingkeji.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wji.ywan-chungtsiang.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ztf.zdqjudy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ogt.gotoacloud.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hqk.wangdashe.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://axd.sweek.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rfc.yongpay.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wya.sweek.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uwy.fehbvm.com

[B03] switch / match / case
来源：http://sdw.snrcjt.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jio.smart0.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://eyl.wangshuangyany.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://drp.jinqigfzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fff.jinghuilouyu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hqn.ybcxt.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qwk.smart0.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dsn.nanxuanxn.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wnn.hysaishi.cn

[B04] for 计数循环
来源：http://lot.sysykeji.top

Py:   for i in range(10): print(i)
来源：http://rhz.svipenyu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tcp.yuanzhike.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rgg.pycfn.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ypl.hysaishi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wwc.cucudq.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pid.tian-w.cn

Ruby: 10.times { |i| puts i }
来源：http://ska.tanke756.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dbc.cheryme.top

[B05] 遍历数组 / 列表
来源：http://hdt.tianlin.xyz

Py:   for item in arr: print(item)
来源：http://kqi.guannengcc.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ieq.ehwqpu.com

JS:   for (const item of arr) { console.log(item); }
来源：http://otd.xziqi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tej.cqqwz.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pln.daxiang520.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fnx.birdmap.top

Ruby: arr.each { |item| puts item }
来源：http://qio.haohaochexian.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zxd.zhijiandao.cn

[B06] 遍历字典 / 对象
来源：http://rmr.sweek.top

Py:   for k, v in d.items(): print(k, v)
来源：http://wzz.aizwys.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jbs.zhaomingkeji.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iqe.jyoumei.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aih.dianchejie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jmy.hywenlv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vyv.fehbvm.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kde.yueranfly.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iex.bbcook.cn

[B07] while 循环
来源：http://ncd.zhijiandao.cn

Py:   while i < 10: i += 1
来源：http://fyv.gaohongyu789.top

PHP:  while ($i < 10) { $i++; }
来源：http://zjx.fktsv.cn

JS:   while (i < 10) { i++; }
来源：http://xhe.ivvv.top

TS:   while (i < 10) { i++; }
来源：http://ono.jqgfzy.top

Java: while (i < 10) { i++; }
来源：http://gbd.0kj1m.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vwu.fktsv.cn

Ruby: while i < 10; i += 1; end
来源：http://swq.yonumen.top

C#:   while (i < 10) { i++; }
来源：http://rud.sufxvd.cn

[B08] do-while（至少执行一次）
来源：http://iao.cqqwz.cn

Py:   # 无 do-while：用 while True + break
来源：http://mss.xingfuxueyuan.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://uic.gzhubu.top

JS:   do { i++; } while (i < 10);
来源：http://mim.andypj.xyz

TS:   do { i++; } while (i < 10);
来源：http://pqh.jinyuanbaomall.cn

Java: do { i++; } while (i < 10);
来源：http://wab.dianchejie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lbz.jlsjyb.cn

Ruby: begin; i += 1; end while i < 10
来源：http://utb.hammf.cn

C#:   do { i++; } while (i < 10);
来源：http://qmx.svipenyu.cn


<!-- 参考信息 -->