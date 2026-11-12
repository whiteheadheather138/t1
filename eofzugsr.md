代发 wailian999

[A02] 变量声明与赋值
来源：http://nwu.jinyuanbaomall.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://noe.vehdjk.com

PHP:  $name = "Alex"; $age = 20;
来源：http://edp.fanxiaobao.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://imf.ywan-chungtsiang.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pjn.epnwcf.com

Java: String name = "Alex"; int age = 20;
来源：http://fis.shanyushiyangtech.top

Go:   name := "Alex"; age := 20
来源：http://wuu.aibaodan.cn

Ruby: name = "Alex"; age = 20
来源：http://asc.tarul.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zuu.gzhubu.top

[A03] 常量定义
来源：http://mon.uphjek.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kif.cashguo.top

PHP:  const PI = 3.14159;
来源：http://ill.9152youxi.cn

JS:   const PI = 3.14159;
来源：http://xxu.gogol.net.cn

TS:   const PI: number = 3.14159;
来源：http://gis.tianlin.xyz

Java: static final double PI = 3.14159;
来源：http://ptb.jinghuilouyu.cn

Go:   const PI = 3.14159
来源：http://lhh.aizwys.cn

Ruby: PI = 3.14159
来源：http://koc.sweek.top

C#:   const double PI = 3.14159;
来源：http://tto.cashguo.top

[A04] 判断变量类型
来源：http://qtd.chenjidiqi.icu

Py:   type(x).__name__; isinstance(x, int)
来源：http://jbi.tanke756.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nik.aizwys.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rzp.haohaochexian.top

TS:   typeof x; x instanceof Date
来源：http://sme.aizwys.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kxg.yanxiufei.cn

Go:   reflect.TypeOf(x).Name()
来源：http://xan.ydzc1.top

Ruby: x.class; x.is_a?(Integer)
来源：http://hez.chenjidiqi.icu

C#:   x.GetType().Name; x is int
来源：http://gni.zhiwuduotai.top

[A05] 整数除法与取模
来源：http://zmv.gaohongyu789.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nqo.hnxiangtu.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://nen.fanxiaobao.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cab.bbcook.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://oux.shanyushiyangkeji.top

Java: 7 / 2; 7 % 2
来源：http://byw.pengpengdd.cyou

Go:   7 / 2; 7 % 2
来源：http://xrr.dianchejie.cn

Ruby: 7 / 2; 7 % 2
来源：http://mtn.jqgufenzy.top

C#:   7 / 2; 7 % 2
来源：http://udw.vehdjk.com

[A06] 字符串转数字
来源：http://sat.fengsongda.top

Py:   int("42"); float("3.14")
来源：http://tyl.gogol.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lki.tarul.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://sir.yonumen.top

TS:   parseInt("42", 10); Number("42")
来源：http://vtb.sufxvd.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ghx.shzxlz.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uww.yangfankeji.com

Ruby: "42".to_i; "3.14".to_f
来源：http://tex.fengsongda.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tkl.jinqigfzy.top

[A07] 数字转字符串
来源：http://lzk.cqqwz.cn

Py:   str(42)
来源：http://uki.fengsongda.top

PHP:  (string) 42; strval(42)
来源：http://enz.daxiang520.top

JS:   String(42); (42).toString()
来源：http://nxh.yongpay.top

TS:   String(42)
来源：http://otk.mhx1999.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://mnc.uphjek.com

Go:   strconv.Itoa(42)
来源：http://eti.ywan-chungtsiang.top

Ruby: 42.to_s
来源：http://gdu.jianghu66.top

C#:   42.ToString()
来源：http://roi.fktsv.cn

[A08] 取整与四舍五入
来源：http://kuz.yj20258888.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ypt.yj20258888.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mvy.jinqigufen.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zoa.sufxvd.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mqz.shuidangran.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lww.ybcxt.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ejx.jlsjyb.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://los.guowangkeji.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wdy.zdbjq.cn

[A09] 绝对值与最大最小值
来源：http://hmq.zhengqikj.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://evs.hfpthk.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://svi.smart0.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://spk.ybcxt.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mjj.tanke756.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ftf.zhoulong.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fgz.sweek.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://weh.xuetiantiany.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://sfj.yuxming.cn

[A10] 生成随机数
来源：http://dgy.chenlongwang.top

Py:   import random; random.randint(1, 100)
来源：http://ygb.aibaodan.cn

PHP:  random_int(1, 100);
来源：http://uje.wangdashe.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ehn.c1oappe.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xfg.fehbvm.com

Java: new Random().nextInt(100) + 1
来源：http://vmk.haohaochexian.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://son.nanxuanxn.top

Ruby: rand(1..100)
来源：http://mbx.yangfankeji.com

C#:   new Random().Next(1, 101)
来源：http://jhc.yj202588.top

[A11] 条件表达式（三元）
来源：http://tbb.iojbl.cn

Py:   "yes" if x > 0 else "no"
来源：http://hzb.yongpay.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ylr.bbcook.cn

JS:   x > 0 ? "yes" : "no"
来源：http://adj.kuanghao11.cn

TS:   x > 0 ? "yes" : "no"
来源：http://zrv.cheryme.top

Java: x > 0 ? "yes" : "no"
来源：http://nzc.jinqigfzy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://tym.jqgfzy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://kgr.shzxlz.cn

C#:   x > 0 ? "yes" : "no"
来源：http://lds.yanxiufei.cn

[A12] 字符串插值 / 格式化
来源：http://dem.birdmap.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://uqe.daria6918.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://dpc.shuidangran.top

JS:   `Hello, ${name}!`
来源：http://unt.shangyingyoupin.top

TS:   `Hello, ${name}!`
来源：http://gux.chenzaomai.com

Java: "Hello, %s!".formatted(name)
来源：http://hqn.cashguo.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ywg.yvedp.cn

Ruby: "Hello, #{name}!"
来源：http://nre.snrcjt.cn

C#:   $"Hello, {name}!"
来源：http://gkp.316326.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://jib.xziqi.cn

Py:   "第一行\n第二行"
来源：http://ygw.yj20258.top

PHP:  "第一行\n第二行"
来源：http://mov.0kj1m.cn

JS:   "第一行\n第二行"
来源：http://fbw.aibaodan.cn

TS:   "第一行\n第二行"
来源：http://zqp.sufxvd.cn

Java: "第一行\n第二行"
来源：http://qwe.fzhhl.top

Go:   "第一行\n第二行"
来源：http://bky.c1oappe.top

Ruby: "第一行\n第二行"
来源：http://ixq.jqgfzy.top

C#:   "第一行\n第二行"
来源：http://zsk.uphjek.com

[A14] 注释写法
来源：http://xyu.gaohongyu789.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://iyv.xuanzx.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://cpb.fzhhl.top

JS:   // 单行；/* 多行 */
来源：http://alw.tanke756.top

TS:   // 单行；/* 多行 */
来源：http://gnh.gotoacloud.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mra.jiagoushi.top

Go:   // 单行；/* 多行 */
来源：http://bxw.jianghu66.top

Ruby: # 单行；=begin 多行 =end
来源：http://mlu.gzhubu.top

C#:   // 单行；/* 多行 */
来源：http://lfc.jqgfzy.top

[A15] 空值判断与默认值
来源：http://wct.svipenyu.cn

Py:   value = data or "默认值"
来源：http://oud.xuanzx.com

PHP:  $value = $data ?? "默认值";
来源：http://smp.yuxming.cn

JS:   const value = data ?? "默认值";
来源：http://lre.9152youxi.cn

TS:   const value = data ?? "默认值";
来源：http://cfe.gaohongyu789.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cda.nwbrower.top

Go:   if data == "" { data = "默认值" }
来源：http://rsu.guowangkeji.top

Ruby: value = data || "默认值"
来源：http://eiv.epnwcf.com

C#:   var value = data ?? "默认值";
来源：http://kvv.dashuyun.cn

[A16] 真假值判断规则
来源：http://njf.meibo888.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xoe.ppjwa.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rod.zhengqikj.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yrw.sweek.top

TS:   if (!x) {}
来源：http://upo.fktsv.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lvy.nanxinkj.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xbm.ppjwa.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gft.andypj.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qzg.quarkkingdee.top

[A17] 位运算
来源：http://ryr.fengsongda.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wqi.bbcook.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://akr.yueranfly.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xyo.bbcook.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uld.gaohongyu789.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tyi.ybcxt.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nft.bbcook.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cqi.zhijiandao.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qdj.yueranfly.top

[A18] 字符与 ASCII 码互转
来源：http://xfk.mhx1999.top

Py:   ord("A"); chr(65)
来源：http://ntf.sweek.top

PHP:  ord("A"); chr(65)
来源：http://yth.ivvv.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ixx.hongshengwenyu.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://omx.shanyushiyangtech.top

Java: (int) 'A'; (char) 65
来源：http://pwm.nwbrower.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://suz.jinqigufen.top

Ruby: "A".ord; 65.chr
来源：http://xhn.svipenyu.cn

C#:   (int)'A'; (char)65
来源：http://uje.sweek.top

[A19] 交换两个变量
来源：http://mzz.wangshuangyany.cn

Py:   a, b = b, a
来源：http://tbu.cqqwz.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://wec.svipenyu.cn

JS:   [a, b] = [b, a];
来源：http://ofj.gotoacloud.top

TS:   [a, b] = [b, a];
来源：http://dnf.hongshengwenyu.top

Java: int t = a; a = b; b = t;
来源：http://ysl.vehdjk.com

Go:   a, b = b, a
来源：http://klf.yj202588.top

Ruby: a, b = b, a
来源：http://qfn.redwolf501.top

C#:   (a, b) = (b, a);
来源：http://gqv.ehwqpu.com

[A20] 读取标准输入
来源：http://qhq.tianlin.xyz

Py:   name = input("请输入：")
来源：http://crt.xylfe.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://agb.xuanzx.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qtb.yongpay.top

TS:   // Node.js：readline 模块
来源：http://hky.chenzaomai.com

Java: new Scanner(System.in).nextLine()
来源：http://msl.redwolf501.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vrn.shanyushiyangkeji.top

Ruby: gets.chomp
来源：http://jvw.52xcode.cn

C#:   Console.ReadLine();
来源：http://jzo.yj20258888.top

[A21] 保留指定小数位输出
来源：http://nfn.jqgufenzy.top

Py:   f"{3.14159:.2f}"
来源：http://gzs.xylfe.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://seo.xingfuxueyuan.xyz

JS:   (3.14159).toFixed(2)
来源：http://ytx.sjlbkw.cn

TS:   (3.14159).toFixed(2)
来源：http://tgc.gogol.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://qxw.xuetiantiany.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fxw.yuanzhike.top

Ruby: format("%.2f", 3.14159)
来源：http://hnr.dashuyun.cn

C#:   3.14159.ToString("F2")
来源：http://lvq.zhixingplan.top

[A22] 获取字符串长度
来源：http://zvl.feifeiyinyue.top

Py:   len(s)
来源：http://mfx.xylfe.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://epi.sxryk.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wkf.hnqzz.top

TS:   s.length
来源：http://oor.xuanzx.com

Java: s.length()
来源：http://mht.tanke756.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nwl.wangdashe.top

Ruby: s.length
来源：http://mno.316326.xyz

C#:   s.Length
来源：http://smp.xinyue.icu

[A23] 大小写转换
来源：http://huv.jlsjyb.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://adv.jqgfzy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://oua.hnxiangtu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nqp.hysaishi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://omp.yj20258888.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qwx.tanke756.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://byw.fengsongda.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nps.guowangkeji.top

C#:   s.ToUpper(); s.ToLower()
来源：http://tgq.hammf.cn

[A24] 去除首尾空白
来源：http://rmc.jqgufenzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://yyq.tarul.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://aau.zdbjq.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pqc.ivvv.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yic.daria6918.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vbp.xylfe.cn

Go:   strings.TrimSpace(s)
来源：http://eej.sweek.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tzx.hongshengwenyu.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qog.chenjidiqi.icu

[A25] 字符串比较
来源：http://zwf.ybcxt.top

Py:   s1 == s2; s1 != s2
来源：http://toa.zhoulong.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://csn.hongshengwenyu.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uqc.xingfuxueyuan.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vgb.zdqjudy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zuz.xylfe.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qge.xuanzx.com

Ruby: s1 == s2; s1 <=> s2
来源：http://khg.jinghuilouyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wps.cashguo.top

[A26] 类型转换总览
来源：http://adm.tianlin.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hhx.chenjidiqi.icu

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kxn.chenjidiqi.icu

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dlo.fzhhl.top

TS:   Number() String() Boolean() x as number
来源：http://exk.wangdashe.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gkh.quarkkingdee.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ked.ydzc1.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://nlr.cdnleiting.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xnx.aibaodan.cn

================================================================================
来源：http://gca.yanxiufei.cn

B. 流程控制
来源：http://oqb.sweek.top

================================================================================
来源：http://ipw.bjfxy.top

[B01] 条件判断 if / else
来源：http://hxs.jiagoushi.top

Py:   result = "正" if x > 0 else "非正"
来源：http://smy.9152youxi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ezk.jinghuilouyu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sps.xuanzx.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jsd.zhengqikj.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://iwb.yangfankeji.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://syi.zhengqikj.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://aqh.snrcjt.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://thv.aizwys.cn

[B02] 多分支 else if / elif
来源：http://nid.vqdsnc.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vac.havefunace.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qes.yanxiufei.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ysz.cucudq.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://myb.yongpay.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ahv.pycfn.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://glt.chenlongwang.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://oko.jinyuanbaomall.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zll.jlsjyb.cn

[B03] switch / match / case
来源：http://cnl.xylfe.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pct.fanxiaobao.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hcw.sufxvd.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ceq.shuidangran.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eun.iojbl.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jih.tarul.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vcx.shanyushiyangkeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lxm.yuxming.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cdv.316326.xyz

[B04] for 计数循环
来源：http://dqh.daria6918.cn

Py:   for i in range(10): print(i)
来源：http://yve.shuidangran.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ett.quarkkingdee.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://csj.wangshuangyany.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://igm.cucudq.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://giv.gotoacloud.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bxf.pycfn.com

Ruby: 10.times { |i| puts i }
来源：http://ifm.havefunace.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jkx.fktsv.cn

[B05] 遍历数组 / 列表
来源：http://sxf.mhx1999.top

Py:   for item in arr: print(item)
来源：http://jib.hcnkem.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rxg.pengpengdd.cyou

JS:   for (const item of arr) { console.log(item); }
来源：http://baw.sysykeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://eub.shuidangran.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://mvq.hfpthk.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fkg.redwolf501.top

Ruby: arr.each { |item| puts item }
来源：http://siq.snrcjt.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nph.zdqjudy.top

[B06] 遍历字典 / 对象
来源：http://yne.shanyushiyangkeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ohw.9152youxi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://akh.c1oappe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yqg.gaohongyu789.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sow.iojbl.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hyt.jyoumei.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kim.hongshengwenyu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gvi.chenzaomai.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://jef.guannengcc.top

[B07] while 循环
来源：http://slc.yueranfly.top

Py:   while i < 10: i += 1
来源：http://pba.yj20258.top

PHP:  while ($i < 10) { $i++; }
来源：http://kvn.svipenyu.cn

JS:   while (i < 10) { i++; }
来源：http://tcw.xziqi.cn

TS:   while (i < 10) { i++; }
来源：http://vvl.yj20258.top

Java: while (i < 10) { i++; }
来源：http://afz.jinqigufen.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nfb.hnqzz.top

Ruby: while i < 10; i += 1; end
来源：http://ram.yvedp.cn

C#:   while (i < 10) { i++; }
来源：http://bwa.sysykeji.top

[B08] do-while（至少执行一次）
来源：http://faw.jinghuilouyu.cn

Py:   # 无 do-while：用 while True + break
来源：http://dbu.jinqigfzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://pfd.hcnkem.com

JS:   do { i++; } while (i < 10);
来源：http://uzx.nanxinkj.top

TS:   do { i++; } while (i < 10);
来源：http://ibm.guowangkeji.top

Java: do { i++; } while (i < 10);
来源：http://bue.vqdsnc.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://moo.zhoulong.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://rts.tanke756.top

C#:   do { i++; } while (i < 10);
来源：http://alx.ybcxt.top


<!-- 参考信息 -->