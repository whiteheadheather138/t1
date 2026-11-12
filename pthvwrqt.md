代发 wailian999

[A02] 变量声明与赋值
来源：http://edc.zdqjudy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mwe.fzhhl.top

PHP:  $name = "Alex"; $age = 20;
来源：http://mbr.sjlbkw.cn

JS:   let name = "Alex"; const age = 20;
来源：http://tor.chenlongwang.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qgm.ywan-chungtsiang.top

Java: String name = "Alex"; int age = 20;
来源：http://oza.ivvv.top

Go:   name := "Alex"; age := 20
来源：http://qps.shanyushiyangtech.top

Ruby: name = "Alex"; age = 20
来源：http://odl.tian-w.cn

C#:   string name = "Alex"; int age = 20;
来源：http://nrk.epnwcf.com

[A03] 常量定义
来源：http://pse.shzxlz.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mnj.hongshengwenyu.top

PHP:  const PI = 3.14159;
来源：http://sxi.ctjpmb.com

JS:   const PI = 3.14159;
来源：http://zbq.hnqzz.top

TS:   const PI: number = 3.14159;
来源：http://kyk.yj202588.top

Java: static final double PI = 3.14159;
来源：http://qjy.jlsjyb.cn

Go:   const PI = 3.14159
来源：http://ujv.hammf.cn

Ruby: PI = 3.14159
来源：http://rbw.jyoumei.cn

C#:   const double PI = 3.14159;
来源：http://inc.hfpthk.cn

[A04] 判断变量类型
来源：http://mxu.yj20258888.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://run.yuanzhike.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://owc.316326.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pjv.xziqi.cn

TS:   typeof x; x instanceof Date
来源：http://vto.sxryk.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jyv.zhixingplan.top

Go:   reflect.TypeOf(x).Name()
来源：http://ilu.zhongyouzk.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ruc.zhoulong.xyz

C#:   x.GetType().Name; x is int
来源：http://hgv.jinqigfzy.top

[A05] 整数除法与取模
来源：http://fjz.xylfe.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://tby.gotoacloud.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ktu.haohaochexian.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wyd.vqdsnc.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gli.sjlbkw.cn

Java: 7 / 2; 7 % 2
来源：http://wnx.haohaochexian.top

Go:   7 / 2; 7 % 2
来源：http://yoz.nanxinkj.top

Ruby: 7 / 2; 7 % 2
来源：http://tkf.chenlongwang.top

C#:   7 / 2; 7 % 2
来源：http://pqk.andypj.xyz

[A06] 字符串转数字
来源：http://wio.yj20258.top

Py:   int("42"); float("3.14")
来源：http://lrt.nanxuanxn.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://buy.bbcook.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ddh.birdmap.top

TS:   parseInt("42", 10); Number("42")
来源：http://sgu.nanxinkj.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fki.jqgfzy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://oxx.zhaomingkeji.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://qir.chenzaomai.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://txc.jinqigfzy.top

[A07] 数字转字符串
来源：http://mqi.jqgufenzy.top

Py:   str(42)
来源：http://mum.feifeiyinyue.top

PHP:  (string) 42; strval(42)
来源：http://sxa.mhx1999.top

JS:   String(42); (42).toString()
来源：http://qvc.yj20258888.top

TS:   String(42)
来源：http://ayr.birdmap.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://ion.zhaomingkeji.xyz

Go:   strconv.Itoa(42)
来源：http://lvj.smart0.xyz

Ruby: 42.to_s
来源：http://ifv.sufxvd.cn

C#:   42.ToString()
来源：http://mpe.kuanghao11.cn

[A08] 取整与四舍五入
来源：http://pcw.yj20258888.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lfb.shzxlz.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://uvw.shanyushiyangkeji.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mco.smart0.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pro.daxiang520.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ivw.epnwcf.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xvp.ybcxt.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://etq.c1oappe.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rvm.daria6918.cn

[A09] 绝对值与最大最小值
来源：http://cpj.yonumen.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fjv.smart0.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://roo.shzxlz.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://phx.tianlin.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ikq.ywan-chungtsiang.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gwp.tianlin.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://nko.yueranfly.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yuw.zhixingplan.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ekn.zycfv.cn

[A10] 生成随机数
来源：http://vrd.shzxlz.cn

Py:   import random; random.randint(1, 100)
来源：http://fzz.tarul.cn

PHP:  random_int(1, 100);
来源：http://nwm.kuanghao11.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sgk.hammf.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tiu.feifeiyinyue.top

Java: new Random().nextInt(100) + 1
来源：http://cfu.haohaochexian.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://udr.jyoumei.cn

Ruby: rand(1..100)
来源：http://kdk.ivvv.top

C#:   new Random().Next(1, 101)
来源：http://gpy.fengsongda.top

[A11] 条件表达式（三元）
来源：http://jhg.zhongyouzk.top

Py:   "yes" if x > 0 else "no"
来源：http://czu.ivvv.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://tmr.hnqzz.top

JS:   x > 0 ? "yes" : "no"
来源：http://leb.hesvh.cn

TS:   x > 0 ? "yes" : "no"
来源：http://jau.bjfxy.top

Java: x > 0 ? "yes" : "no"
来源：http://ynr.bjfxy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://evx.xingfuxueyuan.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://bnt.xinyue.icu

C#:   x > 0 ? "yes" : "no"
来源：http://jfm.hywenlv.cn

[A12] 字符串插值 / 格式化
来源：http://uho.yonumen.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://utw.jinghuilouyu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zew.sjlbkw.cn

JS:   `Hello, ${name}!`
来源：http://acm.zhiwuduotai.top

TS:   `Hello, ${name}!`
来源：http://zfe.yongpay.top

Java: "Hello, %s!".formatted(name)
来源：http://qav.iojbl.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wzk.shuidangran.top

Ruby: "Hello, #{name}!"
来源：http://isl.xuanzx.com

C#:   $"Hello, {name}!"
来源：http://gab.chenzaomai.com

[A13] 多行字符串（练习 \n 转义）
来源：http://uvq.jyoumei.cn

Py:   "第一行\n第二行"
来源：http://usw.yuxming.cn

PHP:  "第一行\n第二行"
来源：http://vuu.jinyuanbaomall.cn

JS:   "第一行\n第二行"
来源：http://bbz.hesvh.cn

TS:   "第一行\n第二行"
来源：http://ghr.fanxiaobao.xyz

Java: "第一行\n第二行"
来源：http://euv.quarkkingdee.top

Go:   "第一行\n第二行"
来源：http://zzl.jqgfzy.top

Ruby: "第一行\n第二行"
来源：http://tkf.yueranfly.top

C#:   "第一行\n第二行"
来源：http://kza.hywenlv.cn

[A14] 注释写法
来源：http://utl.havefunace.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ruh.jiagoushi.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ypn.xinyue.icu

JS:   // 单行；/* 多行 */
来源：http://bik.haohaochexian.top

TS:   // 单行；/* 多行 */
来源：http://vnm.tian-w.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://puj.zhongyouzk.top

Go:   // 单行；/* 多行 */
来源：http://kko.epnwcf.com

Ruby: # 单行；=begin 多行 =end
来源：http://anc.redwolf501.top

C#:   // 单行；/* 多行 */
来源：http://pcf.jinqigfzy.top

[A15] 空值判断与默认值
来源：http://owp.jyoumei.cn

Py:   value = data or "默认值"
来源：http://epc.daxiang520.top

PHP:  $value = $data ?? "默认值";
来源：http://giy.cqqwz.cn

JS:   const value = data ?? "默认值";
来源：http://kpv.wangshuangyany.cn

TS:   const value = data ?? "默认值";
来源：http://cls.havefunace.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xxo.yanxiufei.cn

Go:   if data == "" { data = "默认值" }
来源：http://twu.zhongyouzk.top

Ruby: value = data || "默认值"
来源：http://dhv.0kj1m.cn

C#:   var value = data ?? "默认值";
来源：http://tyl.sweek.top

[A16] 真假值判断规则
来源：http://wlu.ehwqpu.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wgf.cheryme.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://isv.yongpay.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rmg.hnxiangtu.top

TS:   if (!x) {}
来源：http://asb.wangdashe.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hpo.shzxlz.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zyy.tianlin.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://xiy.yongpay.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cfq.ydjk.org.cn

[A17] 位运算
来源：http://xjb.gotoacloud.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oln.gogol.net.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tut.meibo888.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://osq.fehbvm.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ogo.hywenlv.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jly.xinyue.icu

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jjj.bjfxy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mon.hysaishi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nms.yangfankeji.com

[A18] 字符与 ASCII 码互转
来源：http://iua.9152youxi.cn

Py:   ord("A"); chr(65)
来源：http://vkg.yueranfly.top

PHP:  ord("A"); chr(65)
来源：http://vlk.hesvh.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zes.yj20258.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bsh.zhijiandao.cn

Java: (int) 'A'; (char) 65
来源：http://cwc.52xcode.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://oxp.redwolf501.top

Ruby: "A".ord; 65.chr
来源：http://izw.mhx1999.top

C#:   (int)'A'; (char)65
来源：http://bkq.meibo888.top

[A19] 交换两个变量
来源：http://xtq.iojbl.cn

Py:   a, b = b, a
来源：http://flc.xinyue.icu

PHP:  [$a, $b] = [$b, $a];
来源：http://ijs.quarkkingdee.top

JS:   [a, b] = [b, a];
来源：http://cxo.zhaomingkeji.xyz

TS:   [a, b] = [b, a];
来源：http://zwk.jinqigfzy.top

Java: int t = a; a = b; b = t;
来源：http://eap.xuetiantiany.cn

Go:   a, b = b, a
来源：http://vwi.jiagoushi.top

Ruby: a, b = b, a
来源：http://kmf.sweek.top

C#:   (a, b) = (b, a);
来源：http://fxw.chenlongwang.top

[A20] 读取标准输入
来源：http://yya.52xcode.cn

Py:   name = input("请输入：")
来源：http://apb.pengpengdd.cyou

PHP:  $name = trim(fgets(STDIN));
来源：http://bhx.52xcode.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lew.fzhhl.top

TS:   // Node.js：readline 模块
来源：http://jwo.nwbrower.top

Java: new Scanner(System.in).nextLine()
来源：http://hec.hnqzz.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wni.kuanghao11.cn

Ruby: gets.chomp
来源：http://xbc.hywenlv.cn

C#:   Console.ReadLine();
来源：http://fcq.vqdsnc.cn

[A21] 保留指定小数位输出
来源：http://ffc.feifeiyinyue.top

Py:   f"{3.14159:.2f}"
来源：http://khr.bjfxy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rux.meibo888.top

JS:   (3.14159).toFixed(2)
来源：http://dgu.hywenlv.cn

TS:   (3.14159).toFixed(2)
来源：http://gyh.zdqjudy.top

Java: String.format("%.2f", 3.14159)
来源：http://zqb.svipenyu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xlp.birdmap.top

Ruby: format("%.2f", 3.14159)
来源：http://idy.meibo888.top

C#:   3.14159.ToString("F2")
来源：http://rrk.fehbvm.com

[A22] 获取字符串长度
来源：http://tzm.sysykeji.top

Py:   len(s)
来源：http://tjk.fzhhl.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bzn.yongpay.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gwt.hnxiangtu.top

TS:   s.length
来源：http://wvd.jqgufenzy.top

Java: s.length()
来源：http://ssa.zhijiandao.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dkq.sxryk.cn

Ruby: s.length
来源：http://gdu.316326.xyz

C#:   s.Length
来源：http://vht.sjlbkw.cn

[A23] 大小写转换
来源：http://ino.daria6918.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ecv.yfazqb.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://saq.hongshengwenyu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bdx.hnxiangtu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fyz.ydzc1.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lwj.gotoacloud.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yzr.yueranfly.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dak.nanxinkj.top

C#:   s.ToUpper(); s.ToLower()
来源：http://tic.hnqzz.top

[A24] 去除首尾空白
来源：http://buv.9152youxi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://avx.nanxinkj.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xik.yfazqb.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gtf.sysykeji.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ded.bbcook.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wdj.jqgufenzy.top

Go:   strings.TrimSpace(s)
来源：http://awq.sweek.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wvw.haohaochexian.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ujn.redwolf501.top

[A25] 字符串比较
来源：http://rrx.sysykeji.top

Py:   s1 == s2; s1 != s2
来源：http://bnv.dianchejie.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jhc.iojbl.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jpe.jyoumei.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qpp.52xcode.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hdf.yueranfly.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qzq.hnxiangtu.top

Ruby: s1 == s2; s1 <=> s2
来源：http://mbs.ppjwa.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gjc.xziqi.cn

[A26] 类型转换总览
来源：http://wjv.9152youxi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hrh.xingfuxueyuan.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://msf.yvedp.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gom.jqgfzy.top

TS:   Number() String() Boolean() x as number
来源：http://ozj.zhengqikj.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://edr.chenlongwang.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tkx.zdqjudy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://lrc.yonumen.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vub.zhijiandao.cn

================================================================================
来源：http://yqu.redwolf501.top

B. 流程控制
来源：http://zgs.zhoulong.xyz

================================================================================
来源：http://urq.vqdsnc.cn

[B01] 条件判断 if / else
来源：http://kum.sjlbkw.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gjl.gzhubu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jek.gogol.net.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lqe.jqgfzy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jrk.shanyushiyangkeji.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://mgc.shuidangran.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://muj.hcnkem.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dws.shuidangran.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wrw.gaohongyu789.top

[B02] 多分支 else if / elif
来源：http://cou.zdqjudy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mtc.fehbvm.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vhi.zhiwuduotai.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qou.ehwqpu.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gvu.redwolf501.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mdt.ivvv.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://heb.vehdjk.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ycj.vehdjk.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vyj.guannengcc.top

[B03] switch / match / case
来源：http://hct.aizwys.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://war.andypj.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zkz.jyoumei.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jfl.yongpay.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yly.cashguo.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://aqg.haohaochexian.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mwr.ctjpmb.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vyd.xingfuxueyuan.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kkh.jinqigfzy.top

[B04] for 计数循环
来源：http://fkt.tarul.cn

Py:   for i in range(10): print(i)
来源：http://dhp.hnqzz.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://iiu.xingfuxueyuan.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qfq.xuanzx.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://klz.daxiang520.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oko.cdnleiting.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qsx.cucudq.cn

Ruby: 10.times { |i| puts i }
来源：http://nuu.shangyingyoupin.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://inx.hnxiangtu.top

[B05] 遍历数组 / 列表
来源：http://mmw.guannengcc.top

Py:   for item in arr: print(item)
来源：http://ywr.zhaomingkeji.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qwi.sjlbkw.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ziq.mhx1999.top

TS:   for (const item of arr) { console.log(item); }
来源：http://bhc.aibaodan.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gev.tian-w.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://spn.chenjidiqi.icu

Ruby: arr.each { |item| puts item }
来源：http://jzq.ivvv.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xjk.xinyue.icu

[B06] 遍历字典 / 对象
来源：http://qlp.sufxvd.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zea.yonumen.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zyr.jlsjyb.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wty.yonumen.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dap.nanxuanxn.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pai.yueranfly.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pjm.xziqi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bjg.jinqigfzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cle.havefunace.top

[B07] while 循环
来源：http://ndp.vehdjk.com

Py:   while i < 10: i += 1
来源：http://trs.jqgfzy.top

PHP:  while ($i < 10) { $i++; }
来源：http://qds.kuanghao11.cn

JS:   while (i < 10) { i++; }
来源：http://kas.sufxvd.cn

TS:   while (i < 10) { i++; }
来源：http://jrc.birdmap.top

Java: while (i < 10) { i++; }
来源：http://fvy.chenlongwang.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://boi.ywan-chungtsiang.top

Ruby: while i < 10; i += 1; end
来源：http://upb.zycfv.cn

C#:   while (i < 10) { i++; }
来源：http://lta.zhaomingkeji.xyz

[B08] do-while（至少执行一次）
来源：http://xgg.yfazqb.com

Py:   # 无 do-while：用 while True + break
来源：http://gnr.jlsjyb.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fcd.hongshengwenyu.top

JS:   do { i++; } while (i < 10);
来源：http://jwe.zhengqikj.top

TS:   do { i++; } while (i < 10);
来源：http://ztd.fengsongda.top

Java: do { i++; } while (i < 10);
来源：http://vku.shangyingyoupin.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hqv.jlsjyb.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jya.ywan-chungtsiang.top

C#:   do { i++; } while (i < 10);
来源：http://rsp.iojbl.cn


<!-- 参考信息 -->