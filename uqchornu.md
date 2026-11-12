代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://woc.shzxlz.cn

Go:   fmt.Println("Hello, World!")
来源：http://ldr.jianghu66.top

Ruby: puts "Hello, World!"
来源：http://vip.jianghu66.top

C#:   Console.WriteLine("Hello, World!");
来源：http://mpk.yuanzhike.top

[A02] 变量声明与赋值
来源：http://tzj.andypj.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jcy.ydjk.org.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://zok.aibaodan.cn

JS:   let name = "Alex"; const age = 20;
来源：http://fhj.cashguo.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://klf.bjfxy.top

Java: String name = "Alex"; int age = 20;
来源：http://iwc.hysaishi.cn

Go:   name := "Alex"; age := 20
来源：http://caa.hnxiangtu.top

Ruby: name = "Alex"; age = 20
来源：http://lrd.tanke756.top

C#:   string name = "Alex"; int age = 20;
来源：http://xdb.tian-w.cn

[A03] 常量定义
来源：http://cig.wangshuangyany.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nqr.ctjpmb.com

PHP:  const PI = 3.14159;
来源：http://bdi.chenlongwang.top

JS:   const PI = 3.14159;
来源：http://kmq.yangfankeji.com

TS:   const PI: number = 3.14159;
来源：http://uov.chenjidiqi.icu

Java: static final double PI = 3.14159;
来源：http://xle.hnxiangtu.top

Go:   const PI = 3.14159
来源：http://dck.yongpay.top

Ruby: PI = 3.14159
来源：http://zqp.cdnleiting.top

C#:   const double PI = 3.14159;
来源：http://kpy.zhoulong.xyz

[A04] 判断变量类型
来源：http://shp.ctjpmb.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://ohw.xziqi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://njs.sweek.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qjt.tanke756.top

TS:   typeof x; x instanceof Date
来源：http://tlu.shanyushiyangtech.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rvi.jianghu66.top

Go:   reflect.TypeOf(x).Name()
来源：http://bri.ivvv.top

Ruby: x.class; x.is_a?(Integer)
来源：http://tvg.cqqwz.cn

C#:   x.GetType().Name; x is int
来源：http://jqa.yueranfly.top

[A05] 整数除法与取模
来源：http://nro.cqqwz.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kro.jlsjyb.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://pqc.zhongyouzk.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://myu.gotoacloud.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rip.yanxiufei.cn

Java: 7 / 2; 7 % 2
来源：http://sxh.fehbvm.com

Go:   7 / 2; 7 % 2
来源：http://yxh.epnwcf.com

Ruby: 7 / 2; 7 % 2
来源：http://tmb.xylfe.cn

C#:   7 / 2; 7 % 2
来源：http://mta.hammf.cn

[A06] 字符串转数字
来源：http://waq.xinyue.icu

Py:   int("42"); float("3.14")
来源：http://jvn.pycfn.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://moj.xuetiantiany.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vfp.ehwqpu.com

TS:   parseInt("42", 10); Number("42")
来源：http://hqp.tarul.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kes.yonumen.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ifh.svipenyu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ctc.gzhubu.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vpz.zycfv.cn

[A07] 数字转字符串
来源：http://geo.yuanzhike.top

Py:   str(42)
来源：http://akq.aizwys.cn

PHP:  (string) 42; strval(42)
来源：http://bmm.ydzc1.top

JS:   String(42); (42).toString()
来源：http://axg.fktsv.cn

TS:   String(42)
来源：http://osa.gotoacloud.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ffb.quarkkingdee.top

Go:   strconv.Itoa(42)
来源：http://kex.jinyuanbaomall.cn

Ruby: 42.to_s
来源：http://ndn.meibo888.top

C#:   42.ToString()
来源：http://ucj.gzhubu.top

[A08] 取整与四舍五入
来源：http://bjt.yangfankeji.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rds.sweek.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kmv.feifeiyinyue.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qiv.gotoacloud.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xqs.kuanghao11.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hut.gotoacloud.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ufi.aibaodan.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://vox.daria6918.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pjb.zhaomingkeji.xyz

[A09] 绝对值与最大最小值
来源：http://tcz.zhiwuduotai.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lvl.hywenlv.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gyu.yongpay.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wwo.epnwcf.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xxl.xingfuxueyuan.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rol.yanxiufei.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://aqw.jiagoushi.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jhj.daxiang520.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hsf.zdbjq.cn

[A10] 生成随机数
来源：http://mqx.yj20258.top

Py:   import random; random.randint(1, 100)
来源：http://cvb.guowangkeji.top

PHP:  random_int(1, 100);
来源：http://hoj.yuxming.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cfl.hysaishi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qjd.mhx1999.top

Java: new Random().nextInt(100) + 1
来源：http://fxe.gotoacloud.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ijf.redwolf501.top

Ruby: rand(1..100)
来源：http://tqu.epnwcf.com

C#:   new Random().Next(1, 101)
来源：http://tar.ppjwa.cn

[A11] 条件表达式（三元）
来源：http://fwy.shuidangran.top

Py:   "yes" if x > 0 else "no"
来源：http://vas.fehbvm.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://cyh.hnxiangtu.top

JS:   x > 0 ? "yes" : "no"
来源：http://ods.pengpengdd.cyou

TS:   x > 0 ? "yes" : "no"
来源：http://hpl.feifeiyinyue.top

Java: x > 0 ? "yes" : "no"
来源：http://drs.cqqwz.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://jcp.tianlin.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://cno.ivvv.top

C#:   x > 0 ? "yes" : "no"
来源：http://vkl.ctjpmb.com

[A12] 字符串插值 / 格式化
来源：http://hzy.ydjk.org.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ubs.zhongyouzk.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xle.pycfn.com

JS:   `Hello, ${name}!`
来源：http://vtq.chenzaomai.com

TS:   `Hello, ${name}!`
来源：http://iqe.tanke756.top

Java: "Hello, %s!".formatted(name)
来源：http://qag.fengsongda.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xiu.zhijiandao.cn

Ruby: "Hello, #{name}!"
来源：http://ego.jinyuanbaomall.cn

C#:   $"Hello, {name}!"
来源：http://bum.cucudq.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://gkq.jiagoushi.top

Py:   "第一行\n第二行"
来源：http://iln.yvedp.cn

PHP:  "第一行\n第二行"
来源：http://kof.daxiang520.top

JS:   "第一行\n第二行"
来源：http://tdl.nanxuanxn.top

TS:   "第一行\n第二行"
来源：http://two.yonumen.top

Java: "第一行\n第二行"
来源：http://mge.tianlin.xyz

Go:   "第一行\n第二行"
来源：http://nfy.sxryk.cn

Ruby: "第一行\n第二行"
来源：http://sep.aizwys.cn

C#:   "第一行\n第二行"
来源：http://mqr.ehwqpu.com

[A14] 注释写法
来源：http://xsu.hesvh.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://dcg.sxryk.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://oyq.gaohongyu789.top

JS:   // 单行；/* 多行 */
来源：http://gjj.tian-w.cn

TS:   // 单行；/* 多行 */
来源：http://xzw.sweek.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kle.gogol.net.cn

Go:   // 单行；/* 多行 */
来源：http://wnz.pycfn.com

Ruby: # 单行；=begin 多行 =end
来源：http://trh.hesvh.cn

C#:   // 单行；/* 多行 */
来源：http://rke.cashguo.top

[A15] 空值判断与默认值
来源：http://jmm.tarul.cn

Py:   value = data or "默认值"
来源：http://spe.daria6918.cn

PHP:  $value = $data ?? "默认值";
来源：http://ohw.tanke756.top

JS:   const value = data ?? "默认值";
来源：http://ank.bbcook.cn

TS:   const value = data ?? "默认值";
来源：http://kxk.pycfn.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://oje.vqdsnc.cn

Go:   if data == "" { data = "默认值" }
来源：http://adk.yuanzhike.top

Ruby: value = data || "默认值"
来源：http://rbc.tarul.cn

C#:   var value = data ?? "默认值";
来源：http://qoe.jiagoushi.top

[A16] 真假值判断规则
来源：http://lwu.cdnleiting.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fzr.xuetiantiany.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kuj.hnqzz.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ghu.mhx1999.top

TS:   if (!x) {}
来源：http://mjk.hysaishi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bsg.xuanzx.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zjn.shangyingyoupin.top

Ruby: unless x            # nil 与 false 为假
来源：http://ali.daxiang520.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://set.gaohongyu789.top

[A17] 位运算
来源：http://iey.hnxiangtu.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dpv.daria6918.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ycf.jlsjyb.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xdi.haohaochexian.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://agv.xuanzx.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://shh.smart0.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rhg.birdmap.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uye.gzhubu.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ayv.ybcxt.top

[A18] 字符与 ASCII 码互转
来源：http://xur.jqgufenzy.top

Py:   ord("A"); chr(65)
来源：http://wdh.tanke756.top

PHP:  ord("A"); chr(65)
来源：http://wkk.yuanzhike.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oyy.pycfn.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lym.nanxuanxn.top

Java: (int) 'A'; (char) 65
来源：http://xhx.shzxlz.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gzw.xingfuxueyuan.xyz

Ruby: "A".ord; 65.chr
来源：http://rdo.hesvh.cn

C#:   (int)'A'; (char)65
来源：http://fic.jiagoushi.top

[A19] 交换两个变量
来源：http://smm.yuanzhike.top

Py:   a, b = b, a
来源：http://hgp.haohaochexian.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ymq.jinghuilouyu.cn

JS:   [a, b] = [b, a];
来源：http://chh.0kj1m.cn

TS:   [a, b] = [b, a];
来源：http://bqm.yj202588.top

Java: int t = a; a = b; b = t;
来源：http://zxk.zhiwuduotai.top

Go:   a, b = b, a
来源：http://ijg.fengsongda.top

Ruby: a, b = b, a
来源：http://qia.pengpengdd.cyou

C#:   (a, b) = (b, a);
来源：http://yet.andypj.xyz

[A20] 读取标准输入
来源：http://qhx.zhixingplan.top

Py:   name = input("请输入：")
来源：http://aez.hnqzz.top

PHP:  $name = trim(fgets(STDIN));
来源：http://tgi.ywan-chungtsiang.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pbm.ywan-chungtsiang.top

TS:   // Node.js：readline 模块
来源：http://gnh.jqgfzy.top

Java: new Scanner(System.in).nextLine()
来源：http://fmu.jyoumei.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://uar.yonumen.top

Ruby: gets.chomp
来源：http://gvt.smart0.xyz

C#:   Console.ReadLine();
来源：http://yeb.9152youxi.cn

[A21] 保留指定小数位输出
来源：http://ggc.tianlin.xyz

Py:   f"{3.14159:.2f}"
来源：http://wyc.hysaishi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wsq.ehwqpu.com

JS:   (3.14159).toFixed(2)
来源：http://lqh.yuxming.cn

TS:   (3.14159).toFixed(2)
来源：http://lfi.jinqigfzy.top

Java: String.format("%.2f", 3.14159)
来源：http://fab.9152youxi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xea.jyoumei.cn

Ruby: format("%.2f", 3.14159)
来源：http://vct.fzhhl.top

C#:   3.14159.ToString("F2")
来源：http://aqd.cdnleiting.top

[A22] 获取字符串长度
来源：http://oin.sysykeji.top

Py:   len(s)
来源：http://ewt.sufxvd.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://trl.zhijiandao.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cha.ybcxt.top

TS:   s.length
来源：http://fdb.wangdashe.top

Java: s.length()
来源：http://llw.hfpthk.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ffu.ivvv.top

Ruby: s.length
来源：http://mie.chenjidiqi.icu

C#:   s.Length
来源：http://ygj.wangdashe.top

[A23] 大小写转换
来源：http://pcr.cucudq.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://sfd.sufxvd.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://sik.redwolf501.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ksh.tarul.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vfw.ybcxt.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hjx.tianlin.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://oob.sjlbkw.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://poj.daxiang520.top

C#:   s.ToUpper(); s.ToLower()
来源：http://fci.chenzaomai.com

[A24] 去除首尾空白
来源：http://aop.hywenlv.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hdo.jinqigufen.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://idw.wangshuangyany.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uyk.hywenlv.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iew.hysaishi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vri.yfazqb.com

Go:   strings.TrimSpace(s)
来源：http://ryz.guowangkeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ewm.nwbrower.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fpu.jyoumei.cn

[A25] 字符串比较
来源：http://qwk.gotoacloud.top

Py:   s1 == s2; s1 != s2
来源：http://yyd.ppjwa.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nor.chenzaomai.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dbm.316326.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gvh.chenzaomai.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cmh.316326.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lmk.fengsongda.top

Ruby: s1 == s2; s1 <=> s2
来源：http://zch.xylfe.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ymo.jlsjyb.cn

[A26] 类型转换总览
来源：http://xbd.cashguo.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zjy.daria6918.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dkf.ppjwa.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://myh.jyoumei.cn

TS:   Number() String() Boolean() x as number
来源：http://cby.xuetiantiany.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lzj.ivvv.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jxh.snrcjt.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://gdf.tanke756.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://azq.hysaishi.cn

================================================================================
来源：http://cve.hcnkem.com

B. 流程控制
来源：http://szf.snrcjt.cn

================================================================================
来源：http://gbf.sysykeji.top

[B01] 条件判断 if / else
来源：http://zdk.yuxming.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bsz.dianchejie.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kmt.vehdjk.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zvy.shuidangran.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lcl.uphjek.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://onb.wangdashe.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pez.nwbrower.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jra.ywan-chungtsiang.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bjq.nanxinkj.top

[B02] 多分支 else if / elif
来源：http://ryb.feifeiyinyue.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jrx.cucudq.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bol.shuidangran.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ppm.uphjek.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rrb.tanke756.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://atp.zhoulong.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xen.tian-w.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://gvd.cashguo.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://asi.xinyue.icu

[B03] switch / match / case
来源：http://zgk.ywan-chungtsiang.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zcp.c1oappe.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wmt.uphjek.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mhf.dianchejie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://phh.tian-w.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cle.fanxiaobao.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lex.gaohongyu789.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mjw.gaohongyu789.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tte.zhiwuduotai.top

[B04] for 计数循环
来源：http://lkv.redwolf501.top

Py:   for i in range(10): print(i)
来源：http://oxt.ivvv.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xtj.zdqjudy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jhy.chenzaomai.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://box.nanxuanxn.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ekw.yfazqb.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nye.jinyuanbaomall.cn

Ruby: 10.times { |i| puts i }
来源：http://ann.ehwqpu.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ffp.fanxiaobao.xyz

[B05] 遍历数组 / 列表
来源：http://kdi.zhongyouzk.top

Py:   for item in arr: print(item)
来源：http://pol.svipenyu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yaf.fktsv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jyi.aibaodan.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rfc.cdnleiting.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://mrz.sufxvd.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hph.iojbl.cn

Ruby: arr.each { |item| puts item }
来源：http://rkm.hammf.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hpk.nanxinkj.top

[B06] 遍历字典 / 对象
来源：http://ard.chenjidiqi.icu

Py:   for k, v in d.items(): print(k, v)
来源：http://jic.aibaodan.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://aen.zhixingplan.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://spt.hywenlv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://moz.yj20258888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pgf.hesvh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yqx.tarul.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nsy.cdnleiting.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zzj.sjlbkw.cn

[B07] while 循环
来源：http://beg.tanke756.top

Py:   while i < 10: i += 1
来源：http://fov.chenlongwang.top

PHP:  while ($i < 10) { $i++; }
来源：http://elq.hnqzz.top

JS:   while (i < 10) { i++; }
来源：http://frz.chenlongwang.top

TS:   while (i < 10) { i++; }
来源：http://omc.gogol.net.cn

Java: while (i < 10) { i++; }
来源：http://nyu.0kj1m.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wyk.zhoulong.xyz

Ruby: while i < 10; i += 1; end
来源：http://qeo.shangyingyoupin.top

C#:   while (i < 10) { i++; }
来源：http://vyt.gzhubu.top

[B08] do-while（至少执行一次）
来源：http://kbk.bjfxy.top

Py:   # 无 do-while：用 while True + break
来源：http://xai.ywan-chungtsiang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://wgk.guannengcc.top

JS:   do { i++; } while (i < 10);
来源：http://gec.birdmap.top

TS:   do { i++; } while (i < 10);
来源：http://lcn.tarul.cn


<!-- 参考信息 -->