代发 wailian999

Py:   print("Hello, World!")
来源：http://bxy.daxiang520.top

PHP:  echo "Hello, World!";
来源：http://nxj.yuxming.cn

JS:   console.log("Hello, World!");
来源：http://vbt.ehwqpu.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yiu.fzhhl.top

Java: System.out.println("Hello, World!");
来源：http://whv.vqdsnc.cn

Go:   fmt.Println("Hello, World!")
来源：http://atl.jyoumei.cn

Ruby: puts "Hello, World!"
来源：http://pgo.yfazqb.com

C#:   Console.WriteLine("Hello, World!");
来源：http://yyc.andypj.xyz

[A02] 变量声明与赋值
来源：http://abv.fanxiaobao.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ccr.zhijiandao.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://asz.zhaomingkeji.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://wob.nwbrower.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jss.hywenlv.cn

Java: String name = "Alex"; int age = 20;
来源：http://ypo.aibaodan.cn

Go:   name := "Alex"; age := 20
来源：http://qou.fehbvm.com

Ruby: name = "Alex"; age = 20
来源：http://mit.uphjek.com

C#:   string name = "Alex"; int age = 20;
来源：http://qbb.yuanzhike.top

[A03] 常量定义
来源：http://clx.andypj.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rtm.bbcook.cn

PHP:  const PI = 3.14159;
来源：http://iku.shzxlz.cn

JS:   const PI = 3.14159;
来源：http://mmp.nanxinkj.top

TS:   const PI: number = 3.14159;
来源：http://xjz.wangdashe.top

Java: static final double PI = 3.14159;
来源：http://tul.yangfankeji.com

Go:   const PI = 3.14159
来源：http://qwo.andypj.xyz

Ruby: PI = 3.14159
来源：http://hky.iojbl.cn

C#:   const double PI = 3.14159;
来源：http://fuk.zhengqikj.top

[A04] 判断变量类型
来源：http://ynw.jianghu66.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://qpw.xuetiantiany.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wtn.zhengqikj.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xbs.gogol.net.cn

TS:   typeof x; x instanceof Date
来源：http://jxf.yj202588.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lcd.0kj1m.cn

Go:   reflect.TypeOf(x).Name()
来源：http://iyf.daxiang520.top

Ruby: x.class; x.is_a?(Integer)
来源：http://xup.tianlin.xyz

C#:   x.GetType().Name; x is int
来源：http://duy.ehwqpu.com

[A05] 整数除法与取模
来源：http://ydt.andypj.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tyj.52xcode.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://pcx.jyoumei.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://irb.ybcxt.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://upz.xinyue.icu

Java: 7 / 2; 7 % 2
来源：http://dza.hcnkem.com

Go:   7 / 2; 7 % 2
来源：http://cit.cashguo.top

Ruby: 7 / 2; 7 % 2
来源：http://amv.jqgufenzy.top

C#:   7 / 2; 7 % 2
来源：http://zem.haohaochexian.top

[A06] 字符串转数字
来源：http://dby.cqqwz.cn

Py:   int("42"); float("3.14")
来源：http://zxd.zhongyouzk.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kbz.fanxiaobao.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://apt.jinyuanbaomall.cn

TS:   parseInt("42", 10); Number("42")
来源：http://pnx.ydjk.org.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pkb.kuanghao11.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ogc.chenzaomai.com

Ruby: "42".to_i; "3.14".to_f
来源：http://cms.yanxiufei.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://exr.jinqigfzy.top

[A07] 数字转字符串
来源：http://lji.yanxiufei.cn

Py:   str(42)
来源：http://uyr.yangfankeji.com

PHP:  (string) 42; strval(42)
来源：http://zrl.cdnleiting.top

JS:   String(42); (42).toString()
来源：http://hck.cheryme.top

TS:   String(42)
来源：http://zyw.cdnleiting.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://udk.fengsongda.top

Go:   strconv.Itoa(42)
来源：http://tul.feifeiyinyue.top

Ruby: 42.to_s
来源：http://olr.cqqwz.cn

C#:   42.ToString()
来源：http://eaj.shanyushiyangtech.top

[A08] 取整与四舍五入
来源：http://rwj.bjfxy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://spi.yj202588.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://exz.aizwys.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cco.sweek.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hzh.pengpengdd.cyou

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xjh.zhijiandao.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://maz.nanxuanxn.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://bez.chenzaomai.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zej.cqqwz.cn

[A09] 绝对值与最大最小值
来源：http://vfy.sysykeji.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ags.ydzc1.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wea.yvedp.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vdb.tianlin.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yxj.hysaishi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dzc.zhoulong.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mbg.nanxuanxn.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://eor.xuetiantiany.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://doo.hesvh.cn

[A10] 生成随机数
来源：http://zts.hongshengwenyu.top

Py:   import random; random.randint(1, 100)
来源：http://vsp.tian-w.cn

PHP:  random_int(1, 100);
来源：http://jro.yuxming.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ocw.9152youxi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://khe.chenjidiqi.icu

Java: new Random().nextInt(100) + 1
来源：http://fww.feifeiyinyue.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qal.jinyuanbaomall.cn

Ruby: rand(1..100)
来源：http://hcv.tanke756.top

C#:   new Random().Next(1, 101)
来源：http://wgr.zdqjudy.top

[A11] 条件表达式（三元）
来源：http://shv.chenzaomai.com

Py:   "yes" if x > 0 else "no"
来源：http://xcg.9152youxi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://gzs.hfpthk.cn

JS:   x > 0 ? "yes" : "no"
来源：http://yqn.hammf.cn

TS:   x > 0 ? "yes" : "no"
来源：http://naw.xinyue.icu

Java: x > 0 ? "yes" : "no"
来源：http://hft.shangyingyoupin.top

Go:   // 无三元运算符，需用 if 语句
来源：http://qto.pycfn.com

Ruby: x > 0 ? "yes" : "no"
来源：http://luy.ybcxt.top

C#:   x > 0 ? "yes" : "no"
来源：http://hhf.uphjek.com

[A12] 字符串插值 / 格式化
来源：http://nps.zdbjq.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tzy.redwolf501.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xjp.tanke756.top

JS:   `Hello, ${name}!`
来源：http://dnx.birdmap.top

TS:   `Hello, ${name}!`
来源：http://alt.cashguo.top

Java: "Hello, %s!".formatted(name)
来源：http://btf.bbcook.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yit.vehdjk.com

Ruby: "Hello, #{name}!"
来源：http://hqe.shanyushiyangkeji.top

C#:   $"Hello, {name}!"
来源：http://wsx.yj202588.top

[A13] 多行字符串（练习 \n 转义）
来源：http://aod.haohaochexian.top

Py:   "第一行\n第二行"
来源：http://zfk.316326.xyz

PHP:  "第一行\n第二行"
来源：http://ikh.jiagoushi.top

JS:   "第一行\n第二行"
来源：http://anc.svipenyu.cn

TS:   "第一行\n第二行"
来源：http://nza.aibaodan.cn

Java: "第一行\n第二行"
来源：http://kzc.zhijiandao.cn

Go:   "第一行\n第二行"
来源：http://pxk.jiagoushi.top

Ruby: "第一行\n第二行"
来源：http://qxr.vehdjk.com

C#:   "第一行\n第二行"
来源：http://aaw.jlsjyb.cn

[A14] 注释写法
来源：http://enb.ydjk.org.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://zvf.yj202588.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://wkc.meibo888.top

JS:   // 单行；/* 多行 */
来源：http://foe.zhengqikj.top

TS:   // 单行；/* 多行 */
来源：http://aka.sufxvd.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://auv.hnqzz.top

Go:   // 单行；/* 多行 */
来源：http://mbd.shanyushiyangtech.top

Ruby: # 单行；=begin 多行 =end
来源：http://sjv.gaohongyu789.top

C#:   // 单行；/* 多行 */
来源：http://een.gaohongyu789.top

[A15] 空值判断与默认值
来源：http://llz.jiagoushi.top

Py:   value = data or "默认值"
来源：http://pio.dashuyun.cn

PHP:  $value = $data ?? "默认值";
来源：http://gjj.jyoumei.cn

JS:   const value = data ?? "默认值";
来源：http://uef.shzxlz.cn

TS:   const value = data ?? "默认值";
来源：http://awt.sweek.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://osg.snrcjt.cn

Go:   if data == "" { data = "默认值" }
来源：http://xji.shzxlz.cn

Ruby: value = data || "默认值"
来源：http://jux.fehbvm.com

C#:   var value = data ?? "默认值";
来源：http://bit.birdmap.top

[A16] 真假值判断规则
来源：http://orq.yvedp.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nzm.gzhubu.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vmz.ywan-chungtsiang.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://who.hammf.cn

TS:   if (!x) {}
来源：http://scq.9152youxi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mxi.sjlbkw.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hfp.chenzaomai.com

Ruby: unless x            # nil 与 false 为假
来源：http://xog.ywan-chungtsiang.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://div.fanxiaobao.xyz

[A17] 位运算
来源：http://lfd.sjlbkw.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xkg.gzhubu.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ndo.zdqjudy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://seo.cqqwz.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vwy.nanxuanxn.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mgu.quarkkingdee.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tdn.9152youxi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://txy.feifeiyinyue.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://akk.dashuyun.cn

[A18] 字符与 ASCII 码互转
来源：http://laf.sweek.top

Py:   ord("A"); chr(65)
来源：http://pta.nanxinkj.top

PHP:  ord("A"); chr(65)
来源：http://uti.aizwys.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wax.zhiwuduotai.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ijh.snrcjt.cn

Java: (int) 'A'; (char) 65
来源：http://qzu.guannengcc.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ebj.pengpengdd.cyou

Ruby: "A".ord; 65.chr
来源：http://ftd.daria6918.cn

C#:   (int)'A'; (char)65
来源：http://ulm.sxryk.cn

[A19] 交换两个变量
来源：http://itm.jinqigfzy.top

Py:   a, b = b, a
来源：http://yqw.zdqjudy.top

PHP:  [$a, $b] = [$b, $a];
来源：http://hkt.haohaochexian.top

JS:   [a, b] = [b, a];
来源：http://gjd.zhongyouzk.top

TS:   [a, b] = [b, a];
来源：http://tss.cqqwz.cn

Java: int t = a; a = b; b = t;
来源：http://tbi.gogol.net.cn

Go:   a, b = b, a
来源：http://opv.dianchejie.cn

Ruby: a, b = b, a
来源：http://jeo.yonumen.top

C#:   (a, b) = (b, a);
来源：http://som.shzxlz.cn

[A20] 读取标准输入
来源：http://bjr.hcnkem.com

Py:   name = input("请输入：")
来源：http://bna.shanyushiyangtech.top

PHP:  $name = trim(fgets(STDIN));
来源：http://sqs.tian-w.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mel.yj202588.top

TS:   // Node.js：readline 模块
来源：http://rwm.gzhubu.top

Java: new Scanner(System.in).nextLine()
来源：http://yvl.jiagoushi.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kmz.yfazqb.com

Ruby: gets.chomp
来源：http://cyj.zhaomingkeji.xyz

C#:   Console.ReadLine();
来源：http://msr.hfpthk.cn

[A21] 保留指定小数位输出
来源：http://iru.quarkkingdee.top

Py:   f"{3.14159:.2f}"
来源：http://ytm.hcnkem.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jcb.daria6918.cn

JS:   (3.14159).toFixed(2)
来源：http://qxe.ywan-chungtsiang.top

TS:   (3.14159).toFixed(2)
来源：http://vrn.smart0.xyz

Java: String.format("%.2f", 3.14159)
来源：http://ufj.dashuyun.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://agp.zycfv.cn

Ruby: format("%.2f", 3.14159)
来源：http://sxm.zhijiandao.cn

C#:   3.14159.ToString("F2")
来源：http://vjk.vehdjk.com

[A22] 获取字符串长度
来源：http://adm.hysaishi.cn

Py:   len(s)
来源：http://pak.ydzc1.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ivb.yueranfly.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://twm.zhaomingkeji.xyz

TS:   s.length
来源：http://eqm.yueranfly.top

Java: s.length()
来源：http://fpv.ehwqpu.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mgd.hywenlv.cn

Ruby: s.length
来源：http://zdx.cheryme.top

C#:   s.Length
来源：http://und.ivvv.top

[A23] 大小写转换
来源：http://ajg.nanxinkj.top

Py:   s.upper(); s.lower(); s.title()
来源：http://bzq.chenzaomai.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://sxw.wangshuangyany.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jxt.jqgufenzy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hms.xuetiantiany.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pmm.tarul.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://psd.316326.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dxw.gotoacloud.top

C#:   s.ToUpper(); s.ToLower()
来源：http://htc.feifeiyinyue.top

[A24] 去除首尾空白
来源：http://zre.zhaomingkeji.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qpc.dashuyun.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://msb.hysaishi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://czs.cdnleiting.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cvu.aibaodan.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://upr.ydzc1.top

Go:   strings.TrimSpace(s)
来源：http://lby.xylfe.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hvw.9152youxi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yuf.hnqzz.top

[A25] 字符串比较
来源：http://bmy.xingfuxueyuan.xyz

Py:   s1 == s2; s1 != s2
来源：http://bza.haohaochexian.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kbk.bjfxy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pbj.yueranfly.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xjq.xuetiantiany.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tbt.gotoacloud.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bqs.9152youxi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zio.gzhubu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ayh.zhiwuduotai.top

[A26] 类型转换总览
来源：http://hgb.zhijiandao.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lyp.cucudq.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ftc.meibo888.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xyj.meibo888.top

TS:   Number() String() Boolean() x as number
来源：http://ltg.meibo888.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nwx.zycfv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lko.hongshengwenyu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://rsp.chenlongwang.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cti.fanxiaobao.xyz

================================================================================
来源：http://qve.fehbvm.com

B. 流程控制
来源：http://jhj.aibaodan.cn

================================================================================
来源：http://xli.tarul.cn

[B01] 条件判断 if / else
来源：http://zgn.uphjek.com

Py:   result = "正" if x > 0 else "非正"
来源：http://twc.fengsongda.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vlo.shuidangran.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pmf.hnxiangtu.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://png.birdmap.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://afe.pycfn.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gvb.hcnkem.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dgb.jianghu66.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://buh.dashuyun.cn

[B02] 多分支 else if / elif
来源：http://isw.gaohongyu789.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zgs.yangfankeji.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ltl.9152youxi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nni.meibo888.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tho.pycfn.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vef.fanxiaobao.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ots.jlsjyb.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ecs.jiagoushi.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cwm.316326.xyz

[B03] switch / match / case
来源：http://bfy.yj202588.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ihg.jyoumei.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tio.316326.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dsi.birdmap.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uth.aizwys.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vpi.fengsongda.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mzu.chenzaomai.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mtr.ppjwa.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kwq.chenjidiqi.icu

[B04] for 计数循环
来源：http://tzl.vqdsnc.cn

Py:   for i in range(10): print(i)
来源：http://sxe.pycfn.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hkp.ybcxt.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sce.ivvv.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kpx.hesvh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yyy.yonumen.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ade.vehdjk.com

Ruby: 10.times { |i| puts i }
来源：http://bum.0kj1m.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wmv.52xcode.cn

[B05] 遍历数组 / 列表
来源：http://wzp.yonumen.top

Py:   for item in arr: print(item)
来源：http://qbe.cheryme.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dhi.meibo888.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ebi.gogol.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://csl.xuetiantiany.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ycb.zhengqikj.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ewu.quarkkingdee.top

Ruby: arr.each { |item| puts item }
来源：http://bem.yuanzhike.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hqv.tian-w.cn

[B06] 遍历字典 / 对象
来源：http://jwf.hnxiangtu.top

Py:   for k, v in d.items(): print(k, v)
来源：http://tck.tarul.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bal.hywenlv.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kde.xuetiantiany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://osa.zhoulong.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cvi.guowangkeji.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sqr.xuetiantiany.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://trj.yangfankeji.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zjp.gotoacloud.top

[B07] while 循环
来源：http://ywx.jinghuilouyu.cn

Py:   while i < 10: i += 1
来源：http://ppz.sufxvd.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bps.yanxiufei.cn

JS:   while (i < 10) { i++; }
来源：http://xba.hfpthk.cn

TS:   while (i < 10) { i++; }
来源：http://iob.hywenlv.cn

Java: while (i < 10) { i++; }
来源：http://ppy.bbcook.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cxo.fengsongda.top

Ruby: while i < 10; i += 1; end
来源：http://apo.hywenlv.cn

C#:   while (i < 10) { i++; }
来源：http://zgy.fengsongda.top

[B08] do-while（至少执行一次）
来源：http://azj.tianlin.xyz


<!-- 参考信息 -->