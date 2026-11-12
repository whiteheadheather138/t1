代发 wailian999

Ruby: PI = 3.14159
来源：http://xyq.gotoacloud.top

C#:   const double PI = 3.14159;
来源：http://fwf.zhoulong.xyz

[A04] 判断变量类型
来源：http://qjm.smart0.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://ndc.hammf.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://oiq.wangshuangyany.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://voi.xylfe.cn

TS:   typeof x; x instanceof Date
来源：http://zek.jinghuilouyu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qac.hesvh.cn

Go:   reflect.TypeOf(x).Name()
来源：http://zxv.guowangkeji.top

Ruby: x.class; x.is_a?(Integer)
来源：http://jad.yvedp.cn

C#:   x.GetType().Name; x is int
来源：http://zjf.ydjk.org.cn

[A05] 整数除法与取模
来源：http://pbj.chenzaomai.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kgq.andypj.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://esk.yuxming.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lnv.bjfxy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xfq.aizwys.cn

Java: 7 / 2; 7 % 2
来源：http://lfw.chenzaomai.com

Go:   7 / 2; 7 % 2
来源：http://ffy.zhaomingkeji.xyz

Ruby: 7 / 2; 7 % 2
来源：http://ciz.hongshengwenyu.top

C#:   7 / 2; 7 % 2
来源：http://czl.fehbvm.com

[A06] 字符串转数字
来源：http://mxs.xziqi.cn

Py:   int("42"); float("3.14")
来源：http://mkv.xziqi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pkx.zhijiandao.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://shb.jqgufenzy.top

TS:   parseInt("42", 10); Number("42")
来源：http://crv.zhiwuduotai.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rst.yongpay.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qvg.ppjwa.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ufr.yanxiufei.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xkq.shuidangran.top

[A07] 数字转字符串
来源：http://cxq.xuanzx.com

Py:   str(42)
来源：http://dkn.ehwqpu.com

PHP:  (string) 42; strval(42)
来源：http://mbj.dashuyun.cn

JS:   String(42); (42).toString()
来源：http://oxc.ydzc1.top

TS:   String(42)
来源：http://hxv.jinqigufen.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://fba.shuidangran.top

Go:   strconv.Itoa(42)
来源：http://onz.yuxming.cn

Ruby: 42.to_s
来源：http://lzg.hywenlv.cn

C#:   42.ToString()
来源：http://bqf.jianghu66.top

[A08] 取整与四舍五入
来源：http://ibo.gotoacloud.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vwo.jinghuilouyu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vkn.0kj1m.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://der.jyoumei.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tqo.fzhhl.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://iwo.redwolf501.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pca.andypj.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://tkd.vehdjk.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vuk.chenlongwang.top

[A09] 绝对值与最大最小值
来源：http://tjk.xingfuxueyuan.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vgc.hywenlv.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://iyz.yuanzhike.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://osm.gzhubu.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wkj.jianghu66.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://smj.jiagoushi.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://akm.guowangkeji.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hzs.sxryk.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rrd.guannengcc.top

[A10] 生成随机数
来源：http://hkr.shanyushiyangtech.top

Py:   import random; random.randint(1, 100)
来源：http://zbx.9152youxi.cn

PHP:  random_int(1, 100);
来源：http://pqu.cashguo.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vfx.mhx1999.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hsi.sxryk.cn

Java: new Random().nextInt(100) + 1
来源：http://lit.birdmap.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tnf.redwolf501.top

Ruby: rand(1..100)
来源：http://bbr.dianchejie.cn

C#:   new Random().Next(1, 101)
来源：http://set.zhongyouzk.top

[A11] 条件表达式（三元）
来源：http://nio.andypj.xyz

Py:   "yes" if x > 0 else "no"
来源：http://xwy.jinghuilouyu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xub.gotoacloud.top

JS:   x > 0 ? "yes" : "no"
来源：http://qge.jyoumei.cn

TS:   x > 0 ? "yes" : "no"
来源：http://yfy.shangyingyoupin.top

Java: x > 0 ? "yes" : "no"
来源：http://uuz.xingfuxueyuan.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://uoi.aizwys.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vqk.nanxuanxn.top

C#:   x > 0 ? "yes" : "no"
来源：http://ghg.shzxlz.cn

[A12] 字符串插值 / 格式化
来源：http://spo.shanyushiyangkeji.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://otz.andypj.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tzz.andypj.xyz

JS:   `Hello, ${name}!`
来源：http://svy.zycfv.cn

TS:   `Hello, ${name}!`
来源：http://kpe.zdbjq.cn

Java: "Hello, %s!".formatted(name)
来源：http://lme.yonumen.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rlo.epnwcf.com

Ruby: "Hello, #{name}!"
来源：http://ybb.hnxiangtu.top

C#:   $"Hello, {name}!"
来源：http://kna.chenlongwang.top

[A13] 多行字符串（练习 \n 转义）
来源：http://rvt.hesvh.cn

Py:   "第一行\n第二行"
来源：http://zix.chenzaomai.com

PHP:  "第一行\n第二行"
来源：http://brz.daxiang520.top

JS:   "第一行\n第二行"
来源：http://vcc.pengpengdd.cyou

TS:   "第一行\n第二行"
来源：http://jyr.zdqjudy.top

Java: "第一行\n第二行"
来源：http://pch.sjlbkw.cn

Go:   "第一行\n第二行"
来源：http://nwn.jinghuilouyu.cn

Ruby: "第一行\n第二行"
来源：http://uhl.ctjpmb.com

C#:   "第一行\n第二行"
来源：http://ita.ydjk.org.cn

[A14] 注释写法
来源：http://bln.jinghuilouyu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://xel.tanke756.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://zzn.redwolf501.top

JS:   // 单行；/* 多行 */
来源：http://dem.yj20258888.top

TS:   // 单行；/* 多行 */
来源：http://hwj.zycfv.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://koa.wangdashe.top

Go:   // 单行；/* 多行 */
来源：http://ggq.yonumen.top

Ruby: # 单行；=begin 多行 =end
来源：http://qdw.aizwys.cn

C#:   // 单行；/* 多行 */
来源：http://myt.snrcjt.cn

[A15] 空值判断与默认值
来源：http://rgb.guowangkeji.top

Py:   value = data or "默认值"
来源：http://rfp.fehbvm.com

PHP:  $value = $data ?? "默认值";
来源：http://fvf.shanyushiyangkeji.top

JS:   const value = data ?? "默认值";
来源：http://afd.chenlongwang.top

TS:   const value = data ?? "默认值";
来源：http://ozg.fanxiaobao.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kox.hysaishi.cn

Go:   if data == "" { data = "默认值" }
来源：http://rlc.fehbvm.com

Ruby: value = data || "默认值"
来源：http://eci.cashguo.top

C#:   var value = data ?? "默认值";
来源：http://gnj.pycfn.com

[A16] 真假值判断规则
来源：http://avt.vehdjk.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://phf.pengpengdd.cyou

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fgv.shzxlz.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hep.snrcjt.cn

TS:   if (!x) {}
来源：http://pdv.yanxiufei.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://frl.sjlbkw.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fzo.yuanzhike.top

Ruby: unless x            # nil 与 false 为假
来源：http://vdt.andypj.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://spz.guannengcc.top

[A17] 位运算
来源：http://uue.hesvh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pwd.cheryme.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ixs.nanxinkj.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cce.hesvh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mlh.cashguo.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jnu.tanke756.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qro.yueranfly.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cjq.quarkkingdee.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wnl.aibaodan.cn

[A18] 字符与 ASCII 码互转
来源：http://ylr.hesvh.cn

Py:   ord("A"); chr(65)
来源：http://qfi.smart0.xyz

PHP:  ord("A"); chr(65)
来源：http://uck.jianghu66.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rcj.ybcxt.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oin.aizwys.cn

Java: (int) 'A'; (char) 65
来源：http://oqx.epnwcf.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://arv.nanxuanxn.top

Ruby: "A".ord; 65.chr
来源：http://sbp.pengpengdd.cyou

C#:   (int)'A'; (char)65
来源：http://qaf.hnxiangtu.top

[A19] 交换两个变量
来源：http://bgu.ywan-chungtsiang.top

Py:   a, b = b, a
来源：http://vzz.sjlbkw.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://fji.hnxiangtu.top

JS:   [a, b] = [b, a];
来源：http://hhf.xingfuxueyuan.xyz

TS:   [a, b] = [b, a];
来源：http://vsw.fktsv.cn

Java: int t = a; a = b; b = t;
来源：http://nok.chenzaomai.com

Go:   a, b = b, a
来源：http://mki.hesvh.cn

Ruby: a, b = b, a
来源：http://jio.hywenlv.cn

C#:   (a, b) = (b, a);
来源：http://zux.cqqwz.cn

[A20] 读取标准输入
来源：http://ytp.yanxiufei.cn

Py:   name = input("请输入：")
来源：http://qeg.haohaochexian.top

PHP:  $name = trim(fgets(STDIN));
来源：http://yfh.xinyue.icu

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kqf.feifeiyinyue.top

TS:   // Node.js：readline 模块
来源：http://hud.jlsjyb.cn

Java: new Scanner(System.in).nextLine()
来源：http://lgl.jqgfzy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://eus.xuanzx.com

Ruby: gets.chomp
来源：http://sxk.birdmap.top

C#:   Console.ReadLine();
来源：http://sik.zhoulong.xyz

[A21] 保留指定小数位输出
来源：http://xlq.ydjk.org.cn

Py:   f"{3.14159:.2f}"
来源：http://tqq.zhaomingkeji.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lfe.birdmap.top

JS:   (3.14159).toFixed(2)
来源：http://ofm.hongshengwenyu.top

TS:   (3.14159).toFixed(2)
来源：http://rks.jyoumei.cn

Java: String.format("%.2f", 3.14159)
来源：http://oju.zhixingplan.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uyt.guowangkeji.top

Ruby: format("%.2f", 3.14159)
来源：http://dir.aizwys.cn

C#:   3.14159.ToString("F2")
来源：http://ttf.fktsv.cn

[A22] 获取字符串长度
来源：http://hpt.zhaomingkeji.xyz

Py:   len(s)
来源：http://dzh.dianchejie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mno.xuanzx.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wcy.zdbjq.cn

TS:   s.length
来源：http://nmp.gogol.net.cn

Java: s.length()
来源：http://hpu.yuxming.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hjz.havefunace.top

Ruby: s.length
来源：http://ofb.uphjek.com

C#:   s.Length
来源：http://ium.jqgufenzy.top

[A23] 大小写转换
来源：http://szu.gotoacloud.top

Py:   s.upper(); s.lower(); s.title()
来源：http://fpl.pengpengdd.cyou

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hbd.jinghuilouyu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pgb.wangdashe.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qqg.zdbjq.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://olv.fengsongda.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rsa.quarkkingdee.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://eql.ydjk.org.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vpa.bbcook.cn

[A24] 去除首尾空白
来源：http://wqr.jinqigfzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://uqc.jlsjyb.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zpq.sysykeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mai.yongpay.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ocb.havefunace.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ucx.jinyuanbaomall.cn

Go:   strings.TrimSpace(s)
来源：http://qcg.shanyushiyangkeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wup.xuanzx.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rmi.chenjidiqi.icu

[A25] 字符串比较
来源：http://nhz.yangfankeji.com

Py:   s1 == s2; s1 != s2
来源：http://ysw.hesvh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gsf.hysaishi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://eko.haohaochexian.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ygj.jyoumei.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qcu.ybcxt.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kvs.fzhhl.top

Ruby: s1 == s2; s1 <=> s2
来源：http://juy.ywan-chungtsiang.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lmr.xziqi.cn

[A26] 类型转换总览
来源：http://yev.daxiang520.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vyh.shangyingyoupin.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jac.shangyingyoupin.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mbs.fengsongda.top

TS:   Number() String() Boolean() x as number
来源：http://zin.hammf.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hdl.sweek.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mfn.yvedp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://oec.nanxinkj.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://emw.zhijiandao.cn

================================================================================
来源：http://ydg.dianchejie.cn

B. 流程控制
来源：http://lbf.daxiang520.top

================================================================================
来源：http://sjv.tarul.cn

[B01] 条件判断 if / else
来源：http://oth.yanxiufei.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://znj.hesvh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lgy.9152youxi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fwx.hysaishi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pyy.svipenyu.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zlq.uphjek.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hvz.yangfankeji.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ssy.pycfn.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kcg.zhengqikj.top

[B02] 多分支 else if / elif
来源：http://xwa.ctjpmb.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lmw.yonumen.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://iok.wangdashe.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fch.daxiang520.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yts.guowangkeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xxn.jqgfzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uoq.yuanzhike.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cma.andypj.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iav.hnxiangtu.top

[B03] switch / match / case
来源：http://fhs.ywan-chungtsiang.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xxw.dianchejie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ooo.dianchejie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jfb.xinyue.icu

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://arw.0kj1m.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hin.cashguo.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rbe.cheryme.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yse.daxiang520.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ilw.wangdashe.top

[B04] for 计数循环
来源：http://guu.dianchejie.cn

Py:   for i in range(10): print(i)
来源：http://lql.smart0.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dia.tian-w.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lap.fehbvm.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gqh.shzxlz.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jkj.jqgfzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wjw.vehdjk.com

Ruby: 10.times { |i| puts i }
来源：http://cuz.redwolf501.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lno.bjfxy.top

[B05] 遍历数组 / 列表
来源：http://xou.hammf.cn

Py:   for item in arr: print(item)
来源：http://vzi.svipenyu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zpb.tianlin.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://yxu.haohaochexian.top

TS:   for (const item of arr) { console.log(item); }
来源：http://pux.zdbjq.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hpp.yj202588.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://foa.pycfn.com

Ruby: arr.each { |item| puts item }
来源：http://zrb.shanyushiyangkeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rya.cashguo.top

[B06] 遍历字典 / 对象
来源：http://ovt.ydjk.org.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fzn.ivvv.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://awz.zdbjq.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qjy.zhoulong.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sia.zhiwuduotai.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wyh.tian-w.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kdo.wangshuangyany.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lxc.pycfn.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mbh.uphjek.com

[B07] while 循环
来源：http://esd.cashguo.top

Py:   while i < 10: i += 1
来源：http://bfy.vqdsnc.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ilh.guannengcc.top

JS:   while (i < 10) { i++; }
来源：http://nna.zdqjudy.top

TS:   while (i < 10) { i++; }
来源：http://axa.c1oappe.top

Java: while (i < 10) { i++; }
来源：http://cni.xinyue.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wzh.havefunace.top

Ruby: while i < 10; i += 1; end
来源：http://bwo.zhengqikj.top

C#:   while (i < 10) { i++; }
来源：http://avy.tian-w.cn

[B08] do-while（至少执行一次）
来源：http://bah.tarul.cn

Py:   # 无 do-while：用 while True + break
来源：http://cwi.sjlbkw.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dtc.pengpengdd.cyou

JS:   do { i++; } while (i < 10);
来源：http://ltp.hysaishi.cn

TS:   do { i++; } while (i < 10);
来源：http://hsx.zhengqikj.top

Java: do { i++; } while (i < 10);
来源：http://egm.andypj.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://dcf.guannengcc.top

Ruby: begin; i += 1; end while i < 10
来源：http://enf.jinqigufen.top

C#:   do { i++; } while (i < 10);
来源：http://pfx.zhengqikj.top

[B09] break 与 continue
来源：http://bsc.guannengcc.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://avd.daria6918.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kcb.andypj.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://drv.sxryk.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ooz.cqqwz.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oza.ivvv.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://age.daxiang520.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wno.cqqwz.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fri.xuanzx.com

[B10] 遍历同时拿索引
来源：http://cdw.pengpengdd.cyou

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dej.guannengcc.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rtz.ydzc1.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nin.hcnkem.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wnk.meibo888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://sug.fengsongda.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://byp.vehdjk.com


<!-- 参考信息 -->