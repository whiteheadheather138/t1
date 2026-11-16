代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://ipt.iojbl.cn

[A03] 常量定义
来源：http://ubk.yfazqb.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rte.chenzaomai.com

PHP:  const PI = 3.14159;
来源：http://kqb.jqgufenzy.top

JS:   const PI = 3.14159;
来源：http://vvs.ivvv.top

TS:   const PI: number = 3.14159;
来源：http://zkq.epnwcf.com

Java: static final double PI = 3.14159;
来源：http://kpo.daria6918.cn

Go:   const PI = 3.14159
来源：http://spb.cdnleiting.top

Ruby: PI = 3.14159
来源：http://zac.aibaodan.cn

C#:   const double PI = 3.14159;
来源：http://xjn.zhengqikj.top

[A04] 判断变量类型
来源：http://yag.xingfuxueyuan.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://cua.aibaodan.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://oig.sxryk.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qnt.cheryme.top

TS:   typeof x; x instanceof Date
来源：http://qkf.zhengqikj.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qha.dianchejie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ycp.gotoacloud.top

Ruby: x.class; x.is_a?(Integer)
来源：http://hip.andypj.xyz

C#:   x.GetType().Name; x is int
来源：http://ekp.hfpthk.cn

[A05] 整数除法与取模
来源：http://jja.ybcxt.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wkf.gogol.net.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fyd.daxiang520.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mga.jiagoushi.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jxm.ctjpmb.com

Java: 7 / 2; 7 % 2
来源：http://ncl.xziqi.cn

Go:   7 / 2; 7 % 2
来源：http://uwq.wangshuangyany.cn

Ruby: 7 / 2; 7 % 2
来源：http://mhv.haohaochexian.top

C#:   7 / 2; 7 % 2
来源：http://iiy.dashuyun.cn

[A06] 字符串转数字
来源：http://awr.snrcjt.cn

Py:   int("42"); float("3.14")
来源：http://dyw.sufxvd.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xmi.dashuyun.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nih.52xcode.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ydh.xuanzx.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mcr.zdbjq.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ajz.nanxuanxn.top

Ruby: "42".to_i; "3.14".to_f
来源：http://pah.zhoulong.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bmn.hongshengwenyu.top

[A07] 数字转字符串
来源：http://nmd.wangdashe.top

Py:   str(42)
来源：http://sbq.xziqi.cn

PHP:  (string) 42; strval(42)
来源：http://uqg.yj20258.top

JS:   String(42); (42).toString()
来源：http://pwd.jianghu66.top

TS:   String(42)
来源：http://ycu.cheryme.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://iea.jqgfzy.top

Go:   strconv.Itoa(42)
来源：http://idu.sxryk.cn

Ruby: 42.to_s
来源：http://wnm.zdqjudy.top

C#:   42.ToString()
来源：http://vgr.uphjek.com

[A08] 取整与四舍五入
来源：http://ivc.tanke756.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cqb.cheryme.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ntb.fanxiaobao.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gxb.316326.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://udv.hnxiangtu.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ksx.shuidangran.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fgz.hcnkem.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://agz.ybcxt.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ejs.cashguo.top

[A09] 绝对值与最大最小值
来源：http://dxv.zhoulong.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hah.cucudq.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ndn.pycfn.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vzb.birdmap.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ifz.hysaishi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://uby.hammf.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://unh.jyoumei.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jxg.feifeiyinyue.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://eyw.zhiwuduotai.top

[A10] 生成随机数
来源：http://qzv.gotoacloud.top

Py:   import random; random.randint(1, 100)
来源：http://uro.bbcook.cn

PHP:  random_int(1, 100);
来源：http://rzc.ehwqpu.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://azo.316326.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ykh.yfazqb.com

Java: new Random().nextInt(100) + 1
来源：http://sac.52xcode.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xnv.andypj.xyz

Ruby: rand(1..100)
来源：http://agk.ctjpmb.com

C#:   new Random().Next(1, 101)
来源：http://wns.dashuyun.cn

[A11] 条件表达式（三元）
来源：http://joc.sweek.top

Py:   "yes" if x > 0 else "no"
来源：http://ozt.snrcjt.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://eyr.shanyushiyangtech.top

JS:   x > 0 ? "yes" : "no"
来源：http://sdq.zhixingplan.top

TS:   x > 0 ? "yes" : "no"
来源：http://afk.gaohongyu789.top

Java: x > 0 ? "yes" : "no"
来源：http://umn.ybcxt.top

Go:   // 无三元运算符，需用 if 语句
来源：http://vkm.zycfv.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pti.jinghuilouyu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://boz.yfazqb.com

[A12] 字符串插值 / 格式化
来源：http://yiz.zycfv.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bsu.sysykeji.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qtd.sufxvd.cn

JS:   `Hello, ${name}!`
来源：http://bdt.guannengcc.top

TS:   `Hello, ${name}!`
来源：http://cgp.svipenyu.cn

Java: "Hello, %s!".formatted(name)
来源：http://ldf.cashguo.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://zoo.fengsongda.top

Ruby: "Hello, #{name}!"
来源：http://ylz.yanxiufei.cn

C#:   $"Hello, {name}!"
来源：http://exr.xylfe.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jyw.ppjwa.cn

Py:   "第一行\n第二行"
来源：http://joa.hcnkem.com

PHP:  "第一行\n第二行"
来源：http://sri.jlsjyb.cn

JS:   "第一行\n第二行"
来源：http://xni.ivvv.top

TS:   "第一行\n第二行"
来源：http://ohs.redwolf501.top

Java: "第一行\n第二行"
来源：http://rnx.guowangkeji.top

Go:   "第一行\n第二行"
来源：http://mdv.chenlongwang.top

Ruby: "第一行\n第二行"
来源：http://ewb.zhoulong.xyz

C#:   "第一行\n第二行"
来源：http://erz.52xcode.cn

[A14] 注释写法
来源：http://feu.yvedp.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://mem.feifeiyinyue.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://mak.jyoumei.cn

JS:   // 单行；/* 多行 */
来源：http://hpt.fengsongda.top

TS:   // 单行；/* 多行 */
来源：http://ihy.zhongyouzk.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pqj.sysykeji.top

Go:   // 单行；/* 多行 */
来源：http://cfv.c1oappe.top

Ruby: # 单行；=begin 多行 =end
来源：http://mee.yj20258.top

C#:   // 单行；/* 多行 */
来源：http://dku.hnqzz.top

[A15] 空值判断与默认值
来源：http://mqd.andypj.xyz

Py:   value = data or "默认值"
来源：http://afy.wangshuangyany.cn

PHP:  $value = $data ?? "默认值";
来源：http://vje.xziqi.cn

JS:   const value = data ?? "默认值";
来源：http://ucx.gzhubu.top

TS:   const value = data ?? "默认值";
来源：http://sgr.hnqzz.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://okq.gaohongyu789.top

Go:   if data == "" { data = "默认值" }
来源：http://lex.fehbvm.com

Ruby: value = data || "默认值"
来源：http://sqf.jinqigufen.top

C#:   var value = data ?? "默认值";
来源：http://jqz.kuanghao11.cn

[A16] 真假值判断规则
来源：http://uhl.bjfxy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ecb.zycfv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ctq.haohaochexian.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lhu.xylfe.cn

TS:   if (!x) {}
来源：http://dsn.bbcook.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pyo.jqgufenzy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ypq.dianchejie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lap.ctjpmb.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fin.sufxvd.cn

[A17] 位运算
来源：http://hso.yvedp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vfx.fktsv.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bhw.yanxiufei.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xgs.daxiang520.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://duf.316326.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rou.316326.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gey.yj20258.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jas.gaohongyu789.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://min.chenlongwang.top

[A18] 字符与 ASCII 码互转
来源：http://vnx.316326.xyz

Py:   ord("A"); chr(65)
来源：http://fvl.redwolf501.top

PHP:  ord("A"); chr(65)
来源：http://boy.chenjidiqi.icu

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://krw.chenzaomai.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vgg.zhaomingkeji.xyz

Java: (int) 'A'; (char) 65
来源：http://rlm.ehwqpu.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ekq.316326.xyz

Ruby: "A".ord; 65.chr
来源：http://vgr.ehwqpu.com

C#:   (int)'A'; (char)65
来源：http://lqf.shanyushiyangtech.top

[A19] 交换两个变量
来源：http://glq.hcnkem.com

Py:   a, b = b, a
来源：http://ixj.hnxiangtu.top

PHP:  [$a, $b] = [$b, $a];
来源：http://sys.zhiwuduotai.top

JS:   [a, b] = [b, a];
来源：http://xtm.xinyue.icu

TS:   [a, b] = [b, a];
来源：http://wvf.xingfuxueyuan.xyz

Java: int t = a; a = b; b = t;
来源：http://zmw.ivvv.top

Go:   a, b = b, a
来源：http://hgs.jinqigufen.top

Ruby: a, b = b, a
来源：http://chm.c1oappe.top

C#:   (a, b) = (b, a);
来源：http://xgc.sysykeji.top

[A20] 读取标准输入
来源：http://inx.gzhubu.top

Py:   name = input("请输入：")
来源：http://rur.jqgfzy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://psf.hesvh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ojn.yongpay.top

TS:   // Node.js：readline 模块
来源：http://evi.zhaomingkeji.xyz

Java: new Scanner(System.in).nextLine()
来源：http://gwy.meibo888.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ink.yj202588.top

Ruby: gets.chomp
来源：http://grx.zhixingplan.top

C#:   Console.ReadLine();
来源：http://uov.xuetiantiany.cn

[A21] 保留指定小数位输出
来源：http://svk.guowangkeji.top

Py:   f"{3.14159:.2f}"
来源：http://yzu.fanxiaobao.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qtp.shzxlz.cn

JS:   (3.14159).toFixed(2)
来源：http://nfy.snrcjt.cn

TS:   (3.14159).toFixed(2)
来源：http://htl.yongpay.top

Java: String.format("%.2f", 3.14159)
来源：http://zcw.meibo888.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pct.gaohongyu789.top

Ruby: format("%.2f", 3.14159)
来源：http://drh.zhixingplan.top

C#:   3.14159.ToString("F2")
来源：http://xtx.ctjpmb.com

[A22] 获取字符串长度
来源：http://ozt.yj202588.top

Py:   len(s)
来源：http://obj.chenlongwang.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nyc.zhixingplan.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qgg.yj20258888.top

TS:   s.length
来源：http://gdy.zhaomingkeji.xyz

Java: s.length()
来源：http://mrd.ybcxt.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wqd.yvedp.cn

Ruby: s.length
来源：http://nno.52xcode.cn

C#:   s.Length
来源：http://aqi.xziqi.cn

[A23] 大小写转换
来源：http://lqb.pengpengdd.cyou

Py:   s.upper(); s.lower(); s.title()
来源：http://mll.tanke756.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fkh.zhaomingkeji.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lnp.zdqjudy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jde.xylfe.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://afq.yueranfly.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gec.fengsongda.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lht.quarkkingdee.top

C#:   s.ToUpper(); s.ToLower()
来源：http://nzg.jinghuilouyu.cn

[A24] 去除首尾空白
来源：http://bhj.vehdjk.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bny.kuanghao11.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://aaj.yj202588.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bop.zdqjudy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://avd.jinyuanbaomall.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://scp.nanxinkj.top

Go:   strings.TrimSpace(s)
来源：http://xsk.bbcook.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qhu.shzxlz.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vtu.xinyue.icu

[A25] 字符串比较
来源：http://dic.9152youxi.cn

Py:   s1 == s2; s1 != s2
来源：http://khz.svipenyu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rmv.jinqigufen.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ath.cqqwz.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gzg.zdqjudy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jii.zhaomingkeji.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mhv.birdmap.top

Ruby: s1 == s2; s1 <=> s2
来源：http://rtf.ywan-chungtsiang.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hqv.daria6918.cn

[A26] 类型转换总览
来源：http://cxn.jinghuilouyu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://krc.vqdsnc.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hjx.chenzaomai.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ylx.ctjpmb.com

TS:   Number() String() Boolean() x as number
来源：http://nkn.zhiwuduotai.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://loo.birdmap.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mvz.guannengcc.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://nqf.cashguo.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://toq.tian-w.cn

================================================================================
来源：http://bhk.zhixingplan.top

B. 流程控制
来源：http://zif.cqqwz.cn

================================================================================
来源：http://mmy.ydzc1.top

[B01] 条件判断 if / else
来源：http://mrg.jqgfzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://zdl.sjlbkw.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://owe.ivvv.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dlu.guannengcc.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tby.fengsongda.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://cxk.birdmap.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://iqk.ppjwa.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gjq.gotoacloud.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fsl.hongshengwenyu.top

[B02] 多分支 else if / elif
来源：http://ycj.ydjk.org.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jqq.zhixingplan.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://enm.sufxvd.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qiz.hnxiangtu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pjs.sjlbkw.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://exn.nanxinkj.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xzu.yj202588.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cwz.zhaomingkeji.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nym.sysykeji.top

[B03] switch / match / case
来源：http://boc.ybcxt.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://lqh.redwolf501.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uhi.sysykeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dco.zdqjudy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tlz.chenlongwang.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://idu.ybcxt.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://afe.gzhubu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wrt.quarkkingdee.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cem.smart0.xyz

[B04] for 计数循环
来源：http://yib.cqqwz.cn

Py:   for i in range(10): print(i)
来源：http://tkm.zhixingplan.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tai.yonumen.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bdx.jinqigfzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kef.cashguo.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jfb.svipenyu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fxm.wangshuangyany.cn

Ruby: 10.times { |i| puts i }
来源：http://lff.cqqwz.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rtd.dianchejie.cn

[B05] 遍历数组 / 列表
来源：http://fxf.jqgufenzy.top

Py:   for item in arr: print(item)
来源：http://tvm.yongpay.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jer.vehdjk.com

JS:   for (const item of arr) { console.log(item); }
来源：http://fsv.redwolf501.top

TS:   for (const item of arr) { console.log(item); }
来源：http://yqx.daxiang520.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://par.tianlin.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xyx.zhijiandao.cn

Ruby: arr.each { |item| puts item }
来源：http://qgl.fengsongda.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yoo.ydjk.org.cn

[B06] 遍历字典 / 对象
来源：http://nrv.bbcook.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qvn.316326.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zuh.hysaishi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yxh.tianlin.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ebo.quarkkingdee.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://unr.tian-w.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zop.birdmap.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zre.zhiwuduotai.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ojs.andypj.xyz

[B07] while 循环
来源：http://oym.aibaodan.cn

Py:   while i < 10: i += 1
来源：http://vgf.hongshengwenyu.top

PHP:  while ($i < 10) { $i++; }
来源：http://npj.hesvh.cn

JS:   while (i < 10) { i++; }
来源：http://dmy.cdnleiting.top

TS:   while (i < 10) { i++; }
来源：http://mip.pengpengdd.cyou

Java: while (i < 10) { i++; }
来源：http://fss.zycfv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://szt.jqgfzy.top

Ruby: while i < 10; i += 1; end
来源：http://jxb.jinqigufen.top

C#:   while (i < 10) { i++; }
来源：http://ntd.havefunace.top

[B08] do-while（至少执行一次）
来源：http://tsz.yonumen.top

Py:   # 无 do-while：用 while True + break
来源：http://gmn.tanke756.top

PHP:  do { $i++; } while ($i < 10);
来源：http://nlg.ivvv.top

JS:   do { i++; } while (i < 10);
来源：http://mrf.jianghu66.top

TS:   do { i++; } while (i < 10);
来源：http://zkc.cdnleiting.top

Java: do { i++; } while (i < 10);
来源：http://cvo.jinghuilouyu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gja.cheryme.top

Ruby: begin; i += 1; end while i < 10
来源：http://xhi.yanxiufei.cn

C#:   do { i++; } while (i < 10);
来源：http://xdm.vqdsnc.cn

[B09] break 与 continue
来源：http://krn.fzhhl.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ata.hnqzz.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rgv.tanke756.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fpa.cqqwz.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://osp.zhiwuduotai.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fxu.snrcjt.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qan.cucudq.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wtl.vqdsnc.cn


<!-- 参考信息 -->