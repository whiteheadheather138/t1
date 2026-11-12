代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://gpq.xylfe.cn

Go:   fmt.Println("Hello, World!")
来源：http://hxs.hesvh.cn

Ruby: puts "Hello, World!"
来源：http://nwb.jinghuilouyu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://chf.yuanzhike.top

[A02] 变量声明与赋值
来源：http://god.yj20258888.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ysd.snrcjt.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://udm.fanxiaobao.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://xhg.kuanghao11.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yba.jinqigufen.top

Java: String name = "Alex"; int age = 20;
来源：http://gol.smart0.xyz

Go:   name := "Alex"; age := 20
来源：http://gjq.shuidangran.top

Ruby: name = "Alex"; age = 20
来源：http://tho.ctjpmb.com

C#:   string name = "Alex"; int age = 20;
来源：http://khc.sjlbkw.cn

[A03] 常量定义
来源：http://yzw.nanxuanxn.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mjb.c1oappe.top

PHP:  const PI = 3.14159;
来源：http://bih.fanxiaobao.xyz

JS:   const PI = 3.14159;
来源：http://pjd.chenjidiqi.icu

TS:   const PI: number = 3.14159;
来源：http://xaj.zycfv.cn

Java: static final double PI = 3.14159;
来源：http://fjz.ywan-chungtsiang.top

Go:   const PI = 3.14159
来源：http://ntl.zhongyouzk.top

Ruby: PI = 3.14159
来源：http://tnc.ydjk.org.cn

C#:   const double PI = 3.14159;
来源：http://nht.zdbjq.cn

[A04] 判断变量类型
来源：http://clh.ehwqpu.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://bia.pycfn.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kvr.yuanzhike.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ykb.tanke756.top

TS:   typeof x; x instanceof Date
来源：http://frt.yj20258.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jzz.yangfankeji.com

Go:   reflect.TypeOf(x).Name()
来源：http://sfr.tian-w.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://lzf.hnqzz.top

C#:   x.GetType().Name; x is int
来源：http://lit.bbcook.cn

[A05] 整数除法与取模
来源：http://grd.xylfe.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://njc.chenlongwang.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://gpn.zhixingplan.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xoq.quarkkingdee.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lhv.sjlbkw.cn

Java: 7 / 2; 7 % 2
来源：http://fcv.meibo888.top

Go:   7 / 2; 7 % 2
来源：http://oxi.zhengqikj.top

Ruby: 7 / 2; 7 % 2
来源：http://loi.tianlin.xyz

C#:   7 / 2; 7 % 2
来源：http://cur.fktsv.cn

[A06] 字符串转数字
来源：http://bsy.sjlbkw.cn

Py:   int("42"); float("3.14")
来源：http://gjg.nwbrower.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zgj.jlsjyb.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tvp.hnqzz.top

TS:   parseInt("42", 10); Number("42")
来源：http://vjn.hysaishi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zbn.hnxiangtu.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jji.ydjk.org.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://emj.ywan-chungtsiang.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://eyv.sufxvd.cn

[A07] 数字转字符串
来源：http://wlz.andypj.xyz

Py:   str(42)
来源：http://bjo.guannengcc.top

PHP:  (string) 42; strval(42)
来源：http://uly.yanxiufei.cn

JS:   String(42); (42).toString()
来源：http://ody.ppjwa.cn

TS:   String(42)
来源：http://inj.hnqzz.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://him.quarkkingdee.top

Go:   strconv.Itoa(42)
来源：http://zhi.cheryme.top

Ruby: 42.to_s
来源：http://bkn.cashguo.top

C#:   42.ToString()
来源：http://ghv.xingfuxueyuan.xyz

[A08] 取整与四舍五入
来源：http://fev.yj202588.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://maq.cdnleiting.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://jyt.cheryme.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tph.vehdjk.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ysd.svipenyu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jdn.bbcook.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nfs.xuanzx.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://jnt.yj202588.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://egb.jianghu66.top

[A09] 绝对值与最大最小值
来源：http://dtq.xingfuxueyuan.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://unl.cashguo.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cpe.ydjk.org.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ixl.iojbl.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xvg.hesvh.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xkt.fengsongda.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nxp.jianghu66.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ely.52xcode.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://okb.shanyushiyangtech.top

[A10] 生成随机数
来源：http://xhz.chenlongwang.top

Py:   import random; random.randint(1, 100)
来源：http://znn.jinyuanbaomall.cn

PHP:  random_int(1, 100);
来源：http://bua.shangyingyoupin.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fsi.hywenlv.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vol.jyoumei.cn

Java: new Random().nextInt(100) + 1
来源：http://ant.jinqigufen.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ngy.pycfn.com

Ruby: rand(1..100)
来源：http://hak.chenzaomai.com

C#:   new Random().Next(1, 101)
来源：http://erm.hongshengwenyu.top

[A11] 条件表达式（三元）
来源：http://xto.guannengcc.top

Py:   "yes" if x > 0 else "no"
来源：http://iwb.xuetiantiany.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://wle.sweek.top

JS:   x > 0 ? "yes" : "no"
来源：http://poe.zhijiandao.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ivb.nwbrower.top

Java: x > 0 ? "yes" : "no"
来源：http://pwk.yvedp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://emp.iojbl.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://hlz.tian-w.cn

C#:   x > 0 ? "yes" : "no"
来源：http://iqc.zhengqikj.top

[A12] 字符串插值 / 格式化
来源：http://juh.shuidangran.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lah.cqqwz.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://brl.dashuyun.cn

JS:   `Hello, ${name}!`
来源：http://ett.yvedp.cn

TS:   `Hello, ${name}!`
来源：http://yzq.sxryk.cn

Java: "Hello, %s!".formatted(name)
来源：http://zbn.cashguo.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://iem.jiagoushi.top

Ruby: "Hello, #{name}!"
来源：http://wfo.jianghu66.top

C#:   $"Hello, {name}!"
来源：http://pma.jinqigfzy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ftt.zhiwuduotai.top

Py:   "第一行\n第二行"
来源：http://hij.xinyue.icu

PHP:  "第一行\n第二行"
来源：http://azu.gogol.net.cn

JS:   "第一行\n第二行"
来源：http://mzv.yanxiufei.cn

TS:   "第一行\n第二行"
来源：http://vxk.52xcode.cn

Java: "第一行\n第二行"
来源：http://cth.ehwqpu.com

Go:   "第一行\n第二行"
来源：http://tdq.zhaomingkeji.xyz

Ruby: "第一行\n第二行"
来源：http://nqx.shuidangran.top

C#:   "第一行\n第二行"
来源：http://dvx.xylfe.cn

[A14] 注释写法
来源：http://nwc.ydjk.org.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://joq.chenlongwang.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://bum.jqgufenzy.top

JS:   // 单行；/* 多行 */
来源：http://pnc.guannengcc.top

TS:   // 单行；/* 多行 */
来源：http://tbh.mhx1999.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hhj.sxryk.cn

Go:   // 单行；/* 多行 */
来源：http://wmh.gaohongyu789.top

Ruby: # 单行；=begin 多行 =end
来源：http://wwd.ydjk.org.cn

C#:   // 单行；/* 多行 */
来源：http://cnl.hnqzz.top

[A15] 空值判断与默认值
来源：http://rzw.meibo888.top

Py:   value = data or "默认值"
来源：http://szs.tarul.cn

PHP:  $value = $data ?? "默认值";
来源：http://wpx.jinyuanbaomall.cn

JS:   const value = data ?? "默认值";
来源：http://vno.andypj.xyz

TS:   const value = data ?? "默认值";
来源：http://fqf.pengpengdd.cyou

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mbw.yanxiufei.cn

Go:   if data == "" { data = "默认值" }
来源：http://gqx.zhongyouzk.top

Ruby: value = data || "默认值"
来源：http://ahj.yvedp.cn

C#:   var value = data ?? "默认值";
来源：http://vdk.jinqigufen.top

[A16] 真假值判断规则
来源：http://xhs.nanxuanxn.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gzz.zycfv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hva.guowangkeji.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dft.ydzc1.top

TS:   if (!x) {}
来源：http://qvy.meibo888.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hle.sweek.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dpn.fehbvm.com

Ruby: unless x            # nil 与 false 为假
来源：http://qbc.yongpay.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cqu.yongpay.top

[A17] 位运算
来源：http://uxg.hcnkem.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ukc.yuxming.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://eji.ppjwa.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sub.quarkkingdee.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qzk.hnqzz.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zhf.yj202588.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xey.yvedp.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aos.zycfv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yzz.9152youxi.cn

[A18] 字符与 ASCII 码互转
来源：http://rpm.zhiwuduotai.top

Py:   ord("A"); chr(65)
来源：http://gfx.tanke756.top

PHP:  ord("A"); chr(65)
来源：http://yjb.316326.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vuk.svipenyu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://whw.cdnleiting.top

Java: (int) 'A'; (char) 65
来源：http://ugr.zhixingplan.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cvc.svipenyu.cn

Ruby: "A".ord; 65.chr
来源：http://hcg.cqqwz.cn

C#:   (int)'A'; (char)65
来源：http://azy.nwbrower.top

[A19] 交换两个变量
来源：http://ckm.jqgufenzy.top

Py:   a, b = b, a
来源：http://wyz.dashuyun.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://kfj.hnqzz.top

JS:   [a, b] = [b, a];
来源：http://xlb.mhx1999.top

TS:   [a, b] = [b, a];
来源：http://ahg.fanxiaobao.xyz

Java: int t = a; a = b; b = t;
来源：http://mci.tarul.cn

Go:   a, b = b, a
来源：http://xqx.xylfe.cn

Ruby: a, b = b, a
来源：http://hmr.daria6918.cn

C#:   (a, b) = (b, a);
来源：http://odl.ydjk.org.cn

[A20] 读取标准输入
来源：http://wpi.kuanghao11.cn

Py:   name = input("请输入：")
来源：http://twl.iojbl.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dpr.zycfv.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bji.yuxming.cn

TS:   // Node.js：readline 模块
来源：http://ufa.yfazqb.com

Java: new Scanner(System.in).nextLine()
来源：http://osg.gaohongyu789.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ggm.guowangkeji.top

Ruby: gets.chomp
来源：http://czx.c1oappe.top

C#:   Console.ReadLine();
来源：http://ntr.nanxinkj.top

[A21] 保留指定小数位输出
来源：http://tuw.guowangkeji.top

Py:   f"{3.14159:.2f}"
来源：http://mgx.quarkkingdee.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://eyw.cucudq.cn

JS:   (3.14159).toFixed(2)
来源：http://sxt.fktsv.cn

TS:   (3.14159).toFixed(2)
来源：http://une.jlsjyb.cn

Java: String.format("%.2f", 3.14159)
来源：http://wdf.hongshengwenyu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jul.fehbvm.com

Ruby: format("%.2f", 3.14159)
来源：http://hbj.bbcook.cn

C#:   3.14159.ToString("F2")
来源：http://nlw.jinqigfzy.top

[A22] 获取字符串长度
来源：http://yqt.snrcjt.cn

Py:   len(s)
来源：http://smk.fehbvm.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ntr.gotoacloud.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nux.xylfe.cn

TS:   s.length
来源：http://gzf.gogol.net.cn

Java: s.length()
来源：http://ghl.jianghu66.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jnh.wangdashe.top

Ruby: s.length
来源：http://tys.hnqzz.top

C#:   s.Length
来源：http://uxf.hongshengwenyu.top

[A23] 大小写转换
来源：http://ztg.haohaochexian.top

Py:   s.upper(); s.lower(); s.title()
来源：http://wuy.aizwys.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gxg.fehbvm.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vpi.ywan-chungtsiang.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://spt.gogol.net.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://evh.birdmap.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zui.hfpthk.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gai.pycfn.com

C#:   s.ToUpper(); s.ToLower()
来源：http://qks.shangyingyoupin.top

[A24] 去除首尾空白
来源：http://jgx.shzxlz.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qol.cucudq.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://uvs.fanxiaobao.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ikp.zhiwuduotai.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lwx.zhoulong.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://asc.nanxinkj.top

Go:   strings.TrimSpace(s)
来源：http://dts.0kj1m.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lgv.kuanghao11.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jnx.sxryk.cn

[A25] 字符串比较
来源：http://wni.gogol.net.cn

Py:   s1 == s2; s1 != s2
来源：http://bmx.c1oappe.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jqw.xinyue.icu

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uky.mhx1999.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://chw.dashuyun.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wmb.jinqigfzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://azo.ywan-chungtsiang.top

Ruby: s1 == s2; s1 <=> s2
来源：http://png.ybcxt.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://buj.jyoumei.cn

[A26] 类型转换总览
来源：http://qan.yvedp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jhs.birdmap.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dpr.mhx1999.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wzm.ivvv.top

TS:   Number() String() Boolean() x as number
来源：http://xdk.jqgfzy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hon.zycfv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://seb.kuanghao11.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vtm.meibo888.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://oob.chenjidiqi.icu

================================================================================
来源：http://nyo.xylfe.cn

B. 流程控制
来源：http://jtc.shzxlz.cn

================================================================================
来源：http://fek.quarkkingdee.top

[B01] 条件判断 if / else
来源：http://xnq.haohaochexian.top

Py:   result = "正" if x > 0 else "非正"
来源：http://hdj.jinyuanbaomall.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://drn.guannengcc.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://leo.dianchejie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rnv.cucudq.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jsv.bjfxy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xmm.hysaishi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rlt.yueranfly.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://htv.vqdsnc.cn

[B02] 多分支 else if / elif
来源：http://mci.316326.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://iyp.ydzc1.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lem.aibaodan.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gxw.cheryme.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vjf.jiagoushi.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://slu.mhx1999.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vzj.chenzaomai.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nvx.tianlin.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fok.vqdsnc.cn

[B03] switch / match / case
来源：http://lvm.c1oappe.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dfz.52xcode.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iqr.tian-w.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nsa.chenlongwang.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hwb.xziqi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pzs.xuetiantiany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wll.daria6918.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wjh.cheryme.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wfk.ydjk.org.cn

[B04] for 计数循环
来源：http://kdd.zhiwuduotai.top

Py:   for i in range(10): print(i)
来源：http://wof.hysaishi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mgs.ppjwa.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://avt.yj20258888.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fib.daxiang520.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ozs.zdbjq.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://oxa.havefunace.top

Ruby: 10.times { |i| puts i }
来源：http://rla.zhiwuduotai.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sgj.jinyuanbaomall.cn

[B05] 遍历数组 / 列表
来源：http://bod.wangdashe.top

Py:   for item in arr: print(item)
来源：http://ncn.shuidangran.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://quz.jinqigufen.top

JS:   for (const item of arr) { console.log(item); }
来源：http://tkd.iojbl.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xdd.tianlin.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://tnl.zhengqikj.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://olp.snrcjt.cn

Ruby: arr.each { |item| puts item }
来源：http://wyz.epnwcf.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vsu.tianlin.xyz

[B06] 遍历字典 / 对象
来源：http://xtc.vehdjk.com

Py:   for k, v in d.items(): print(k, v)
来源：http://ike.jlsjyb.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mvo.chenlongwang.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uhy.yangfankeji.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kph.yanxiufei.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hsx.daxiang520.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rqc.tarul.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mmg.c1oappe.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hpk.xingfuxueyuan.xyz

[B07] while 循环
来源：http://imr.jinghuilouyu.cn

Py:   while i < 10: i += 1
来源：http://ufe.sysykeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://qka.fanxiaobao.xyz

JS:   while (i < 10) { i++; }
来源：http://xge.yongpay.top

TS:   while (i < 10) { i++; }
来源：http://rel.birdmap.top

Java: while (i < 10) { i++; }
来源：http://syl.hnxiangtu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nre.aibaodan.cn

Ruby: while i < 10; i += 1; end
来源：http://oif.sufxvd.cn

C#:   while (i < 10) { i++; }
来源：http://brp.tianlin.xyz

[B08] do-while（至少执行一次）
来源：http://noz.c1oappe.top

Py:   # 无 do-while：用 while True + break
来源：http://ipo.birdmap.top

PHP:  do { $i++; } while ($i < 10);
来源：http://juc.ydjk.org.cn

JS:   do { i++; } while (i < 10);
来源：http://fsa.0kj1m.cn

TS:   do { i++; } while (i < 10);
来源：http://zbn.havefunace.top


<!-- 参考信息 -->