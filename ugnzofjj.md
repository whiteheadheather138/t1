代发 wailian999

[A02] 变量声明与赋值
来源：http://pak.nwbrower.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mzq.dashuyun.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://baa.wangshuangyany.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wca.c1oappe.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rbt.hcnkem.com

Java: String name = "Alex"; int age = 20;
来源：http://lnz.jlsjyb.cn

Go:   name := "Alex"; age := 20
来源：http://new.iojbl.cn

Ruby: name = "Alex"; age = 20
来源：http://utj.nanxinkj.top

C#:   string name = "Alex"; int age = 20;
来源：http://mvb.dashuyun.cn

[A03] 常量定义
来源：http://ict.jinqigfzy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ezn.jqgfzy.top

PHP:  const PI = 3.14159;
来源：http://pwt.quarkkingdee.top

JS:   const PI = 3.14159;
来源：http://vmu.hfpthk.cn

TS:   const PI: number = 3.14159;
来源：http://nuo.hammf.cn

Java: static final double PI = 3.14159;
来源：http://mtj.hesvh.cn

Go:   const PI = 3.14159
来源：http://eue.yj20258.top

Ruby: PI = 3.14159
来源：http://wrd.jlsjyb.cn

C#:   const double PI = 3.14159;
来源：http://gyi.cqqwz.cn

[A04] 判断变量类型
来源：http://cwa.birdmap.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://nzg.yongpay.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hhu.zhiwuduotai.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hxz.yuxming.cn

TS:   typeof x; x instanceof Date
来源：http://yfk.0kj1m.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sri.xziqi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://cex.shuidangran.top

Ruby: x.class; x.is_a?(Integer)
来源：http://hwh.ydzc1.top

C#:   x.GetType().Name; x is int
来源：http://ojj.ivvv.top

[A05] 整数除法与取模
来源：http://dcg.ctjpmb.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ase.daria6918.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://tel.feifeiyinyue.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cep.cashguo.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ajv.yj202588.top

Java: 7 / 2; 7 % 2
来源：http://rtj.bbcook.cn

Go:   7 / 2; 7 % 2
来源：http://mgx.nwbrower.top

Ruby: 7 / 2; 7 % 2
来源：http://zsl.hysaishi.cn

C#:   7 / 2; 7 % 2
来源：http://xvh.yueranfly.top

[A06] 字符串转数字
来源：http://wmm.ehwqpu.com

Py:   int("42"); float("3.14")
来源：http://gtz.zhixingplan.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://spd.bbcook.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cnt.yuanzhike.top

TS:   parseInt("42", 10); Number("42")
来源：http://fuh.c1oappe.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vbf.zycfv.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ubc.yj20258888.top

Ruby: "42".to_i; "3.14".to_f
来源：http://nmx.ybcxt.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uyp.xinyue.icu

[A07] 数字转字符串
来源：http://mrt.gaohongyu789.top

Py:   str(42)
来源：http://dpf.yueranfly.top

PHP:  (string) 42; strval(42)
来源：http://awd.c1oappe.top

JS:   String(42); (42).toString()
来源：http://dbb.shanyushiyangtech.top

TS:   String(42)
来源：http://omx.meibo888.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://xkz.jqgufenzy.top

Go:   strconv.Itoa(42)
来源：http://dtd.nanxuanxn.top

Ruby: 42.to_s
来源：http://wha.jlsjyb.cn

C#:   42.ToString()
来源：http://vbt.9152youxi.cn

[A08] 取整与四舍五入
来源：http://bdf.xingfuxueyuan.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tum.mhx1999.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nku.kuanghao11.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nub.aizwys.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hfv.meibo888.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cnn.iojbl.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gpm.guowangkeji.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://jjf.ybcxt.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://utg.tian-w.cn

[A09] 绝对值与最大最小值
来源：http://qqe.zhiwuduotai.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://brn.yonumen.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bbk.yj20258.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cdd.uphjek.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://rgm.cheryme.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://agj.zdqjudy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vcz.zhengqikj.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pyy.pycfn.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vat.jqgufenzy.top

[A10] 生成随机数
来源：http://axa.ivvv.top

Py:   import random; random.randint(1, 100)
来源：http://rrl.fengsongda.top

PHP:  random_int(1, 100);
来源：http://chc.hesvh.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hhi.jiagoushi.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mib.fzhhl.top

Java: new Random().nextInt(100) + 1
来源：http://rsq.cashguo.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qfe.hcnkem.com

Ruby: rand(1..100)
来源：http://elr.yonumen.top

C#:   new Random().Next(1, 101)
来源：http://zjo.dianchejie.cn

[A11] 条件表达式（三元）
来源：http://lpy.cqqwz.cn

Py:   "yes" if x > 0 else "no"
来源：http://mec.jqgufenzy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://vad.ppjwa.cn

JS:   x > 0 ? "yes" : "no"
来源：http://gxp.feifeiyinyue.top

TS:   x > 0 ? "yes" : "no"
来源：http://qej.wangshuangyany.cn

Java: x > 0 ? "yes" : "no"
来源：http://vda.nanxinkj.top

Go:   // 无三元运算符，需用 if 语句
来源：http://xsp.chenzaomai.com

Ruby: x > 0 ? "yes" : "no"
来源：http://irc.yuanzhike.top

C#:   x > 0 ? "yes" : "no"
来源：http://fcp.mhx1999.top

[A12] 字符串插值 / 格式化
来源：http://lcb.52xcode.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zqs.yanxiufei.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jvm.wangdashe.top

JS:   `Hello, ${name}!`
来源：http://cmo.yongpay.top

TS:   `Hello, ${name}!`
来源：http://yrr.redwolf501.top

Java: "Hello, %s!".formatted(name)
来源：http://loo.iojbl.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qla.hysaishi.cn

Ruby: "Hello, #{name}!"
来源：http://llv.jinghuilouyu.cn

C#:   $"Hello, {name}!"
来源：http://ttb.jqgfzy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://jng.yuxming.cn

Py:   "第一行\n第二行"
来源：http://aoo.zhixingplan.top

PHP:  "第一行\n第二行"
来源：http://ecb.shanyushiyangtech.top

JS:   "第一行\n第二行"
来源：http://ehz.xuanzx.com

TS:   "第一行\n第二行"
来源：http://ivm.zycfv.cn

Java: "第一行\n第二行"
来源：http://xmk.hywenlv.cn

Go:   "第一行\n第二行"
来源：http://wfy.zhaomingkeji.xyz

Ruby: "第一行\n第二行"
来源：http://bua.zhongyouzk.top

C#:   "第一行\n第二行"
来源：http://rwa.shanyushiyangkeji.top

[A14] 注释写法
来源：http://qtx.jinqigufen.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://khe.xuanzx.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://jll.cashguo.top

JS:   // 单行；/* 多行 */
来源：http://mrb.zdqjudy.top

TS:   // 单行；/* 多行 */
来源：http://azr.yangfankeji.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pau.ydjk.org.cn

Go:   // 单行；/* 多行 */
来源：http://oek.shuidangran.top

Ruby: # 单行；=begin 多行 =end
来源：http://afh.uphjek.com

C#:   // 单行；/* 多行 */
来源：http://hia.tarul.cn

[A15] 空值判断与默认值
来源：http://xzf.tanke756.top

Py:   value = data or "默认值"
来源：http://egx.vqdsnc.cn

PHP:  $value = $data ?? "默认值";
来源：http://ykk.dianchejie.cn

JS:   const value = data ?? "默认值";
来源：http://uwf.yj202588.top

TS:   const value = data ?? "默认值";
来源：http://gia.zycfv.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rfm.smart0.xyz

Go:   if data == "" { data = "默认值" }
来源：http://bas.nwbrower.top

Ruby: value = data || "默认值"
来源：http://spw.hywenlv.cn

C#:   var value = data ?? "默认值";
来源：http://pvz.vqdsnc.cn

[A16] 真假值判断规则
来源：http://fuz.cucudq.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qao.yangfankeji.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vhb.aizwys.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ibw.shanyushiyangkeji.top

TS:   if (!x) {}
来源：http://bsk.svipenyu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jpg.hnxiangtu.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pkt.yueranfly.top

Ruby: unless x            # nil 与 false 为假
来源：http://boo.ydzc1.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fpm.fengsongda.top

[A17] 位运算
来源：http://dvj.hesvh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vuw.nanxinkj.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ige.shangyingyoupin.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ljk.snrcjt.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jre.zhaomingkeji.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xek.kuanghao11.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://emk.zdqjudy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kkq.jlsjyb.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cvd.shzxlz.cn

[A18] 字符与 ASCII 码互转
来源：http://bvb.zycfv.cn

Py:   ord("A"); chr(65)
来源：http://uqv.zhongyouzk.top

PHP:  ord("A"); chr(65)
来源：http://dve.fanxiaobao.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vil.bbcook.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wgf.cucudq.cn

Java: (int) 'A'; (char) 65
来源：http://hjt.yangfankeji.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tfn.ybcxt.top

Ruby: "A".ord; 65.chr
来源：http://vlz.jqgufenzy.top

C#:   (int)'A'; (char)65
来源：http://ivt.xinyue.icu

[A19] 交换两个变量
来源：http://ibr.xziqi.cn

Py:   a, b = b, a
来源：http://rxm.sysykeji.top

PHP:  [$a, $b] = [$b, $a];
来源：http://rws.fzhhl.top

JS:   [a, b] = [b, a];
来源：http://qpz.316326.xyz

TS:   [a, b] = [b, a];
来源：http://evu.snrcjt.cn

Java: int t = a; a = b; b = t;
来源：http://arz.chenlongwang.top

Go:   a, b = b, a
来源：http://gys.c1oappe.top

Ruby: a, b = b, a
来源：http://fjj.gogol.net.cn

C#:   (a, b) = (b, a);
来源：http://cbq.vqdsnc.cn

[A20] 读取标准输入
来源：http://trk.birdmap.top

Py:   name = input("请输入：")
来源：http://lwz.redwolf501.top

PHP:  $name = trim(fgets(STDIN));
来源：http://uyi.ydjk.org.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qnq.jqgfzy.top

TS:   // Node.js：readline 模块
来源：http://moy.tarul.cn

Java: new Scanner(System.in).nextLine()
来源：http://cuv.xuanzx.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xoh.vehdjk.com

Ruby: gets.chomp
来源：http://ieg.jyoumei.cn

C#:   Console.ReadLine();
来源：http://fqy.hesvh.cn

[A21] 保留指定小数位输出
来源：http://qdd.zycfv.cn

Py:   f"{3.14159:.2f}"
来源：http://tlz.fanxiaobao.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ezq.daria6918.cn

JS:   (3.14159).toFixed(2)
来源：http://ruy.dashuyun.cn

TS:   (3.14159).toFixed(2)
来源：http://fhk.andypj.xyz

Java: String.format("%.2f", 3.14159)
来源：http://yjp.aibaodan.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gfd.nwbrower.top

Ruby: format("%.2f", 3.14159)
来源：http://xsj.yueranfly.top

C#:   3.14159.ToString("F2")
来源：http://lbu.zhoulong.xyz

[A22] 获取字符串长度
来源：http://uki.hfpthk.cn

Py:   len(s)
来源：http://vmy.andypj.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wlx.jlsjyb.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jjh.cqqwz.cn

TS:   s.length
来源：http://erg.9152youxi.cn

Java: s.length()
来源：http://aqa.nanxuanxn.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ttj.birdmap.top

Ruby: s.length
来源：http://ibe.yonumen.top

C#:   s.Length
来源：http://chk.tanke756.top

[A23] 大小写转换
来源：http://agr.tarul.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vli.chenlongwang.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zer.sjlbkw.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pba.xziqi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://exe.jinyuanbaomall.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qfy.ivvv.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bzl.zdbjq.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qll.0kj1m.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ltj.daria6918.cn

[A24] 去除首尾空白
来源：http://pem.ydzc1.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://axl.ywan-chungtsiang.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ogb.xylfe.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://frz.vehdjk.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bgl.hysaishi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://uxi.yuanzhike.top

Go:   strings.TrimSpace(s)
来源：http://juj.bbcook.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ray.yj20258888.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://szq.cdnleiting.top

[A25] 字符串比较
来源：http://ozz.fktsv.cn

Py:   s1 == s2; s1 != s2
来源：http://yhe.hcnkem.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mkq.sjlbkw.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qic.hfpthk.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cig.chenlongwang.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bte.redwolf501.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dvy.hongshengwenyu.top

Ruby: s1 == s2; s1 <=> s2
来源：http://udi.xziqi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sli.zhoulong.xyz

[A26] 类型转换总览
来源：http://lxo.nwbrower.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lcr.zycfv.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dvz.zycfv.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://swi.tian-w.cn

TS:   Number() String() Boolean() x as number
来源：http://afb.vehdjk.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uih.hcnkem.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jhv.fktsv.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://siz.xylfe.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ttf.daxiang520.top

================================================================================
来源：http://mjk.ehwqpu.com

B. 流程控制
来源：http://mav.cqqwz.cn

================================================================================
来源：http://qmg.cucudq.cn

[B01] 条件判断 if / else
来源：http://twz.birdmap.top

Py:   result = "正" if x > 0 else "非正"
来源：http://yfr.aizwys.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pop.pengpengdd.cyou

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dvr.hesvh.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lxy.zhongyouzk.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://bjz.fengsongda.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ntu.daxiang520.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uqv.jinyuanbaomall.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pxq.zhixingplan.top

[B02] 多分支 else if / elif
来源：http://yro.feifeiyinyue.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xcj.zycfv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://txu.andypj.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cyt.xuetiantiany.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pfj.uphjek.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gis.zhoulong.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yne.cucudq.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fbx.cheryme.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://apt.hcnkem.com

[B03] switch / match / case
来源：http://pca.haohaochexian.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qoz.fzhhl.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mwl.c1oappe.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qyp.vqdsnc.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://isa.gogol.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ifg.jinghuilouyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://iei.ybcxt.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zwe.aizwys.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qkm.fehbvm.com

[B04] for 计数循环
来源：http://aab.c1oappe.top

Py:   for i in range(10): print(i)
来源：http://brg.cashguo.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jlf.haohaochexian.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kqy.cucudq.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ona.hammf.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://boe.9152youxi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rmn.tanke756.top

Ruby: 10.times { |i| puts i }
来源：http://tgd.jinqigufen.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mks.yj20258.top

[B05] 遍历数组 / 列表
来源：http://dor.hcnkem.com

Py:   for item in arr: print(item)
来源：http://xjq.gaohongyu789.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ffn.redwolf501.top

JS:   for (const item of arr) { console.log(item); }
来源：http://yvp.uphjek.com

TS:   for (const item of arr) { console.log(item); }
来源：http://vik.redwolf501.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://hhn.gzhubu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ddw.jinqigufen.top

Ruby: arr.each { |item| puts item }
来源：http://bdl.yvedp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://orb.cucudq.cn

[B06] 遍历字典 / 对象
来源：http://nul.sweek.top

Py:   for k, v in d.items(): print(k, v)
来源：http://uqx.uphjek.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://eap.fengsongda.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vet.cqqwz.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://beh.aibaodan.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xrj.jinqigfzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cgk.bjfxy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hxs.ydzc1.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://efy.hysaishi.cn

[B07] while 循环
来源：http://kjo.epnwcf.com

Py:   while i < 10: i += 1
来源：http://tjv.dianchejie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mjz.iojbl.cn

JS:   while (i < 10) { i++; }
来源：http://spo.c1oappe.top

TS:   while (i < 10) { i++; }
来源：http://rmg.iojbl.cn

Java: while (i < 10) { i++; }
来源：http://mem.feifeiyinyue.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zpd.daxiang520.top

Ruby: while i < 10; i += 1; end
来源：http://pnm.hnxiangtu.top

C#:   while (i < 10) { i++; }
来源：http://vuw.gzhubu.top

[B08] do-while（至少执行一次）
来源：http://tey.zhengqikj.top

Py:   # 无 do-while：用 while True + break
来源：http://xkn.bbcook.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://rrp.gaohongyu789.top

JS:   do { i++; } while (i < 10);
来源：http://seb.fanxiaobao.xyz

TS:   do { i++; } while (i < 10);
来源：http://xwq.ywan-chungtsiang.top

Java: do { i++; } while (i < 10);
来源：http://oti.shzxlz.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://exc.shangyingyoupin.top

Ruby: begin; i += 1; end while i < 10
来源：http://iry.pycfn.com

C#:   do { i++; } while (i < 10);
来源：http://eim.shuidangran.top


<!-- 参考信息 -->