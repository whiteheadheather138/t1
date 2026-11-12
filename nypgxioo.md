代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://pcl.c1oappe.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lby.svipenyu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lbh.jinqigufen.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ivn.epnwcf.com

================================================================================
来源：http://uso.shuidangran.top

A. 基础语法与类型
来源：http://fsh.yj202588.top

================================================================================
来源：http://wyc.smart0.xyz

[A01] Hello World
来源：http://kpj.hesvh.cn

Py:   print("Hello, World!")
来源：http://pcp.hongshengwenyu.top

PHP:  echo "Hello, World!";
来源：http://kpg.yonumen.top

JS:   console.log("Hello, World!");
来源：http://ygf.sysykeji.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zgv.chenjidiqi.icu

Java: System.out.println("Hello, World!");
来源：http://vsi.shanyushiyangkeji.top

Go:   fmt.Println("Hello, World!")
来源：http://lgi.havefunace.top

Ruby: puts "Hello, World!"
来源：http://wjj.ivvv.top

C#:   Console.WriteLine("Hello, World!");
来源：http://seg.ppjwa.cn

[A02] 变量声明与赋值
来源：http://rds.jiagoushi.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kak.wangshuangyany.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ozz.jyoumei.cn

JS:   let name = "Alex"; const age = 20;
来源：http://lsj.ivvv.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://otb.zhiwuduotai.top

Java: String name = "Alex"; int age = 20;
来源：http://czs.zhongyouzk.top

Go:   name := "Alex"; age := 20
来源：http://pwk.sweek.top

Ruby: name = "Alex"; age = 20
来源：http://mmc.gotoacloud.top

C#:   string name = "Alex"; int age = 20;
来源：http://pgp.yongpay.top

[A03] 常量定义
来源：http://pyu.quarkkingdee.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pcn.ivvv.top

PHP:  const PI = 3.14159;
来源：http://sdr.yj20258888.top

JS:   const PI = 3.14159;
来源：http://jby.xuanzx.com

TS:   const PI: number = 3.14159;
来源：http://fqt.52xcode.cn

Java: static final double PI = 3.14159;
来源：http://zof.zhijiandao.cn

Go:   const PI = 3.14159
来源：http://ukn.aizwys.cn

Ruby: PI = 3.14159
来源：http://hrs.gogol.net.cn

C#:   const double PI = 3.14159;
来源：http://cma.chenjidiqi.icu

[A04] 判断变量类型
来源：http://cmo.dianchejie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ogr.epnwcf.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vdt.tanke756.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xqp.ctjpmb.com

TS:   typeof x; x instanceof Date
来源：http://jhd.yanxiufei.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mlf.birdmap.top

Go:   reflect.TypeOf(x).Name()
来源：http://gyk.yueranfly.top

Ruby: x.class; x.is_a?(Integer)
来源：http://lvz.tianlin.xyz

C#:   x.GetType().Name; x is int
来源：http://wfb.zdbjq.cn

[A05] 整数除法与取模
来源：http://ajf.cdnleiting.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jgm.yangfankeji.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://dhr.zhongyouzk.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jgf.jqgufenzy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xvw.havefunace.top

Java: 7 / 2; 7 % 2
来源：http://ufw.xylfe.cn

Go:   7 / 2; 7 % 2
来源：http://mjw.c1oappe.top

Ruby: 7 / 2; 7 % 2
来源：http://gsm.aibaodan.cn

C#:   7 / 2; 7 % 2
来源：http://hku.cqqwz.cn

[A06] 字符串转数字
来源：http://gsy.wangshuangyany.cn

Py:   int("42"); float("3.14")
来源：http://dwb.yueranfly.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bmh.fehbvm.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mwg.vqdsnc.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ivp.pycfn.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ejt.wangdashe.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rnc.yj20258.top

Ruby: "42".to_i; "3.14".to_f
来源：http://yzn.haohaochexian.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cdl.aizwys.cn

[A07] 数字转字符串
来源：http://ctg.mhx1999.top

Py:   str(42)
来源：http://kmy.ppjwa.cn

PHP:  (string) 42; strval(42)
来源：http://zcq.tian-w.cn

JS:   String(42); (42).toString()
来源：http://une.vqdsnc.cn

TS:   String(42)
来源：http://mky.aibaodan.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bqj.bbcook.cn

Go:   strconv.Itoa(42)
来源：http://pcl.9152youxi.cn

Ruby: 42.to_s
来源：http://gvx.zhaomingkeji.xyz

C#:   42.ToString()
来源：http://aum.guannengcc.top

[A08] 取整与四舍五入
来源：http://piw.bbcook.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://sdx.chenzaomai.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gsw.hywenlv.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vun.gotoacloud.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://smv.hnqzz.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fwh.sjlbkw.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qbu.hcnkem.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://dun.sweek.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fav.chenzaomai.com

[A09] 绝对值与最大最小值
来源：http://dlp.zdqjudy.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ehm.ydjk.org.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cqw.zhixingplan.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jpe.ctjpmb.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hnk.zdbjq.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://orq.havefunace.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ctp.zhengqikj.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kwv.hammf.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rml.316326.xyz

[A10] 生成随机数
来源：http://dlj.hnqzz.top

Py:   import random; random.randint(1, 100)
来源：http://lpb.cdnleiting.top

PHP:  random_int(1, 100);
来源：http://jcu.redwolf501.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cyt.cdnleiting.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://czn.fanxiaobao.xyz

Java: new Random().nextInt(100) + 1
来源：http://pay.yongpay.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rxg.yj202588.top

Ruby: rand(1..100)
来源：http://ncr.zhoulong.xyz

C#:   new Random().Next(1, 101)
来源：http://pxr.zhengqikj.top

[A11] 条件表达式（三元）
来源：http://pwz.fengsongda.top

Py:   "yes" if x > 0 else "no"
来源：http://xwo.fehbvm.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://wvm.hesvh.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vkn.zhoulong.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://ame.shzxlz.cn

Java: x > 0 ? "yes" : "no"
来源：http://eps.dashuyun.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://dfb.iojbl.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://smb.cheryme.top

C#:   x > 0 ? "yes" : "no"
来源：http://fkw.zhiwuduotai.top

[A12] 字符串插值 / 格式化
来源：http://ryr.birdmap.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://juh.jianghu66.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://epw.zhaomingkeji.xyz

JS:   `Hello, ${name}!`
来源：http://hym.dashuyun.cn

TS:   `Hello, ${name}!`
来源：http://uaf.zdbjq.cn

Java: "Hello, %s!".formatted(name)
来源：http://wvl.ehwqpu.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wlc.shanyushiyangtech.top

Ruby: "Hello, #{name}!"
来源：http://get.yangfankeji.com

C#:   $"Hello, {name}!"
来源：http://ckj.cdnleiting.top

[A13] 多行字符串（练习 \n 转义）
来源：http://zoo.hysaishi.cn

Py:   "第一行\n第二行"
来源：http://aqo.jlsjyb.cn

PHP:  "第一行\n第二行"
来源：http://vot.uphjek.com

JS:   "第一行\n第二行"
来源：http://adu.jqgfzy.top

TS:   "第一行\n第二行"
来源：http://ycf.ybcxt.top

Java: "第一行\n第二行"
来源：http://frj.hnxiangtu.top

Go:   "第一行\n第二行"
来源：http://ifx.tianlin.xyz

Ruby: "第一行\n第二行"
来源：http://dcf.wangshuangyany.cn

C#:   "第一行\n第二行"
来源：http://uez.smart0.xyz

[A14] 注释写法
来源：http://cki.gotoacloud.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://wya.cdnleiting.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://zzp.snrcjt.cn

JS:   // 单行；/* 多行 */
来源：http://yuo.iojbl.cn

TS:   // 单行；/* 多行 */
来源：http://vkn.sweek.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://phl.kuanghao11.cn

Go:   // 单行；/* 多行 */
来源：http://dyi.ppjwa.cn

Ruby: # 单行；=begin 多行 =end
来源：http://zbd.fanxiaobao.xyz

C#:   // 单行；/* 多行 */
来源：http://doi.havefunace.top

[A15] 空值判断与默认值
来源：http://zuw.jlsjyb.cn

Py:   value = data or "默认值"
来源：http://kpp.gaohongyu789.top

PHP:  $value = $data ?? "默认值";
来源：http://lfo.wangshuangyany.cn

JS:   const value = data ?? "默认值";
来源：http://eqk.xinyue.icu

TS:   const value = data ?? "默认值";
来源：http://qov.smart0.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://qjn.chenjidiqi.icu

Go:   if data == "" { data = "默认值" }
来源：http://zdv.zycfv.cn

Ruby: value = data || "默认值"
来源：http://xfm.cashguo.top

C#:   var value = data ?? "默认值";
来源：http://khq.cashguo.top

[A16] 真假值判断规则
来源：http://pqn.yonumen.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wcv.svipenyu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hrf.snrcjt.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://shs.0kj1m.cn

TS:   if (!x) {}
来源：http://tdd.yongpay.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jpe.snrcjt.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vkz.gaohongyu789.top

Ruby: unless x            # nil 与 false 为假
来源：http://iuw.bjfxy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wrx.meibo888.top

[A17] 位运算
来源：http://het.dashuyun.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kbo.pengpengdd.cyou

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://knv.jiagoushi.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://veq.gotoacloud.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ezt.hywenlv.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mtu.shanyushiyangkeji.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tkl.chenzaomai.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://opm.smart0.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vym.havefunace.top

[A18] 字符与 ASCII 码互转
来源：http://htp.hcnkem.com

Py:   ord("A"); chr(65)
来源：http://bzo.sxryk.cn

PHP:  ord("A"); chr(65)
来源：http://uco.fzhhl.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qqq.vqdsnc.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sun.yueranfly.top

Java: (int) 'A'; (char) 65
来源：http://fmq.zhaomingkeji.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hzx.aizwys.cn

Ruby: "A".ord; 65.chr
来源：http://oeq.andypj.xyz

C#:   (int)'A'; (char)65
来源：http://mll.meibo888.top

[A19] 交换两个变量
来源：http://vdw.fktsv.cn

Py:   a, b = b, a
来源：http://awn.yj20258.top

PHP:  [$a, $b] = [$b, $a];
来源：http://mjt.jinghuilouyu.cn

JS:   [a, b] = [b, a];
来源：http://ycm.hysaishi.cn

TS:   [a, b] = [b, a];
来源：http://lrd.chenzaomai.com

Java: int t = a; a = b; b = t;
来源：http://dfk.wangshuangyany.cn

Go:   a, b = b, a
来源：http://wls.mhx1999.top

Ruby: a, b = b, a
来源：http://lbq.fktsv.cn

C#:   (a, b) = (b, a);
来源：http://dxk.aizwys.cn

[A20] 读取标准输入
来源：http://kss.tian-w.cn

Py:   name = input("请输入：")
来源：http://plm.yfazqb.com

PHP:  $name = trim(fgets(STDIN));
来源：http://fkf.fzhhl.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rkr.fehbvm.com

TS:   // Node.js：readline 模块
来源：http://ijn.hesvh.cn

Java: new Scanner(System.in).nextLine()
来源：http://spx.ydzc1.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wic.yj20258.top

Ruby: gets.chomp
来源：http://hch.svipenyu.cn

C#:   Console.ReadLine();
来源：http://bsc.hywenlv.cn

[A21] 保留指定小数位输出
来源：http://dqu.fanxiaobao.xyz

Py:   f"{3.14159:.2f}"
来源：http://ddv.tian-w.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xhn.fengsongda.top

JS:   (3.14159).toFixed(2)
来源：http://ehq.tianlin.xyz

TS:   (3.14159).toFixed(2)
来源：http://ogt.nwbrower.top

Java: String.format("%.2f", 3.14159)
来源：http://xxm.shanyushiyangkeji.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nqp.yonumen.top

Ruby: format("%.2f", 3.14159)
来源：http://ohy.guannengcc.top

C#:   3.14159.ToString("F2")
来源：http://itx.cqqwz.cn

[A22] 获取字符串长度
来源：http://egg.gotoacloud.top

Py:   len(s)
来源：http://wre.chenlongwang.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://svt.0kj1m.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://did.vqdsnc.cn

TS:   s.length
来源：http://qno.vqdsnc.cn

Java: s.length()
来源：http://abj.tian-w.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uhj.zhongyouzk.top

Ruby: s.length
来源：http://cqy.wangdashe.top

C#:   s.Length
来源：http://zwp.zhijiandao.cn

[A23] 大小写转换
来源：http://rvb.kuanghao11.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://bgr.aibaodan.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qym.nwbrower.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ltw.tanke756.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xuy.aibaodan.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mxk.ywan-chungtsiang.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kpc.chenjidiqi.icu

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ooz.cucudq.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qpq.hnxiangtu.top

[A24] 去除首尾空白
来源：http://mme.zhoulong.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dju.zhixingplan.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tip.andypj.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ncr.sysykeji.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xqa.zhongyouzk.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qgz.ywan-chungtsiang.top

Go:   strings.TrimSpace(s)
来源：http://war.daria6918.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hsz.jinqigfzy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dar.zhaomingkeji.xyz

[A25] 字符串比较
来源：http://sqe.shuidangran.top

Py:   s1 == s2; s1 != s2
来源：http://mqp.fengsongda.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://olc.jiagoushi.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rox.yueranfly.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://uzn.jianghu66.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ojb.xuetiantiany.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wzf.wangdashe.top

Ruby: s1 == s2; s1 <=> s2
来源：http://lom.zhiwuduotai.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://onr.ivvv.top

[A26] 类型转换总览
来源：http://pzm.zycfv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bnm.hesvh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ygn.iojbl.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pmo.shangyingyoupin.top

TS:   Number() String() Boolean() x as number
来源：http://jpf.cucudq.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://oac.ybcxt.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rdh.vehdjk.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://bhx.shuidangran.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://peu.zhongyouzk.top

================================================================================
来源：http://xet.nanxuanxn.top

B. 流程控制
来源：http://sag.cashguo.top

================================================================================
来源：http://xwh.tanke756.top

[B01] 条件判断 if / else
来源：http://nhh.jlsjyb.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ynv.hongshengwenyu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kvd.cashguo.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xsz.pycfn.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dre.sufxvd.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zfu.fzhhl.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cix.ctjpmb.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qbm.xylfe.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pwe.jyoumei.cn

[B02] 多分支 else if / elif
来源：http://ldz.shuidangran.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lku.shuidangran.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://elg.yueranfly.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bus.yfazqb.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://msy.zhixingplan.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qfm.xuetiantiany.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nub.jinqigufen.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uwn.hongshengwenyu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hwo.jinghuilouyu.cn

[B03] switch / match / case
来源：http://jih.fengsongda.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dtr.sxryk.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://trn.gotoacloud.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mgs.jiagoushi.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fqi.hnqzz.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hzv.fanxiaobao.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qiz.daxiang520.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://snl.dianchejie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://juc.mhx1999.top

[B04] for 计数循环
来源：http://jci.jinqigfzy.top

Py:   for i in range(10): print(i)
来源：http://mti.hammf.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ooz.ywan-chungtsiang.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://alg.jianghu66.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mov.aibaodan.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://aru.ywan-chungtsiang.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sxb.yonumen.top

Ruby: 10.times { |i| puts i }
来源：http://oiz.shangyingyoupin.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://chx.cashguo.top

[B05] 遍历数组 / 列表
来源：http://pls.gotoacloud.top

Py:   for item in arr: print(item)
来源：http://ekm.yfazqb.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://irh.yuxming.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hxa.fzhhl.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ahz.zhijiandao.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yyo.xziqi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jae.ivvv.top

Ruby: arr.each { |item| puts item }
来源：http://tlq.sweek.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://okl.yanxiufei.cn

[B06] 遍历字典 / 对象
来源：http://djh.sjlbkw.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://oeb.yj20258888.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xya.jqgfzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kct.zdqjudy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lju.pycfn.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lgq.hywenlv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://shw.ywan-chungtsiang.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://oom.pengpengdd.cyou

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vgn.hywenlv.cn

[B07] while 循环
来源：http://tgs.wangdashe.top

Py:   while i < 10: i += 1
来源：http://sfi.yj20258.top


<!-- 参考信息 -->