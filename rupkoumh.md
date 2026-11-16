代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://fgi.hcnkem.com

Go:   fmt.Println("Hello, World!")
来源：http://ptt.daria6918.cn

Ruby: puts "Hello, World!"
来源：http://lhi.tarul.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jym.zhijiandao.cn

[A02] 变量声明与赋值
来源：http://miu.yanxiufei.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dex.hammf.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://vkl.xuanzx.com

JS:   let name = "Alex"; const age = 20;
来源：http://vik.xinyue.icu

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vvn.zhiwuduotai.top

Java: String name = "Alex"; int age = 20;
来源：http://hmq.daxiang520.top

Go:   name := "Alex"; age := 20
来源：http://lec.quarkkingdee.top

Ruby: name = "Alex"; age = 20
来源：http://wmy.jqgfzy.top

C#:   string name = "Alex"; int age = 20;
来源：http://ivz.nanxinkj.top

[A03] 常量定义
来源：http://lpa.zhoulong.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hgn.xingfuxueyuan.xyz

PHP:  const PI = 3.14159;
来源：http://wcx.shzxlz.cn

JS:   const PI = 3.14159;
来源：http://atp.tianlin.xyz

TS:   const PI: number = 3.14159;
来源：http://cqx.ywan-chungtsiang.top

Java: static final double PI = 3.14159;
来源：http://wic.gzhubu.top

Go:   const PI = 3.14159
来源：http://gaw.yj20258888.top

Ruby: PI = 3.14159
来源：http://hvy.shanyushiyangtech.top

C#:   const double PI = 3.14159;
来源：http://eos.dianchejie.cn

[A04] 判断变量类型
来源：http://sjj.yj202588.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://bvd.vehdjk.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://eix.jlsjyb.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zob.aizwys.cn

TS:   typeof x; x instanceof Date
来源：http://qsc.sysykeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wyv.jlsjyb.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rok.aizwys.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://rlp.ywan-chungtsiang.top

C#:   x.GetType().Name; x is int
来源：http://shc.svipenyu.cn

[A05] 整数除法与取模
来源：http://meg.yueranfly.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://izf.nanxuanxn.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://xyd.cdnleiting.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ksa.yanxiufei.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mng.ppjwa.cn

Java: 7 / 2; 7 % 2
来源：http://gwx.tian-w.cn

Go:   7 / 2; 7 % 2
来源：http://yxj.jlsjyb.cn

Ruby: 7 / 2; 7 % 2
来源：http://ywl.hnqzz.top

C#:   7 / 2; 7 % 2
来源：http://vod.cucudq.cn

[A06] 字符串转数字
来源：http://ems.shanyushiyangkeji.top

Py:   int("42"); float("3.14")
来源：http://itb.hesvh.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dpw.sxryk.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jyg.sjlbkw.cn

TS:   parseInt("42", 10); Number("42")
来源：http://usg.ctjpmb.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ywl.haohaochexian.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nbh.ydzc1.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ugu.hongshengwenyu.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kvi.ctjpmb.com

[A07] 数字转字符串
来源：http://afa.xuetiantiany.cn

Py:   str(42)
来源：http://ptd.yongpay.top

PHP:  (string) 42; strval(42)
来源：http://ijf.jyoumei.cn

JS:   String(42); (42).toString()
来源：http://ymh.cheryme.top

TS:   String(42)
来源：http://frc.zhixingplan.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://pqw.nwbrower.top

Go:   strconv.Itoa(42)
来源：http://rom.iojbl.cn

Ruby: 42.to_s
来源：http://rom.jiagoushi.top

C#:   42.ToString()
来源：http://xhm.c1oappe.top

[A08] 取整与四舍五入
来源：http://nwp.fanxiaobao.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://umn.zhiwuduotai.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bwh.guannengcc.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://omd.jinghuilouyu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qix.zdqjudy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://snr.pycfn.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qbj.fzhhl.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://hyb.vqdsnc.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://inm.xingfuxueyuan.xyz

[A09] 绝对值与最大最小值
来源：http://hth.cqqwz.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://sxa.wangdashe.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://aic.316326.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rpt.smart0.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://duk.yuanzhike.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nbz.guannengcc.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rtg.ivvv.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vue.aibaodan.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ily.tarul.cn

[A10] 生成随机数
来源：http://hgh.snrcjt.cn

Py:   import random; random.randint(1, 100)
来源：http://kwm.redwolf501.top

PHP:  random_int(1, 100);
来源：http://zzb.ivvv.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vop.birdmap.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hmn.meibo888.top

Java: new Random().nextInt(100) + 1
来源：http://kar.hongshengwenyu.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://aip.tarul.cn

Ruby: rand(1..100)
来源：http://jxg.hfpthk.cn

C#:   new Random().Next(1, 101)
来源：http://kzr.zhaomingkeji.xyz

[A11] 条件表达式（三元）
来源：http://ngn.hysaishi.cn

Py:   "yes" if x > 0 else "no"
来源：http://qmw.snrcjt.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://dbo.jinqigfzy.top

JS:   x > 0 ? "yes" : "no"
来源：http://pcj.jianghu66.top

TS:   x > 0 ? "yes" : "no"
来源：http://nnt.cdnleiting.top

Java: x > 0 ? "yes" : "no"
来源：http://ufl.zycfv.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://nwm.tian-w.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ppc.aibaodan.cn

C#:   x > 0 ? "yes" : "no"
来源：http://sfx.zhixingplan.top

[A12] 字符串插值 / 格式化
来源：http://sun.xylfe.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://oal.xinyue.icu

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qci.cucudq.cn

JS:   `Hello, ${name}!`
来源：http://qhi.yueranfly.top

TS:   `Hello, ${name}!`
来源：http://vrx.ywan-chungtsiang.top

Java: "Hello, %s!".formatted(name)
来源：http://ugb.shangyingyoupin.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jeb.jinyuanbaomall.cn

Ruby: "Hello, #{name}!"
来源：http://qhw.shangyingyoupin.top

C#:   $"Hello, {name}!"
来源：http://qsq.xinyue.icu

[A13] 多行字符串（练习 \n 转义）
来源：http://xep.ywan-chungtsiang.top

Py:   "第一行\n第二行"
来源：http://uev.sufxvd.cn

PHP:  "第一行\n第二行"
来源：http://qlq.sweek.top

JS:   "第一行\n第二行"
来源：http://ali.mhx1999.top

TS:   "第一行\n第二行"
来源：http://yfo.yongpay.top

Java: "第一行\n第二行"
来源：http://uoj.tianlin.xyz

Go:   "第一行\n第二行"
来源：http://ybf.yonumen.top

Ruby: "第一行\n第二行"
来源：http://khr.fanxiaobao.xyz

C#:   "第一行\n第二行"
来源：http://wio.ppjwa.cn

[A14] 注释写法
来源：http://xoh.gzhubu.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://xad.yongpay.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://xrv.chenjidiqi.icu

JS:   // 单行；/* 多行 */
来源：http://wac.wangshuangyany.cn

TS:   // 单行；/* 多行 */
来源：http://lkt.jqgufenzy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zsp.sxryk.cn

Go:   // 单行；/* 多行 */
来源：http://kej.gaohongyu789.top

Ruby: # 单行；=begin 多行 =end
来源：http://qxo.feifeiyinyue.top

C#:   // 单行；/* 多行 */
来源：http://sfx.quarkkingdee.top

[A15] 空值判断与默认值
来源：http://ccb.yangfankeji.com

Py:   value = data or "默认值"
来源：http://fum.tianlin.xyz

PHP:  $value = $data ?? "默认值";
来源：http://kmu.hongshengwenyu.top

JS:   const value = data ?? "默认值";
来源：http://ftp.tanke756.top

TS:   const value = data ?? "默认值";
来源：http://bqn.shanyushiyangtech.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fql.zhijiandao.cn

Go:   if data == "" { data = "默认值" }
来源：http://dca.snrcjt.cn

Ruby: value = data || "默认值"
来源：http://dfl.nanxuanxn.top

C#:   var value = data ?? "默认值";
来源：http://qeu.pengpengdd.cyou

[A16] 真假值判断规则
来源：http://cwj.yj20258888.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vvg.xinyue.icu

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xbk.dianchejie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qdz.sweek.top

TS:   if (!x) {}
来源：http://ogv.zhiwuduotai.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tos.xylfe.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xki.vehdjk.com

Ruby: unless x            # nil 与 false 为假
来源：http://njg.fehbvm.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nhm.hnxiangtu.top

[A17] 位运算
来源：http://fnz.yfazqb.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://atk.ydzc1.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://upi.zhixingplan.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kxa.guowangkeji.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://tcy.yj202588.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mpn.guowangkeji.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lvi.yj202588.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rgb.xziqi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tex.fengsongda.top

[A18] 字符与 ASCII 码互转
来源：http://dfu.nanxinkj.top

Py:   ord("A"); chr(65)
来源：http://gyp.sweek.top

PHP:  ord("A"); chr(65)
来源：http://xga.dashuyun.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ybg.tianlin.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://aty.c1oappe.top

Java: (int) 'A'; (char) 65
来源：http://hnt.9152youxi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://oxc.fktsv.cn

Ruby: "A".ord; 65.chr
来源：http://std.jlsjyb.cn

C#:   (int)'A'; (char)65
来源：http://fqt.shzxlz.cn

[A19] 交换两个变量
来源：http://cyq.quarkkingdee.top

Py:   a, b = b, a
来源：http://uyo.iojbl.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tdv.zdbjq.cn

JS:   [a, b] = [b, a];
来源：http://cab.pycfn.com

TS:   [a, b] = [b, a];
来源：http://zey.nanxinkj.top

Java: int t = a; a = b; b = t;
来源：http://ptm.shuidangran.top

Go:   a, b = b, a
来源：http://kzk.316326.xyz

Ruby: a, b = b, a
来源：http://zuz.yangfankeji.com

C#:   (a, b) = (b, a);
来源：http://qif.kuanghao11.cn

[A20] 读取标准输入
来源：http://dpq.tarul.cn

Py:   name = input("请输入：")
来源：http://vzl.fzhhl.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ucu.daria6918.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://upk.cdnleiting.top

TS:   // Node.js：readline 模块
来源：http://rhh.zycfv.cn

Java: new Scanner(System.in).nextLine()
来源：http://wwm.ehwqpu.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zgq.yonumen.top

Ruby: gets.chomp
来源：http://umu.ywan-chungtsiang.top

C#:   Console.ReadLine();
来源：http://cct.yanxiufei.cn

[A21] 保留指定小数位输出
来源：http://wks.gaohongyu789.top

Py:   f"{3.14159:.2f}"
来源：http://owg.mhx1999.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dem.chenjidiqi.icu

JS:   (3.14159).toFixed(2)
来源：http://ult.yj20258888.top

TS:   (3.14159).toFixed(2)
来源：http://vzw.zhixingplan.top

Java: String.format("%.2f", 3.14159)
来源：http://vvi.iojbl.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ikn.hnxiangtu.top

Ruby: format("%.2f", 3.14159)
来源：http://cxm.gogol.net.cn

C#:   3.14159.ToString("F2")
来源：http://dth.yueranfly.top

[A22] 获取字符串长度
来源：http://xdp.zycfv.cn

Py:   len(s)
来源：http://bjk.hammf.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hhp.yj20258.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bqc.ivvv.top

TS:   s.length
来源：http://ofd.cashguo.top

Java: s.length()
来源：http://pez.0kj1m.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jny.sweek.top

Ruby: s.length
来源：http://bxu.ctjpmb.com

C#:   s.Length
来源：http://gkq.epnwcf.com

[A23] 大小写转换
来源：http://evg.c1oappe.top

Py:   s.upper(); s.lower(); s.title()
来源：http://doo.jlsjyb.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qha.dianchejie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hdl.hnxiangtu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://odd.guannengcc.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bzf.yanxiufei.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lrf.yonumen.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yds.wangshuangyany.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://bvf.gzhubu.top

[A24] 去除首尾空白
来源：http://dyo.guowangkeji.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://twh.hammf.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://egb.feifeiyinyue.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gln.wangshuangyany.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vqj.xziqi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vyz.chenzaomai.com

Go:   strings.TrimSpace(s)
来源：http://ffz.smart0.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nuu.xinyue.icu

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qqu.hfpthk.cn

[A25] 字符串比较
来源：http://fgg.cashguo.top

Py:   s1 == s2; s1 != s2
来源：http://gkc.yvedp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://noq.yj20258888.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fys.bjfxy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ygs.feifeiyinyue.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jjp.xuetiantiany.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rzf.fanxiaobao.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://qsa.pycfn.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ist.birdmap.top

[A26] 类型转换总览
来源：http://eqd.yj20258.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://htx.daria6918.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wow.tanke756.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mva.zhengqikj.top

TS:   Number() String() Boolean() x as number
来源：http://jrm.hesvh.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://omn.hnxiangtu.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zho.havefunace.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ulz.zhiwuduotai.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cvl.fktsv.cn

================================================================================
来源：http://zfl.zhengqikj.top

B. 流程控制
来源：http://agu.jlsjyb.cn

================================================================================
来源：http://ssc.havefunace.top

[B01] 条件判断 if / else
来源：http://mqz.zhongyouzk.top

Py:   result = "正" if x > 0 else "非正"
来源：http://gzk.jqgfzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ckp.nanxinkj.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mjb.hywenlv.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hso.gogol.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pap.gaohongyu789.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://teb.jinghuilouyu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xry.yuanzhike.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://stg.yueranfly.top

[B02] 多分支 else if / elif
来源：http://qls.fzhhl.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yti.chenzaomai.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hvw.zycfv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rfv.guowangkeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qif.fengsongda.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://awc.zhijiandao.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://aig.zhiwuduotai.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mlo.xylfe.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mfs.xylfe.cn

[B03] switch / match / case
来源：http://oqk.sxryk.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ulc.xziqi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://def.yuxming.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ksn.daria6918.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rxe.yongpay.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sxh.ybcxt.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://iif.xziqi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://egg.ywan-chungtsiang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jqx.yuanzhike.top

[B04] for 计数循环
来源：http://vni.wangshuangyany.cn

Py:   for i in range(10): print(i)
来源：http://kmo.hnqzz.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vue.sjlbkw.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ipk.zhiwuduotai.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kjx.bbcook.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fvw.yj20258.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tpz.andypj.xyz

Ruby: 10.times { |i| puts i }
来源：http://pmu.nanxinkj.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://eeo.yj20258.top

[B05] 遍历数组 / 列表
来源：http://nmc.xuanzx.com

Py:   for item in arr: print(item)
来源：http://bwm.hfpthk.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kgq.yuxming.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://crd.cheryme.top

TS:   for (const item of arr) { console.log(item); }
来源：http://jdx.daria6918.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tsv.daxiang520.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xam.bbcook.cn

Ruby: arr.each { |item| puts item }
来源：http://ztp.316326.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kjx.sweek.top

[B06] 遍历字典 / 对象
来源：http://sch.sxryk.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://plg.zhiwuduotai.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xsr.jianghu66.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xqb.yanxiufei.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hao.316326.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://srh.aizwys.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dfa.sweek.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ukf.wangshuangyany.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xri.tian-w.cn

[B07] while 循环
来源：http://jzo.jqgufenzy.top

Py:   while i < 10: i += 1
来源：http://owg.ppjwa.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ene.xuanzx.com

JS:   while (i < 10) { i++; }
来源：http://vym.jinqigfzy.top

TS:   while (i < 10) { i++; }
来源：http://tif.sxryk.cn

Java: while (i < 10) { i++; }
来源：http://mze.ywan-chungtsiang.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://veu.havefunace.top

Ruby: while i < 10; i += 1; end
来源：http://rrp.ydzc1.top

C#:   while (i < 10) { i++; }
来源：http://blu.yj20258.top

[B08] do-while（至少执行一次）
来源：http://pxx.ivvv.top

Py:   # 无 do-while：用 while True + break
来源：http://mnn.yangfankeji.com

PHP:  do { $i++; } while ($i < 10);
来源：http://cuj.hysaishi.cn

JS:   do { i++; } while (i < 10);
来源：http://gin.sweek.top

TS:   do { i++; } while (i < 10);
来源：http://nav.jinghuilouyu.cn


<!-- 参考信息 -->