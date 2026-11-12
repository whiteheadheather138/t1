代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://gre.fanxiaobao.xyz

[A03] 常量定义
来源：http://pcq.guowangkeji.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bom.c1oappe.top

PHP:  const PI = 3.14159;
来源：http://qnj.cashguo.top

JS:   const PI = 3.14159;
来源：http://com.xziqi.cn

TS:   const PI: number = 3.14159;
来源：http://gia.xuanzx.com

Java: static final double PI = 3.14159;
来源：http://luu.zhengqikj.top

Go:   const PI = 3.14159
来源：http://pcs.hywenlv.cn

Ruby: PI = 3.14159
来源：http://ysc.pengpengdd.cyou

C#:   const double PI = 3.14159;
来源：http://xai.sysykeji.top

[A04] 判断变量类型
来源：http://kgk.zhaomingkeji.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://vnb.xuanzx.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ann.shzxlz.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kec.sweek.top

TS:   typeof x; x instanceof Date
来源：http://gnu.yongpay.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://uqu.gogol.net.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bin.52xcode.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://jju.fktsv.cn

C#:   x.GetType().Name; x is int
来源：http://ruw.yuanzhike.top

[A05] 整数除法与取模
来源：http://utb.gaohongyu789.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qcf.wangshuangyany.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xon.zdqjudy.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jfs.yanxiufei.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wdt.52xcode.cn

Java: 7 / 2; 7 % 2
来源：http://ldg.zycfv.cn

Go:   7 / 2; 7 % 2
来源：http://glg.feifeiyinyue.top

Ruby: 7 / 2; 7 % 2
来源：http://mgd.feifeiyinyue.top

C#:   7 / 2; 7 % 2
来源：http://air.hesvh.cn

[A06] 字符串转数字
来源：http://oot.birdmap.top

Py:   int("42"); float("3.14")
来源：http://jso.chenzaomai.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://uag.sxryk.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jqq.bjfxy.top

TS:   parseInt("42", 10); Number("42")
来源：http://cyv.ydjk.org.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nei.gogol.net.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lom.hongshengwenyu.top

Ruby: "42".to_i; "3.14".to_f
来源：http://wge.zhaomingkeji.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zdb.jianghu66.top

[A07] 数字转字符串
来源：http://cwu.tanke756.top

Py:   str(42)
来源：http://fpo.yanxiufei.cn

PHP:  (string) 42; strval(42)
来源：http://pbh.hnxiangtu.top

JS:   String(42); (42).toString()
来源：http://dch.jqgufenzy.top

TS:   String(42)
来源：http://gtd.sufxvd.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://fwu.fengsongda.top

Go:   strconv.Itoa(42)
来源：http://arl.guowangkeji.top

Ruby: 42.to_s
来源：http://qmf.zhongyouzk.top

C#:   42.ToString()
来源：http://xgl.kuanghao11.cn

[A08] 取整与四舍五入
来源：http://rfr.smart0.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://brt.ivvv.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pnu.haohaochexian.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tmm.ivvv.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://eet.yueranfly.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gwu.gogol.net.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://trn.ydjk.org.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mbc.jianghu66.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://drt.zdqjudy.top

[A09] 绝对值与最大最小值
来源：http://iaf.chenlongwang.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://low.xingfuxueyuan.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://aat.guannengcc.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jqb.feifeiyinyue.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kye.jianghu66.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cwr.zdqjudy.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ljo.vqdsnc.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://unl.haohaochexian.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tpd.nanxinkj.top

[A10] 生成随机数
来源：http://hfu.andypj.xyz

Py:   import random; random.randint(1, 100)
来源：http://hjb.nanxuanxn.top

PHP:  random_int(1, 100);
来源：http://iid.ctjpmb.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ppo.tanke756.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zwz.jlsjyb.cn

Java: new Random().nextInt(100) + 1
来源：http://oyp.xziqi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qzx.epnwcf.com

Ruby: rand(1..100)
来源：http://fiy.yuxming.cn

C#:   new Random().Next(1, 101)
来源：http://rlf.sysykeji.top

[A11] 条件表达式（三元）
来源：http://iqz.zdbjq.cn

Py:   "yes" if x > 0 else "no"
来源：http://jsv.yj202588.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://dbv.nanxuanxn.top

JS:   x > 0 ? "yes" : "no"
来源：http://gpb.gaohongyu789.top

TS:   x > 0 ? "yes" : "no"
来源：http://xcn.havefunace.top

Java: x > 0 ? "yes" : "no"
来源：http://hvz.dashuyun.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hko.fzhhl.top

Ruby: x > 0 ? "yes" : "no"
来源：http://wxj.birdmap.top

C#:   x > 0 ? "yes" : "no"
来源：http://qyd.iojbl.cn

[A12] 字符串插值 / 格式化
来源：http://lfx.9152youxi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jsr.xziqi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hiq.gaohongyu789.top

JS:   `Hello, ${name}!`
来源：http://tcg.chenjidiqi.icu

TS:   `Hello, ${name}!`
来源：http://iiv.fzhhl.top

Java: "Hello, %s!".formatted(name)
来源：http://hql.hammf.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://eov.hammf.cn

Ruby: "Hello, #{name}!"
来源：http://yrw.xylfe.cn

C#:   $"Hello, {name}!"
来源：http://dfe.chenlongwang.top

[A13] 多行字符串（练习 \n 转义）
来源：http://lmc.yuxming.cn

Py:   "第一行\n第二行"
来源：http://iyd.meibo888.top

PHP:  "第一行\n第二行"
来源：http://xsw.yongpay.top

JS:   "第一行\n第二行"
来源：http://hsg.316326.xyz

TS:   "第一行\n第二行"
来源：http://mrz.nanxinkj.top

Java: "第一行\n第二行"
来源：http://brc.tian-w.cn

Go:   "第一行\n第二行"
来源：http://usu.xuanzx.com

Ruby: "第一行\n第二行"
来源：http://ice.uphjek.com

C#:   "第一行\n第二行"
来源：http://ons.chenzaomai.com

[A14] 注释写法
来源：http://rzu.ivvv.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://xer.jinqigfzy.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://iqe.zdbjq.cn

JS:   // 单行；/* 多行 */
来源：http://wlc.jinghuilouyu.cn

TS:   // 单行；/* 多行 */
来源：http://rzz.zhijiandao.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://utx.yangfankeji.com

Go:   // 单行；/* 多行 */
来源：http://zyc.xuetiantiany.cn

Ruby: # 单行；=begin 多行 =end
来源：http://fcj.yj202588.top

C#:   // 单行；/* 多行 */
来源：http://rgd.316326.xyz

[A15] 空值判断与默认值
来源：http://sjh.pengpengdd.cyou

Py:   value = data or "默认值"
来源：http://baq.chenzaomai.com

PHP:  $value = $data ?? "默认值";
来源：http://tml.xuetiantiany.cn

JS:   const value = data ?? "默认值";
来源：http://pdd.nanxuanxn.top

TS:   const value = data ?? "默认值";
来源：http://kwv.haohaochexian.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://maw.hnxiangtu.top

Go:   if data == "" { data = "默认值" }
来源：http://cvp.jqgfzy.top

Ruby: value = data || "默认值"
来源：http://toi.chenzaomai.com

C#:   var value = data ?? "默认值";
来源：http://jkn.chenzaomai.com

[A16] 真假值判断规则
来源：http://xow.redwolf501.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pmr.jiagoushi.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lze.hnxiangtu.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yls.havefunace.top

TS:   if (!x) {}
来源：http://xnn.guowangkeji.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rqq.shangyingyoupin.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rcp.jinyuanbaomall.cn

Ruby: unless x            # nil 与 false 为假
来源：http://nnw.shzxlz.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yeu.zycfv.cn

[A17] 位运算
来源：http://oqu.ppjwa.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tub.zhaomingkeji.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://djn.tanke756.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oxs.xingfuxueyuan.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://yzk.haohaochexian.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bia.9152youxi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://azu.zdqjudy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ltb.shanyushiyangtech.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ipl.fktsv.cn

[A18] 字符与 ASCII 码互转
来源：http://mdg.xuetiantiany.cn

Py:   ord("A"); chr(65)
来源：http://rmd.hammf.cn

PHP:  ord("A"); chr(65)
来源：http://vir.sufxvd.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kau.jyoumei.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dje.pengpengdd.cyou

Java: (int) 'A'; (char) 65
来源：http://ifm.shzxlz.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rfm.sufxvd.cn

Ruby: "A".ord; 65.chr
来源：http://hit.meibo888.top

C#:   (int)'A'; (char)65
来源：http://hvo.yfazqb.com

[A19] 交换两个变量
来源：http://thi.jyoumei.cn

Py:   a, b = b, a
来源：http://uwv.jqgufenzy.top

PHP:  [$a, $b] = [$b, $a];
来源：http://cbz.wangshuangyany.cn

JS:   [a, b] = [b, a];
来源：http://myp.gzhubu.top

TS:   [a, b] = [b, a];
来源：http://cfh.yvedp.cn

Java: int t = a; a = b; b = t;
来源：http://qws.bjfxy.top

Go:   a, b = b, a
来源：http://rsm.c1oappe.top

Ruby: a, b = b, a
来源：http://vtq.birdmap.top

C#:   (a, b) = (b, a);
来源：http://axm.xuanzx.com

[A20] 读取标准输入
来源：http://zzw.yongpay.top

Py:   name = input("请输入：")
来源：http://klt.tianlin.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://rtt.shangyingyoupin.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://slw.epnwcf.com

TS:   // Node.js：readline 模块
来源：http://dab.yuxming.cn

Java: new Scanner(System.in).nextLine()
来源：http://ptd.haohaochexian.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nzk.ivvv.top

Ruby: gets.chomp
来源：http://lar.yanxiufei.cn

C#:   Console.ReadLine();
来源：http://ejy.zhengqikj.top

[A21] 保留指定小数位输出
来源：http://sot.feifeiyinyue.top

Py:   f"{3.14159:.2f}"
来源：http://tjl.cqqwz.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zlt.ydzc1.top

JS:   (3.14159).toFixed(2)
来源：http://das.yonumen.top

TS:   (3.14159).toFixed(2)
来源：http://pap.yj20258888.top

Java: String.format("%.2f", 3.14159)
来源：http://avw.uphjek.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ojc.mhx1999.top

Ruby: format("%.2f", 3.14159)
来源：http://lfa.gaohongyu789.top

C#:   3.14159.ToString("F2")
来源：http://wjx.yj202588.top

[A22] 获取字符串长度
来源：http://oip.sufxvd.cn

Py:   len(s)
来源：http://iah.daxiang520.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ekd.hesvh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vpm.iojbl.cn

TS:   s.length
来源：http://jvc.havefunace.top

Java: s.length()
来源：http://won.c1oappe.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gaw.ivvv.top

Ruby: s.length
来源：http://kol.svipenyu.cn

C#:   s.Length
来源：http://mbm.yonumen.top

[A23] 大小写转换
来源：http://eys.gzhubu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://gpb.xziqi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dpb.0kj1m.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qss.xylfe.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yir.jinqigfzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gje.jinyuanbaomall.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mtw.daria6918.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://usv.hcnkem.com

C#:   s.ToUpper(); s.ToLower()
来源：http://htv.gaohongyu789.top

[A24] 去除首尾空白
来源：http://vqq.tianlin.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dzu.ybcxt.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fjm.bbcook.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qol.xingfuxueyuan.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gus.ehwqpu.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tbo.aizwys.cn

Go:   strings.TrimSpace(s)
来源：http://ydn.cheryme.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://grd.mhx1999.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mfy.guowangkeji.top

[A25] 字符串比较
来源：http://ilr.sufxvd.cn

Py:   s1 == s2; s1 != s2
来源：http://ebi.hesvh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uzv.hongshengwenyu.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kgj.tian-w.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pod.xuanzx.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ehl.cheryme.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fyd.sxryk.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://txm.wangshuangyany.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qoa.daxiang520.top

[A26] 类型转换总览
来源：http://blg.gaohongyu789.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vxp.hysaishi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zoh.cashguo.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hfv.tian-w.cn

TS:   Number() String() Boolean() x as number
来源：http://vua.tian-w.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vbs.nwbrower.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ylb.fehbvm.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://zmc.tanke756.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vlu.xziqi.cn

================================================================================
来源：http://pac.fktsv.cn

B. 流程控制
来源：http://udc.chenzaomai.com

================================================================================
来源：http://bxh.ybcxt.top

[B01] 条件判断 if / else
来源：http://bkb.0kj1m.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jbn.uphjek.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wsl.sysykeji.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tly.tian-w.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ond.shzxlz.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gwt.bbcook.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vma.hysaishi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dkd.gogol.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kft.cucudq.cn

[B02] 多分支 else if / elif
来源：http://yso.ydjk.org.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ezt.mhx1999.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rsp.hfpthk.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://erq.epnwcf.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oto.meibo888.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vzm.cucudq.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mbq.bbcook.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://elt.gogol.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://brl.feifeiyinyue.top

[B03] switch / match / case
来源：http://uck.yj20258.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bgg.dianchejie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ncj.jqgufenzy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xdf.shangyingyoupin.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lbu.shanyushiyangtech.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xsq.zhiwuduotai.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ezl.jinqigfzy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lcm.xziqi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kaa.xinyue.icu

[B04] for 计数循环
来源：http://jdz.0kj1m.cn

Py:   for i in range(10): print(i)
来源：http://btn.jiagoushi.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dfw.ywan-chungtsiang.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ybl.yuxming.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lwe.snrcjt.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vjs.yueranfly.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://iwz.epnwcf.com

Ruby: 10.times { |i| puts i }
来源：http://aqa.svipenyu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rgd.cucudq.cn

[B05] 遍历数组 / 列表
来源：http://jvv.shanyushiyangkeji.top

Py:   for item in arr: print(item)
来源：http://whi.ydzc1.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://acc.52xcode.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qln.ydzc1.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qtk.jinyuanbaomall.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://nyv.316326.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zak.sysykeji.top

Ruby: arr.each { |item| puts item }
来源：http://rnk.aibaodan.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cea.52xcode.cn

[B06] 遍历字典 / 对象
来源：http://tej.fzhhl.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ggk.zhijiandao.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rcd.shanyushiyangtech.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ura.jinqigfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hsf.feifeiyinyue.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mbr.zhixingplan.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hyl.ctjpmb.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mko.sysykeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iso.meibo888.top

[B07] while 循环
来源：http://oid.yj202588.top

Py:   while i < 10: i += 1
来源：http://jhn.hywenlv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://uiz.ctjpmb.com

JS:   while (i < 10) { i++; }
来源：http://clt.ybcxt.top

TS:   while (i < 10) { i++; }
来源：http://jqn.fzhhl.top

Java: while (i < 10) { i++; }
来源：http://ccw.fzhhl.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sii.ehwqpu.com

Ruby: while i < 10; i += 1; end
来源：http://jqu.tarul.cn

C#:   while (i < 10) { i++; }
来源：http://yfb.guowangkeji.top

[B08] do-while（至少执行一次）
来源：http://tec.xingfuxueyuan.xyz

Py:   # 无 do-while：用 while True + break
来源：http://zlg.epnwcf.com

PHP:  do { $i++; } while ($i < 10);
来源：http://dzm.yueranfly.top

JS:   do { i++; } while (i < 10);
来源：http://nks.fktsv.cn

TS:   do { i++; } while (i < 10);
来源：http://ufr.shanyushiyangtech.top

Java: do { i++; } while (i < 10);
来源：http://djr.ivvv.top

Go:   for { i++; if i >= 10 { break } }
来源：http://kon.nanxinkj.top

Ruby: begin; i += 1; end while i < 10
来源：http://pmu.hnxiangtu.top

C#:   do { i++; } while (i < 10);
来源：http://aqv.ctjpmb.com

[B09] break 与 continue
来源：http://kfc.wangdashe.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zvq.ydzc1.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://obv.zycfv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mog.wangshuangyany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vzk.zhoulong.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kci.nwbrower.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bda.sysykeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mpf.daria6918.cn


<!-- 参考信息 -->