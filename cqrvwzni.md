代发 wailian999

[A02] 变量声明与赋值
来源：http://iwm.zhoulong.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rww.yfazqb.com

PHP:  $name = "Alex"; $age = 20;
来源：http://tri.bjfxy.top

JS:   let name = "Alex"; const age = 20;
来源：http://wlx.ivvv.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mgy.wangshuangyany.cn

Java: String name = "Alex"; int age = 20;
来源：http://mrq.dashuyun.cn

Go:   name := "Alex"; age := 20
来源：http://qqn.andypj.xyz

Ruby: name = "Alex"; age = 20
来源：http://tom.yj20258.top

C#:   string name = "Alex"; int age = 20;
来源：http://vwb.svipenyu.cn

[A03] 常量定义
来源：http://cgv.yuanzhike.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zrw.vqdsnc.cn

PHP:  const PI = 3.14159;
来源：http://equ.nanxuanxn.top

JS:   const PI = 3.14159;
来源：http://tdf.fehbvm.com

TS:   const PI: number = 3.14159;
来源：http://kpi.yanxiufei.cn

Java: static final double PI = 3.14159;
来源：http://fby.jinyuanbaomall.cn

Go:   const PI = 3.14159
来源：http://tpr.cqqwz.cn

Ruby: PI = 3.14159
来源：http://gqv.jinghuilouyu.cn

C#:   const double PI = 3.14159;
来源：http://lfu.yanxiufei.cn

[A04] 判断变量类型
来源：http://ome.hongshengwenyu.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://jvy.ctjpmb.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rmn.sufxvd.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ods.jinqigfzy.top

TS:   typeof x; x instanceof Date
来源：http://pbg.meibo888.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ilb.hnxiangtu.top

Go:   reflect.TypeOf(x).Name()
来源：http://aqr.jinqigfzy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://eze.hfpthk.cn

C#:   x.GetType().Name; x is int
来源：http://bdg.52xcode.cn

[A05] 整数除法与取模
来源：http://wnv.xinyue.icu

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yhf.hnqzz.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://syu.jqgfzy.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://frw.tianlin.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://iiq.jiagoushi.top

Java: 7 / 2; 7 % 2
来源：http://jyw.iojbl.cn

Go:   7 / 2; 7 % 2
来源：http://xug.yueranfly.top

Ruby: 7 / 2; 7 % 2
来源：http://wth.gotoacloud.top

C#:   7 / 2; 7 % 2
来源：http://sjz.52xcode.cn

[A06] 字符串转数字
来源：http://oyk.ivvv.top

Py:   int("42"); float("3.14")
来源：http://xzw.jyoumei.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jtk.cheryme.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hbw.cucudq.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qxs.yanxiufei.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lho.dianchejie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://maz.fzhhl.top

Ruby: "42".to_i; "3.14".to_f
来源：http://rhh.feifeiyinyue.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fff.hongshengwenyu.top

[A07] 数字转字符串
来源：http://hzh.jiagoushi.top

Py:   str(42)
来源：http://xve.zhixingplan.top

PHP:  (string) 42; strval(42)
来源：http://rgo.316326.xyz

JS:   String(42); (42).toString()
来源：http://did.ivvv.top

TS:   String(42)
来源：http://gka.shangyingyoupin.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://bvx.tanke756.top

Go:   strconv.Itoa(42)
来源：http://tos.wangshuangyany.cn

Ruby: 42.to_s
来源：http://dbx.guannengcc.top

C#:   42.ToString()
来源：http://gfp.xylfe.cn

[A08] 取整与四舍五入
来源：http://lof.yanxiufei.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wep.ehwqpu.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xih.tian-w.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://teb.zhongyouzk.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wxv.ppjwa.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://smn.daria6918.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mnl.zycfv.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://vdo.tianlin.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ool.bbcook.cn

[A09] 绝对值与最大最小值
来源：http://cly.cucudq.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dbv.tian-w.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://agv.sjlbkw.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fnf.hnxiangtu.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lkm.zdqjudy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rpd.shuidangran.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wee.cheryme.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zwm.yueranfly.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://yhz.cashguo.top

[A10] 生成随机数
来源：http://bfs.tarul.cn

Py:   import random; random.randint(1, 100)
来源：http://oqo.yuanzhike.top

PHP:  random_int(1, 100);
来源：http://nlo.jinqigfzy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xyp.feifeiyinyue.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://evq.sufxvd.cn

Java: new Random().nextInt(100) + 1
来源：http://yaq.nanxuanxn.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://nxd.sjlbkw.cn

Ruby: rand(1..100)
来源：http://vdj.yanxiufei.cn

C#:   new Random().Next(1, 101)
来源：http://bqi.ppjwa.cn

[A11] 条件表达式（三元）
来源：http://yui.jinyuanbaomall.cn

Py:   "yes" if x > 0 else "no"
来源：http://voe.yuanzhike.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ykn.quarkkingdee.top

JS:   x > 0 ? "yes" : "no"
来源：http://opy.fanxiaobao.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://nue.xylfe.cn

Java: x > 0 ? "yes" : "no"
来源：http://rec.jyoumei.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://zqn.nanxuanxn.top

Ruby: x > 0 ? "yes" : "no"
来源：http://fvv.redwolf501.top

C#:   x > 0 ? "yes" : "no"
来源：http://cax.pengpengdd.cyou

[A12] 字符串插值 / 格式化
来源：http://hcv.hcnkem.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wft.jlsjyb.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://aov.havefunace.top

JS:   `Hello, ${name}!`
来源：http://nkd.iojbl.cn

TS:   `Hello, ${name}!`
来源：http://efb.shzxlz.cn

Java: "Hello, %s!".formatted(name)
来源：http://oxp.hnxiangtu.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gtn.sysykeji.top

Ruby: "Hello, #{name}!"
来源：http://gcy.epnwcf.com

C#:   $"Hello, {name}!"
来源：http://mso.wangshuangyany.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://dkr.andypj.xyz

Py:   "第一行\n第二行"
来源：http://rzo.yueranfly.top

PHP:  "第一行\n第二行"
来源：http://boj.pengpengdd.cyou

JS:   "第一行\n第二行"
来源：http://gzd.kuanghao11.cn

TS:   "第一行\n第二行"
来源：http://ggl.fanxiaobao.xyz

Java: "第一行\n第二行"
来源：http://vyg.fengsongda.top

Go:   "第一行\n第二行"
来源：http://pwz.nanxuanxn.top

Ruby: "第一行\n第二行"
来源：http://axr.mhx1999.top

C#:   "第一行\n第二行"
来源：http://vgr.uphjek.com

[A14] 注释写法
来源：http://wcz.hammf.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://jkl.yangfankeji.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://lbi.ydzc1.top

JS:   // 单行；/* 多行 */
来源：http://ifv.nanxuanxn.top

TS:   // 单行；/* 多行 */
来源：http://inc.zdqjudy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mdz.gaohongyu789.top

Go:   // 单行；/* 多行 */
来源：http://ojw.ehwqpu.com

Ruby: # 单行；=begin 多行 =end
来源：http://hci.shangyingyoupin.top

C#:   // 单行；/* 多行 */
来源：http://zvi.jinqigfzy.top

[A15] 空值判断与默认值
来源：http://zei.jinqigfzy.top

Py:   value = data or "默认值"
来源：http://riw.fzhhl.top

PHP:  $value = $data ?? "默认值";
来源：http://gxi.tanke756.top

JS:   const value = data ?? "默认值";
来源：http://ege.guannengcc.top

TS:   const value = data ?? "默认值";
来源：http://ury.pycfn.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wlg.yvedp.cn

Go:   if data == "" { data = "默认值" }
来源：http://eaq.zdbjq.cn

Ruby: value = data || "默认值"
来源：http://bck.zhiwuduotai.top

C#:   var value = data ?? "默认值";
来源：http://ztb.shzxlz.cn

[A16] 真假值判断规则
来源：http://lja.yonumen.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dbp.ivvv.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ybd.guowangkeji.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qgp.nanxinkj.top

TS:   if (!x) {}
来源：http://oll.yfazqb.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bjn.smart0.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rxc.zdqjudy.top

Ruby: unless x            # nil 与 false 为假
来源：http://sun.tian-w.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bfm.gotoacloud.top

[A17] 位运算
来源：http://cod.zhijiandao.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yjv.birdmap.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://afj.fanxiaobao.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xmw.andypj.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wcx.jqgfzy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kog.hammf.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zar.gotoacloud.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ync.zdqjudy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rre.sweek.top

[A18] 字符与 ASCII 码互转
来源：http://urc.feifeiyinyue.top

Py:   ord("A"); chr(65)
来源：http://ztt.9152youxi.cn

PHP:  ord("A"); chr(65)
来源：http://kcp.smart0.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://axs.zhaomingkeji.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ifq.zhongyouzk.top

Java: (int) 'A'; (char) 65
来源：http://wbq.zhengqikj.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://sfs.hysaishi.cn

Ruby: "A".ord; 65.chr
来源：http://tvi.nanxinkj.top

C#:   (int)'A'; (char)65
来源：http://jnf.316326.xyz

[A19] 交换两个变量
来源：http://uow.guowangkeji.top

Py:   a, b = b, a
来源：http://ojk.xuetiantiany.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://mxd.zdqjudy.top

JS:   [a, b] = [b, a];
来源：http://liv.zhoulong.xyz

TS:   [a, b] = [b, a];
来源：http://utt.zhixingplan.top

Java: int t = a; a = b; b = t;
来源：http://ddm.shangyingyoupin.top

Go:   a, b = b, a
来源：http://ahw.shzxlz.cn

Ruby: a, b = b, a
来源：http://vhu.zycfv.cn

C#:   (a, b) = (b, a);
来源：http://ctj.jyoumei.cn

[A20] 读取标准输入
来源：http://kkp.fanxiaobao.xyz

Py:   name = input("请输入：")
来源：http://wix.0kj1m.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xzv.dianchejie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://amn.yj202588.top

TS:   // Node.js：readline 模块
来源：http://hmk.cqqwz.cn

Java: new Scanner(System.in).nextLine()
来源：http://hqp.bjfxy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rbc.tanke756.top

Ruby: gets.chomp
来源：http://qlp.zhijiandao.cn

C#:   Console.ReadLine();
来源：http://gwx.xuanzx.com

[A21] 保留指定小数位输出
来源：http://qnn.quarkkingdee.top

Py:   f"{3.14159:.2f}"
来源：http://uvh.sufxvd.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cis.haohaochexian.top

JS:   (3.14159).toFixed(2)
来源：http://vba.vehdjk.com

TS:   (3.14159).toFixed(2)
来源：http://xhc.zdbjq.cn

Java: String.format("%.2f", 3.14159)
来源：http://ihr.yj20258888.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://cdk.nanxuanxn.top

Ruby: format("%.2f", 3.14159)
来源：http://ipv.ppjwa.cn

C#:   3.14159.ToString("F2")
来源：http://pou.epnwcf.com

[A22] 获取字符串长度
来源：http://lnf.yueranfly.top

Py:   len(s)
来源：http://xbn.yanxiufei.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://plj.zhaomingkeji.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tgf.guowangkeji.top

TS:   s.length
来源：http://hel.jqgufenzy.top

Java: s.length()
来源：http://bjj.shangyingyoupin.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ala.zhaomingkeji.xyz

Ruby: s.length
来源：http://zuz.uphjek.com

C#:   s.Length
来源：http://ruj.shzxlz.cn

[A23] 大小写转换
来源：http://njf.vehdjk.com

Py:   s.upper(); s.lower(); s.title()
来源：http://wgb.yonumen.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qng.bjfxy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zkd.zhoulong.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bxc.andypj.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xgu.fzhhl.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://oru.yfazqb.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://itw.sweek.top

C#:   s.ToUpper(); s.ToLower()
来源：http://zsc.shuidangran.top

[A24] 去除首尾空白
来源：http://amc.shuidangran.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dxw.shanyushiyangkeji.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xad.zdqjudy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mfl.ydjk.org.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://svj.hfpthk.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pts.hnqzz.top

Go:   strings.TrimSpace(s)
来源：http://qhz.zhongyouzk.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bhl.xingfuxueyuan.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gse.haohaochexian.top

[A25] 字符串比较
来源：http://gbw.daria6918.cn

Py:   s1 == s2; s1 != s2
来源：http://mxc.hesvh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mso.yvedp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kqq.smart0.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://srl.xziqi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yfd.jqgufenzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://anl.zdbjq.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://sho.pycfn.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://edg.mhx1999.top

[A26] 类型转换总览
来源：http://tlv.ywan-chungtsiang.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vhj.nanxuanxn.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wrm.daxiang520.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wno.hysaishi.cn

TS:   Number() String() Boolean() x as number
来源：http://ika.shzxlz.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mzx.tianlin.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ksl.fzhhl.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://mgn.cashguo.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kaw.sysykeji.top

================================================================================
来源：http://qbj.ppjwa.cn

B. 流程控制
来源：http://tfl.shanyushiyangkeji.top

================================================================================
来源：http://mlm.316326.xyz

[B01] 条件判断 if / else
来源：http://umj.ppjwa.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nlh.ctjpmb.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://feg.cdnleiting.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fjd.cqqwz.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gek.fzhhl.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://vvb.hammf.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gpf.316326.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pwu.smart0.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ffz.kuanghao11.cn

[B02] 多分支 else if / elif
来源：http://els.9152youxi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://adk.tian-w.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pge.sufxvd.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iqy.chenlongwang.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fip.hysaishi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hzm.yonumen.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ajv.9152youxi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://obz.vqdsnc.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rba.cashguo.top

[B03] switch / match / case
来源：http://qfl.zhaomingkeji.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://slk.jinqigfzy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jgu.cheryme.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qmg.pycfn.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rxd.daxiang520.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wvd.hnqzz.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pkq.guowangkeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kgx.9152youxi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zlc.ivvv.top

[B04] for 计数循环
来源：http://lga.cucudq.cn

Py:   for i in range(10): print(i)
来源：http://fhy.xinyue.icu

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://utr.yfazqb.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jkr.jinghuilouyu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bqr.yuxming.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cxv.wangshuangyany.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dku.zhixingplan.top

Ruby: 10.times { |i| puts i }
来源：http://vhp.ctjpmb.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sdl.jinqigfzy.top

[B05] 遍历数组 / 列表
来源：http://haf.snrcjt.cn

Py:   for item in arr: print(item)
来源：http://ycf.sufxvd.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://shp.xuetiantiany.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bfy.sweek.top

TS:   for (const item of arr) { console.log(item); }
来源：http://lvk.hcnkem.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://mpz.ppjwa.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dke.aizwys.cn

Ruby: arr.each { |item| puts item }
来源：http://ufd.yonumen.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ztx.shangyingyoupin.top

[B06] 遍历字典 / 对象
来源：http://hhp.hysaishi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gan.fktsv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://aks.pycfn.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://elq.gaohongyu789.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kri.snrcjt.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://iwi.sysykeji.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ykj.xinyue.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://aub.hesvh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rrj.fengsongda.top

[B07] while 循环
来源：http://bjp.shangyingyoupin.top

Py:   while i < 10: i += 1
来源：http://iga.shanyushiyangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://tnt.aizwys.cn

JS:   while (i < 10) { i++; }
来源：http://rcw.jyoumei.cn

TS:   while (i < 10) { i++; }
来源：http://tii.snrcjt.cn

Java: while (i < 10) { i++; }
来源：http://mbl.chenlongwang.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cac.zhoulong.xyz

Ruby: while i < 10; i += 1; end
来源：http://xhg.jyoumei.cn

C#:   while (i < 10) { i++; }
来源：http://zvb.chenzaomai.com

[B08] do-while（至少执行一次）
来源：http://xgd.yonumen.top

Py:   # 无 do-while：用 while True + break
来源：http://frl.havefunace.top

PHP:  do { $i++; } while ($i < 10);
来源：http://weq.hysaishi.cn

JS:   do { i++; } while (i < 10);
来源：http://ckt.wangshuangyany.cn

TS:   do { i++; } while (i < 10);
来源：http://iic.jinqigufen.top

Java: do { i++; } while (i < 10);
来源：http://uju.daxiang520.top

Go:   for { i++; if i >= 10 { break } }
来源：http://qsh.wangdashe.top

Ruby: begin; i += 1; end while i < 10
来源：http://mjn.jianghu66.top

C#:   do { i++; } while (i < 10);
来源：http://pot.andypj.xyz


<!-- 参考信息 -->