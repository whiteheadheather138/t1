代发 wailian999

Ruby: PI = 3.14159
来源：http://drn.nanxinkj.top

C#:   const double PI = 3.14159;
来源：http://jri.epnwcf.com

[A04] 判断变量类型
来源：http://xai.yanxiufei.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://eln.dianchejie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fzj.meibo888.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ala.zhongyouzk.top

TS:   typeof x; x instanceof Date
来源：http://brg.snrcjt.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ugq.sweek.top

Go:   reflect.TypeOf(x).Name()
来源：http://lvp.c1oappe.top

Ruby: x.class; x.is_a?(Integer)
来源：http://tgz.wangshuangyany.cn

C#:   x.GetType().Name; x is int
来源：http://ofk.vehdjk.com

[A05] 整数除法与取模
来源：http://cxg.birdmap.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pfs.fengsongda.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://hdj.xinyue.icu

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qid.jinghuilouyu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pqx.c1oappe.top

Java: 7 / 2; 7 % 2
来源：http://kjf.hywenlv.cn

Go:   7 / 2; 7 % 2
来源：http://mjo.sufxvd.cn

Ruby: 7 / 2; 7 % 2
来源：http://bpm.ydjk.org.cn

C#:   7 / 2; 7 % 2
来源：http://fac.gaohongyu789.top

[A06] 字符串转数字
来源：http://zrg.dashuyun.cn

Py:   int("42"); float("3.14")
来源：http://urb.gotoacloud.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://iat.bbcook.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://eja.zhiwuduotai.top

TS:   parseInt("42", 10); Number("42")
来源：http://nbg.yanxiufei.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://otp.daxiang520.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://beo.yanxiufei.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://kxr.ybcxt.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yak.ydzc1.top

[A07] 数字转字符串
来源：http://emm.havefunace.top

Py:   str(42)
来源：http://tlv.9152youxi.cn

PHP:  (string) 42; strval(42)
来源：http://gmj.jyoumei.cn

JS:   String(42); (42).toString()
来源：http://hgn.0kj1m.cn

TS:   String(42)
来源：http://yrd.ivvv.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://som.zdqjudy.top

Go:   strconv.Itoa(42)
来源：http://gkt.nwbrower.top

Ruby: 42.to_s
来源：http://vmk.redwolf501.top

C#:   42.ToString()
来源：http://end.ehwqpu.com

[A08] 取整与四舍五入
来源：http://jwl.hnqzz.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kyw.hysaishi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ewc.meibo888.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://isc.hesvh.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ehp.birdmap.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lyo.c1oappe.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ffe.bjfxy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://agh.hnxiangtu.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pei.dianchejie.cn

[A09] 绝对值与最大最小值
来源：http://jux.uphjek.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nvg.svipenyu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://uiw.hfpthk.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rrk.zhixingplan.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kvn.yonumen.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rkq.daria6918.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vvb.sweek.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xld.hnxiangtu.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wbi.redwolf501.top

[A10] 生成随机数
来源：http://poh.guowangkeji.top

Py:   import random; random.randint(1, 100)
来源：http://qyn.cucudq.cn

PHP:  random_int(1, 100);
来源：http://ylr.birdmap.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dmf.cucudq.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://kav.ctjpmb.com

Java: new Random().nextInt(100) + 1
来源：http://zay.vqdsnc.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kga.zhiwuduotai.top

Ruby: rand(1..100)
来源：http://dsi.mhx1999.top

C#:   new Random().Next(1, 101)
来源：http://mpg.daxiang520.top

[A11] 条件表达式（三元）
来源：http://stf.wangdashe.top

Py:   "yes" if x > 0 else "no"
来源：http://ivd.yj20258888.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ojq.yj202588.top

JS:   x > 0 ? "yes" : "no"
来源：http://kqf.tarul.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dro.yfazqb.com

Java: x > 0 ? "yes" : "no"
来源：http://tjv.smart0.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://vog.0kj1m.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://zqu.bjfxy.top

C#:   x > 0 ? "yes" : "no"
来源：http://ukd.316326.xyz

[A12] 字符串插值 / 格式化
来源：http://grx.yuanzhike.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ryl.haohaochexian.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://feu.andypj.xyz

JS:   `Hello, ${name}!`
来源：http://ktb.bbcook.cn

TS:   `Hello, ${name}!`
来源：http://pxo.sufxvd.cn

Java: "Hello, %s!".formatted(name)
来源：http://bfe.wangshuangyany.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gpd.xziqi.cn

Ruby: "Hello, #{name}!"
来源：http://fxb.zhijiandao.cn

C#:   $"Hello, {name}!"
来源：http://ptp.jlsjyb.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://kqk.jqgufenzy.top

Py:   "第一行\n第二行"
来源：http://sso.hcnkem.com

PHP:  "第一行\n第二行"
来源：http://rmo.ehwqpu.com

JS:   "第一行\n第二行"
来源：http://iyr.iojbl.cn

TS:   "第一行\n第二行"
来源：http://xnx.yanxiufei.cn

Java: "第一行\n第二行"
来源：http://dvq.zhaomingkeji.xyz

Go:   "第一行\n第二行"
来源：http://kxp.sufxvd.cn

Ruby: "第一行\n第二行"
来源：http://mwr.fehbvm.com

C#:   "第一行\n第二行"
来源：http://hmx.gotoacloud.top

[A14] 注释写法
来源：http://knj.pengpengdd.cyou

Py:   # 单行；三引号字符串可作多行说明
来源：http://rot.cdnleiting.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://smr.chenlongwang.top

JS:   // 单行；/* 多行 */
来源：http://moa.sjlbkw.cn

TS:   // 单行；/* 多行 */
来源：http://ijx.hnqzz.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kps.hywenlv.cn

Go:   // 单行；/* 多行 */
来源：http://tzv.52xcode.cn

Ruby: # 单行；=begin 多行 =end
来源：http://knn.redwolf501.top

C#:   // 单行；/* 多行 */
来源：http://zqk.wangshuangyany.cn

[A15] 空值判断与默认值
来源：http://uan.xuetiantiany.cn

Py:   value = data or "默认值"
来源：http://fwv.daria6918.cn

PHP:  $value = $data ?? "默认值";
来源：http://kne.yueranfly.top

JS:   const value = data ?? "默认值";
来源：http://vrh.ctjpmb.com

TS:   const value = data ?? "默认值";
来源：http://ozi.aibaodan.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rum.gaohongyu789.top

Go:   if data == "" { data = "默认值" }
来源：http://uce.shuidangran.top

Ruby: value = data || "默认值"
来源：http://fnu.fehbvm.com

C#:   var value = data ?? "默认值";
来源：http://srn.wangdashe.top

[A16] 真假值判断规则
来源：http://xgc.c1oappe.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ngd.wangdashe.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://eiy.feifeiyinyue.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fth.ivvv.top

TS:   if (!x) {}
来源：http://ipu.daxiang520.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mrs.sweek.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ril.zhijiandao.cn

Ruby: unless x            # nil 与 false 为假
来源：http://nnu.vqdsnc.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mxy.andypj.xyz

[A17] 位运算
来源：http://vdi.yfazqb.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kiz.hcnkem.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zhb.chenzaomai.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vos.jqgfzy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bne.shangyingyoupin.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ogu.ehwqpu.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://szk.sjlbkw.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://flz.shuidangran.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wte.sufxvd.cn

[A18] 字符与 ASCII 码互转
来源：http://onu.dianchejie.cn

Py:   ord("A"); chr(65)
来源：http://fyg.aibaodan.cn

PHP:  ord("A"); chr(65)
来源：http://dei.gaohongyu789.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lzn.shuidangran.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cqh.gzhubu.top

Java: (int) 'A'; (char) 65
来源：http://kdt.yuxming.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rfm.tarul.cn

Ruby: "A".ord; 65.chr
来源：http://hfb.shzxlz.cn

C#:   (int)'A'; (char)65
来源：http://xef.yueranfly.top

[A19] 交换两个变量
来源：http://qav.yangfankeji.com

Py:   a, b = b, a
来源：http://ieb.zhaomingkeji.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://sng.fanxiaobao.xyz

JS:   [a, b] = [b, a];
来源：http://dta.aibaodan.cn

TS:   [a, b] = [b, a];
来源：http://cjr.ywan-chungtsiang.top

Java: int t = a; a = b; b = t;
来源：http://pvf.nanxinkj.top

Go:   a, b = b, a
来源：http://pap.pycfn.com

Ruby: a, b = b, a
来源：http://upw.xuetiantiany.cn

C#:   (a, b) = (b, a);
来源：http://wvx.fehbvm.com

[A20] 读取标准输入
来源：http://fim.fzhhl.top

Py:   name = input("请输入：")
来源：http://wfg.shanyushiyangtech.top

PHP:  $name = trim(fgets(STDIN));
来源：http://yub.0kj1m.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://smp.shzxlz.cn

TS:   // Node.js：readline 模块
来源：http://iqk.svipenyu.cn

Java: new Scanner(System.in).nextLine()
来源：http://zsr.0kj1m.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zfs.yj202588.top

Ruby: gets.chomp
来源：http://lxy.havefunace.top

C#:   Console.ReadLine();
来源：http://hqp.zhiwuduotai.top

[A21] 保留指定小数位输出
来源：http://ace.jianghu66.top

Py:   f"{3.14159:.2f}"
来源：http://bhs.dashuyun.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bcv.fehbvm.com

JS:   (3.14159).toFixed(2)
来源：http://exj.bjfxy.top

TS:   (3.14159).toFixed(2)
来源：http://ecz.xinyue.icu

Java: String.format("%.2f", 3.14159)
来源：http://mez.zhiwuduotai.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pvx.hfpthk.cn

Ruby: format("%.2f", 3.14159)
来源：http://vlo.jianghu66.top

C#:   3.14159.ToString("F2")
来源：http://xxf.yj202588.top

[A22] 获取字符串长度
来源：http://pni.aizwys.cn

Py:   len(s)
来源：http://heu.pengpengdd.cyou

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ddl.yuxming.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hrc.smart0.xyz

TS:   s.length
来源：http://oiu.andypj.xyz

Java: s.length()
来源：http://gop.shanyushiyangtech.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://box.tian-w.cn

Ruby: s.length
来源：http://klj.gogol.net.cn

C#:   s.Length
来源：http://bom.zycfv.cn

[A23] 大小写转换
来源：http://qbv.ctjpmb.com

Py:   s.upper(); s.lower(); s.title()
来源：http://lom.tanke756.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qqe.redwolf501.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ltj.ywan-chungtsiang.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fxn.yj20258.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vyx.ybcxt.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://igs.zycfv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xiy.chenjidiqi.icu

C#:   s.ToUpper(); s.ToLower()
来源：http://xbt.aizwys.cn

[A24] 去除首尾空白
来源：http://itt.xylfe.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xlj.feifeiyinyue.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://aql.c1oappe.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pmu.9152youxi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://swb.hammf.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://arc.xinyue.icu

Go:   strings.TrimSpace(s)
来源：http://wwv.hongshengwenyu.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hkq.ppjwa.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bje.pengpengdd.cyou

[A25] 字符串比较
来源：http://xvz.hnqzz.top

Py:   s1 == s2; s1 != s2
来源：http://xoa.9152youxi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bxl.sysykeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ude.shzxlz.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mxj.shanyushiyangtech.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gye.cqqwz.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pok.0kj1m.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://fxt.chenlongwang.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tsj.jiagoushi.top

[A26] 类型转换总览
来源：http://mtl.shanyushiyangkeji.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ukb.jinghuilouyu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xfo.gaohongyu789.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ahi.yuxming.cn

TS:   Number() String() Boolean() x as number
来源：http://kck.jlsjyb.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dwv.tianlin.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://khq.zhijiandao.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://tyh.ehwqpu.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hkc.zhoulong.xyz

================================================================================
来源：http://pas.jianghu66.top

B. 流程控制
来源：http://yoe.fengsongda.top

================================================================================
来源：http://srq.guowangkeji.top

[B01] 条件判断 if / else
来源：http://brt.pycfn.com

Py:   result = "正" if x > 0 else "非正"
来源：http://eqf.nwbrower.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fbl.hnxiangtu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://oze.birdmap.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xvb.pycfn.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://nfw.gogol.net.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ara.tianlin.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vpj.tanke756.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pit.shangyingyoupin.top

[B02] 多分支 else if / elif
来源：http://erv.9152youxi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qbw.zdbjq.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dkj.gzhubu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ksk.yanxiufei.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vbr.ppjwa.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iuc.9152youxi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kru.fengsongda.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kkz.epnwcf.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nua.zhoulong.xyz

[B03] switch / match / case
来源：http://tum.xuanzx.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bci.tian-w.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kpv.zdqjudy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lru.nanxuanxn.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nkg.fehbvm.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wrx.hongshengwenyu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sbe.haohaochexian.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://isv.yonumen.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uze.xuetiantiany.cn

[B04] for 计数循环
来源：http://zhb.zhijiandao.cn

Py:   for i in range(10): print(i)
来源：http://jvt.yueranfly.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://afq.xuanzx.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xqb.smart0.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tgu.yonumen.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://esd.yonumen.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jux.uphjek.com

Ruby: 10.times { |i| puts i }
来源：http://qsr.kuanghao11.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://clc.ydzc1.top

[B05] 遍历数组 / 列表
来源：http://aso.gaohongyu789.top

Py:   for item in arr: print(item)
来源：http://hdd.dianchejie.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ckt.wangshuangyany.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://itw.zhixingplan.top

TS:   for (const item of arr) { console.log(item); }
来源：http://lzm.daria6918.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wae.yanxiufei.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cmf.jinqigfzy.top

Ruby: arr.each { |item| puts item }
来源：http://bct.chenjidiqi.icu

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wnq.52xcode.cn

[B06] 遍历字典 / 对象
来源：http://crf.yuxming.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rkd.gaohongyu789.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://grt.yj20258888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dlp.shanyushiyangkeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://din.smart0.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tpu.smart0.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://quo.ehwqpu.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qdf.sjlbkw.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://faq.quarkkingdee.top

[B07] while 循环
来源：http://sqs.yfazqb.com

Py:   while i < 10: i += 1
来源：http://fog.316326.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://vaa.bjfxy.top

JS:   while (i < 10) { i++; }
来源：http://wdk.nanxinkj.top

TS:   while (i < 10) { i++; }
来源：http://jwp.zhixingplan.top

Java: while (i < 10) { i++; }
来源：http://zdz.tianlin.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dsk.yfazqb.com

Ruby: while i < 10; i += 1; end
来源：http://mam.wangshuangyany.cn

C#:   while (i < 10) { i++; }
来源：http://eyv.pengpengdd.cyou

[B08] do-while（至少执行一次）
来源：http://lrv.ctjpmb.com

Py:   # 无 do-while：用 while True + break
来源：http://rwa.yuanzhike.top

PHP:  do { $i++; } while ($i < 10);
来源：http://qwr.fzhhl.top

JS:   do { i++; } while (i < 10);
来源：http://bsi.jyoumei.cn

TS:   do { i++; } while (i < 10);
来源：http://jtc.xingfuxueyuan.xyz

Java: do { i++; } while (i < 10);
来源：http://jil.hcnkem.com

Go:   for { i++; if i >= 10 { break } }
来源：http://xhu.zycfv.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vxq.tianlin.xyz

C#:   do { i++; } while (i < 10);
来源：http://hye.kuanghao11.cn

[B09] break 与 continue
来源：http://tzd.ctjpmb.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://whv.vehdjk.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sfl.cashguo.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ojn.shanyushiyangkeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nab.sjlbkw.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cet.yanxiufei.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bws.ydzc1.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xex.wangdashe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://msn.jinyuanbaomall.cn

[B10] 遍历同时拿索引
来源：http://tkx.ydzc1.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nxf.aibaodan.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dmo.zhongyouzk.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lkk.yj202588.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nin.yvedp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://olt.hnqzz.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://scu.sysykeji.top


<!-- 参考信息 -->