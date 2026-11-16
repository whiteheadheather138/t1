代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://wts.tianlin.xyz

[A03] 常量定义
来源：http://zci.bbcook.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dae.fengsongda.top

PHP:  const PI = 3.14159;
来源：http://lud.quarkkingdee.top

JS:   const PI = 3.14159;
来源：http://ajx.zdbjq.cn

TS:   const PI: number = 3.14159;
来源：http://zli.ppjwa.cn

Java: static final double PI = 3.14159;
来源：http://siw.fzhhl.top

Go:   const PI = 3.14159
来源：http://lid.pycfn.com

Ruby: PI = 3.14159
来源：http://uzv.vehdjk.com

C#:   const double PI = 3.14159;
来源：http://fws.yueranfly.top

[A04] 判断变量类型
来源：http://jjr.shuidangran.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://huk.9152youxi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uhi.birdmap.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tgo.xziqi.cn

TS:   typeof x; x instanceof Date
来源：http://jex.bjfxy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rlg.fktsv.cn

Go:   reflect.TypeOf(x).Name()
来源：http://zip.chenjidiqi.icu

Ruby: x.class; x.is_a?(Integer)
来源：http://vbv.jinghuilouyu.cn

C#:   x.GetType().Name; x is int
来源：http://psi.snrcjt.cn

[A05] 整数除法与取模
来源：http://kie.fehbvm.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jgq.fanxiaobao.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://hux.sxryk.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mki.hongshengwenyu.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://leb.yj20258888.top

Java: 7 / 2; 7 % 2
来源：http://jjp.fzhhl.top

Go:   7 / 2; 7 % 2
来源：http://dri.cdnleiting.top

Ruby: 7 / 2; 7 % 2
来源：http://oev.yuxming.cn

C#:   7 / 2; 7 % 2
来源：http://aqx.cucudq.cn

[A06] 字符串转数字
来源：http://gxi.9152youxi.cn

Py:   int("42"); float("3.14")
来源：http://qxo.c1oappe.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ikp.zhijiandao.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://amo.cqqwz.cn

TS:   parseInt("42", 10); Number("42")
来源：http://rkq.ydzc1.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pib.mhx1999.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://aod.sufxvd.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://smq.quarkkingdee.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fkx.9152youxi.cn

[A07] 数字转字符串
来源：http://iql.chenlongwang.top

Py:   str(42)
来源：http://cws.shanyushiyangtech.top

PHP:  (string) 42; strval(42)
来源：http://brj.aizwys.cn

JS:   String(42); (42).toString()
来源：http://rmt.kuanghao11.cn

TS:   String(42)
来源：http://aal.chenzaomai.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://nnm.ydjk.org.cn

Go:   strconv.Itoa(42)
来源：http://era.quarkkingdee.top

Ruby: 42.to_s
来源：http://uzb.redwolf501.top

C#:   42.ToString()
来源：http://vlj.andypj.xyz

[A08] 取整与四舍五入
来源：http://wne.dashuyun.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qxd.vqdsnc.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tvk.nanxuanxn.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nwa.xuanzx.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ybi.gzhubu.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ugi.fzhhl.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nzq.snrcjt.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://bdx.ydzc1.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://inm.sufxvd.cn

[A09] 绝对值与最大最小值
来源：http://mgr.sweek.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://sto.ydjk.org.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://msf.haohaochexian.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lwg.yuanzhike.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://shj.yongpay.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://duw.jqgufenzy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qyx.svipenyu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ipm.c1oappe.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zym.vehdjk.com

[A10] 生成随机数
来源：http://ypi.yj20258888.top

Py:   import random; random.randint(1, 100)
来源：http://tyk.chenzaomai.com

PHP:  random_int(1, 100);
来源：http://kzr.snrcjt.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fso.jianghu66.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dvw.xuanzx.com

Java: new Random().nextInt(100) + 1
来源：http://rty.gotoacloud.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rcu.shanyushiyangkeji.top

Ruby: rand(1..100)
来源：http://pbt.yongpay.top

C#:   new Random().Next(1, 101)
来源：http://yzc.daria6918.cn

[A11] 条件表达式（三元）
来源：http://gbk.jinqigfzy.top

Py:   "yes" if x > 0 else "no"
来源：http://fwq.jiagoushi.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ore.zdbjq.cn

JS:   x > 0 ? "yes" : "no"
来源：http://fla.hnxiangtu.top

TS:   x > 0 ? "yes" : "no"
来源：http://vfq.jinqigufen.top

Java: x > 0 ? "yes" : "no"
来源：http://qwf.jqgfzy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ofc.ybcxt.top

Ruby: x > 0 ? "yes" : "no"
来源：http://glv.9152youxi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://nih.hcnkem.com

[A12] 字符串插值 / 格式化
来源：http://hdc.dashuyun.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vag.ybcxt.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://dby.dianchejie.cn

JS:   `Hello, ${name}!`
来源：http://wmp.yj202588.top

TS:   `Hello, ${name}!`
来源：http://slv.gogol.net.cn

Java: "Hello, %s!".formatted(name)
来源：http://nxi.xuanzx.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gdn.smart0.xyz

Ruby: "Hello, #{name}!"
来源：http://afd.sjlbkw.cn

C#:   $"Hello, {name}!"
来源：http://lyk.jyoumei.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://nja.yj202588.top

Py:   "第一行\n第二行"
来源：http://abj.9152youxi.cn

PHP:  "第一行\n第二行"
来源：http://wzo.jianghu66.top

JS:   "第一行\n第二行"
来源：http://oaz.chenlongwang.top

TS:   "第一行\n第二行"
来源：http://pmn.zdqjudy.top

Java: "第一行\n第二行"
来源：http://lzy.hongshengwenyu.top

Go:   "第一行\n第二行"
来源：http://ejf.tanke756.top

Ruby: "第一行\n第二行"
来源：http://ruf.yanxiufei.cn

C#:   "第一行\n第二行"
来源：http://vzu.tian-w.cn

[A14] 注释写法
来源：http://gpf.daxiang520.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://cdp.meibo888.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ttw.shzxlz.cn

JS:   // 单行；/* 多行 */
来源：http://hol.snrcjt.cn

TS:   // 单行；/* 多行 */
来源：http://jtn.pengpengdd.cyou

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wll.vqdsnc.cn

Go:   // 单行；/* 多行 */
来源：http://tfk.yongpay.top

Ruby: # 单行；=begin 多行 =end
来源：http://wtk.pycfn.com

C#:   // 单行；/* 多行 */
来源：http://tjt.jinghuilouyu.cn

[A15] 空值判断与默认值
来源：http://ymy.sysykeji.top

Py:   value = data or "默认值"
来源：http://dvd.jinyuanbaomall.cn

PHP:  $value = $data ?? "默认值";
来源：http://zcs.nanxinkj.top

JS:   const value = data ?? "默认值";
来源：http://ivu.xinyue.icu

TS:   const value = data ?? "默认值";
来源：http://ciq.gzhubu.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mbi.tian-w.cn

Go:   if data == "" { data = "默认值" }
来源：http://yti.gogol.net.cn

Ruby: value = data || "默认值"
来源：http://sri.xingfuxueyuan.xyz

C#:   var value = data ?? "默认值";
来源：http://psm.hysaishi.cn

[A16] 真假值判断规则
来源：http://tan.uphjek.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lht.52xcode.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kyq.xuanzx.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://asd.gogol.net.cn

TS:   if (!x) {}
来源：http://lxt.ppjwa.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://glm.jinqigfzy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fte.gogol.net.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zze.xziqi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nsu.ywan-chungtsiang.top

[A17] 位运算
来源：http://vvi.tarul.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://srp.iojbl.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rle.yangfankeji.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vmc.sjlbkw.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rhh.zhoulong.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xcc.zhijiandao.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://uaj.fanxiaobao.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gnk.yj202588.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pch.zhixingplan.top

[A18] 字符与 ASCII 码互转
来源：http://jfz.jqgfzy.top

Py:   ord("A"); chr(65)
来源：http://qgc.zhengqikj.top

PHP:  ord("A"); chr(65)
来源：http://rdo.hcnkem.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dic.havefunace.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gdh.chenjidiqi.icu

Java: (int) 'A'; (char) 65
来源：http://kuw.yj20258.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dau.zycfv.cn

Ruby: "A".ord; 65.chr
来源：http://amc.sysykeji.top

C#:   (int)'A'; (char)65
来源：http://lkj.zhixingplan.top

[A19] 交换两个变量
来源：http://gwz.jyoumei.cn

Py:   a, b = b, a
来源：http://qqm.dashuyun.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://czo.ywan-chungtsiang.top

JS:   [a, b] = [b, a];
来源：http://rmu.xuanzx.com

TS:   [a, b] = [b, a];
来源：http://yas.jlsjyb.cn

Java: int t = a; a = b; b = t;
来源：http://zkx.fengsongda.top

Go:   a, b = b, a
来源：http://mwk.daxiang520.top

Ruby: a, b = b, a
来源：http://zpr.hywenlv.cn

C#:   (a, b) = (b, a);
来源：http://osn.daxiang520.top

[A20] 读取标准输入
来源：http://owu.hesvh.cn

Py:   name = input("请输入：")
来源：http://wyt.shanyushiyangkeji.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ccm.zdbjq.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://epk.jianghu66.top

TS:   // Node.js：readline 模块
来源：http://tcd.ydjk.org.cn

Java: new Scanner(System.in).nextLine()
来源：http://kiq.xuanzx.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gfi.chenlongwang.top

Ruby: gets.chomp
来源：http://xlh.epnwcf.com

C#:   Console.ReadLine();
来源：http://wcd.sxryk.cn

[A21] 保留指定小数位输出
来源：http://qfz.cdnleiting.top

Py:   f"{3.14159:.2f}"
来源：http://opa.gotoacloud.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://edy.0kj1m.cn

JS:   (3.14159).toFixed(2)
来源：http://ffp.birdmap.top

TS:   (3.14159).toFixed(2)
来源：http://crz.sysykeji.top

Java: String.format("%.2f", 3.14159)
来源：http://dky.wangdashe.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ztc.c1oappe.top

Ruby: format("%.2f", 3.14159)
来源：http://mns.tanke756.top

C#:   3.14159.ToString("F2")
来源：http://vnm.jqgufenzy.top

[A22] 获取字符串长度
来源：http://mlv.ywan-chungtsiang.top

Py:   len(s)
来源：http://wfa.ivvv.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nae.jqgufenzy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tnd.daria6918.cn

TS:   s.length
来源：http://rko.nanxinkj.top

Java: s.length()
来源：http://hho.chenzaomai.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ikk.yuanzhike.top

Ruby: s.length
来源：http://sdk.cheryme.top

C#:   s.Length
来源：http://pfh.vqdsnc.cn

[A23] 大小写转换
来源：http://bjx.wangshuangyany.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ivx.0kj1m.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kdc.zhengqikj.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hmk.fengsongda.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zbe.yuxming.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vca.ywan-chungtsiang.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pap.shzxlz.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hof.feifeiyinyue.top

C#:   s.ToUpper(); s.ToLower()
来源：http://hsd.yfazqb.com

[A24] 去除首尾空白
来源：http://nko.fehbvm.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pxt.nwbrower.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hni.chenzaomai.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://znx.ydjk.org.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gxu.ctjpmb.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wek.zhongyouzk.top

Go:   strings.TrimSpace(s)
来源：http://qvr.nanxuanxn.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vsm.cashguo.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nkv.ppjwa.cn

[A25] 字符串比较
来源：http://cbg.aibaodan.cn

Py:   s1 == s2; s1 != s2
来源：http://dwn.uphjek.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ark.cheryme.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yqd.xinyue.icu

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gsg.shzxlz.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qfm.jinyuanbaomall.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jic.shuidangran.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ssh.fktsv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ezk.sysykeji.top

[A26] 类型转换总览
来源：http://qbe.tanke756.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ueg.ydzc1.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rqz.wangshuangyany.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hcg.yongpay.top

TS:   Number() String() Boolean() x as number
来源：http://ozl.pengpengdd.cyou

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://flz.haohaochexian.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mqm.wangdashe.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://cbe.yonumen.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://eab.hesvh.cn

================================================================================
来源：http://elr.yueranfly.top

B. 流程控制
来源：http://kzz.yueranfly.top

================================================================================
来源：http://eap.zdqjudy.top

[B01] 条件判断 if / else
来源：http://csi.tianlin.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://bxl.ivvv.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yvx.snrcjt.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yja.daxiang520.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yxo.hnqzz.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://mnx.tanke756.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xig.ywan-chungtsiang.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ccc.sysykeji.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ela.chenlongwang.top

[B02] 多分支 else if / elif
来源：http://epm.guowangkeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uzs.zhixingplan.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bhv.xziqi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rve.hywenlv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qrk.meibo888.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rne.havefunace.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dza.xuetiantiany.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jrj.sjlbkw.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nau.hnqzz.top

[B03] switch / match / case
来源：http://oeb.cucudq.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mzv.meibo888.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dru.zdbjq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fxc.dianchejie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cte.yj202588.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lhg.cashguo.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jzu.hcnkem.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dsu.vqdsnc.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zcj.tian-w.cn

[B04] for 计数循环
来源：http://xxk.nanxuanxn.top

Py:   for i in range(10): print(i)
来源：http://lgd.aizwys.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jwp.kuanghao11.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fye.cheryme.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://myd.shzxlz.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kfk.sjlbkw.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bva.shanyushiyangkeji.top

Ruby: 10.times { |i| puts i }
来源：http://pdt.yj202588.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sgj.hcnkem.com

[B05] 遍历数组 / 列表
来源：http://ntg.jinqigfzy.top

Py:   for item in arr: print(item)
来源：http://ooo.nanxuanxn.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pmh.birdmap.top

JS:   for (const item of arr) { console.log(item); }
来源：http://mik.chenlongwang.top

TS:   for (const item of arr) { console.log(item); }
来源：http://eib.ivvv.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rfw.fzhhl.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://oht.jinyuanbaomall.cn

Ruby: arr.each { |item| puts item }
来源：http://sed.iojbl.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fiv.jinqigufen.top

[B06] 遍历字典 / 对象
来源：http://zoc.fzhhl.top

Py:   for k, v in d.items(): print(k, v)
来源：http://rzs.cheryme.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rqy.dashuyun.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vya.yj20258888.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yku.snrcjt.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bgw.haohaochexian.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uqm.cucudq.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pbc.cdnleiting.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sbr.ppjwa.cn

[B07] while 循环
来源：http://sbc.fzhhl.top

Py:   while i < 10: i += 1
来源：http://ijj.zhoulong.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://vam.ywan-chungtsiang.top

JS:   while (i < 10) { i++; }
来源：http://lxu.yonumen.top

TS:   while (i < 10) { i++; }
来源：http://gcj.chenlongwang.top

Java: while (i < 10) { i++; }
来源：http://ksw.fzhhl.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sss.jianghu66.top

Ruby: while i < 10; i += 1; end
来源：http://cjn.mhx1999.top

C#:   while (i < 10) { i++; }
来源：http://dbf.quarkkingdee.top

[B08] do-while（至少执行一次）
来源：http://xwj.epnwcf.com

Py:   # 无 do-while：用 while True + break
来源：http://ema.shanyushiyangkeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://sln.yuxming.cn

JS:   do { i++; } while (i < 10);
来源：http://hwi.sweek.top

TS:   do { i++; } while (i < 10);
来源：http://ilk.guannengcc.top

Java: do { i++; } while (i < 10);
来源：http://yjb.pycfn.com

Go:   for { i++; if i >= 10 { break } }
来源：http://buw.hywenlv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://djr.shangyingyoupin.top

C#:   do { i++; } while (i < 10);
来源：http://yrc.316326.xyz

[B09] break 与 continue
来源：http://sdn.zhixingplan.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mfz.sufxvd.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mvs.daxiang520.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hyt.yj20258.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wia.vehdjk.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qei.jinqigufen.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bxm.hywenlv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yjx.yueranfly.top


<!-- 参考信息 -->