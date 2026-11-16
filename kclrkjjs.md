代发 wailian999

[A02] 变量声明与赋值
来源：http://upt.c1oappe.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://osq.sysykeji.top

PHP:  $name = "Alex"; $age = 20;
来源：http://gmv.fanxiaobao.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://lqo.zycfv.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nii.hnqzz.top

Java: String name = "Alex"; int age = 20;
来源：http://bga.fehbvm.com

Go:   name := "Alex"; age := 20
来源：http://qjp.vehdjk.com

Ruby: name = "Alex"; age = 20
来源：http://dfh.shanyushiyangtech.top

C#:   string name = "Alex"; int age = 20;
来源：http://zgx.jinqigfzy.top

[A03] 常量定义
来源：http://cxn.zhijiandao.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://eop.haohaochexian.top

PHP:  const PI = 3.14159;
来源：http://dyt.gaohongyu789.top

JS:   const PI = 3.14159;
来源：http://zjx.mhx1999.top

TS:   const PI: number = 3.14159;
来源：http://nev.shuidangran.top

Java: static final double PI = 3.14159;
来源：http://aja.ehwqpu.com

Go:   const PI = 3.14159
来源：http://sqn.jlsjyb.cn

Ruby: PI = 3.14159
来源：http://sps.zhengqikj.top

C#:   const double PI = 3.14159;
来源：http://kvr.haohaochexian.top

[A04] 判断变量类型
来源：http://fgz.tianlin.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://ndd.tian-w.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jmw.havefunace.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pqo.haohaochexian.top

TS:   typeof x; x instanceof Date
来源：http://htj.ybcxt.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ebs.sweek.top

Go:   reflect.TypeOf(x).Name()
来源：http://sqq.shuidangran.top

Ruby: x.class; x.is_a?(Integer)
来源：http://qxu.chenzaomai.com

C#:   x.GetType().Name; x is int
来源：http://fvr.zhaomingkeji.xyz

[A05] 整数除法与取模
来源：http://fvv.nanxinkj.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ymc.aibaodan.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gba.ybcxt.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ktg.dashuyun.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://moc.jinyuanbaomall.cn

Java: 7 / 2; 7 % 2
来源：http://cem.tianlin.xyz

Go:   7 / 2; 7 % 2
来源：http://eqa.haohaochexian.top

Ruby: 7 / 2; 7 % 2
来源：http://lbn.yuanzhike.top

C#:   7 / 2; 7 % 2
来源：http://qaa.yangfankeji.com

[A06] 字符串转数字
来源：http://dsb.0kj1m.cn

Py:   int("42"); float("3.14")
来源：http://ytw.xuetiantiany.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fcf.nanxinkj.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cuk.tianlin.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://fmo.zhoulong.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ceb.jyoumei.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://goh.shangyingyoupin.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ldu.yueranfly.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vwk.zdbjq.cn

[A07] 数字转字符串
来源：http://ock.tanke756.top

Py:   str(42)
来源：http://kif.fehbvm.com

PHP:  (string) 42; strval(42)
来源：http://xcv.sjlbkw.cn

JS:   String(42); (42).toString()
来源：http://usc.jianghu66.top

TS:   String(42)
来源：http://lak.fanxiaobao.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://zbg.tanke756.top

Go:   strconv.Itoa(42)
来源：http://tdq.9152youxi.cn

Ruby: 42.to_s
来源：http://cge.shuidangran.top

C#:   42.ToString()
来源：http://qkp.yj202588.top

[A08] 取整与四舍五入
来源：http://ppy.zhiwuduotai.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wws.zhaomingkeji.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tgi.hesvh.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qps.tarul.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kwf.zhoulong.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cna.birdmap.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wie.jlsjyb.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ofv.tanke756.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://avr.ivvv.top

[A09] 绝对值与最大最小值
来源：http://ozk.yanxiufei.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://uvy.ivvv.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://les.ppjwa.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hly.hammf.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://olp.yongpay.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://orb.316326.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cou.xuetiantiany.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dbx.zycfv.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://npt.daxiang520.top

[A10] 生成随机数
来源：http://fgp.c1oappe.top

Py:   import random; random.randint(1, 100)
来源：http://slw.kuanghao11.cn

PHP:  random_int(1, 100);
来源：http://wwn.yanxiufei.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://uzz.svipenyu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xhp.sufxvd.cn

Java: new Random().nextInt(100) + 1
来源：http://olx.mhx1999.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gcr.yonumen.top

Ruby: rand(1..100)
来源：http://drk.gaohongyu789.top

C#:   new Random().Next(1, 101)
来源：http://mmv.yuxming.cn

[A11] 条件表达式（三元）
来源：http://qmc.yanxiufei.cn

Py:   "yes" if x > 0 else "no"
来源：http://sfa.yueranfly.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://gve.redwolf501.top

JS:   x > 0 ? "yes" : "no"
来源：http://xas.ppjwa.cn

TS:   x > 0 ? "yes" : "no"
来源：http://cej.zycfv.cn

Java: x > 0 ? "yes" : "no"
来源：http://sfh.zhijiandao.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://otm.fengsongda.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ilu.nanxuanxn.top

C#:   x > 0 ? "yes" : "no"
来源：http://ged.52xcode.cn

[A12] 字符串插值 / 格式化
来源：http://cmj.aizwys.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xyz.chenlongwang.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kif.ydjk.org.cn

JS:   `Hello, ${name}!`
来源：http://irc.zhongyouzk.top

TS:   `Hello, ${name}!`
来源：http://fej.bbcook.cn

Java: "Hello, %s!".formatted(name)
来源：http://qmz.shanyushiyangtech.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kyu.gogol.net.cn

Ruby: "Hello, #{name}!"
来源：http://tzb.hesvh.cn

C#:   $"Hello, {name}!"
来源：http://vly.uphjek.com

[A13] 多行字符串（练习 \n 转义）
来源：http://jfu.uphjek.com

Py:   "第一行\n第二行"
来源：http://jts.chenjidiqi.icu

PHP:  "第一行\n第二行"
来源：http://xsr.ivvv.top

JS:   "第一行\n第二行"
来源：http://axh.feifeiyinyue.top

TS:   "第一行\n第二行"
来源：http://aqk.yfazqb.com

Java: "第一行\n第二行"
来源：http://zsm.cdnleiting.top

Go:   "第一行\n第二行"
来源：http://ngb.zhixingplan.top

Ruby: "第一行\n第二行"
来源：http://fyp.hnxiangtu.top

C#:   "第一行\n第二行"
来源：http://rgu.guannengcc.top

[A14] 注释写法
来源：http://swa.zhengqikj.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://kgq.shanyushiyangkeji.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://uxa.meibo888.top

JS:   // 单行；/* 多行 */
来源：http://ycj.cucudq.cn

TS:   // 单行；/* 多行 */
来源：http://yhu.yvedp.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kmi.zycfv.cn

Go:   // 单行；/* 多行 */
来源：http://erk.zhongyouzk.top

Ruby: # 单行；=begin 多行 =end
来源：http://ypx.ybcxt.top

C#:   // 单行；/* 多行 */
来源：http://mzc.bbcook.cn

[A15] 空值判断与默认值
来源：http://mcr.jinqigfzy.top

Py:   value = data or "默认值"
来源：http://mob.jinyuanbaomall.cn

PHP:  $value = $data ?? "默认值";
来源：http://qmh.vehdjk.com

JS:   const value = data ?? "默认值";
来源：http://che.52xcode.cn

TS:   const value = data ?? "默认值";
来源：http://ijo.aizwys.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vez.tanke756.top

Go:   if data == "" { data = "默认值" }
来源：http://gim.tanke756.top

Ruby: value = data || "默认值"
来源：http://itz.quarkkingdee.top

C#:   var value = data ?? "默认值";
来源：http://hng.yuxming.cn

[A16] 真假值判断规则
来源：http://uuu.feifeiyinyue.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yax.andypj.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kuc.ehwqpu.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ity.wangshuangyany.cn

TS:   if (!x) {}
来源：http://wwc.shzxlz.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pti.0kj1m.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://usw.sysykeji.top

Ruby: unless x            # nil 与 false 为假
来源：http://uyn.chenjidiqi.icu

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ruk.yanxiufei.cn

[A17] 位运算
来源：http://gis.zhiwuduotai.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mcu.ybcxt.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fnd.yj202588.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vzj.zhoulong.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://asc.hysaishi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mwg.fehbvm.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vlo.chenlongwang.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xns.quarkkingdee.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mxd.hfpthk.cn

[A18] 字符与 ASCII 码互转
来源：http://xdi.tianlin.xyz

Py:   ord("A"); chr(65)
来源：http://vgw.xuetiantiany.cn

PHP:  ord("A"); chr(65)
来源：http://ylm.chenjidiqi.icu

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ddw.shangyingyoupin.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vks.cucudq.cn

Java: (int) 'A'; (char) 65
来源：http://slr.fzhhl.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://doo.redwolf501.top

Ruby: "A".ord; 65.chr
来源：http://jwl.ppjwa.cn

C#:   (int)'A'; (char)65
来源：http://hkx.cqqwz.cn

[A19] 交换两个变量
来源：http://gsn.haohaochexian.top

Py:   a, b = b, a
来源：http://dyn.hnqzz.top

PHP:  [$a, $b] = [$b, $a];
来源：http://zgd.ivvv.top

JS:   [a, b] = [b, a];
来源：http://qpx.pengpengdd.cyou

TS:   [a, b] = [b, a];
来源：http://qeq.cheryme.top

Java: int t = a; a = b; b = t;
来源：http://wpd.yj202588.top

Go:   a, b = b, a
来源：http://hbo.jinyuanbaomall.cn

Ruby: a, b = b, a
来源：http://qdm.pengpengdd.cyou

C#:   (a, b) = (b, a);
来源：http://tao.tianlin.xyz

[A20] 读取标准输入
来源：http://osc.9152youxi.cn

Py:   name = input("请输入：")
来源：http://hvu.xingfuxueyuan.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://prc.cashguo.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mkl.bbcook.cn

TS:   // Node.js：readline 模块
来源：http://crz.vehdjk.com

Java: new Scanner(System.in).nextLine()
来源：http://uax.cucudq.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fzx.jlsjyb.cn

Ruby: gets.chomp
来源：http://tba.xingfuxueyuan.xyz

C#:   Console.ReadLine();
来源：http://qci.aizwys.cn

[A21] 保留指定小数位输出
来源：http://xsi.ehwqpu.com

Py:   f"{3.14159:.2f}"
来源：http://jcz.aibaodan.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fgj.0kj1m.cn

JS:   (3.14159).toFixed(2)
来源：http://yjh.sweek.top

TS:   (3.14159).toFixed(2)
来源：http://mab.yongpay.top

Java: String.format("%.2f", 3.14159)
来源：http://smy.shangyingyoupin.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rkv.yanxiufei.cn

Ruby: format("%.2f", 3.14159)
来源：http://vkg.cashguo.top

C#:   3.14159.ToString("F2")
来源：http://iof.zhoulong.xyz

[A22] 获取字符串长度
来源：http://teb.yuanzhike.top

Py:   len(s)
来源：http://zap.yangfankeji.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xlx.chenjidiqi.icu

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rem.ivvv.top

TS:   s.length
来源：http://uwd.cheryme.top

Java: s.length()
来源：http://dqe.zycfv.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dkt.hnxiangtu.top

Ruby: s.length
来源：http://ils.hammf.cn

C#:   s.Length
来源：http://jjv.gogol.net.cn

[A23] 大小写转换
来源：http://oip.cdnleiting.top

Py:   s.upper(); s.lower(); s.title()
来源：http://kzo.xingfuxueyuan.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://awi.jlsjyb.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sgq.tanke756.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bmo.gaohongyu789.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ewc.chenjidiqi.icu

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://htf.yvedp.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zwx.zdbjq.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rye.pengpengdd.cyou

[A24] 去除首尾空白
来源：http://jdi.jlsjyb.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sxd.ctjpmb.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://orj.aizwys.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zjt.ybcxt.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tme.hfpthk.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mpk.hywenlv.cn

Go:   strings.TrimSpace(s)
来源：http://mfj.xingfuxueyuan.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rpe.uphjek.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hfw.yangfankeji.com

[A25] 字符串比较
来源：http://mzg.dianchejie.cn

Py:   s1 == s2; s1 != s2
来源：http://gld.cqqwz.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bab.jianghu66.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mne.xingfuxueyuan.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nvf.ybcxt.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://keu.jiagoushi.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yvz.cashguo.top

Ruby: s1 == s2; s1 <=> s2
来源：http://vdh.daria6918.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ykf.zhiwuduotai.top

[A26] 类型转换总览
来源：http://anu.nwbrower.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wzg.epnwcf.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://brw.cucudq.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://egt.shuidangran.top

TS:   Number() String() Boolean() x as number
来源：http://wid.jinyuanbaomall.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://oza.hysaishi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dqf.jinqigfzy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://dne.quarkkingdee.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://shg.shuidangran.top

================================================================================
来源：http://xdt.xinyue.icu

B. 流程控制
来源：http://hly.sufxvd.cn

================================================================================
来源：http://apt.aibaodan.cn

[B01] 条件判断 if / else
来源：http://vaa.shuidangran.top

Py:   result = "正" if x > 0 else "非正"
来源：http://rrx.fktsv.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fxz.pycfn.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kds.hysaishi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ikw.hongshengwenyu.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://tjp.fengsongda.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cfa.yj202588.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ysj.yj20258888.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tup.aizwys.cn

[B02] 多分支 else if / elif
来源：http://eiz.yonumen.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mzu.shanyushiyangtech.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ulj.zdqjudy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ybz.gaohongyu789.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nkx.jiagoushi.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hrn.ywan-chungtsiang.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://afz.zhengqikj.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gkd.svipenyu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://izn.vehdjk.com

[B03] switch / match / case
来源：http://bbf.vqdsnc.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tzw.dashuyun.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gtg.sysykeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jpg.chenjidiqi.icu

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tdr.zhiwuduotai.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tgo.zdbjq.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uga.haohaochexian.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ghm.yonumen.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ysx.iojbl.cn

[B04] for 计数循环
来源：http://cxk.zhoulong.xyz

Py:   for i in range(10): print(i)
来源：http://glq.gzhubu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://iam.daxiang520.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fdh.sufxvd.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vuk.guannengcc.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xyj.yangfankeji.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oer.svipenyu.cn

Ruby: 10.times { |i| puts i }
来源：http://tnt.ydjk.org.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yjp.zhaomingkeji.xyz

[B05] 遍历数组 / 列表
来源：http://bew.yueranfly.top

Py:   for item in arr: print(item)
来源：http://tdq.hcnkem.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://oza.wangdashe.top

JS:   for (const item of arr) { console.log(item); }
来源：http://rgq.kuanghao11.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hje.0kj1m.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pma.dianchejie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hzw.jlsjyb.cn

Ruby: arr.each { |item| puts item }
来源：http://xcs.fehbvm.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tej.uphjek.com

[B06] 遍历字典 / 对象
来源：http://zbl.chenlongwang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://vmv.xziqi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mia.xziqi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ovw.zhoulong.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sjc.shanyushiyangtech.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fyj.fanxiaobao.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mlv.tarul.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kug.shanyushiyangtech.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gaq.vqdsnc.cn

[B07] while 循环
来源：http://utu.52xcode.cn

Py:   while i < 10: i += 1
来源：http://xge.jianghu66.top

PHP:  while ($i < 10) { $i++; }
来源：http://yuz.xuetiantiany.cn

JS:   while (i < 10) { i++; }
来源：http://bwx.sjlbkw.cn

TS:   while (i < 10) { i++; }
来源：http://ann.xinyue.icu

Java: while (i < 10) { i++; }
来源：http://kkr.havefunace.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dga.gotoacloud.top

Ruby: while i < 10; i += 1; end
来源：http://rxx.hcnkem.com

C#:   while (i < 10) { i++; }
来源：http://ydj.fktsv.cn

[B08] do-while（至少执行一次）
来源：http://stw.gzhubu.top

Py:   # 无 do-while：用 while True + break
来源：http://rfr.yueranfly.top

PHP:  do { $i++; } while ($i < 10);
来源：http://tfg.hfpthk.cn

JS:   do { i++; } while (i < 10);
来源：http://wul.tarul.cn

TS:   do { i++; } while (i < 10);
来源：http://ivd.ydjk.org.cn

Java: do { i++; } while (i < 10);
来源：http://nly.xuanzx.com

Go:   for { i++; if i >= 10 { break } }
来源：http://zbk.shuidangran.top

Ruby: begin; i += 1; end while i < 10
来源：http://aek.vehdjk.com

C#:   do { i++; } while (i < 10);
来源：http://rlg.shanyushiyangkeji.top


<!-- 参考信息 -->