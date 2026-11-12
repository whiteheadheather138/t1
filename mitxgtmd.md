代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://jmq.shanyushiyangkeji.top

Go:   fmt.Println("Hello, World!")
来源：http://yet.yvedp.cn

Ruby: puts "Hello, World!"
来源：http://ihu.yuxming.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://efm.dashuyun.cn

[A02] 变量声明与赋值
来源：http://ggt.ydzc1.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ibg.smart0.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://lpx.zycfv.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wka.fehbvm.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gxq.9152youxi.cn

Java: String name = "Alex"; int age = 20;
来源：http://lnt.zdqjudy.top

Go:   name := "Alex"; age := 20
来源：http://are.yanxiufei.cn

Ruby: name = "Alex"; age = 20
来源：http://vxb.ybcxt.top

C#:   string name = "Alex"; int age = 20;
来源：http://xtz.dianchejie.cn

[A03] 常量定义
来源：http://amf.9152youxi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hkj.yfazqb.com

PHP:  const PI = 3.14159;
来源：http://rhv.xuanzx.com

JS:   const PI = 3.14159;
来源：http://hbj.fanxiaobao.xyz

TS:   const PI: number = 3.14159;
来源：http://wju.jinqigufen.top

Java: static final double PI = 3.14159;
来源：http://eyu.yangfankeji.com

Go:   const PI = 3.14159
来源：http://drm.jinghuilouyu.cn

Ruby: PI = 3.14159
来源：http://gcs.cqqwz.cn

C#:   const double PI = 3.14159;
来源：http://yng.dianchejie.cn

[A04] 判断变量类型
来源：http://nnc.chenzaomai.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://oyz.guannengcc.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bok.jyoumei.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nle.sysykeji.top

TS:   typeof x; x instanceof Date
来源：http://plg.jqgfzy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ilo.yongpay.top

Go:   reflect.TypeOf(x).Name()
来源：http://tpl.fktsv.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ibm.fzhhl.top

C#:   x.GetType().Name; x is int
来源：http://rtb.nwbrower.top

[A05] 整数除法与取模
来源：http://fyi.hammf.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://upr.zhoulong.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://pxe.gzhubu.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://sum.yj20258.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ans.chenlongwang.top

Java: 7 / 2; 7 % 2
来源：http://idd.xinyue.icu

Go:   7 / 2; 7 % 2
来源：http://fyn.bjfxy.top

Ruby: 7 / 2; 7 % 2
来源：http://qic.dianchejie.cn

C#:   7 / 2; 7 % 2
来源：http://ilj.sufxvd.cn

[A06] 字符串转数字
来源：http://kgd.ppjwa.cn

Py:   int("42"); float("3.14")
来源：http://pst.hfpthk.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ziz.jinqigufen.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pkj.jlsjyb.cn

TS:   parseInt("42", 10); Number("42")
来源：http://cno.fengsongda.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gcv.zhongyouzk.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lzk.hongshengwenyu.top

Ruby: "42".to_i; "3.14".to_f
来源：http://cnk.vqdsnc.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lye.nanxuanxn.top

[A07] 数字转字符串
来源：http://hrm.jinghuilouyu.cn

Py:   str(42)
来源：http://hkg.bjfxy.top

PHP:  (string) 42; strval(42)
来源：http://zbj.cheryme.top

JS:   String(42); (42).toString()
来源：http://flc.chenjidiqi.icu

TS:   String(42)
来源：http://egc.zhijiandao.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xyt.tian-w.cn

Go:   strconv.Itoa(42)
来源：http://dcb.smart0.xyz

Ruby: 42.to_s
来源：http://asz.fengsongda.top

C#:   42.ToString()
来源：http://yzf.0kj1m.cn

[A08] 取整与四舍五入
来源：http://jty.cucudq.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rfj.vehdjk.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dyi.vehdjk.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vgy.hnqzz.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://oyr.hnqzz.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tmi.hesvh.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hbc.jlsjyb.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://tjy.jinqigfzy.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://uwe.aizwys.cn

[A09] 绝对值与最大最小值
来源：http://mwx.svipenyu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://shs.wangshuangyany.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lur.chenlongwang.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zqw.bbcook.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://njl.ywan-chungtsiang.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tfr.ywan-chungtsiang.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ewq.jinqigfzy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ycv.xuetiantiany.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mzs.9152youxi.cn

[A10] 生成随机数
来源：http://ywb.jqgfzy.top

Py:   import random; random.randint(1, 100)
来源：http://wsh.nanxuanxn.top

PHP:  random_int(1, 100);
来源：http://hds.sufxvd.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://aul.xinyue.icu

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hwg.yfazqb.com

Java: new Random().nextInt(100) + 1
来源：http://ibq.shuidangran.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wab.ywan-chungtsiang.top

Ruby: rand(1..100)
来源：http://yoe.jinyuanbaomall.cn

C#:   new Random().Next(1, 101)
来源：http://bba.guannengcc.top

[A11] 条件表达式（三元）
来源：http://nzv.zhengqikj.top

Py:   "yes" if x > 0 else "no"
来源：http://nms.iojbl.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://vwg.yongpay.top

JS:   x > 0 ? "yes" : "no"
来源：http://jjp.nwbrower.top

TS:   x > 0 ? "yes" : "no"
来源：http://plh.gzhubu.top

Java: x > 0 ? "yes" : "no"
来源：http://jgf.fengsongda.top

Go:   // 无三元运算符，需用 if 语句
来源：http://sya.jiagoushi.top

Ruby: x > 0 ? "yes" : "no"
来源：http://gqi.dianchejie.cn

C#:   x > 0 ? "yes" : "no"
来源：http://yzs.jinqigufen.top

[A12] 字符串插值 / 格式化
来源：http://yih.hammf.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ltv.zhaomingkeji.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ptj.fanxiaobao.xyz

JS:   `Hello, ${name}!`
来源：http://vvk.feifeiyinyue.top

TS:   `Hello, ${name}!`
来源：http://jww.xingfuxueyuan.xyz

Java: "Hello, %s!".formatted(name)
来源：http://oap.jqgufenzy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kal.gotoacloud.top

Ruby: "Hello, #{name}!"
来源：http://nqr.yfazqb.com

C#:   $"Hello, {name}!"
来源：http://ryc.zhaomingkeji.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://ymb.ydjk.org.cn

Py:   "第一行\n第二行"
来源：http://jcs.haohaochexian.top

PHP:  "第一行\n第二行"
来源：http://wlu.pengpengdd.cyou

JS:   "第一行\n第二行"
来源：http://prt.cucudq.cn

TS:   "第一行\n第二行"
来源：http://fjl.yonumen.top

Java: "第一行\n第二行"
来源：http://wyf.ppjwa.cn

Go:   "第一行\n第二行"
来源：http://gjh.tanke756.top

Ruby: "第一行\n第二行"
来源：http://ssf.jinghuilouyu.cn

C#:   "第一行\n第二行"
来源：http://tuq.mhx1999.top

[A14] 注释写法
来源：http://jij.zhongyouzk.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://hfl.hnqzz.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://fsp.nanxuanxn.top

JS:   // 单行；/* 多行 */
来源：http://oxl.jinyuanbaomall.cn

TS:   // 单行；/* 多行 */
来源：http://doh.fzhhl.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xta.daxiang520.top

Go:   // 单行；/* 多行 */
来源：http://eqq.tarul.cn

Ruby: # 单行；=begin 多行 =end
来源：http://pvh.shuidangran.top

C#:   // 单行；/* 多行 */
来源：http://nhw.haohaochexian.top

[A15] 空值判断与默认值
来源：http://kcu.svipenyu.cn

Py:   value = data or "默认值"
来源：http://lwr.ppjwa.cn

PHP:  $value = $data ?? "默认值";
来源：http://cbt.birdmap.top

JS:   const value = data ?? "默认值";
来源：http://rjm.yanxiufei.cn

TS:   const value = data ?? "默认值";
来源：http://iea.zhiwuduotai.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hkl.ybcxt.top

Go:   if data == "" { data = "默认值" }
来源：http://sle.andypj.xyz

Ruby: value = data || "默认值"
来源：http://ibg.hesvh.cn

C#:   var value = data ?? "默认值";
来源：http://cub.cashguo.top

[A16] 真假值判断规则
来源：http://qzj.guowangkeji.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vbc.hysaishi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zqq.hywenlv.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fez.daxiang520.top

TS:   if (!x) {}
来源：http://att.yangfankeji.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qsz.redwolf501.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mal.nanxuanxn.top

Ruby: unless x            # nil 与 false 为假
来源：http://fjt.jlsjyb.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://uad.zdbjq.cn

[A17] 位运算
来源：http://ard.yj20258.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kdc.shanyushiyangkeji.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fwk.guannengcc.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ldm.jinqigfzy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://btc.cdnleiting.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cvq.0kj1m.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wkf.9152youxi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fvo.fengsongda.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kaq.sysykeji.top

[A18] 字符与 ASCII 码互转
来源：http://pus.meibo888.top

Py:   ord("A"); chr(65)
来源：http://hgd.zhaomingkeji.xyz

PHP:  ord("A"); chr(65)
来源：http://pvv.ydzc1.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wwt.hysaishi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ytb.jianghu66.top

Java: (int) 'A'; (char) 65
来源：http://txj.ydjk.org.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ufj.sjlbkw.cn

Ruby: "A".ord; 65.chr
来源：http://ads.hysaishi.cn

C#:   (int)'A'; (char)65
来源：http://rzu.ivvv.top

[A19] 交换两个变量
来源：http://lkh.tanke756.top

Py:   a, b = b, a
来源：http://hdn.yuanzhike.top

PHP:  [$a, $b] = [$b, $a];
来源：http://toe.gzhubu.top

JS:   [a, b] = [b, a];
来源：http://jzr.zhixingplan.top

TS:   [a, b] = [b, a];
来源：http://zkb.316326.xyz

Java: int t = a; a = b; b = t;
来源：http://sis.bjfxy.top

Go:   a, b = b, a
来源：http://lxw.xinyue.icu

Ruby: a, b = b, a
来源：http://jtd.chenjidiqi.icu

C#:   (a, b) = (b, a);
来源：http://her.zdbjq.cn

[A20] 读取标准输入
来源：http://qdt.tianlin.xyz

Py:   name = input("请输入：")
来源：http://fzy.zdqjudy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://yjn.fktsv.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ktk.zhengqikj.top

TS:   // Node.js：readline 模块
来源：http://wmr.yonumen.top

Java: new Scanner(System.in).nextLine()
来源：http://vsn.ehwqpu.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://slu.sxryk.cn

Ruby: gets.chomp
来源：http://mer.hnqzz.top

C#:   Console.ReadLine();
来源：http://cuk.nwbrower.top

[A21] 保留指定小数位输出
来源：http://jwm.ehwqpu.com

Py:   f"{3.14159:.2f}"
来源：http://hdq.chenzaomai.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://eit.guannengcc.top

JS:   (3.14159).toFixed(2)
来源：http://nkz.wangdashe.top

TS:   (3.14159).toFixed(2)
来源：http://jwm.hysaishi.cn

Java: String.format("%.2f", 3.14159)
来源：http://vvx.hnqzz.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://eaj.yj202588.top

Ruby: format("%.2f", 3.14159)
来源：http://abf.yuanzhike.top

C#:   3.14159.ToString("F2")
来源：http://eah.kuanghao11.cn

[A22] 获取字符串长度
来源：http://ums.yj20258.top

Py:   len(s)
来源：http://yat.yj20258.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hho.chenzaomai.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sed.fzhhl.top

TS:   s.length
来源：http://gyu.aibaodan.cn

Java: s.length()
来源：http://xvq.52xcode.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qwp.yueranfly.top

Ruby: s.length
来源：http://jff.hnxiangtu.top

C#:   s.Length
来源：http://hey.zhiwuduotai.top

[A23] 大小写转换
来源：http://rmu.yfazqb.com

Py:   s.upper(); s.lower(); s.title()
来源：http://vge.zhijiandao.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ssw.daxiang520.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ivf.zycfv.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nqn.ppjwa.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://twf.xziqi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kkq.316326.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qbk.xinyue.icu

C#:   s.ToUpper(); s.ToLower()
来源：http://xrm.jqgufenzy.top

[A24] 去除首尾空白
来源：http://qpt.wangshuangyany.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tnv.nwbrower.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://grn.jinghuilouyu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://olc.xziqi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fft.bbcook.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fdb.wangshuangyany.cn

Go:   strings.TrimSpace(s)
来源：http://rza.dianchejie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lco.sweek.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lcc.uphjek.com

[A25] 字符串比较
来源：http://oat.jyoumei.cn

Py:   s1 == s2; s1 != s2
来源：http://ymb.ctjpmb.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://svm.vehdjk.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://woj.hesvh.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xbs.vehdjk.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fjv.daria6918.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dei.cashguo.top

Ruby: s1 == s2; s1 <=> s2
来源：http://uoe.epnwcf.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pom.mhx1999.top

[A26] 类型转换总览
来源：http://skq.jqgufenzy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://soh.cheryme.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lmd.hfpthk.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yha.tian-w.cn

TS:   Number() String() Boolean() x as number
来源：http://amp.ivvv.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dpb.vqdsnc.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sab.hnxiangtu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://bdb.chenjidiqi.icu

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vtc.havefunace.top

================================================================================
来源：http://biv.cucudq.cn

B. 流程控制
来源：http://rxr.aizwys.cn

================================================================================
来源：http://rao.zhengqikj.top

[B01] 条件判断 if / else
来源：http://uzp.hcnkem.com

Py:   result = "正" if x > 0 else "非正"
来源：http://oxq.fengsongda.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ejb.yj202588.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pih.yvedp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kxb.nanxinkj.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ogb.yvedp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mcn.ehwqpu.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dav.9152youxi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rkv.hnxiangtu.top

[B02] 多分支 else if / elif
来源：http://fnr.yangfankeji.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bln.chenzaomai.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ybo.9152youxi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mff.sysykeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fhb.hywenlv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hef.yonumen.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rzy.yuanzhike.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hxa.shzxlz.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vwn.snrcjt.cn

[B03] switch / match / case
来源：http://rtx.snrcjt.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bgv.jianghu66.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gwo.kuanghao11.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yok.dashuyun.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dre.sjlbkw.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wce.jinyuanbaomall.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ymh.iojbl.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://stn.hcnkem.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iws.fehbvm.com

[B04] for 计数循环
来源：http://wbi.yangfankeji.com

Py:   for i in range(10): print(i)
来源：http://scp.zhongyouzk.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ryt.mhx1999.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://foo.jinyuanbaomall.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jnb.ctjpmb.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mct.ppjwa.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yoa.jiagoushi.top

Ruby: 10.times { |i| puts i }
来源：http://pcq.cheryme.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://aut.pengpengdd.cyou

[B05] 遍历数组 / 列表
来源：http://gus.zhiwuduotai.top

Py:   for item in arr: print(item)
来源：http://wge.yj20258.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pxv.yanxiufei.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tce.nanxuanxn.top

TS:   for (const item of arr) { console.log(item); }
来源：http://gvj.svipenyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qgv.jinqigufen.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rgl.ydjk.org.cn

Ruby: arr.each { |item| puts item }
来源：http://txi.zhiwuduotai.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tjq.yueranfly.top

[B06] 遍历字典 / 对象
来源：http://xgj.nwbrower.top

Py:   for k, v in d.items(): print(k, v)
来源：http://nop.fehbvm.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bwj.xuetiantiany.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rgb.jqgufenzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://edy.fktsv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kse.fzhhl.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xyf.aizwys.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kic.bbcook.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qcj.hfpthk.cn

[B07] while 循环
来源：http://ssu.ctjpmb.com

Py:   while i < 10: i += 1
来源：http://jwa.ppjwa.cn

PHP:  while ($i < 10) { $i++; }
来源：http://zfx.yangfankeji.com

JS:   while (i < 10) { i++; }
来源：http://bir.hammf.cn

TS:   while (i < 10) { i++; }
来源：http://cmk.shangyingyoupin.top

Java: while (i < 10) { i++; }
来源：http://mbi.ywan-chungtsiang.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qdb.gzhubu.top

Ruby: while i < 10; i += 1; end
来源：http://acv.vqdsnc.cn

C#:   while (i < 10) { i++; }
来源：http://nfj.dianchejie.cn

[B08] do-while（至少执行一次）
来源：http://akq.cheryme.top

Py:   # 无 do-while：用 while True + break
来源：http://cxd.shuidangran.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jxr.dianchejie.cn

JS:   do { i++; } while (i < 10);
来源：http://tkr.andypj.xyz

TS:   do { i++; } while (i < 10);
来源：http://ydq.ydzc1.top


<!-- 参考信息 -->