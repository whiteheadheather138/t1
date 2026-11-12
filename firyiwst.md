代发 wailian999

Py:   print("Hello, World!")
来源：http://fby.ctjpmb.com

PHP:  echo "Hello, World!";
来源：http://dpw.tianlin.xyz

JS:   console.log("Hello, World!");
来源：http://zwo.zycfv.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xyr.zhijiandao.cn

Java: System.out.println("Hello, World!");
来源：http://tvd.cashguo.top

Go:   fmt.Println("Hello, World!")
来源：http://apo.hnxiangtu.top

Ruby: puts "Hello, World!"
来源：http://ydr.yfazqb.com

C#:   Console.WriteLine("Hello, World!");
来源：http://sqa.yj202588.top

[A02] 变量声明与赋值
来源：http://gxz.fehbvm.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ywv.52xcode.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://txf.redwolf501.top

JS:   let name = "Alex"; const age = 20;
来源：http://ivy.fengsongda.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xsi.jqgufenzy.top

Java: String name = "Alex"; int age = 20;
来源：http://vmp.zhiwuduotai.top

Go:   name := "Alex"; age := 20
来源：http://bnd.vehdjk.com

Ruby: name = "Alex"; age = 20
来源：http://grg.9152youxi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://gcw.wangshuangyany.cn

[A03] 常量定义
来源：http://wed.ydjk.org.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rlt.cdnleiting.top

PHP:  const PI = 3.14159;
来源：http://ojc.yangfankeji.com

JS:   const PI = 3.14159;
来源：http://agz.guowangkeji.top

TS:   const PI: number = 3.14159;
来源：http://tbd.dianchejie.cn

Java: static final double PI = 3.14159;
来源：http://rzw.sysykeji.top

Go:   const PI = 3.14159
来源：http://saa.haohaochexian.top

Ruby: PI = 3.14159
来源：http://gse.tian-w.cn

C#:   const double PI = 3.14159;
来源：http://gya.smart0.xyz

[A04] 判断变量类型
来源：http://taz.xuetiantiany.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://drs.ivvv.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ink.dianchejie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mdr.sjlbkw.cn

TS:   typeof x; x instanceof Date
来源：http://wpt.birdmap.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zqh.tanke756.top

Go:   reflect.TypeOf(x).Name()
来源：http://mfq.havefunace.top

Ruby: x.class; x.is_a?(Integer)
来源：http://cxy.xuanzx.com

C#:   x.GetType().Name; x is int
来源：http://mfu.yuanzhike.top

[A05] 整数除法与取模
来源：http://emg.zhoulong.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tjd.xuanzx.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://cqt.svipenyu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vyy.cqqwz.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fhl.shanyushiyangtech.top

Java: 7 / 2; 7 % 2
来源：http://dvx.vqdsnc.cn

Go:   7 / 2; 7 % 2
来源：http://pvw.yvedp.cn

Ruby: 7 / 2; 7 % 2
来源：http://yzo.fzhhl.top

C#:   7 / 2; 7 % 2
来源：http://xxd.quarkkingdee.top

[A06] 字符串转数字
来源：http://mwi.kuanghao11.cn

Py:   int("42"); float("3.14")
来源：http://ayc.cheryme.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ast.gzhubu.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kzd.hcnkem.com

TS:   parseInt("42", 10); Number("42")
来源：http://amn.hnxiangtu.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yvd.chenlongwang.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hpm.hnxiangtu.top

Ruby: "42".to_i; "3.14".to_f
来源：http://xsl.52xcode.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fqe.zhixingplan.top

[A07] 数字转字符串
来源：http://hvb.ctjpmb.com

Py:   str(42)
来源：http://uwx.zhaomingkeji.xyz

PHP:  (string) 42; strval(42)
来源：http://xqo.sweek.top

JS:   String(42); (42).toString()
来源：http://fup.jlsjyb.cn

TS:   String(42)
来源：http://har.sjlbkw.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bzr.yj20258888.top

Go:   strconv.Itoa(42)
来源：http://ljf.52xcode.cn

Ruby: 42.to_s
来源：http://ewx.yj20258888.top

C#:   42.ToString()
来源：http://dgf.zhaomingkeji.xyz

[A08] 取整与四舍五入
来源：http://lbr.c1oappe.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zjb.fzhhl.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mve.dashuyun.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ohf.xziqi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kwj.jlsjyb.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qea.hnqzz.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://scu.ywan-chungtsiang.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://vtc.yj20258888.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jvb.vqdsnc.cn

[A09] 绝对值与最大最小值
来源：http://odn.fanxiaobao.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xuo.ydzc1.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://eij.tian-w.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tbj.jqgfzy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fjj.xuetiantiany.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gab.fengsongda.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kic.jinqigufen.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jgy.vehdjk.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wqc.uphjek.com

[A10] 生成随机数
来源：http://asl.jinghuilouyu.cn

Py:   import random; random.randint(1, 100)
来源：http://xbl.cdnleiting.top

PHP:  random_int(1, 100);
来源：http://rnm.pengpengdd.cyou

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ceo.yj20258.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ztm.kuanghao11.cn

Java: new Random().nextInt(100) + 1
来源：http://klu.yuxming.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://twl.chenlongwang.top

Ruby: rand(1..100)
来源：http://wko.aibaodan.cn

C#:   new Random().Next(1, 101)
来源：http://vna.chenlongwang.top

[A11] 条件表达式（三元）
来源：http://nie.shuidangran.top

Py:   "yes" if x > 0 else "no"
来源：http://pmt.jqgufenzy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://asu.chenjidiqi.icu

JS:   x > 0 ? "yes" : "no"
来源：http://tkf.xylfe.cn

TS:   x > 0 ? "yes" : "no"
来源：http://cnv.ybcxt.top

Java: x > 0 ? "yes" : "no"
来源：http://aac.epnwcf.com

Go:   // 无三元运算符，需用 if 语句
来源：http://nim.daria6918.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://erj.hongshengwenyu.top

C#:   x > 0 ? "yes" : "no"
来源：http://xhq.sxryk.cn

[A12] 字符串插值 / 格式化
来源：http://rwu.fktsv.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wpo.hnqzz.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://njj.yj202588.top

JS:   `Hello, ${name}!`
来源：http://uvw.jqgufenzy.top

TS:   `Hello, ${name}!`
来源：http://ihb.yfazqb.com

Java: "Hello, %s!".formatted(name)
来源：http://eli.hesvh.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dtg.ydjk.org.cn

Ruby: "Hello, #{name}!"
来源：http://ddz.guannengcc.top

C#:   $"Hello, {name}!"
来源：http://nuu.aizwys.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://wco.andypj.xyz

Py:   "第一行\n第二行"
来源：http://fzl.gaohongyu789.top

PHP:  "第一行\n第二行"
来源：http://lba.tarul.cn

JS:   "第一行\n第二行"
来源：http://gzq.hysaishi.cn

TS:   "第一行\n第二行"
来源：http://ssh.jyoumei.cn

Java: "第一行\n第二行"
来源：http://xqf.xylfe.cn

Go:   "第一行\n第二行"
来源：http://lxx.svipenyu.cn

Ruby: "第一行\n第二行"
来源：http://gjq.yuanzhike.top

C#:   "第一行\n第二行"
来源：http://tcy.tanke756.top

[A14] 注释写法
来源：http://gxs.0kj1m.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://qtl.aibaodan.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://skk.snrcjt.cn

JS:   // 单行；/* 多行 */
来源：http://zvs.hywenlv.cn

TS:   // 单行；/* 多行 */
来源：http://qko.hywenlv.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rba.aizwys.cn

Go:   // 单行；/* 多行 */
来源：http://ner.svipenyu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://nyi.hnxiangtu.top

C#:   // 单行；/* 多行 */
来源：http://qth.jiagoushi.top

[A15] 空值判断与默认值
来源：http://bql.jinghuilouyu.cn

Py:   value = data or "默认值"
来源：http://lkc.sjlbkw.cn

PHP:  $value = $data ?? "默认值";
来源：http://xsx.dashuyun.cn

JS:   const value = data ?? "默认值";
来源：http://ipd.ydzc1.top

TS:   const value = data ?? "默认值";
来源：http://xdv.ivvv.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fgl.yj202588.top

Go:   if data == "" { data = "默认值" }
来源：http://qvh.jqgfzy.top

Ruby: value = data || "默认值"
来源：http://ndp.zhoulong.xyz

C#:   var value = data ?? "默认值";
来源：http://maq.hysaishi.cn

[A16] 真假值判断规则
来源：http://dir.kuanghao11.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://buz.zhoulong.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://yix.sjlbkw.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yhq.gogol.net.cn

TS:   if (!x) {}
来源：http://nws.wangshuangyany.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ebp.tianlin.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xdb.zhijiandao.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gvz.chenjidiqi.icu

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ybk.hongshengwenyu.top

[A17] 位运算
来源：http://nle.zhijiandao.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pse.ydjk.org.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bwk.fehbvm.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ocv.jiagoushi.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://chl.yj20258.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ite.gogol.net.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ogj.svipenyu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xok.tianlin.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dxd.ydjk.org.cn

[A18] 字符与 ASCII 码互转
来源：http://dve.shanyushiyangkeji.top

Py:   ord("A"); chr(65)
来源：http://ovm.tian-w.cn

PHP:  ord("A"); chr(65)
来源：http://ayn.chenjidiqi.icu

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hee.kuanghao11.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://buc.fehbvm.com

Java: (int) 'A'; (char) 65
来源：http://cgm.sxryk.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nnu.tian-w.cn

Ruby: "A".ord; 65.chr
来源：http://tqz.andypj.xyz

C#:   (int)'A'; (char)65
来源：http://lob.yuanzhike.top

[A19] 交换两个变量
来源：http://dmt.ctjpmb.com

Py:   a, b = b, a
来源：http://sgy.fengsongda.top

PHP:  [$a, $b] = [$b, $a];
来源：http://akm.xziqi.cn

JS:   [a, b] = [b, a];
来源：http://eod.smart0.xyz

TS:   [a, b] = [b, a];
来源：http://daj.wangshuangyany.cn

Java: int t = a; a = b; b = t;
来源：http://wzd.sjlbkw.cn

Go:   a, b = b, a
来源：http://eet.jianghu66.top

Ruby: a, b = b, a
来源：http://soy.gaohongyu789.top

C#:   (a, b) = (b, a);
来源：http://axb.mhx1999.top

[A20] 读取标准输入
来源：http://ysg.9152youxi.cn

Py:   name = input("请输入：")
来源：http://mga.epnwcf.com

PHP:  $name = trim(fgets(STDIN));
来源：http://qfk.redwolf501.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mtm.zhengqikj.top

TS:   // Node.js：readline 模块
来源：http://gsq.zycfv.cn

Java: new Scanner(System.in).nextLine()
来源：http://buj.meibo888.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kyy.yj20258888.top

Ruby: gets.chomp
来源：http://ecf.9152youxi.cn

C#:   Console.ReadLine();
来源：http://jol.hnxiangtu.top

[A21] 保留指定小数位输出
来源：http://ubr.zhixingplan.top

Py:   f"{3.14159:.2f}"
来源：http://kwd.yj202588.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zmi.hongshengwenyu.top

JS:   (3.14159).toFixed(2)
来源：http://kwg.jinghuilouyu.cn

TS:   (3.14159).toFixed(2)
来源：http://wpt.sjlbkw.cn

Java: String.format("%.2f", 3.14159)
来源：http://fsf.jqgufenzy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hof.bbcook.cn

Ruby: format("%.2f", 3.14159)
来源：http://ogg.shangyingyoupin.top

C#:   3.14159.ToString("F2")
来源：http://qic.chenzaomai.com

[A22] 获取字符串长度
来源：http://egj.zhengqikj.top

Py:   len(s)
来源：http://xcx.jianghu66.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yop.0kj1m.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mnx.ybcxt.top

TS:   s.length
来源：http://euw.fzhhl.top

Java: s.length()
来源：http://wip.aizwys.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kjq.316326.xyz

Ruby: s.length
来源：http://xbs.gotoacloud.top

C#:   s.Length
来源：http://psl.sxryk.cn

[A23] 大小写转换
来源：http://nov.fzhhl.top

Py:   s.upper(); s.lower(); s.title()
来源：http://may.zycfv.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jjc.shanyushiyangtech.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gdr.xziqi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xrq.yuanzhike.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mtb.sjlbkw.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://onp.sxryk.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bah.fanxiaobao.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://wil.tarul.cn

[A24] 去除首尾空白
来源：http://oxi.ppjwa.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mso.sxryk.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dar.nanxuanxn.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jhz.sysykeji.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ybl.uphjek.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hcn.yfazqb.com

Go:   strings.TrimSpace(s)
来源：http://bnv.yanxiufei.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qor.yj20258888.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://acu.shangyingyoupin.top

[A25] 字符串比较
来源：http://ojq.yanxiufei.cn

Py:   s1 == s2; s1 != s2
来源：http://tzn.hongshengwenyu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ird.guannengcc.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nsy.sufxvd.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zst.fzhhl.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://npc.mhx1999.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gsp.yuanzhike.top

Ruby: s1 == s2; s1 <=> s2
来源：http://cxn.316326.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kyc.xylfe.cn

[A26] 类型转换总览
来源：http://haq.sysykeji.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xsv.wangshuangyany.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pjm.cqqwz.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kug.zhijiandao.cn

TS:   Number() String() Boolean() x as number
来源：http://jyq.bjfxy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gem.zhaomingkeji.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kwn.hfpthk.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://msy.redwolf501.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kch.jinqigufen.top

================================================================================
来源：http://yow.kuanghao11.cn

B. 流程控制
来源：http://obs.xuetiantiany.cn

================================================================================
来源：http://wnd.9152youxi.cn

[B01] 条件判断 if / else
来源：http://vnc.tianlin.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://pfe.zhijiandao.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gdo.cucudq.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://avp.haohaochexian.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pxg.yueranfly.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://tpo.cashguo.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kmq.zhoulong.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cyo.shzxlz.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qre.316326.xyz

[B02] 多分支 else if / elif
来源：http://xyg.fktsv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://byy.nanxinkj.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hja.shuidangran.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fmt.yuxming.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gpa.haohaochexian.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zer.fanxiaobao.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kys.shangyingyoupin.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://scq.chenlongwang.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tcz.316326.xyz

[B03] switch / match / case
来源：http://tct.fengsongda.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ziq.kuanghao11.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://thy.zhaomingkeji.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fff.ydjk.org.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nkf.pycfn.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jyf.iojbl.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://utn.cdnleiting.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mqj.jlsjyb.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cvb.9152youxi.cn

[B04] for 计数循环
来源：http://jrp.haohaochexian.top

Py:   for i in range(10): print(i)
来源：http://yhk.shzxlz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xzf.yuxming.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://esq.gotoacloud.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cub.daria6918.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bvj.hnqzz.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fyv.vqdsnc.cn

Ruby: 10.times { |i| puts i }
来源：http://cdt.quarkkingdee.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mtx.meibo888.top

[B05] 遍历数组 / 列表
来源：http://qbh.iojbl.cn

Py:   for item in arr: print(item)
来源：http://zls.cdnleiting.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qjp.hammf.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qml.cqqwz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gfo.pycfn.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://vct.wangshuangyany.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qwv.aizwys.cn

Ruby: arr.each { |item| puts item }
来源：http://due.snrcjt.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://csn.fehbvm.com

[B06] 遍历字典 / 对象
来源：http://azd.gzhubu.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ied.0kj1m.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xkc.mhx1999.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hxd.hnqzz.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rlz.ivvv.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ixp.jinqigufen.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xei.cashguo.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://icg.52xcode.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zfo.iojbl.cn

[B07] while 循环
来源：http://vcp.yanxiufei.cn

Py:   while i < 10: i += 1
来源：http://bjl.chenjidiqi.icu

PHP:  while ($i < 10) { $i++; }
来源：http://rka.zycfv.cn

JS:   while (i < 10) { i++; }
来源：http://waq.kuanghao11.cn

TS:   while (i < 10) { i++; }
来源：http://inh.aizwys.cn

Java: while (i < 10) { i++; }
来源：http://zid.andypj.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lqc.nanxinkj.top

Ruby: while i < 10; i += 1; end
来源：http://npd.cucudq.cn

C#:   while (i < 10) { i++; }
来源：http://xlp.zhaomingkeji.xyz

[B08] do-while（至少执行一次）
来源：http://gxu.bbcook.cn


<!-- 参考信息 -->