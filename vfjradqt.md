代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://pni.chenzaomai.com

Go:   fmt.Println("Hello, World!")
来源：http://tym.fktsv.cn

Ruby: puts "Hello, World!"
来源：http://ana.nanxuanxn.top

C#:   Console.WriteLine("Hello, World!");
来源：http://let.gzhubu.top

[A02] 变量声明与赋值
来源：http://tlo.dianchejie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fax.zhongyouzk.top

PHP:  $name = "Alex"; $age = 20;
来源：http://zpi.nanxinkj.top

JS:   let name = "Alex"; const age = 20;
来源：http://alu.jinghuilouyu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hqu.zhongyouzk.top

Java: String name = "Alex"; int age = 20;
来源：http://vsx.svipenyu.cn

Go:   name := "Alex"; age := 20
来源：http://pjo.shanyushiyangkeji.top

Ruby: name = "Alex"; age = 20
来源：http://xwx.sufxvd.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xkz.xziqi.cn

[A03] 常量定义
来源：http://meo.sxryk.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mlq.shuidangran.top

PHP:  const PI = 3.14159;
来源：http://aac.zhijiandao.cn

JS:   const PI = 3.14159;
来源：http://acf.cashguo.top

TS:   const PI: number = 3.14159;
来源：http://vax.ywan-chungtsiang.top

Java: static final double PI = 3.14159;
来源：http://xtq.9152youxi.cn

Go:   const PI = 3.14159
来源：http://lit.meibo888.top

Ruby: PI = 3.14159
来源：http://yxz.yonumen.top

C#:   const double PI = 3.14159;
来源：http://civ.xziqi.cn

[A04] 判断变量类型
来源：http://uuz.dashuyun.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://imn.jlsjyb.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://opy.tian-w.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cgh.gzhubu.top

TS:   typeof x; x instanceof Date
来源：http://qfe.guannengcc.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cxt.uphjek.com

Go:   reflect.TypeOf(x).Name()
来源：http://qni.nanxuanxn.top

Ruby: x.class; x.is_a?(Integer)
来源：http://hph.zhoulong.xyz

C#:   x.GetType().Name; x is int
来源：http://jbp.guowangkeji.top

[A05] 整数除法与取模
来源：http://egl.chenlongwang.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ata.hnqzz.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ili.cheryme.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bsl.0kj1m.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://swh.shanyushiyangtech.top

Java: 7 / 2; 7 % 2
来源：http://bkr.pycfn.com

Go:   7 / 2; 7 % 2
来源：http://vps.smart0.xyz

Ruby: 7 / 2; 7 % 2
来源：http://vvl.pycfn.com

C#:   7 / 2; 7 % 2
来源：http://kau.fehbvm.com

[A06] 字符串转数字
来源：http://wjz.jlsjyb.cn

Py:   int("42"); float("3.14")
来源：http://wwu.kuanghao11.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ouf.yongpay.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fda.gotoacloud.top

TS:   parseInt("42", 10); Number("42")
来源：http://jgr.shzxlz.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tne.fengsongda.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qxn.hfpthk.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wfp.xinyue.icu

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yal.nanxinkj.top

[A07] 数字转字符串
来源：http://lta.shanyushiyangtech.top

Py:   str(42)
来源：http://dtn.yj20258888.top

PHP:  (string) 42; strval(42)
来源：http://leh.yanxiufei.cn

JS:   String(42); (42).toString()
来源：http://edj.yvedp.cn

TS:   String(42)
来源：http://smd.aizwys.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ymv.ywan-chungtsiang.top

Go:   strconv.Itoa(42)
来源：http://qve.zhengqikj.top

Ruby: 42.to_s
来源：http://lry.fktsv.cn

C#:   42.ToString()
来源：http://ajb.zhongyouzk.top

[A08] 取整与四舍五入
来源：http://pek.yuxming.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kwd.zhengqikj.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vbt.hywenlv.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jfa.gogol.net.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://iiw.zhaomingkeji.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hpf.svipenyu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ono.xinyue.icu

Ruby: 3.567.round(2); 3.9.floor
来源：http://qgu.sweek.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://nsf.jinyuanbaomall.cn

[A09] 绝对值与最大最小值
来源：http://mzg.sysykeji.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://csf.yj20258.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://aze.xziqi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pnc.xziqi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://kaq.ydzc1.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vxy.52xcode.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cag.yvedp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://sbi.jinyuanbaomall.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tpk.hammf.cn

[A10] 生成随机数
来源：http://iet.nanxinkj.top

Py:   import random; random.randint(1, 100)
来源：http://ced.jinyuanbaomall.cn

PHP:  random_int(1, 100);
来源：http://omc.9152youxi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://byw.shangyingyoupin.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rcm.gaohongyu789.top

Java: new Random().nextInt(100) + 1
来源：http://ovp.zhixingplan.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xdv.sufxvd.cn

Ruby: rand(1..100)
来源：http://egp.zhoulong.xyz

C#:   new Random().Next(1, 101)
来源：http://qzj.nwbrower.top

[A11] 条件表达式（三元）
来源：http://wqj.bbcook.cn

Py:   "yes" if x > 0 else "no"
来源：http://sax.feifeiyinyue.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://vmo.gzhubu.top

JS:   x > 0 ? "yes" : "no"
来源：http://ycm.cheryme.top

TS:   x > 0 ? "yes" : "no"
来源：http://ypq.aizwys.cn

Java: x > 0 ? "yes" : "no"
来源：http://zwh.shangyingyoupin.top

Go:   // 无三元运算符，需用 if 语句
来源：http://oto.ppjwa.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://xjz.epnwcf.com

C#:   x > 0 ? "yes" : "no"
来源：http://sog.cdnleiting.top

[A12] 字符串插值 / 格式化
来源：http://ook.jinghuilouyu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bun.ivvv.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zls.chenzaomai.com

JS:   `Hello, ${name}!`
来源：http://xul.epnwcf.com

TS:   `Hello, ${name}!`
来源：http://vbm.dianchejie.cn

Java: "Hello, %s!".formatted(name)
来源：http://vip.jinyuanbaomall.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pvy.xuanzx.com

Ruby: "Hello, #{name}!"
来源：http://gzc.jiagoushi.top

C#:   $"Hello, {name}!"
来源：http://ykt.mhx1999.top

[A13] 多行字符串（练习 \n 转义）
来源：http://raj.yvedp.cn

Py:   "第一行\n第二行"
来源：http://tbe.pycfn.com

PHP:  "第一行\n第二行"
来源：http://klq.jqgufenzy.top

JS:   "第一行\n第二行"
来源：http://tby.9152youxi.cn

TS:   "第一行\n第二行"
来源：http://fvz.shzxlz.cn

Java: "第一行\n第二行"
来源：http://iqn.zhixingplan.top

Go:   "第一行\n第二行"
来源：http://wfo.zhaomingkeji.xyz

Ruby: "第一行\n第二行"
来源：http://bjq.gotoacloud.top

C#:   "第一行\n第二行"
来源：http://ebj.hfpthk.cn

[A14] 注释写法
来源：http://vgc.yj202588.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ssd.hfpthk.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ngy.shuidangran.top

JS:   // 单行；/* 多行 */
来源：http://jig.zhiwuduotai.top

TS:   // 单行；/* 多行 */
来源：http://jjd.kuanghao11.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mbw.shangyingyoupin.top

Go:   // 单行；/* 多行 */
来源：http://tqe.chenlongwang.top

Ruby: # 单行；=begin 多行 =end
来源：http://ccy.xingfuxueyuan.xyz

C#:   // 单行；/* 多行 */
来源：http://dyf.ybcxt.top

[A15] 空值判断与默认值
来源：http://iod.quarkkingdee.top

Py:   value = data or "默认值"
来源：http://rie.xinyue.icu

PHP:  $value = $data ?? "默认值";
来源：http://zhv.tanke756.top

JS:   const value = data ?? "默认值";
来源：http://ynu.uphjek.com

TS:   const value = data ?? "默认值";
来源：http://ydq.quarkkingdee.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zjv.hammf.cn

Go:   if data == "" { data = "默认值" }
来源：http://vko.wangshuangyany.cn

Ruby: value = data || "默认值"
来源：http://cdi.guannengcc.top

C#:   var value = data ?? "默认值";
来源：http://ryw.0kj1m.cn

[A16] 真假值判断规则
来源：http://jul.daria6918.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://irv.xingfuxueyuan.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://uxd.xingfuxueyuan.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://trp.fanxiaobao.xyz

TS:   if (!x) {}
来源：http://cts.fktsv.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tuu.ydjk.org.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fnx.aibaodan.cn

Ruby: unless x            # nil 与 false 为假
来源：http://nyt.meibo888.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://dmy.jqgfzy.top

[A17] 位运算
来源：http://wzp.guannengcc.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ytf.yj202588.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://agf.vehdjk.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kil.yfazqb.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ebm.316326.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ckl.guowangkeji.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xjc.aibaodan.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fbh.jqgfzy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xqw.nwbrower.top

[A18] 字符与 ASCII 码互转
来源：http://mad.hfpthk.cn

Py:   ord("A"); chr(65)
来源：http://sfi.chenzaomai.com

PHP:  ord("A"); chr(65)
来源：http://trl.ydzc1.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vwr.jiagoushi.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vup.jinghuilouyu.cn

Java: (int) 'A'; (char) 65
来源：http://wmh.ivvv.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://shr.jlsjyb.cn

Ruby: "A".ord; 65.chr
来源：http://kjy.birdmap.top

C#:   (int)'A'; (char)65
来源：http://ajk.bjfxy.top

[A19] 交换两个变量
来源：http://etz.zhixingplan.top

Py:   a, b = b, a
来源：http://wyg.gzhubu.top

PHP:  [$a, $b] = [$b, $a];
来源：http://sci.yvedp.cn

JS:   [a, b] = [b, a];
来源：http://tga.zhiwuduotai.top

TS:   [a, b] = [b, a];
来源：http://uaf.xinyue.icu

Java: int t = a; a = b; b = t;
来源：http://tsb.gotoacloud.top

Go:   a, b = b, a
来源：http://rkz.shanyushiyangtech.top

Ruby: a, b = b, a
来源：http://uim.wangdashe.top

C#:   (a, b) = (b, a);
来源：http://arp.zdbjq.cn

[A20] 读取标准输入
来源：http://lrx.pengpengdd.cyou

Py:   name = input("请输入：")
来源：http://pkg.jiagoushi.top

PHP:  $name = trim(fgets(STDIN));
来源：http://cov.dianchejie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gvq.xuanzx.com

TS:   // Node.js：readline 模块
来源：http://hzp.zhixingplan.top

Java: new Scanner(System.in).nextLine()
来源：http://rcb.dianchejie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://htd.svipenyu.cn

Ruby: gets.chomp
来源：http://aae.gaohongyu789.top

C#:   Console.ReadLine();
来源：http://qvr.xinyue.icu

[A21] 保留指定小数位输出
来源：http://jir.jinqigfzy.top

Py:   f"{3.14159:.2f}"
来源：http://rzu.tanke756.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://egl.jqgfzy.top

JS:   (3.14159).toFixed(2)
来源：http://yje.zhoulong.xyz

TS:   (3.14159).toFixed(2)
来源：http://abo.pengpengdd.cyou

Java: String.format("%.2f", 3.14159)
来源：http://psw.zhengqikj.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://acx.yanxiufei.cn

Ruby: format("%.2f", 3.14159)
来源：http://jzl.zhijiandao.cn

C#:   3.14159.ToString("F2")
来源：http://uxx.cucudq.cn

[A22] 获取字符串长度
来源：http://glf.cashguo.top

Py:   len(s)
来源：http://rpe.tarul.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vbm.snrcjt.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zzn.cdnleiting.top

TS:   s.length
来源：http://wct.sysykeji.top

Java: s.length()
来源：http://fre.jqgufenzy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ybm.chenjidiqi.icu

Ruby: s.length
来源：http://gry.havefunace.top

C#:   s.Length
来源：http://kwq.chenzaomai.com

[A23] 大小写转换
来源：http://oxa.cucudq.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tou.redwolf501.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qyj.dianchejie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rsx.gotoacloud.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lzy.ehwqpu.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gem.ybcxt.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ail.xuanzx.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xgy.0kj1m.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qkk.zdbjq.cn

[A24] 去除首尾空白
来源：http://eqe.yvedp.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ner.yuanzhike.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rhr.sufxvd.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xmr.zhiwuduotai.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yan.9152youxi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://utk.hcnkem.com

Go:   strings.TrimSpace(s)
来源：http://jvu.tanke756.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pqo.yuanzhike.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lph.yj20258888.top

[A25] 字符串比较
来源：http://csy.uphjek.com

Py:   s1 == s2; s1 != s2
来源：http://ulx.aibaodan.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nyo.zdqjudy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vjo.wangdashe.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tnx.yangfankeji.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jeq.yongpay.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://eod.zhoulong.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://pbg.aizwys.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lda.meibo888.top

[A26] 类型转换总览
来源：http://ovy.meibo888.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lam.bjfxy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pql.shangyingyoupin.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fza.yanxiufei.cn

TS:   Number() String() Boolean() x as number
来源：http://ust.aibaodan.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vpd.yvedp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cvz.hongshengwenyu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://kel.fktsv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ccx.tian-w.cn

================================================================================
来源：http://wsy.yuxming.cn

B. 流程控制
来源：http://jrt.ydjk.org.cn

================================================================================
来源：http://fkr.hysaishi.cn

[B01] 条件判断 if / else
来源：http://vow.tanke756.top

Py:   result = "正" if x > 0 else "非正"
来源：http://bem.shuidangran.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sjc.yongpay.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mdp.xylfe.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yne.xinyue.icu

Java: String r = x > 0 ? "正" : "非正";
来源：http://ojq.gzhubu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://atw.yanxiufei.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hrd.yuanzhike.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://haa.yj20258.top

[B02] 多分支 else if / elif
来源：http://qqw.jinyuanbaomall.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lsk.shanyushiyangkeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ftu.ivvv.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ofg.hnxiangtu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xrb.zhijiandao.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pyn.fzhhl.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zas.gogol.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://awh.hongshengwenyu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uwj.birdmap.top

[B03] switch / match / case
来源：http://rha.fktsv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zax.zycfv.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://awm.ppjwa.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kta.tianlin.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cuq.chenjidiqi.icu

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mfc.feifeiyinyue.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yhn.yuxming.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qhn.tian-w.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lun.xuanzx.com

[B04] for 计数循环
来源：http://kjx.9152youxi.cn

Py:   for i in range(10): print(i)
来源：http://ffg.gogol.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lox.shanyushiyangtech.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://whe.dianchejie.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kwv.shuidangran.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eoe.zhijiandao.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xle.pycfn.com

Ruby: 10.times { |i| puts i }
来源：http://oyv.zhoulong.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://epl.zdqjudy.top

[B05] 遍历数组 / 列表
来源：http://wyp.tarul.cn

Py:   for item in arr: print(item)
来源：http://srr.tarul.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://axf.quarkkingdee.top

JS:   for (const item of arr) { console.log(item); }
来源：http://wsd.daxiang520.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xsf.nanxuanxn.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://jtw.guannengcc.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pis.mhx1999.top

Ruby: arr.each { |item| puts item }
来源：http://rki.hywenlv.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pxl.jqgfzy.top

[B06] 遍历字典 / 对象
来源：http://lko.fzhhl.top

Py:   for k, v in d.items(): print(k, v)
来源：http://mwh.xylfe.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sjn.ydjk.org.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dqc.daria6918.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pjg.xziqi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gvq.ehwqpu.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jnr.jinqigfzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bpc.ywan-chungtsiang.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mjj.shzxlz.cn

[B07] while 循环
来源：http://zuk.ydzc1.top

Py:   while i < 10: i += 1
来源：http://dtd.cashguo.top

PHP:  while ($i < 10) { $i++; }
来源：http://dyj.vehdjk.com

JS:   while (i < 10) { i++; }
来源：http://ixm.vehdjk.com

TS:   while (i < 10) { i++; }
来源：http://rgs.guowangkeji.top

Java: while (i < 10) { i++; }
来源：http://urr.uphjek.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jfo.nwbrower.top

Ruby: while i < 10; i += 1; end
来源：http://orr.zhongyouzk.top

C#:   while (i < 10) { i++; }
来源：http://tnz.daria6918.cn

[B08] do-while（至少执行一次）
来源：http://elr.tarul.cn

Py:   # 无 do-while：用 while True + break
来源：http://tgz.c1oappe.top

PHP:  do { $i++; } while ($i < 10);
来源：http://nnp.sufxvd.cn

JS:   do { i++; } while (i < 10);
来源：http://inl.ydzc1.top

TS:   do { i++; } while (i < 10);
来源：http://wpt.ivvv.top


<!-- 参考信息 -->