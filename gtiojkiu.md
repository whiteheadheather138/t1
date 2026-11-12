代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://ceb.jyoumei.cn

Go:   fmt.Println("Hello, World!")
来源：http://key.cdnleiting.top

Ruby: puts "Hello, World!"
来源：http://txz.hnxiangtu.top

C#:   Console.WriteLine("Hello, World!");
来源：http://urk.chenlongwang.top

[A02] 变量声明与赋值
来源：http://zau.vqdsnc.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qea.jinghuilouyu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://jja.jqgfzy.top

JS:   let name = "Alex"; const age = 20;
来源：http://udp.gogol.net.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gmh.shzxlz.cn

Java: String name = "Alex"; int age = 20;
来源：http://mvz.aibaodan.cn

Go:   name := "Alex"; age := 20
来源：http://zrs.tianlin.xyz

Ruby: name = "Alex"; age = 20
来源：http://gys.ctjpmb.com

C#:   string name = "Alex"; int age = 20;
来源：http://tsa.hammf.cn

[A03] 常量定义
来源：http://toc.fanxiaobao.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ais.dashuyun.cn

PHP:  const PI = 3.14159;
来源：http://pis.zhoulong.xyz

JS:   const PI = 3.14159;
来源：http://ocs.iojbl.cn

TS:   const PI: number = 3.14159;
来源：http://oht.vqdsnc.cn

Java: static final double PI = 3.14159;
来源：http://ebf.nanxuanxn.top

Go:   const PI = 3.14159
来源：http://ptv.shangyingyoupin.top

Ruby: PI = 3.14159
来源：http://ika.nwbrower.top

C#:   const double PI = 3.14159;
来源：http://wfz.andypj.xyz

[A04] 判断变量类型
来源：http://pvo.xinyue.icu

Py:   type(x).__name__; isinstance(x, int)
来源：http://sbn.hcnkem.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hru.redwolf501.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://srk.shanyushiyangtech.top

TS:   typeof x; x instanceof Date
来源：http://phl.sysykeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://krk.fehbvm.com

Go:   reflect.TypeOf(x).Name()
来源：http://vun.zhoulong.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://oem.daxiang520.top

C#:   x.GetType().Name; x is int
来源：http://nac.hnqzz.top

[A05] 整数除法与取模
来源：http://mdo.nwbrower.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ocq.snrcjt.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fti.bjfxy.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://auc.mhx1999.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yav.hongshengwenyu.top

Java: 7 / 2; 7 % 2
来源：http://jri.jqgfzy.top

Go:   7 / 2; 7 % 2
来源：http://cdn.jlsjyb.cn

Ruby: 7 / 2; 7 % 2
来源：http://utf.yueranfly.top

C#:   7 / 2; 7 % 2
来源：http://dxv.jyoumei.cn

[A06] 字符串转数字
来源：http://wqu.gzhubu.top

Py:   int("42"); float("3.14")
来源：http://vew.fktsv.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://svt.jqgfzy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wxd.zhijiandao.cn

TS:   parseInt("42", 10); Number("42")
来源：http://yfx.hnqzz.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wpn.sxryk.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lle.uphjek.com

Ruby: "42".to_i; "3.14".to_f
来源：http://ows.bbcook.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://scu.kuanghao11.cn

[A07] 数字转字符串
来源：http://qhn.chenlongwang.top

Py:   str(42)
来源：http://kpq.zhixingplan.top

PHP:  (string) 42; strval(42)
来源：http://fie.yanxiufei.cn

JS:   String(42); (42).toString()
来源：http://hkt.cdnleiting.top

TS:   String(42)
来源：http://fwi.mhx1999.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://wwe.tianlin.xyz

Go:   strconv.Itoa(42)
来源：http://kcw.fktsv.cn

Ruby: 42.to_s
来源：http://wob.bbcook.cn

C#:   42.ToString()
来源：http://dtr.redwolf501.top

[A08] 取整与四舍五入
来源：http://miz.meibo888.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kph.yfazqb.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://irp.ydzc1.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nhk.yueranfly.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://oyy.zdqjudy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sec.jinghuilouyu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vom.hnxiangtu.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://scl.ybcxt.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sna.ctjpmb.com

[A09] 绝对值与最大最小值
来源：http://gdk.aibaodan.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xjw.zhaomingkeji.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rbo.haohaochexian.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pvg.jianghu66.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kel.fehbvm.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lby.pengpengdd.cyou

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tfk.c1oappe.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jdq.andypj.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://uak.sxryk.cn

[A10] 生成随机数
来源：http://tli.cdnleiting.top

Py:   import random; random.randint(1, 100)
来源：http://jkf.hfpthk.cn

PHP:  random_int(1, 100);
来源：http://iud.zhiwuduotai.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hry.chenlongwang.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dtz.tanke756.top

Java: new Random().nextInt(100) + 1
来源：http://ezm.sjlbkw.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://etu.birdmap.top

Ruby: rand(1..100)
来源：http://jxp.zhijiandao.cn

C#:   new Random().Next(1, 101)
来源：http://bsh.0kj1m.cn

[A11] 条件表达式（三元）
来源：http://pog.cashguo.top

Py:   "yes" if x > 0 else "no"
来源：http://zaq.fehbvm.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://hor.zhixingplan.top

JS:   x > 0 ? "yes" : "no"
来源：http://yei.sxryk.cn

TS:   x > 0 ? "yes" : "no"
来源：http://udh.tian-w.cn

Java: x > 0 ? "yes" : "no"
来源：http://kkq.yonumen.top

Go:   // 无三元运算符，需用 if 语句
来源：http://cmq.dashuyun.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jmm.cheryme.top

C#:   x > 0 ? "yes" : "no"
来源：http://uea.c1oappe.top

[A12] 字符串插值 / 格式化
来源：http://sum.nanxinkj.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hce.yvedp.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ciq.zdbjq.cn

JS:   `Hello, ${name}!`
来源：http://zlm.guowangkeji.top

TS:   `Hello, ${name}!`
来源：http://bvq.fengsongda.top

Java: "Hello, %s!".formatted(name)
来源：http://hlh.ydzc1.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://acs.ydjk.org.cn

Ruby: "Hello, #{name}!"
来源：http://yvj.fehbvm.com

C#:   $"Hello, {name}!"
来源：http://hyp.iojbl.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://cur.chenlongwang.top

Py:   "第一行\n第二行"
来源：http://qwq.bjfxy.top

PHP:  "第一行\n第二行"
来源：http://bph.xuetiantiany.cn

JS:   "第一行\n第二行"
来源：http://iil.yanxiufei.cn

TS:   "第一行\n第二行"
来源：http://sma.jlsjyb.cn

Java: "第一行\n第二行"
来源：http://opb.ivvv.top

Go:   "第一行\n第二行"
来源：http://ptn.haohaochexian.top

Ruby: "第一行\n第二行"
来源：http://vqc.epnwcf.com

C#:   "第一行\n第二行"
来源：http://oet.daxiang520.top

[A14] 注释写法
来源：http://awj.yj202588.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://jkl.haohaochexian.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://sdl.yfazqb.com

JS:   // 单行；/* 多行 */
来源：http://mju.xinyue.icu

TS:   // 单行；/* 多行 */
来源：http://qwe.ivvv.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yvw.mhx1999.top

Go:   // 单行；/* 多行 */
来源：http://ivh.birdmap.top

Ruby: # 单行；=begin 多行 =end
来源：http://zbk.zdqjudy.top

C#:   // 单行；/* 多行 */
来源：http://bjc.shuidangran.top

[A15] 空值判断与默认值
来源：http://zrm.hnqzz.top

Py:   value = data or "默认值"
来源：http://sxc.jianghu66.top

PHP:  $value = $data ?? "默认值";
来源：http://ohg.yonumen.top

JS:   const value = data ?? "默认值";
来源：http://ltt.gotoacloud.top

TS:   const value = data ?? "默认值";
来源：http://tff.sufxvd.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://uen.fehbvm.com

Go:   if data == "" { data = "默认值" }
来源：http://pad.aizwys.cn

Ruby: value = data || "默认值"
来源：http://hqx.jianghu66.top

C#:   var value = data ?? "默认值";
来源：http://bwu.fanxiaobao.xyz

[A16] 真假值判断规则
来源：http://gjg.ywan-chungtsiang.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fvc.jyoumei.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mwy.jlsjyb.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ach.aizwys.cn

TS:   if (!x) {}
来源：http://kdp.shanyushiyangtech.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://htb.jqgufenzy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rwt.pycfn.com

Ruby: unless x            # nil 与 false 为假
来源：http://hwe.fehbvm.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://amu.pycfn.com

[A17] 位运算
来源：http://bzf.aizwys.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wrz.ppjwa.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ecp.tian-w.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ape.hcnkem.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://umq.cqqwz.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hbe.nwbrower.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jwj.zdbjq.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tsh.yonumen.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fxj.hesvh.cn

[A18] 字符与 ASCII 码互转
来源：http://lag.zhijiandao.cn

Py:   ord("A"); chr(65)
来源：http://qrn.yj20258888.top

PHP:  ord("A"); chr(65)
来源：http://xby.zhaomingkeji.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lnf.zhaomingkeji.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ebp.yueranfly.top

Java: (int) 'A'; (char) 65
来源：http://rlw.nanxinkj.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yun.hysaishi.cn

Ruby: "A".ord; 65.chr
来源：http://ymn.gzhubu.top

C#:   (int)'A'; (char)65
来源：http://qva.quarkkingdee.top

[A19] 交换两个变量
来源：http://pzj.ivvv.top

Py:   a, b = b, a
来源：http://scx.yueranfly.top

PHP:  [$a, $b] = [$b, $a];
来源：http://lim.pengpengdd.cyou

JS:   [a, b] = [b, a];
来源：http://bza.zhoulong.xyz

TS:   [a, b] = [b, a];
来源：http://dzd.xylfe.cn

Java: int t = a; a = b; b = t;
来源：http://wqw.chenzaomai.com

Go:   a, b = b, a
来源：http://ovx.sufxvd.cn

Ruby: a, b = b, a
来源：http://cah.zhixingplan.top

C#:   (a, b) = (b, a);
来源：http://cxi.chenlongwang.top

[A20] 读取标准输入
来源：http://vvw.316326.xyz

Py:   name = input("请输入：")
来源：http://iqa.jinyuanbaomall.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://iug.tian-w.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://due.shuidangran.top

TS:   // Node.js：readline 模块
来源：http://hxq.yanxiufei.cn

Java: new Scanner(System.in).nextLine()
来源：http://jkd.ywan-chungtsiang.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qww.hnxiangtu.top

Ruby: gets.chomp
来源：http://fef.dianchejie.cn

C#:   Console.ReadLine();
来源：http://ljf.jinqigfzy.top

[A21] 保留指定小数位输出
来源：http://vai.gaohongyu789.top

Py:   f"{3.14159:.2f}"
来源：http://bwd.ctjpmb.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mip.hcnkem.com

JS:   (3.14159).toFixed(2)
来源：http://nbx.zdqjudy.top

TS:   (3.14159).toFixed(2)
来源：http://oya.dashuyun.cn

Java: String.format("%.2f", 3.14159)
来源：http://vat.fktsv.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://syk.gzhubu.top

Ruby: format("%.2f", 3.14159)
来源：http://ljj.nwbrower.top

C#:   3.14159.ToString("F2")
来源：http://hvy.sysykeji.top

[A22] 获取字符串长度
来源：http://fyy.jqgufenzy.top

Py:   len(s)
来源：http://juy.aibaodan.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ise.yangfankeji.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jkc.jinqigfzy.top

TS:   s.length
来源：http://vjf.yonumen.top

Java: s.length()
来源：http://gfj.smart0.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://eod.aibaodan.cn

Ruby: s.length
来源：http://fqo.jqgufenzy.top

C#:   s.Length
来源：http://myw.hywenlv.cn

[A23] 大小写转换
来源：http://qbd.ybcxt.top

Py:   s.upper(); s.lower(); s.title()
来源：http://gtx.cheryme.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ffr.wangdashe.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xns.gaohongyu789.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://obr.zhongyouzk.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rkj.birdmap.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://lix.zhoulong.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ryr.sysykeji.top

C#:   s.ToUpper(); s.ToLower()
来源：http://hes.cdnleiting.top

[A24] 去除首尾空白
来源：http://hyn.hammf.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xlf.birdmap.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qot.guannengcc.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ogs.xuetiantiany.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://llx.zycfv.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mjr.svipenyu.cn

Go:   strings.TrimSpace(s)
来源：http://gcr.nwbrower.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jkf.epnwcf.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cpo.yj20258888.top

[A25] 字符串比较
来源：http://vnf.feifeiyinyue.top

Py:   s1 == s2; s1 != s2
来源：http://nlx.bjfxy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://prn.sxryk.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ycu.zhoulong.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sos.yangfankeji.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jzd.fengsongda.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://smz.xziqi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zmp.zhongyouzk.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wbv.vehdjk.com

[A26] 类型转换总览
来源：http://dkj.cdnleiting.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cax.gaohongyu789.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baj.shanyushiyangtech.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fop.zhiwuduotai.top

TS:   Number() String() Boolean() x as number
来源：http://sbg.hfpthk.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gni.hfpthk.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://omj.hfpthk.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://tpa.chenlongwang.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vnl.yongpay.top

================================================================================
来源：http://vsw.zhixingplan.top

B. 流程控制
来源：http://ofa.zdbjq.cn

================================================================================
来源：http://cpk.yuanzhike.top

[B01] 条件判断 if / else
来源：http://kux.xuetiantiany.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://onu.shanyushiyangtech.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rsm.chenjidiqi.icu

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tan.daria6918.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rnc.jianghu66.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://rfj.chenlongwang.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xel.smart0.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://azb.sysykeji.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lat.chenzaomai.com

[B02] 多分支 else if / elif
来源：http://yyz.sjlbkw.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fha.zhongyouzk.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fmr.zhaomingkeji.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tru.daxiang520.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://syw.52xcode.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vah.epnwcf.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jfd.xziqi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vot.ppjwa.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bug.sysykeji.top

[B03] switch / match / case
来源：http://hib.sufxvd.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bzd.zhongyouzk.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://aln.birdmap.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kwd.jinqigufen.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xjz.zdqjudy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cdo.zycfv.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tqg.redwolf501.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hrw.shanyushiyangkeji.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ybk.wangdashe.top

[B04] for 计数循环
来源：http://tez.zdbjq.cn

Py:   for i in range(10): print(i)
来源：http://bge.xylfe.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kvn.jinqigfzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wwa.hcnkem.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://azh.zycfv.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qmk.zhiwuduotai.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://iml.epnwcf.com

Ruby: 10.times { |i| puts i }
来源：http://byu.andypj.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://thm.wangshuangyany.cn

[B05] 遍历数组 / 列表
来源：http://sgs.yuxming.cn

Py:   for item in arr: print(item)
来源：http://dof.wangshuangyany.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wtl.zycfv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hoc.guannengcc.top

TS:   for (const item of arr) { console.log(item); }
来源：http://nvp.epnwcf.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://gcd.chenjidiqi.icu

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ssv.daxiang520.top

Ruby: arr.each { |item| puts item }
来源：http://los.yj202588.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hyu.daxiang520.top

[B06] 遍历字典 / 对象
来源：http://gve.hnxiangtu.top

Py:   for k, v in d.items(): print(k, v)
来源：http://zmu.guowangkeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://klh.shuidangran.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://atf.hongshengwenyu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tkm.jianghu66.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://saw.jqgufenzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pth.sjlbkw.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fyy.bbcook.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iwc.sweek.top

[B07] while 循环
来源：http://mcq.xingfuxueyuan.xyz

Py:   while i < 10: i += 1
来源：http://inx.xinyue.icu

PHP:  while ($i < 10) { $i++; }
来源：http://nof.gogol.net.cn

JS:   while (i < 10) { i++; }
来源：http://prh.fehbvm.com

TS:   while (i < 10) { i++; }
来源：http://unk.xingfuxueyuan.xyz

Java: while (i < 10) { i++; }
来源：http://fuw.yj202588.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uox.shanyushiyangkeji.top

Ruby: while i < 10; i += 1; end
来源：http://xuw.zhijiandao.cn

C#:   while (i < 10) { i++; }
来源：http://fom.jqgfzy.top

[B08] do-while（至少执行一次）
来源：http://gek.nanxuanxn.top

Py:   # 无 do-while：用 while True + break
来源：http://xlu.quarkkingdee.top

PHP:  do { $i++; } while ($i < 10);
来源：http://bec.zhijiandao.cn

JS:   do { i++; } while (i < 10);
来源：http://qul.hnqzz.top

TS:   do { i++; } while (i < 10);
来源：http://plb.aibaodan.cn


<!-- 参考信息 -->