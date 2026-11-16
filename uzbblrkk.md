代发 wailian999

[A02] 变量声明与赋值
来源：http://ilr.shzxlz.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://oog.zhiwuduotai.top

PHP:  $name = "Alex"; $age = 20;
来源：http://gka.hongshengwenyu.top

JS:   let name = "Alex"; const age = 20;
来源：http://iyo.xingfuxueyuan.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vcc.xingfuxueyuan.xyz

Java: String name = "Alex"; int age = 20;
来源：http://ros.quarkkingdee.top

Go:   name := "Alex"; age := 20
来源：http://xoz.jinghuilouyu.cn

Ruby: name = "Alex"; age = 20
来源：http://tjb.kuanghao11.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ocu.shzxlz.cn

[A03] 常量定义
来源：http://yce.fanxiaobao.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://phv.nwbrower.top

PHP:  const PI = 3.14159;
来源：http://iiu.guannengcc.top

JS:   const PI = 3.14159;
来源：http://eie.yongpay.top

TS:   const PI: number = 3.14159;
来源：http://dyb.fanxiaobao.xyz

Java: static final double PI = 3.14159;
来源：http://spc.ppjwa.cn

Go:   const PI = 3.14159
来源：http://vel.yj20258888.top

Ruby: PI = 3.14159
来源：http://ovh.zhixingplan.top

C#:   const double PI = 3.14159;
来源：http://vas.ydzc1.top

[A04] 判断变量类型
来源：http://mks.chenjidiqi.icu

Py:   type(x).__name__; isinstance(x, int)
来源：http://twl.tian-w.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ipu.fktsv.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zkm.sysykeji.top

TS:   typeof x; x instanceof Date
来源：http://ohk.sufxvd.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://etv.daxiang520.top

Go:   reflect.TypeOf(x).Name()
来源：http://xwr.shanyushiyangkeji.top

Ruby: x.class; x.is_a?(Integer)
来源：http://bng.ehwqpu.com

C#:   x.GetType().Name; x is int
来源：http://edc.birdmap.top

[A05] 整数除法与取模
来源：http://gfq.jyoumei.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fqu.zdqjudy.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://zbh.jinqigfzy.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mif.jinqigfzy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://oup.sxryk.cn

Java: 7 / 2; 7 % 2
来源：http://cty.tian-w.cn

Go:   7 / 2; 7 % 2
来源：http://abs.ybcxt.top

Ruby: 7 / 2; 7 % 2
来源：http://eij.yj20258.top

C#:   7 / 2; 7 % 2
来源：http://ova.ywan-chungtsiang.top

[A06] 字符串转数字
来源：http://fpm.daxiang520.top

Py:   int("42"); float("3.14")
来源：http://lez.jinqigfzy.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ukr.cashguo.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ymf.sxryk.cn

TS:   parseInt("42", 10); Number("42")
来源：http://hwa.zdbjq.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nyi.bbcook.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vzc.havefunace.top

Ruby: "42".to_i; "3.14".to_f
来源：http://orv.dianchejie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bva.wangdashe.top

[A07] 数字转字符串
来源：http://fev.zhongyouzk.top

Py:   str(42)
来源：http://vxx.meibo888.top

PHP:  (string) 42; strval(42)
来源：http://uyz.yangfankeji.com

JS:   String(42); (42).toString()
来源：http://esw.xuanzx.com

TS:   String(42)
来源：http://uhe.jyoumei.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ldi.haohaochexian.top

Go:   strconv.Itoa(42)
来源：http://zfe.jianghu66.top

Ruby: 42.to_s
来源：http://ctr.tianlin.xyz

C#:   42.ToString()
来源：http://syu.hfpthk.cn

[A08] 取整与四舍五入
来源：http://ilq.shuidangran.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yey.hysaishi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zde.yj20258.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://din.316326.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://azt.yj20258.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ebh.hywenlv.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://umy.yj20258.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://vrw.yongpay.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dvd.jianghu66.top

[A09] 绝对值与最大最小值
来源：http://xuy.hongshengwenyu.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://evs.shanyushiyangtech.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jxq.aibaodan.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sef.chenjidiqi.icu

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rvs.tianlin.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zqa.9152youxi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vwq.jinqigufen.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fej.cdnleiting.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ahu.xziqi.cn

[A10] 生成随机数
来源：http://hxb.yanxiufei.cn

Py:   import random; random.randint(1, 100)
来源：http://pcp.guowangkeji.top

PHP:  random_int(1, 100);
来源：http://zbu.chenzaomai.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://tue.dashuyun.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dmh.ydzc1.top

Java: new Random().nextInt(100) + 1
来源：http://esk.wangshuangyany.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://brw.haohaochexian.top

Ruby: rand(1..100)
来源：http://vac.cdnleiting.top

C#:   new Random().Next(1, 101)
来源：http://ttb.quarkkingdee.top

[A11] 条件表达式（三元）
来源：http://ipj.yonumen.top

Py:   "yes" if x > 0 else "no"
来源：http://ptz.aibaodan.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ykq.xuetiantiany.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ysh.svipenyu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://kdy.52xcode.cn

Java: x > 0 ? "yes" : "no"
来源：http://iwd.316326.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://jby.cheryme.top

Ruby: x > 0 ? "yes" : "no"
来源：http://tgw.9152youxi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xyr.jyoumei.cn

[A12] 字符串插值 / 格式化
来源：http://now.cheryme.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jjd.zhaomingkeji.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://epr.yj20258.top

JS:   `Hello, ${name}!`
来源：http://vtm.zhixingplan.top

TS:   `Hello, ${name}!`
来源：http://bdk.cucudq.cn

Java: "Hello, %s!".formatted(name)
来源：http://ypz.jinghuilouyu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lgf.zhixingplan.top

Ruby: "Hello, #{name}!"
来源：http://dwd.smart0.xyz

C#:   $"Hello, {name}!"
来源：http://gua.shangyingyoupin.top

[A13] 多行字符串（练习 \n 转义）
来源：http://jwx.gotoacloud.top

Py:   "第一行\n第二行"
来源：http://rdi.jyoumei.cn

PHP:  "第一行\n第二行"
来源：http://wqd.zhengqikj.top

JS:   "第一行\n第二行"
来源：http://vuw.jinqigufen.top

TS:   "第一行\n第二行"
来源：http://ysb.bbcook.cn

Java: "第一行\n第二行"
来源：http://rab.sufxvd.cn

Go:   "第一行\n第二行"
来源：http://aig.daria6918.cn

Ruby: "第一行\n第二行"
来源：http://dlw.jinghuilouyu.cn

C#:   "第一行\n第二行"
来源：http://xhk.shzxlz.cn

[A14] 注释写法
来源：http://xej.jianghu66.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://zge.chenjidiqi.icu

PHP:  // 或 # 单行；/* 多行 */
来源：http://rjr.zhaomingkeji.xyz

JS:   // 单行；/* 多行 */
来源：http://xzp.zdqjudy.top

TS:   // 单行；/* 多行 */
来源：http://efw.hnqzz.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wju.c1oappe.top

Go:   // 单行；/* 多行 */
来源：http://wmc.aizwys.cn

Ruby: # 单行；=begin 多行 =end
来源：http://tpp.yj20258.top

C#:   // 单行；/* 多行 */
来源：http://nke.hcnkem.com

[A15] 空值判断与默认值
来源：http://qla.vqdsnc.cn

Py:   value = data or "默认值"
来源：http://dai.andypj.xyz

PHP:  $value = $data ?? "默认值";
来源：http://wdc.sysykeji.top

JS:   const value = data ?? "默认值";
来源：http://wzp.haohaochexian.top

TS:   const value = data ?? "默认值";
来源：http://irl.vqdsnc.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://alr.uphjek.com

Go:   if data == "" { data = "默认值" }
来源：http://deo.dashuyun.cn

Ruby: value = data || "默认值"
来源：http://owk.jiagoushi.top

C#:   var value = data ?? "默认值";
来源：http://ltj.zdbjq.cn

[A16] 真假值判断规则
来源：http://prg.hysaishi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wbj.tanke756.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mhz.fktsv.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wei.andypj.xyz

TS:   if (!x) {}
来源：http://xxm.0kj1m.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://huv.ehwqpu.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sot.vqdsnc.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lva.daxiang520.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tyr.guannengcc.top

[A17] 位运算
来源：http://yme.cheryme.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gxv.birdmap.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kmj.hfpthk.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ppx.shzxlz.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://drk.tian-w.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qms.jinghuilouyu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://avp.mhx1999.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hnb.nwbrower.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://drz.cdnleiting.top

[A18] 字符与 ASCII 码互转
来源：http://hjv.shanyushiyangkeji.top

Py:   ord("A"); chr(65)
来源：http://whh.hammf.cn

PHP:  ord("A"); chr(65)
来源：http://ssa.jinqigfzy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pmb.jianghu66.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ncq.smart0.xyz

Java: (int) 'A'; (char) 65
来源：http://fii.bjfxy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nkz.sysykeji.top

Ruby: "A".ord; 65.chr
来源：http://phd.yangfankeji.com

C#:   (int)'A'; (char)65
来源：http://joi.shangyingyoupin.top

[A19] 交换两个变量
来源：http://sim.shuidangran.top

Py:   a, b = b, a
来源：http://art.ydzc1.top

PHP:  [$a, $b] = [$b, $a];
来源：http://fns.jyoumei.cn

JS:   [a, b] = [b, a];
来源：http://tqm.9152youxi.cn

TS:   [a, b] = [b, a];
来源：http://frr.zhijiandao.cn

Java: int t = a; a = b; b = t;
来源：http://peg.chenzaomai.com

Go:   a, b = b, a
来源：http://qmq.zdqjudy.top

Ruby: a, b = b, a
来源：http://tpf.smart0.xyz

C#:   (a, b) = (b, a);
来源：http://zrp.cqqwz.cn

[A20] 读取标准输入
来源：http://hbu.cucudq.cn

Py:   name = input("请输入：")
来源：http://qnt.tanke756.top

PHP:  $name = trim(fgets(STDIN));
来源：http://dsf.cheryme.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wxb.vqdsnc.cn

TS:   // Node.js：readline 模块
来源：http://gzg.guannengcc.top

Java: new Scanner(System.in).nextLine()
来源：http://mhs.cqqwz.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ghd.0kj1m.cn

Ruby: gets.chomp
来源：http://cze.hongshengwenyu.top

C#:   Console.ReadLine();
来源：http://bov.jinqigufen.top

[A21] 保留指定小数位输出
来源：http://kgj.ybcxt.top

Py:   f"{3.14159:.2f}"
来源：http://wvv.aibaodan.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pvl.hcnkem.com

JS:   (3.14159).toFixed(2)
来源：http://mwp.jinyuanbaomall.cn

TS:   (3.14159).toFixed(2)
来源：http://ktx.yueranfly.top

Java: String.format("%.2f", 3.14159)
来源：http://xme.zdbjq.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bgh.svipenyu.cn

Ruby: format("%.2f", 3.14159)
来源：http://voo.quarkkingdee.top

C#:   3.14159.ToString("F2")
来源：http://cag.hcnkem.com

[A22] 获取字符串长度
来源：http://tbs.yuanzhike.top

Py:   len(s)
来源：http://rhf.316326.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qhc.yanxiufei.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lvm.sysykeji.top

TS:   s.length
来源：http://jyn.bjfxy.top

Java: s.length()
来源：http://cyh.jlsjyb.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zeu.jyoumei.cn

Ruby: s.length
来源：http://yau.zdqjudy.top

C#:   s.Length
来源：http://inx.yfazqb.com

[A23] 大小写转换
来源：http://ssz.zhiwuduotai.top

Py:   s.upper(); s.lower(); s.title()
来源：http://bhg.xuetiantiany.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ijz.jinyuanbaomall.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://luy.hywenlv.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://iqh.zhijiandao.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nxk.fehbvm.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://agu.yj20258.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uyp.snrcjt.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://igh.dianchejie.cn

[A24] 去除首尾空白
来源：http://pjt.yj202588.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gkm.smart0.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kgi.cqqwz.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zkc.shzxlz.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://coh.chenlongwang.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zut.daria6918.cn

Go:   strings.TrimSpace(s)
来源：http://mdt.smart0.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pxd.gotoacloud.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wsl.pengpengdd.cyou

[A25] 字符串比较
来源：http://wrd.xuanzx.com

Py:   s1 == s2; s1 != s2
来源：http://zam.yj20258888.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://psf.yonumen.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sqy.hcnkem.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://trb.ivvv.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://irq.xinyue.icu

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qgj.aizwys.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jdw.mhx1999.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jib.nanxuanxn.top

[A26] 类型转换总览
来源：http://nes.iojbl.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dyh.daxiang520.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vec.meibo888.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://esc.kuanghao11.cn

TS:   Number() String() Boolean() x as number
来源：http://pwr.gzhubu.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tri.ywan-chungtsiang.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mwh.jlsjyb.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pia.zycfv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://prk.ydzc1.top

================================================================================
来源：http://mmc.shuidangran.top

B. 流程控制
来源：http://acb.svipenyu.cn

================================================================================
来源：http://dbj.dashuyun.cn

[B01] 条件判断 if / else
来源：http://udq.jiagoushi.top

Py:   result = "正" if x > 0 else "非正"
来源：http://snx.0kj1m.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gos.aizwys.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jon.gotoacloud.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hjx.chenlongwang.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://rop.bbcook.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ipw.haohaochexian.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uhw.c1oappe.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vjf.c1oappe.top

[B02] 多分支 else if / elif
来源：http://ptz.ctjpmb.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rlp.haohaochexian.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pnw.zhoulong.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nph.andypj.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://big.andypj.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rfj.c1oappe.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wrq.smart0.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://alc.tian-w.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wvk.andypj.xyz

[B03] switch / match / case
来源：http://jap.xuetiantiany.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ntl.yonumen.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://err.havefunace.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oey.snrcjt.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://onw.cucudq.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://myb.yj20258.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uqo.fktsv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kxw.sufxvd.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cvs.zhengqikj.top

[B04] for 计数循环
来源：http://vjp.zdqjudy.top

Py:   for i in range(10): print(i)
来源：http://zhg.zdbjq.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wnt.jqgufenzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qml.hesvh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ugf.zhongyouzk.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mob.hnqzz.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jiy.wangdashe.top

Ruby: 10.times { |i| puts i }
来源：http://tuj.uphjek.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://aso.xziqi.cn

[B05] 遍历数组 / 列表
来源：http://hmt.hywenlv.cn

Py:   for item in arr: print(item)
来源：http://xzw.fzhhl.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sue.hongshengwenyu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://nqp.nanxuanxn.top

TS:   for (const item of arr) { console.log(item); }
来源：http://erq.hammf.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hhp.daxiang520.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yua.chenlongwang.top

Ruby: arr.each { |item| puts item }
来源：http://gtm.smart0.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vqm.jinyuanbaomall.cn

[B06] 遍历字典 / 对象
来源：http://ajt.yfazqb.com

Py:   for k, v in d.items(): print(k, v)
来源：http://azs.bbcook.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fbb.chenlongwang.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://efv.hfpthk.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kfz.vehdjk.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qxg.chenjidiqi.icu

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rqb.c1oappe.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lix.feifeiyinyue.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nrk.zhaomingkeji.xyz

[B07] while 循环
来源：http://eqw.jqgfzy.top

Py:   while i < 10: i += 1
来源：http://dox.xingfuxueyuan.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://eud.kuanghao11.cn

JS:   while (i < 10) { i++; }
来源：http://xjl.uphjek.com

TS:   while (i < 10) { i++; }
来源：http://baf.sweek.top

Java: while (i < 10) { i++; }
来源：http://cur.0kj1m.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ggs.wangshuangyany.cn

Ruby: while i < 10; i += 1; end
来源：http://fru.guowangkeji.top

C#:   while (i < 10) { i++; }
来源：http://uwd.shuidangran.top

[B08] do-while（至少执行一次）
来源：http://rvd.ctjpmb.com

Py:   # 无 do-while：用 while True + break
来源：http://yks.yuxming.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://upt.birdmap.top

JS:   do { i++; } while (i < 10);
来源：http://cqx.sysykeji.top

TS:   do { i++; } while (i < 10);
来源：http://jjh.cucudq.cn

Java: do { i++; } while (i < 10);
来源：http://uzm.shanyushiyangkeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://gyo.aibaodan.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gso.sysykeji.top

C#:   do { i++; } while (i < 10);
来源：http://dgz.nanxuanxn.top


<!-- 参考信息 -->