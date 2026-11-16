代发 wailian999

================================================================================
来源：http://cjx.jlsjyb.cn

A. 基础语法与类型
来源：http://zcn.zhixingplan.top

================================================================================
来源：http://chl.sxryk.cn

[A01] Hello World
来源：http://nqh.redwolf501.top

Py:   print("Hello, World!")
来源：http://tmf.xinyue.icu

PHP:  echo "Hello, World!";
来源：http://dea.andypj.xyz

JS:   console.log("Hello, World!");
来源：http://mnm.hongshengwenyu.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ilz.cqqwz.cn

Java: System.out.println("Hello, World!");
来源：http://dnn.chenlongwang.top

Go:   fmt.Println("Hello, World!")
来源：http://xuj.meibo888.top

Ruby: puts "Hello, World!"
来源：http://tdk.vehdjk.com

C#:   Console.WriteLine("Hello, World!");
来源：http://fyt.vqdsnc.cn

[A02] 变量声明与赋值
来源：http://yew.pengpengdd.cyou

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tzo.iojbl.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://sfm.redwolf501.top

JS:   let name = "Alex"; const age = 20;
来源：http://ocx.yueranfly.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qwz.tarul.cn

Java: String name = "Alex"; int age = 20;
来源：http://ukl.zdqjudy.top

Go:   name := "Alex"; age := 20
来源：http://zvt.sxryk.cn

Ruby: name = "Alex"; age = 20
来源：http://ydr.aizwys.cn

C#:   string name = "Alex"; int age = 20;
来源：http://hxs.sufxvd.cn

[A03] 常量定义
来源：http://nbq.0kj1m.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rim.uphjek.com

PHP:  const PI = 3.14159;
来源：http://pqg.hongshengwenyu.top

JS:   const PI = 3.14159;
来源：http://qss.dashuyun.cn

TS:   const PI: number = 3.14159;
来源：http://vgw.chenlongwang.top

Java: static final double PI = 3.14159;
来源：http://bdg.dianchejie.cn

Go:   const PI = 3.14159
来源：http://iux.9152youxi.cn

Ruby: PI = 3.14159
来源：http://mxy.gzhubu.top

C#:   const double PI = 3.14159;
来源：http://ert.hnxiangtu.top

[A04] 判断变量类型
来源：http://uzm.ydjk.org.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://oxx.tianlin.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hkr.jianghu66.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nsy.gotoacloud.top

TS:   typeof x; x instanceof Date
来源：http://zmq.andypj.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qph.daxiang520.top

Go:   reflect.TypeOf(x).Name()
来源：http://tym.yonumen.top

Ruby: x.class; x.is_a?(Integer)
来源：http://mah.xingfuxueyuan.xyz

C#:   x.GetType().Name; x is int
来源：http://het.hnqzz.top

[A05] 整数除法与取模
来源：http://bfv.nanxinkj.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://isl.ybcxt.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://bzf.uphjek.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cdw.hywenlv.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vhj.jinqigfzy.top

Java: 7 / 2; 7 % 2
来源：http://zkf.shzxlz.cn

Go:   7 / 2; 7 % 2
来源：http://nke.fengsongda.top

Ruby: 7 / 2; 7 % 2
来源：http://gok.gzhubu.top

C#:   7 / 2; 7 % 2
来源：http://npi.jqgufenzy.top

[A06] 字符串转数字
来源：http://alc.iojbl.cn

Py:   int("42"); float("3.14")
来源：http://atr.zhaomingkeji.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fxl.9152youxi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tzy.xuetiantiany.cn

TS:   parseInt("42", 10); Number("42")
来源：http://sgy.havefunace.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lqc.0kj1m.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uph.0kj1m.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bmr.tian-w.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://oif.zhaomingkeji.xyz

[A07] 数字转字符串
来源：http://aze.smart0.xyz

Py:   str(42)
来源：http://tyb.yuanzhike.top

PHP:  (string) 42; strval(42)
来源：http://pfa.fehbvm.com

JS:   String(42); (42).toString()
来源：http://tyl.ydzc1.top

TS:   String(42)
来源：http://yjh.sysykeji.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://lvs.bjfxy.top

Go:   strconv.Itoa(42)
来源：http://uoo.nanxinkj.top

Ruby: 42.to_s
来源：http://iao.aibaodan.cn

C#:   42.ToString()
来源：http://utq.yuanzhike.top

[A08] 取整与四舍五入
来源：http://mzf.fzhhl.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://eef.snrcjt.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pjc.zycfv.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pgq.shuidangran.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hqm.daria6918.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lzb.snrcjt.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ajy.zycfv.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://srf.tianlin.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kxo.ivvv.top

[A09] 绝对值与最大最小值
来源：http://mhi.redwolf501.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tvw.xingfuxueyuan.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hid.yj20258888.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rrb.9152youxi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ehn.hysaishi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nrb.nanxinkj.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jma.shangyingyoupin.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tcx.bbcook.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bwq.smart0.xyz

[A10] 生成随机数
来源：http://igx.nwbrower.top

Py:   import random; random.randint(1, 100)
来源：http://acy.havefunace.top

PHP:  random_int(1, 100);
来源：http://cdw.shzxlz.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ygh.316326.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://uhf.vqdsnc.cn

Java: new Random().nextInt(100) + 1
来源：http://ucq.yj20258.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://acm.mhx1999.top

Ruby: rand(1..100)
来源：http://mge.sysykeji.top

C#:   new Random().Next(1, 101)
来源：http://xnm.shanyushiyangtech.top

[A11] 条件表达式（三元）
来源：http://cie.hammf.cn

Py:   "yes" if x > 0 else "no"
来源：http://ror.kuanghao11.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://tun.tarul.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xhu.uphjek.com

TS:   x > 0 ? "yes" : "no"
来源：http://iou.havefunace.top

Java: x > 0 ? "yes" : "no"
来源：http://owd.chenlongwang.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ard.zdbjq.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tbz.vehdjk.com

C#:   x > 0 ? "yes" : "no"
来源：http://pot.jyoumei.cn

[A12] 字符串插值 / 格式化
来源：http://xvg.hammf.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://uqt.tanke756.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kvm.fengsongda.top

JS:   `Hello, ${name}!`
来源：http://pxe.guannengcc.top

TS:   `Hello, ${name}!`
来源：http://dsz.redwolf501.top

Java: "Hello, %s!".formatted(name)
来源：http://ysi.hysaishi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yok.jinqigufen.top

Ruby: "Hello, #{name}!"
来源：http://yoi.ppjwa.cn

C#:   $"Hello, {name}!"
来源：http://cxs.xuetiantiany.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vqv.uphjek.com

Py:   "第一行\n第二行"
来源：http://ssx.vqdsnc.cn

PHP:  "第一行\n第二行"
来源：http://erk.feifeiyinyue.top

JS:   "第一行\n第二行"
来源：http://cis.guowangkeji.top

TS:   "第一行\n第二行"
来源：http://tsg.fehbvm.com

Java: "第一行\n第二行"
来源：http://dki.9152youxi.cn

Go:   "第一行\n第二行"
来源：http://ymm.gzhubu.top

Ruby: "第一行\n第二行"
来源：http://rnj.cheryme.top

C#:   "第一行\n第二行"
来源：http://gtn.ehwqpu.com

[A14] 注释写法
来源：http://vso.jinqigfzy.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://rqy.smart0.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://qls.zhoulong.xyz

JS:   // 单行；/* 多行 */
来源：http://usw.sxryk.cn

TS:   // 单行；/* 多行 */
来源：http://bil.sxryk.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xxj.fehbvm.com

Go:   // 单行；/* 多行 */
来源：http://vcf.uphjek.com

Ruby: # 单行；=begin 多行 =end
来源：http://iie.chenzaomai.com

C#:   // 单行；/* 多行 */
来源：http://mjm.dianchejie.cn

[A15] 空值判断与默认值
来源：http://wcg.xylfe.cn

Py:   value = data or "默认值"
来源：http://jel.bbcook.cn

PHP:  $value = $data ?? "默认值";
来源：http://xbl.yvedp.cn

JS:   const value = data ?? "默认值";
来源：http://rud.zycfv.cn

TS:   const value = data ?? "默认值";
来源：http://gsf.nanxuanxn.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cfz.0kj1m.cn

Go:   if data == "" { data = "默认值" }
来源：http://lrg.zycfv.cn

Ruby: value = data || "默认值"
来源：http://qlb.tian-w.cn

C#:   var value = data ?? "默认值";
来源：http://bdb.cqqwz.cn

[A16] 真假值判断规则
来源：http://lab.hcnkem.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://odl.cqqwz.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mlm.zhengqikj.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pma.ehwqpu.com

TS:   if (!x) {}
来源：http://aae.pengpengdd.cyou

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gmr.fzhhl.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://owu.xylfe.cn

Ruby: unless x            # nil 与 false 为假
来源：http://khs.ydzc1.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://myg.fengsongda.top

[A17] 位运算
来源：http://jgu.yj20258.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gjz.hnxiangtu.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ppv.316326.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oer.havefunace.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rok.shanyushiyangkeji.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://owf.cucudq.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vhl.fzhhl.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rhf.yangfankeji.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cug.hcnkem.com

[A18] 字符与 ASCII 码互转
来源：http://ixt.xingfuxueyuan.xyz

Py:   ord("A"); chr(65)
来源：http://xye.zdqjudy.top

PHP:  ord("A"); chr(65)
来源：http://akv.iojbl.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uja.yj20258.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qxs.jianghu66.top

Java: (int) 'A'; (char) 65
来源：http://pyj.havefunace.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uzd.sysykeji.top

Ruby: "A".ord; 65.chr
来源：http://bwz.daxiang520.top

C#:   (int)'A'; (char)65
来源：http://fdd.zhijiandao.cn

[A19] 交换两个变量
来源：http://fmd.jyoumei.cn

Py:   a, b = b, a
来源：http://jhp.jinghuilouyu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://nfv.vqdsnc.cn

JS:   [a, b] = [b, a];
来源：http://hee.shangyingyoupin.top

TS:   [a, b] = [b, a];
来源：http://exe.yj202588.top

Java: int t = a; a = b; b = t;
来源：http://bsp.fzhhl.top

Go:   a, b = b, a
来源：http://tvb.yonumen.top

Ruby: a, b = b, a
来源：http://yfl.hywenlv.cn

C#:   (a, b) = (b, a);
来源：http://ijz.zhijiandao.cn

[A20] 读取标准输入
来源：http://qrm.xziqi.cn

Py:   name = input("请输入：")
来源：http://ypy.hammf.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ymk.shzxlz.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://akd.sysykeji.top

TS:   // Node.js：readline 模块
来源：http://yhp.shanyushiyangkeji.top

Java: new Scanner(System.in).nextLine()
来源：http://qot.zhiwuduotai.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://uyj.bjfxy.top

Ruby: gets.chomp
来源：http://leg.bjfxy.top

C#:   Console.ReadLine();
来源：http://wpu.ivvv.top

[A21] 保留指定小数位输出
来源：http://smr.andypj.xyz

Py:   f"{3.14159:.2f}"
来源：http://eho.jqgfzy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://shq.jiagoushi.top

JS:   (3.14159).toFixed(2)
来源：http://nbq.smart0.xyz

TS:   (3.14159).toFixed(2)
来源：http://qkn.zhongyouzk.top

Java: String.format("%.2f", 3.14159)
来源：http://lgi.zdqjudy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sbr.zycfv.cn

Ruby: format("%.2f", 3.14159)
来源：http://jas.nwbrower.top

C#:   3.14159.ToString("F2")
来源：http://djv.hongshengwenyu.top

[A22] 获取字符串长度
来源：http://pyt.svipenyu.cn

Py:   len(s)
来源：http://uae.zhaomingkeji.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tor.svipenyu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hfo.epnwcf.com

TS:   s.length
来源：http://rdh.jyoumei.cn

Java: s.length()
来源：http://zdj.hnqzz.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zqi.aizwys.cn

Ruby: s.length
来源：http://asq.hfpthk.cn

C#:   s.Length
来源：http://pva.nanxuanxn.top

[A23] 大小写转换
来源：http://vsb.vqdsnc.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://sve.wangshuangyany.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jsu.guannengcc.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dmb.jyoumei.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://chu.meibo888.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yrc.sjlbkw.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://uws.svipenyu.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://aps.ydjk.org.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gir.yfazqb.com

[A24] 去除首尾空白
来源：http://yeu.shangyingyoupin.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jdf.yvedp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hup.fktsv.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hqz.hesvh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rzf.fengsongda.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sbl.daria6918.cn

Go:   strings.TrimSpace(s)
来源：http://vkr.gzhubu.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://voa.0kj1m.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tgb.9152youxi.cn

[A25] 字符串比较
来源：http://uhk.shanyushiyangtech.top

Py:   s1 == s2; s1 != s2
来源：http://nlz.guannengcc.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xln.guannengcc.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ira.guowangkeji.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ils.ydjk.org.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tcj.xinyue.icu

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ivc.cheryme.top

Ruby: s1 == s2; s1 <=> s2
来源：http://xia.wangdashe.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cee.nwbrower.top

[A26] 类型转换总览
来源：http://bgt.zhongyouzk.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lug.vqdsnc.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uyi.jqgufenzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uxq.jinyuanbaomall.cn

TS:   Number() String() Boolean() x as number
来源：http://xgs.dashuyun.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://azz.nanxuanxn.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lgk.mhx1999.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://bcl.ywan-chungtsiang.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://aso.yonumen.top

================================================================================
来源：http://gmo.dianchejie.cn

B. 流程控制
来源：http://rvg.ppjwa.cn

================================================================================
来源：http://ypb.dashuyun.cn

[B01] 条件判断 if / else
来源：http://pug.fengsongda.top

Py:   result = "正" if x > 0 else "非正"
来源：http://tzy.ppjwa.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xpx.guannengcc.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cxo.hesvh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://efh.mhx1999.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://qbx.xuetiantiany.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fll.hnqzz.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jju.fktsv.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lnd.gzhubu.top

[B02] 多分支 else if / elif
来源：http://uuu.jqgfzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bxy.cqqwz.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://svg.nanxinkj.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bgv.zhixingplan.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lad.yanxiufei.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dkg.hfpthk.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yrv.yfazqb.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sjh.vqdsnc.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://icm.feifeiyinyue.top

[B03] switch / match / case
来源：http://oxm.jqgufenzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wmh.hammf.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cce.yonumen.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vju.c1oappe.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wwr.pycfn.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gkq.redwolf501.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dug.bbcook.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dyc.ivvv.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kea.yj202588.top

[B04] for 计数循环
来源：http://uiu.zhixingplan.top

Py:   for i in range(10): print(i)
来源：http://neh.ydjk.org.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://oot.zycfv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qaj.uphjek.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://igm.chenjidiqi.icu

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rcm.shanyushiyangtech.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tzd.haohaochexian.top

Ruby: 10.times { |i| puts i }
来源：http://twi.sysykeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://omt.gzhubu.top

[B05] 遍历数组 / 列表
来源：http://oih.hesvh.cn

Py:   for item in arr: print(item)
来源：http://wpz.meibo888.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jze.ydjk.org.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://efl.jianghu66.top

TS:   for (const item of arr) { console.log(item); }
来源：http://naw.jqgfzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://lod.sufxvd.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ylu.xinyue.icu

Ruby: arr.each { |item| puts item }
来源：http://pmc.jianghu66.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qkw.fanxiaobao.xyz

[B06] 遍历字典 / 对象
来源：http://sdi.yj202588.top

Py:   for k, v in d.items(): print(k, v)
来源：http://gfp.tarul.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cwr.0kj1m.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mzl.ydjk.org.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vqj.9152youxi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://com.birdmap.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cwr.haohaochexian.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://svv.xylfe.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://equ.nanxuanxn.top

[B07] while 循环
来源：http://bzs.zhijiandao.cn

Py:   while i < 10: i += 1
来源：http://ygy.yonumen.top

PHP:  while ($i < 10) { $i++; }
来源：http://zaa.shuidangran.top

JS:   while (i < 10) { i++; }
来源：http://nmx.tarul.cn

TS:   while (i < 10) { i++; }
来源：http://btr.vehdjk.com

Java: while (i < 10) { i++; }
来源：http://iie.zdbjq.cn


<!-- 参考信息 -->