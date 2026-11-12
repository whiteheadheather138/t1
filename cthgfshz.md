代发 wailian999

================================================================================
来源：http://qdu.tian-w.cn

A. 基础语法与类型
来源：http://zbu.yj20258888.top

================================================================================
来源：http://lrh.gzhubu.top

[A01] Hello World
来源：http://yax.mhx1999.top

Py:   print("Hello, World!")
来源：http://aaj.kuanghao11.cn

PHP:  echo "Hello, World!";
来源：http://bzw.hnxiangtu.top

JS:   console.log("Hello, World!");
来源：http://naa.shanyushiyangkeji.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://puo.tianlin.xyz

Java: System.out.println("Hello, World!");
来源：http://zxx.hesvh.cn

Go:   fmt.Println("Hello, World!")
来源：http://juh.xuetiantiany.cn

Ruby: puts "Hello, World!"
来源：http://dde.sjlbkw.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xrh.sufxvd.cn

[A02] 变量声明与赋值
来源：http://abz.cdnleiting.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mny.zhongyouzk.top

PHP:  $name = "Alex"; $age = 20;
来源：http://erv.zycfv.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xag.chenjidiqi.icu

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ytm.fengsongda.top

Java: String name = "Alex"; int age = 20;
来源：http://wkj.yj202588.top

Go:   name := "Alex"; age := 20
来源：http://phw.cheryme.top

Ruby: name = "Alex"; age = 20
来源：http://tdp.zhixingplan.top

C#:   string name = "Alex"; int age = 20;
来源：http://qnf.jinghuilouyu.cn

[A03] 常量定义
来源：http://thb.zdqjudy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lmq.dashuyun.cn

PHP:  const PI = 3.14159;
来源：http://dlx.shanyushiyangkeji.top

JS:   const PI = 3.14159;
来源：http://efa.dianchejie.cn

TS:   const PI: number = 3.14159;
来源：http://gml.fzhhl.top

Java: static final double PI = 3.14159;
来源：http://bzk.mhx1999.top

Go:   const PI = 3.14159
来源：http://pmf.daxiang520.top

Ruby: PI = 3.14159
来源：http://jmc.nwbrower.top

C#:   const double PI = 3.14159;
来源：http://amq.cqqwz.cn

[A04] 判断变量类型
来源：http://moz.daxiang520.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ktx.ivvv.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uxk.kuanghao11.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rzd.tanke756.top

TS:   typeof x; x instanceof Date
来源：http://jne.smart0.xyz

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kol.xuanzx.com

Go:   reflect.TypeOf(x).Name()
来源：http://nvb.fanxiaobao.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://zzj.zhaomingkeji.xyz

C#:   x.GetType().Name; x is int
来源：http://qsn.jinghuilouyu.cn

[A05] 整数除法与取模
来源：http://tkr.pengpengdd.cyou

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://iqx.chenlongwang.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://uqv.jyoumei.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cml.ivvv.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ivy.jinyuanbaomall.cn

Java: 7 / 2; 7 % 2
来源：http://oue.52xcode.cn

Go:   7 / 2; 7 % 2
来源：http://uum.dianchejie.cn

Ruby: 7 / 2; 7 % 2
来源：http://aih.zhaomingkeji.xyz

C#:   7 / 2; 7 % 2
来源：http://aet.ydjk.org.cn

[A06] 字符串转数字
来源：http://isz.yuxming.cn

Py:   int("42"); float("3.14")
来源：http://vyp.sxryk.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gcr.svipenyu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gvy.epnwcf.com

TS:   parseInt("42", 10); Number("42")
来源：http://tqd.mhx1999.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ylw.hywenlv.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cnv.cdnleiting.top

Ruby: "42".to_i; "3.14".to_f
来源：http://orf.wangshuangyany.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://apq.yueranfly.top

[A07] 数字转字符串
来源：http://jgt.cheryme.top

Py:   str(42)
来源：http://rtz.smart0.xyz

PHP:  (string) 42; strval(42)
来源：http://ggq.bbcook.cn

JS:   String(42); (42).toString()
来源：http://xmz.tian-w.cn

TS:   String(42)
来源：http://wse.jinqigfzy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://rzr.wangshuangyany.cn

Go:   strconv.Itoa(42)
来源：http://tme.svipenyu.cn

Ruby: 42.to_s
来源：http://oyn.guannengcc.top

C#:   42.ToString()
来源：http://gdb.ivvv.top

[A08] 取整与四舍五入
来源：http://vpz.ydjk.org.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://boz.quarkkingdee.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://leb.havefunace.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tzz.zhaomingkeji.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kpc.ctjpmb.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rat.zhoulong.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://csd.vehdjk.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://wec.yonumen.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://uyy.nwbrower.top

[A09] 绝对值与最大最小值
来源：http://ybn.guowangkeji.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rgh.jlsjyb.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wgf.shuidangran.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pss.nanxinkj.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tte.aizwys.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://iki.pengpengdd.cyou

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ius.zhixingplan.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tzu.yj20258.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://eqv.yueranfly.top

[A10] 生成随机数
来源：http://rfm.aizwys.cn

Py:   import random; random.randint(1, 100)
来源：http://fwz.ydjk.org.cn

PHP:  random_int(1, 100);
来源：http://pjj.chenlongwang.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qfn.shuidangran.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://uva.gzhubu.top

Java: new Random().nextInt(100) + 1
来源：http://zos.tian-w.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jdj.zhengqikj.top

Ruby: rand(1..100)
来源：http://hcm.uphjek.com

C#:   new Random().Next(1, 101)
来源：http://pob.zdbjq.cn

[A11] 条件表达式（三元）
来源：http://kyz.316326.xyz

Py:   "yes" if x > 0 else "no"
来源：http://cfj.gotoacloud.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ygn.cashguo.top

JS:   x > 0 ? "yes" : "no"
来源：http://xrr.zhiwuduotai.top

TS:   x > 0 ? "yes" : "no"
来源：http://buj.xuetiantiany.cn

Java: x > 0 ? "yes" : "no"
来源：http://wca.vqdsnc.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://quk.sufxvd.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://oli.pengpengdd.cyou

C#:   x > 0 ? "yes" : "no"
来源：http://yoh.jyoumei.cn

[A12] 字符串插值 / 格式化
来源：http://yww.yonumen.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://msz.hywenlv.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xuc.ehwqpu.com

JS:   `Hello, ${name}!`
来源：http://ngi.aibaodan.cn

TS:   `Hello, ${name}!`
来源：http://heq.kuanghao11.cn

Java: "Hello, %s!".formatted(name)
来源：http://mxi.gotoacloud.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ybc.zdqjudy.top

Ruby: "Hello, #{name}!"
来源：http://pyb.gaohongyu789.top

C#:   $"Hello, {name}!"
来源：http://zgz.xziqi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://vsu.zdqjudy.top

Py:   "第一行\n第二行"
来源：http://vwc.tian-w.cn

PHP:  "第一行\n第二行"
来源：http://tvr.jiagoushi.top

JS:   "第一行\n第二行"
来源：http://ymo.ydjk.org.cn

TS:   "第一行\n第二行"
来源：http://ore.ywan-chungtsiang.top

Java: "第一行\n第二行"
来源：http://olh.ybcxt.top

Go:   "第一行\n第二行"
来源：http://uen.zhiwuduotai.top

Ruby: "第一行\n第二行"
来源：http://huc.zhixingplan.top

C#:   "第一行\n第二行"
来源：http://cgn.zhengqikj.top

[A14] 注释写法
来源：http://fbw.quarkkingdee.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://kzp.daxiang520.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://gfr.wangdashe.top

JS:   // 单行；/* 多行 */
来源：http://bsp.yj20258.top

TS:   // 单行；/* 多行 */
来源：http://boo.hesvh.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://phu.yfazqb.com

Go:   // 单行；/* 多行 */
来源：http://cym.hammf.cn

Ruby: # 单行；=begin 多行 =end
来源：http://oct.svipenyu.cn

C#:   // 单行；/* 多行 */
来源：http://cno.nanxuanxn.top

[A15] 空值判断与默认值
来源：http://uzh.quarkkingdee.top

Py:   value = data or "默认值"
来源：http://mcg.jinqigufen.top

PHP:  $value = $data ?? "默认值";
来源：http://xad.hnxiangtu.top

JS:   const value = data ?? "默认值";
来源：http://kqx.9152youxi.cn

TS:   const value = data ?? "默认值";
来源：http://pwi.ydzc1.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zol.xylfe.cn

Go:   if data == "" { data = "默认值" }
来源：http://pkg.iojbl.cn

Ruby: value = data || "默认值"
来源：http://kux.pengpengdd.cyou

C#:   var value = data ?? "默认值";
来源：http://dxh.ehwqpu.com

[A16] 真假值判断规则
来源：http://jqd.uphjek.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bke.tanke756.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ovs.daria6918.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ehe.xuetiantiany.cn

TS:   if (!x) {}
来源：http://azl.shzxlz.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lqq.pycfn.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jbl.xingfuxueyuan.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://wjt.jlsjyb.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pkl.zhiwuduotai.top

[A17] 位运算
来源：http://aqq.xinyue.icu

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xju.kuanghao11.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pkr.xziqi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fll.ehwqpu.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://htl.tarul.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bbf.jinqigfzy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ltx.hnqzz.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vkt.cashguo.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rcg.gzhubu.top

[A18] 字符与 ASCII 码互转
来源：http://qkg.gotoacloud.top

Py:   ord("A"); chr(65)
来源：http://atg.tian-w.cn

PHP:  ord("A"); chr(65)
来源：http://iyj.zhoulong.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qvd.jinqigufen.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://prp.shzxlz.cn

Java: (int) 'A'; (char) 65
来源：http://dkt.fktsv.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fbb.fehbvm.com

Ruby: "A".ord; 65.chr
来源：http://crj.shanyushiyangkeji.top

C#:   (int)'A'; (char)65
来源：http://xqs.zdqjudy.top

[A19] 交换两个变量
来源：http://xwr.wangdashe.top

Py:   a, b = b, a
来源：http://qva.cdnleiting.top

PHP:  [$a, $b] = [$b, $a];
来源：http://mhc.vqdsnc.cn

JS:   [a, b] = [b, a];
来源：http://joe.nanxuanxn.top

TS:   [a, b] = [b, a];
来源：http://fyf.gzhubu.top

Java: int t = a; a = b; b = t;
来源：http://kwh.zycfv.cn

Go:   a, b = b, a
来源：http://lwc.0kj1m.cn

Ruby: a, b = b, a
来源：http://fig.jinyuanbaomall.cn

C#:   (a, b) = (b, a);
来源：http://uvv.yj20258.top

[A20] 读取标准输入
来源：http://dbg.jqgfzy.top

Py:   name = input("请输入：")
来源：http://hoi.cashguo.top

PHP:  $name = trim(fgets(STDIN));
来源：http://hzv.iojbl.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sea.shangyingyoupin.top

TS:   // Node.js：readline 模块
来源：http://fvu.hcnkem.com

Java: new Scanner(System.in).nextLine()
来源：http://lfk.zhongyouzk.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lau.tanke756.top

Ruby: gets.chomp
来源：http://lng.jlsjyb.cn

C#:   Console.ReadLine();
来源：http://tkn.ybcxt.top

[A21] 保留指定小数位输出
来源：http://spr.jinyuanbaomall.cn

Py:   f"{3.14159:.2f}"
来源：http://pqo.cqqwz.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jvp.zhijiandao.cn

JS:   (3.14159).toFixed(2)
来源：http://fss.nanxuanxn.top

TS:   (3.14159).toFixed(2)
来源：http://tbo.tian-w.cn

Java: String.format("%.2f", 3.14159)
来源：http://bep.gotoacloud.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ezw.hesvh.cn

Ruby: format("%.2f", 3.14159)
来源：http://xgt.yongpay.top

C#:   3.14159.ToString("F2")
来源：http://dht.cashguo.top

[A22] 获取字符串长度
来源：http://arz.bbcook.cn

Py:   len(s)
来源：http://qeb.jiagoushi.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ipq.xziqi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tff.yvedp.cn

TS:   s.length
来源：http://mlr.shuidangran.top

Java: s.length()
来源：http://smd.vehdjk.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bjh.hysaishi.cn

Ruby: s.length
来源：http://xvv.guannengcc.top

C#:   s.Length
来源：http://rzk.zhaomingkeji.xyz

[A23] 大小写转换
来源：http://xnx.yj20258888.top

Py:   s.upper(); s.lower(); s.title()
来源：http://fgh.mhx1999.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jpe.jqgfzy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kzz.ppjwa.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hhq.ybcxt.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xnc.sufxvd.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rla.yangfankeji.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://det.gotoacloud.top

C#:   s.ToUpper(); s.ToLower()
来源：http://jqq.zdbjq.cn

[A24] 去除首尾空白
来源：http://lil.jlsjyb.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://eci.cashguo.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fyu.yangfankeji.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hge.ydjk.org.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qoo.fengsongda.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hsl.vqdsnc.cn

Go:   strings.TrimSpace(s)
来源：http://hjm.zhiwuduotai.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mkv.ivvv.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ggr.hongshengwenyu.top

[A25] 字符串比较
来源：http://ffj.cheryme.top

Py:   s1 == s2; s1 != s2
来源：http://hei.ywan-chungtsiang.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kpx.shanyushiyangkeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://aen.xziqi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ned.ctjpmb.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xzw.yanxiufei.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gsq.yuanzhike.top

Ruby: s1 == s2; s1 <=> s2
来源：http://wet.chenjidiqi.icu

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lxp.jinyuanbaomall.cn

[A26] 类型转换总览
来源：http://wis.svipenyu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kwq.tarul.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dtv.yfazqb.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oqf.birdmap.top

TS:   Number() String() Boolean() x as number
来源：http://wtg.sufxvd.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zur.pycfn.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vza.pengpengdd.cyou

Ruby: to_i to_f to_s to_sym to_a
来源：http://wic.dianchejie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wob.hywenlv.cn

================================================================================
来源：http://jhr.sjlbkw.cn

B. 流程控制
来源：http://igh.ppjwa.cn

================================================================================
来源：http://sia.feifeiyinyue.top

[B01] 条件判断 if / else
来源：http://dik.zdqjudy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://khp.sufxvd.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ojw.daria6918.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zme.ivvv.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tiv.xziqi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gdw.chenzaomai.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xmh.pengpengdd.cyou

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nlq.cheryme.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wmj.zhongyouzk.top

[B02] 多分支 else if / elif
来源：http://eak.nwbrower.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://olq.mhx1999.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uug.pengpengdd.cyou

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wkz.redwolf501.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pxv.chenjidiqi.icu

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bai.ctjpmb.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dxi.aibaodan.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jin.hesvh.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mmi.vehdjk.com

[B03] switch / match / case
来源：http://mgf.aibaodan.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yyf.xylfe.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wjd.birdmap.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jsl.zdqjudy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hnw.gogol.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oos.nanxuanxn.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xoa.chenzaomai.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://amu.yfazqb.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bwu.haohaochexian.top

[B04] for 计数循环
来源：http://ufh.ivvv.top

Py:   for i in range(10): print(i)
来源：http://ssl.aibaodan.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bhw.yfazqb.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qkw.tarul.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zpg.chenlongwang.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nof.aibaodan.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nsi.shangyingyoupin.top

Ruby: 10.times { |i| puts i }
来源：http://jyr.aibaodan.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jsy.cashguo.top

[B05] 遍历数组 / 列表
来源：http://ehc.xingfuxueyuan.xyz

Py:   for item in arr: print(item)
来源：http://jul.ehwqpu.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://thv.aibaodan.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lhl.havefunace.top

TS:   for (const item of arr) { console.log(item); }
来源：http://knq.fzhhl.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://cac.yfazqb.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://acx.tarul.cn

Ruby: arr.each { |item| puts item }
来源：http://bhh.dianchejie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xjd.aibaodan.cn

[B06] 遍历字典 / 对象
来源：http://bfr.9152youxi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rtv.dashuyun.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lls.yueranfly.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zjd.jinqigufen.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://apm.tianlin.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://phk.zdqjudy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mnq.chenzaomai.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xmo.nwbrower.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bwz.9152youxi.cn

[B07] while 循环
来源：http://qtj.jinqigfzy.top

Py:   while i < 10: i += 1
来源：http://nca.yanxiufei.cn

PHP:  while ($i < 10) { $i++; }
来源：http://chp.fzhhl.top

JS:   while (i < 10) { i++; }
来源：http://gjq.chenlongwang.top

TS:   while (i < 10) { i++; }
来源：http://yct.shzxlz.cn

Java: while (i < 10) { i++; }
来源：http://mas.zycfv.cn


<!-- 参考信息 -->