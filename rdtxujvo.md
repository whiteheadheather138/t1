代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://jgr.svipenyu.cn

Go:   fmt.Println("Hello, World!")
来源：http://fxi.jqgufenzy.top

Ruby: puts "Hello, World!"
来源：http://zjc.shanyushiyangkeji.top

C#:   Console.WriteLine("Hello, World!");
来源：http://jsc.jiagoushi.top

[A02] 变量声明与赋值
来源：http://rgd.smart0.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://whb.meibo888.top

PHP:  $name = "Alex"; $age = 20;
来源：http://pbc.jinghuilouyu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ohg.hesvh.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jlu.chenjidiqi.icu

Java: String name = "Alex"; int age = 20;
来源：http://gut.yj202588.top

Go:   name := "Alex"; age := 20
来源：http://nok.daria6918.cn

Ruby: name = "Alex"; age = 20
来源：http://adr.iojbl.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xqe.jinqigfzy.top

[A03] 常量定义
来源：http://kvq.yanxiufei.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kbp.hnqzz.top

PHP:  const PI = 3.14159;
来源：http://rsk.hammf.cn

JS:   const PI = 3.14159;
来源：http://kaf.fengsongda.top

TS:   const PI: number = 3.14159;
来源：http://now.dianchejie.cn

Java: static final double PI = 3.14159;
来源：http://ojd.smart0.xyz

Go:   const PI = 3.14159
来源：http://mhk.hnqzz.top

Ruby: PI = 3.14159
来源：http://hdu.gotoacloud.top

C#:   const double PI = 3.14159;
来源：http://qbn.sjlbkw.cn

[A04] 判断变量类型
来源：http://eaa.zycfv.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://rdi.yangfankeji.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mdz.zdbjq.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xob.sysykeji.top

TS:   typeof x; x instanceof Date
来源：http://dzp.fktsv.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xks.0kj1m.cn

Go:   reflect.TypeOf(x).Name()
来源：http://xkq.jqgufenzy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ctq.sjlbkw.cn

C#:   x.GetType().Name; x is int
来源：http://ats.fengsongda.top

[A05] 整数除法与取模
来源：http://frp.gaohongyu789.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://oab.ydjk.org.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://vwd.hywenlv.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xtx.feifeiyinyue.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dwc.bbcook.cn

Java: 7 / 2; 7 % 2
来源：http://jkb.xziqi.cn

Go:   7 / 2; 7 % 2
来源：http://fnq.yangfankeji.com

Ruby: 7 / 2; 7 % 2
来源：http://pww.yuanzhike.top

C#:   7 / 2; 7 % 2
来源：http://ozw.quarkkingdee.top

[A06] 字符串转数字
来源：http://inb.yfazqb.com

Py:   int("42"); float("3.14")
来源：http://cig.jianghu66.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hhx.smart0.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pal.xylfe.cn

TS:   parseInt("42", 10); Number("42")
来源：http://sok.nwbrower.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tad.smart0.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uxp.yj202588.top

Ruby: "42".to_i; "3.14".to_f
来源：http://dqk.c1oappe.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qhy.fzhhl.top

[A07] 数字转字符串
来源：http://mea.shanyushiyangkeji.top

Py:   str(42)
来源：http://fqt.zhijiandao.cn

PHP:  (string) 42; strval(42)
来源：http://yff.hywenlv.cn

JS:   String(42); (42).toString()
来源：http://ctm.yonumen.top

TS:   String(42)
来源：http://pji.cqqwz.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://jym.haohaochexian.top

Go:   strconv.Itoa(42)
来源：http://zqs.chenlongwang.top

Ruby: 42.to_s
来源：http://xwd.316326.xyz

C#:   42.ToString()
来源：http://eez.gzhubu.top

[A08] 取整与四舍五入
来源：http://sho.snrcjt.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://urn.9152youxi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nzr.yvedp.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ude.chenjidiqi.icu

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cnr.uphjek.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rdo.vqdsnc.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xgd.cdnleiting.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://gjh.haohaochexian.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gqt.feifeiyinyue.top

[A09] 绝对值与最大最小值
来源：http://vaf.hcnkem.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wim.ctjpmb.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xab.daria6918.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nxk.fzhhl.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xmg.gaohongyu789.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xlt.shangyingyoupin.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ash.shzxlz.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jbb.ydjk.org.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pty.jiagoushi.top

[A10] 生成随机数
来源：http://drc.haohaochexian.top

Py:   import random; random.randint(1, 100)
来源：http://zgu.fktsv.cn

PHP:  random_int(1, 100);
来源：http://qwd.fengsongda.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://aeg.sxryk.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xex.ydzc1.top

Java: new Random().nextInt(100) + 1
来源：http://bki.jqgufenzy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://uyi.zhoulong.xyz

Ruby: rand(1..100)
来源：http://ufq.guowangkeji.top

C#:   new Random().Next(1, 101)
来源：http://cag.chenlongwang.top

[A11] 条件表达式（三元）
来源：http://xce.shuidangran.top

Py:   "yes" if x > 0 else "no"
来源：http://uqv.xziqi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://nfq.shzxlz.cn

JS:   x > 0 ? "yes" : "no"
来源：http://scf.dianchejie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://zzt.birdmap.top

Java: x > 0 ? "yes" : "no"
来源：http://typ.gotoacloud.top

Go:   // 无三元运算符，需用 if 语句
来源：http://nlu.daria6918.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://lvd.yuxming.cn

C#:   x > 0 ? "yes" : "no"
来源：http://cfw.cucudq.cn

[A12] 字符串插值 / 格式化
来源：http://xeq.dianchejie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kjc.jianghu66.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sdn.cheryme.top

JS:   `Hello, ${name}!`
来源：http://kpc.yueranfly.top

TS:   `Hello, ${name}!`
来源：http://awx.zhengqikj.top

Java: "Hello, %s!".formatted(name)
来源：http://yqj.zhongyouzk.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fop.yongpay.top

Ruby: "Hello, #{name}!"
来源：http://nlx.yj202588.top

C#:   $"Hello, {name}!"
来源：http://rnh.tanke756.top

[A13] 多行字符串（练习 \n 转义）
来源：http://nmr.yanxiufei.cn

Py:   "第一行\n第二行"
来源：http://epx.jyoumei.cn

PHP:  "第一行\n第二行"
来源：http://whf.jinyuanbaomall.cn

JS:   "第一行\n第二行"
来源：http://hqv.vehdjk.com

TS:   "第一行\n第二行"
来源：http://bus.0kj1m.cn

Java: "第一行\n第二行"
来源：http://cll.jlsjyb.cn

Go:   "第一行\n第二行"
来源：http://lkf.hongshengwenyu.top

Ruby: "第一行\n第二行"
来源：http://wap.shangyingyoupin.top

C#:   "第一行\n第二行"
来源：http://dyg.chenjidiqi.icu

[A14] 注释写法
来源：http://vek.ydzc1.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://wbg.jyoumei.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://qna.yj202588.top

JS:   // 单行；/* 多行 */
来源：http://jlf.tarul.cn

TS:   // 单行；/* 多行 */
来源：http://lek.ydzc1.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gzc.daxiang520.top

Go:   // 单行；/* 多行 */
来源：http://bfo.shangyingyoupin.top

Ruby: # 单行；=begin 多行 =end
来源：http://uip.havefunace.top

C#:   // 单行；/* 多行 */
来源：http://xni.bbcook.cn

[A15] 空值判断与默认值
来源：http://gwo.jinqigufen.top

Py:   value = data or "默认值"
来源：http://pdu.ybcxt.top

PHP:  $value = $data ?? "默认值";
来源：http://pjj.shanyushiyangkeji.top

JS:   const value = data ?? "默认值";
来源：http://qrd.guowangkeji.top

TS:   const value = data ?? "默认值";
来源：http://pmh.yangfankeji.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wit.zhixingplan.top

Go:   if data == "" { data = "默认值" }
来源：http://gqq.pycfn.com

Ruby: value = data || "默认值"
来源：http://bov.shzxlz.cn

C#:   var value = data ?? "默认值";
来源：http://rnh.chenjidiqi.icu

[A16] 真假值判断规则
来源：http://gbs.zdbjq.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nzk.yj20258888.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bnt.hywenlv.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gjr.ivvv.top

TS:   if (!x) {}
来源：http://wnx.zdqjudy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fyu.zhoulong.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hcd.yfazqb.com

Ruby: unless x            # nil 与 false 为假
来源：http://zst.hfpthk.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mpo.hesvh.cn

[A17] 位运算
来源：http://ntb.hnxiangtu.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ssh.vehdjk.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mcc.fengsongda.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blq.zycfv.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gpc.pengpengdd.cyou

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://giw.wangdashe.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rvb.birdmap.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eyt.gzhubu.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jhv.jinghuilouyu.cn

[A18] 字符与 ASCII 码互转
来源：http://xhw.316326.xyz

Py:   ord("A"); chr(65)
来源：http://tfg.zhongyouzk.top

PHP:  ord("A"); chr(65)
来源：http://pjo.316326.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tdg.guannengcc.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jgx.ydzc1.top

Java: (int) 'A'; (char) 65
来源：http://pfx.fehbvm.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vxk.ppjwa.cn

Ruby: "A".ord; 65.chr
来源：http://qgl.aizwys.cn

C#:   (int)'A'; (char)65
来源：http://fka.hcnkem.com

[A19] 交换两个变量
来源：http://oek.tianlin.xyz

Py:   a, b = b, a
来源：http://aaf.jqgufenzy.top

PHP:  [$a, $b] = [$b, $a];
来源：http://kxr.daxiang520.top

JS:   [a, b] = [b, a];
来源：http://fvp.yuxming.cn

TS:   [a, b] = [b, a];
来源：http://cpu.haohaochexian.top

Java: int t = a; a = b; b = t;
来源：http://pjp.shzxlz.cn

Go:   a, b = b, a
来源：http://fpn.yj20258888.top

Ruby: a, b = b, a
来源：http://niv.ehwqpu.com

C#:   (a, b) = (b, a);
来源：http://lpk.zhiwuduotai.top

[A20] 读取标准输入
来源：http://khe.jianghu66.top

Py:   name = input("请输入：")
来源：http://qwq.yfazqb.com

PHP:  $name = trim(fgets(STDIN));
来源：http://tgp.gogol.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ske.jlsjyb.cn

TS:   // Node.js：readline 模块
来源：http://iov.jqgufenzy.top

Java: new Scanner(System.in).nextLine()
来源：http://ysd.9152youxi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dab.gogol.net.cn

Ruby: gets.chomp
来源：http://iqa.ydzc1.top

C#:   Console.ReadLine();
来源：http://esd.zhijiandao.cn

[A21] 保留指定小数位输出
来源：http://uom.feifeiyinyue.top

Py:   f"{3.14159:.2f}"
来源：http://lrt.bbcook.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://khw.bjfxy.top

JS:   (3.14159).toFixed(2)
来源：http://ehs.zhiwuduotai.top

TS:   (3.14159).toFixed(2)
来源：http://mpn.pycfn.com

Java: String.format("%.2f", 3.14159)
来源：http://gdd.hnqzz.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://oiw.vehdjk.com

Ruby: format("%.2f", 3.14159)
来源：http://zzl.jlsjyb.cn

C#:   3.14159.ToString("F2")
来源：http://qoi.sxryk.cn

[A22] 获取字符串长度
来源：http://ioj.redwolf501.top

Py:   len(s)
来源：http://jhc.tian-w.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ftk.bjfxy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zdy.ywan-chungtsiang.top

TS:   s.length
来源：http://exf.xylfe.cn

Java: s.length()
来源：http://lmc.yanxiufei.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ghw.daxiang520.top

Ruby: s.length
来源：http://zao.9152youxi.cn

C#:   s.Length
来源：http://koj.guowangkeji.top

[A23] 大小写转换
来源：http://egw.tian-w.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zrr.dianchejie.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bsn.ydjk.org.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bca.guannengcc.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://krl.yanxiufei.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sfe.yj20258.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://utr.sufxvd.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://isr.nanxuanxn.top

C#:   s.ToUpper(); s.ToLower()
来源：http://yur.chenjidiqi.icu

[A24] 去除首尾空白
来源：http://jpe.yuxming.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zej.52xcode.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cmw.jinghuilouyu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://apq.zhengqikj.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qmp.yangfankeji.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://uzm.nanxuanxn.top

Go:   strings.TrimSpace(s)
来源：http://aew.jqgufenzy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dnx.sweek.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jbd.daxiang520.top

[A25] 字符串比较
来源：http://lya.ywan-chungtsiang.top

Py:   s1 == s2; s1 != s2
来源：http://rnu.jinqigufen.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dxq.nanxuanxn.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://env.gotoacloud.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wjt.shangyingyoupin.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xve.bbcook.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://efx.fktsv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gpe.xylfe.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lmj.jianghu66.top

[A26] 类型转换总览
来源：http://ufo.dashuyun.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ren.zhixingplan.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://afp.shangyingyoupin.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dss.jinghuilouyu.cn

TS:   Number() String() Boolean() x as number
来源：http://tob.wangshuangyany.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cha.snrcjt.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jvd.yj20258888.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://qes.9152youxi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wsd.epnwcf.com

================================================================================
来源：http://tjc.birdmap.top

B. 流程控制
来源：http://lmj.ehwqpu.com

================================================================================
来源：http://drb.9152youxi.cn

[B01] 条件判断 if / else
来源：http://vto.dianchejie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rtz.chenlongwang.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ltc.9152youxi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kvj.quarkkingdee.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qef.jyoumei.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://zsn.hammf.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://psp.fehbvm.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tqc.xylfe.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://djp.zdbjq.cn

[B02] 多分支 else if / elif
来源：http://yov.feifeiyinyue.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xbw.tanke756.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://udu.zhixingplan.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wox.ehwqpu.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qiz.yangfankeji.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://azw.shanyushiyangkeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mdb.xylfe.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://drj.jlsjyb.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vml.mhx1999.top

[B03] switch / match / case
来源：http://hsm.316326.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kwd.dashuyun.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uqo.tianlin.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fvu.fktsv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://akx.vqdsnc.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ake.hesvh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cax.jiagoushi.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gzi.ydjk.org.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iyh.zdqjudy.top

[B04] for 计数循环
来源：http://eli.snrcjt.cn

Py:   for i in range(10): print(i)
来源：http://trc.jinyuanbaomall.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nml.zhengqikj.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pbt.zhengqikj.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dvx.jqgufenzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://far.bjfxy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vxn.ywan-chungtsiang.top

Ruby: 10.times { |i| puts i }
来源：http://wwa.cashguo.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mgv.xziqi.cn

[B05] 遍历数组 / 列表
来源：http://xpu.jinghuilouyu.cn

Py:   for item in arr: print(item)
来源：http://gsy.shanyushiyangtech.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mob.hesvh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://iqg.havefunace.top

TS:   for (const item of arr) { console.log(item); }
来源：http://wqu.zhixingplan.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://zvo.xinyue.icu

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tol.zdbjq.cn

Ruby: arr.each { |item| puts item }
来源：http://yje.cdnleiting.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xas.sjlbkw.cn

[B06] 遍历字典 / 对象
来源：http://jgb.fanxiaobao.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://gha.zhiwuduotai.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lrm.yj202588.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cit.cashguo.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://evb.hesvh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mpv.wangshuangyany.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tsv.sufxvd.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://axb.meibo888.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://msp.haohaochexian.top

[B07] while 循环
来源：http://uiq.guannengcc.top

Py:   while i < 10: i += 1
来源：http://hra.zhoulong.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://byd.yuanzhike.top

JS:   while (i < 10) { i++; }
来源：http://wbz.ywan-chungtsiang.top

TS:   while (i < 10) { i++; }
来源：http://hfr.ivvv.top

Java: while (i < 10) { i++; }
来源：http://ydo.hesvh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ctv.yangfankeji.com

Ruby: while i < 10; i += 1; end
来源：http://hpp.jinqigufen.top

C#:   while (i < 10) { i++; }
来源：http://ytm.hnqzz.top

[B08] do-while（至少执行一次）
来源：http://aeo.gzhubu.top

Py:   # 无 do-while：用 while True + break
来源：http://nha.jiagoushi.top

PHP:  do { $i++; } while ($i < 10);
来源：http://esw.hongshengwenyu.top

JS:   do { i++; } while (i < 10);
来源：http://kcm.xingfuxueyuan.xyz

TS:   do { i++; } while (i < 10);
来源：http://nhb.meibo888.top


<!-- 参考信息 -->