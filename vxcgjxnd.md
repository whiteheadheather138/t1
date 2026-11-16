代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://kny.ppjwa.cn

Go:   fmt.Println("Hello, World!")
来源：http://bxj.hfpthk.cn

Ruby: puts "Hello, World!"
来源：http://jyf.xinyue.icu

C#:   Console.WriteLine("Hello, World!");
来源：http://dqk.jinghuilouyu.cn

[A02] 变量声明与赋值
来源：http://zhl.jqgfzy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ecc.hywenlv.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://mum.guannengcc.top

JS:   let name = "Alex"; const age = 20;
来源：http://knr.ydjk.org.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ghu.wangdashe.top

Java: String name = "Alex"; int age = 20;
来源：http://fmk.jqgufenzy.top

Go:   name := "Alex"; age := 20
来源：http://tjo.feifeiyinyue.top

Ruby: name = "Alex"; age = 20
来源：http://lui.mhx1999.top

C#:   string name = "Alex"; int age = 20;
来源：http://gyg.epnwcf.com

[A03] 常量定义
来源：http://ggn.ybcxt.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kob.dashuyun.cn

PHP:  const PI = 3.14159;
来源：http://hfl.ctjpmb.com

JS:   const PI = 3.14159;
来源：http://vxz.jinyuanbaomall.cn

TS:   const PI: number = 3.14159;
来源：http://huk.havefunace.top

Java: static final double PI = 3.14159;
来源：http://svc.gotoacloud.top

Go:   const PI = 3.14159
来源：http://kkz.haohaochexian.top

Ruby: PI = 3.14159
来源：http://ffc.haohaochexian.top

C#:   const double PI = 3.14159;
来源：http://fku.zhiwuduotai.top

[A04] 判断变量类型
来源：http://pws.fzhhl.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://jaw.wangshuangyany.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ail.yangfankeji.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://imx.sxryk.cn

TS:   typeof x; x instanceof Date
来源：http://jyx.dianchejie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zch.yj202588.top

Go:   reflect.TypeOf(x).Name()
来源：http://zxk.hesvh.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://yba.hcnkem.com

C#:   x.GetType().Name; x is int
来源：http://nnv.havefunace.top

[A05] 整数除法与取模
来源：http://eav.xylfe.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tck.zycfv.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://tgt.xziqi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nnh.meibo888.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ert.jyoumei.cn

Java: 7 / 2; 7 % 2
来源：http://ent.chenlongwang.top

Go:   7 / 2; 7 % 2
来源：http://twd.hesvh.cn

Ruby: 7 / 2; 7 % 2
来源：http://pam.jinyuanbaomall.cn

C#:   7 / 2; 7 % 2
来源：http://kzr.gogol.net.cn

[A06] 字符串转数字
来源：http://mgr.zhijiandao.cn

Py:   int("42"); float("3.14")
来源：http://okd.pycfn.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kwf.tianlin.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wjx.uphjek.com

TS:   parseInt("42", 10); Number("42")
来源：http://oup.daria6918.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xpd.yuanzhike.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tae.sjlbkw.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://mqj.zdbjq.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zxp.chenlongwang.top

[A07] 数字转字符串
来源：http://mzz.havefunace.top

Py:   str(42)
来源：http://wet.smart0.xyz

PHP:  (string) 42; strval(42)
来源：http://zar.vehdjk.com

JS:   String(42); (42).toString()
来源：http://iol.vehdjk.com

TS:   String(42)
来源：http://oww.daria6918.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://cfa.vehdjk.com

Go:   strconv.Itoa(42)
来源：http://kte.snrcjt.cn

Ruby: 42.to_s
来源：http://dvi.pycfn.com

C#:   42.ToString()
来源：http://kut.zhijiandao.cn

[A08] 取整与四舍五入
来源：http://qvv.guowangkeji.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://shw.c1oappe.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://uju.guannengcc.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mux.vehdjk.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gub.ppjwa.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://emf.ehwqpu.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dwh.fehbvm.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://mbw.nanxuanxn.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://nhj.jlsjyb.cn

[A09] 绝对值与最大最小值
来源：http://ffh.andypj.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jju.sxryk.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mmk.0kj1m.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dqw.tianlin.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://occ.yueranfly.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vvv.xinyue.icu

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://las.xuanzx.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wyg.hammf.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://cvg.nanxuanxn.top

[A10] 生成随机数
来源：http://tnw.0kj1m.cn

Py:   import random; random.randint(1, 100)
来源：http://kzp.quarkkingdee.top

PHP:  random_int(1, 100);
来源：http://asj.vqdsnc.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gon.ivvv.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cwu.uphjek.com

Java: new Random().nextInt(100) + 1
来源：http://qma.yj202588.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://daz.nwbrower.top

Ruby: rand(1..100)
来源：http://ktz.yonumen.top

C#:   new Random().Next(1, 101)
来源：http://hmd.sufxvd.cn

[A11] 条件表达式（三元）
来源：http://shp.zdbjq.cn

Py:   "yes" if x > 0 else "no"
来源：http://asu.shanyushiyangkeji.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://pfd.sxryk.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pit.9152youxi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://fsg.ydjk.org.cn

Java: x > 0 ? "yes" : "no"
来源：http://ins.jinqigfzy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ysl.jqgfzy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://arw.feifeiyinyue.top

C#:   x > 0 ? "yes" : "no"
来源：http://oiz.shuidangran.top

[A12] 字符串插值 / 格式化
来源：http://nkc.jinghuilouyu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://uir.ehwqpu.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zfm.andypj.xyz

JS:   `Hello, ${name}!`
来源：http://dgz.fktsv.cn

TS:   `Hello, ${name}!`
来源：http://gal.sxryk.cn

Java: "Hello, %s!".formatted(name)
来源：http://hwr.hammf.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yrd.nwbrower.top

Ruby: "Hello, #{name}!"
来源：http://mhe.zdbjq.cn

C#:   $"Hello, {name}!"
来源：http://pwd.kuanghao11.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://man.shangyingyoupin.top

Py:   "第一行\n第二行"
来源：http://lse.aizwys.cn

PHP:  "第一行\n第二行"
来源：http://qqx.haohaochexian.top

JS:   "第一行\n第二行"
来源：http://maw.hnxiangtu.top

TS:   "第一行\n第二行"
来源：http://wlx.ybcxt.top

Java: "第一行\n第二行"
来源：http://fan.daria6918.cn

Go:   "第一行\n第二行"
来源：http://qwc.hnqzz.top

Ruby: "第一行\n第二行"
来源：http://izl.yvedp.cn

C#:   "第一行\n第二行"
来源：http://aqg.fengsongda.top

[A14] 注释写法
来源：http://lwb.svipenyu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gkb.fanxiaobao.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://zoi.cashguo.top

JS:   // 单行；/* 多行 */
来源：http://cgp.kuanghao11.cn

TS:   // 单行；/* 多行 */
来源：http://zbu.wangshuangyany.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vlw.shzxlz.cn

Go:   // 单行；/* 多行 */
来源：http://kon.hongshengwenyu.top

Ruby: # 单行；=begin 多行 =end
来源：http://cby.xuetiantiany.cn

C#:   // 单行；/* 多行 */
来源：http://vut.jyoumei.cn

[A15] 空值判断与默认值
来源：http://cmw.9152youxi.cn

Py:   value = data or "默认值"
来源：http://oka.hcnkem.com

PHP:  $value = $data ?? "默认值";
来源：http://bkf.fktsv.cn

JS:   const value = data ?? "默认值";
来源：http://vtb.tarul.cn

TS:   const value = data ?? "默认值";
来源：http://gfy.birdmap.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dte.ydjk.org.cn

Go:   if data == "" { data = "默认值" }
来源：http://bel.hysaishi.cn

Ruby: value = data || "默认值"
来源：http://lcq.yuxming.cn

C#:   var value = data ?? "默认值";
来源：http://ltx.shanyushiyangtech.top

[A16] 真假值判断规则
来源：http://riu.ivvv.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://too.wangshuangyany.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://sas.ybcxt.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mrn.cdnleiting.top

TS:   if (!x) {}
来源：http://yuj.quarkkingdee.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ite.haohaochexian.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rnw.yj20258888.top

Ruby: unless x            # nil 与 false 为假
来源：http://umg.shanyushiyangkeji.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zrk.dashuyun.cn

[A17] 位运算
来源：http://jwt.hcnkem.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rfa.ppjwa.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gph.redwolf501.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kkt.meibo888.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dbj.gaohongyu789.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lym.sysykeji.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dss.dashuyun.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lgf.jinqigufen.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cyv.hongshengwenyu.top

[A18] 字符与 ASCII 码互转
来源：http://agp.vehdjk.com

Py:   ord("A"); chr(65)
来源：http://dck.yuanzhike.top

PHP:  ord("A"); chr(65)
来源：http://tau.sweek.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fxv.yj20258888.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mne.meibo888.top

Java: (int) 'A'; (char) 65
来源：http://udg.quarkkingdee.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ifv.yanxiufei.cn

Ruby: "A".ord; 65.chr
来源：http://uej.zycfv.cn

C#:   (int)'A'; (char)65
来源：http://wwk.hesvh.cn

[A19] 交换两个变量
来源：http://xfh.sufxvd.cn

Py:   a, b = b, a
来源：http://ipf.smart0.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://cyw.hysaishi.cn

JS:   [a, b] = [b, a];
来源：http://bty.chenzaomai.com

TS:   [a, b] = [b, a];
来源：http://gak.cdnleiting.top

Java: int t = a; a = b; b = t;
来源：http://pga.fanxiaobao.xyz

Go:   a, b = b, a
来源：http://iiq.dashuyun.cn

Ruby: a, b = b, a
来源：http://whd.zdqjudy.top

C#:   (a, b) = (b, a);
来源：http://yqu.yj20258888.top

[A20] 读取标准输入
来源：http://dxa.9152youxi.cn

Py:   name = input("请输入：")
来源：http://nko.xinyue.icu

PHP:  $name = trim(fgets(STDIN));
来源：http://aes.sysykeji.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rzb.gaohongyu789.top

TS:   // Node.js：readline 模块
来源：http://gux.pengpengdd.cyou

Java: new Scanner(System.in).nextLine()
来源：http://mnw.fehbvm.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hup.tianlin.xyz

Ruby: gets.chomp
来源：http://jvf.316326.xyz

C#:   Console.ReadLine();
来源：http://qle.sysykeji.top

[A21] 保留指定小数位输出
来源：http://zzu.iojbl.cn

Py:   f"{3.14159:.2f}"
来源：http://pub.zhoulong.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ovy.c1oappe.top

JS:   (3.14159).toFixed(2)
来源：http://urg.sweek.top

TS:   (3.14159).toFixed(2)
来源：http://awe.fengsongda.top

Java: String.format("%.2f", 3.14159)
来源：http://acf.316326.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lsk.sweek.top

Ruby: format("%.2f", 3.14159)
来源：http://mlt.feifeiyinyue.top

C#:   3.14159.ToString("F2")
来源：http://hke.jiagoushi.top

[A22] 获取字符串长度
来源：http://tns.hnqzz.top

Py:   len(s)
来源：http://tuy.xuetiantiany.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bxj.feifeiyinyue.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://iql.bjfxy.top

TS:   s.length
来源：http://qwl.ydjk.org.cn

Java: s.length()
来源：http://rmc.nwbrower.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uyr.wangshuangyany.cn

Ruby: s.length
来源：http://wuu.jianghu66.top

C#:   s.Length
来源：http://mdq.zhongyouzk.top

[A23] 大小写转换
来源：http://xon.9152youxi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://aym.xuanzx.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lkj.sjlbkw.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kgk.sxryk.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tqw.ybcxt.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hpf.jianghu66.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://usj.birdmap.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mli.shzxlz.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qfq.guowangkeji.top

[A24] 去除首尾空白
来源：http://dma.svipenyu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nrt.xylfe.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://oms.jinyuanbaomall.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bhb.yongpay.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://swn.redwolf501.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rqg.xuanzx.com

Go:   strings.TrimSpace(s)
来源：http://ryy.zhixingplan.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sst.gaohongyu789.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pep.tarul.cn

[A25] 字符串比较
来源：http://neu.ppjwa.cn

Py:   s1 == s2; s1 != s2
来源：http://tni.shzxlz.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yqg.ehwqpu.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wug.ehwqpu.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bws.cqqwz.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qeu.yuanzhike.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://iyi.cashguo.top

Ruby: s1 == s2; s1 <=> s2
来源：http://lhq.zdbjq.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bva.uphjek.com

[A26] 类型转换总览
来源：http://rne.iojbl.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vrm.shangyingyoupin.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hdm.pycfn.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dnp.gzhubu.top

TS:   Number() String() Boolean() x as number
来源：http://dfa.ydjk.org.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uiy.ehwqpu.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nde.sxryk.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nhc.yuanzhike.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mqa.mhx1999.top

================================================================================
来源：http://oov.chenzaomai.com

B. 流程控制
来源：http://jag.cucudq.cn

================================================================================
来源：http://aga.feifeiyinyue.top

[B01] 条件判断 if / else
来源：http://qtr.zhoulong.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://epe.wangshuangyany.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lpf.tanke756.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ykw.yongpay.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://abw.jinyuanbaomall.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://itr.sufxvd.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sap.yuanzhike.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jie.yuanzhike.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tfg.yongpay.top

[B02] 多分支 else if / elif
来源：http://coe.wangdashe.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rhu.jlsjyb.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yog.andypj.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://amo.feifeiyinyue.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xwl.zhongyouzk.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eks.snrcjt.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kje.yj202588.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://waq.cqqwz.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ypb.guannengcc.top

[B03] switch / match / case
来源：http://mrj.tarul.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://syd.pengpengdd.cyou

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vzz.smart0.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://avf.jyoumei.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://knq.hammf.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tpo.fzhhl.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ooz.jyoumei.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xuw.cqqwz.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uoa.vqdsnc.cn

[B04] for 计数循环
来源：http://ssj.yongpay.top

Py:   for i in range(10): print(i)
来源：http://xlj.dashuyun.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kkp.sysykeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dgf.tianlin.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ofo.chenzaomai.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xgt.yj20258.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xty.hongshengwenyu.top

Ruby: 10.times { |i| puts i }
来源：http://wzp.hysaishi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lqp.havefunace.top

[B05] 遍历数组 / 列表
来源：http://rpy.xziqi.cn

Py:   for item in arr: print(item)
来源：http://jsp.52xcode.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ljv.nwbrower.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hzi.tian-w.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://btt.yangfankeji.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://mld.zycfv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://htc.daxiang520.top

Ruby: arr.each { |item| puts item }
来源：http://wys.zhengqikj.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yfp.cucudq.cn

[B06] 遍历字典 / 对象
来源：http://kto.ydzc1.top

Py:   for k, v in d.items(): print(k, v)
来源：http://fad.0kj1m.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://brr.zhiwuduotai.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://agz.yfazqb.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nfb.tianlin.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gqb.yj202588.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yqp.kuanghao11.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mwv.hammf.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://oys.ydzc1.top

[B07] while 循环
来源：http://ewn.gotoacloud.top

Py:   while i < 10: i += 1
来源：http://jew.jinyuanbaomall.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tdz.xziqi.cn

JS:   while (i < 10) { i++; }
来源：http://trn.xinyue.icu

TS:   while (i < 10) { i++; }
来源：http://emx.shangyingyoupin.top

Java: while (i < 10) { i++; }
来源：http://jpz.andypj.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nqq.ctjpmb.com

Ruby: while i < 10; i += 1; end
来源：http://sbr.jlsjyb.cn

C#:   while (i < 10) { i++; }
来源：http://mpj.zhijiandao.cn

[B08] do-while（至少执行一次）
来源：http://eri.dashuyun.cn

Py:   # 无 do-while：用 while True + break
来源：http://ojs.iojbl.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cwg.ydzc1.top

JS:   do { i++; } while (i < 10);
来源：http://emw.yj20258.top

TS:   do { i++; } while (i < 10);
来源：http://rqb.havefunace.top


<!-- 参考信息 -->