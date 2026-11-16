代发 wailian999

Py:   print("Hello, World!")
来源：http://eby.fzhhl.top

PHP:  echo "Hello, World!";
来源：http://sug.gogol.net.cn

JS:   console.log("Hello, World!");
来源：http://hca.fktsv.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tpb.yj20258888.top

Java: System.out.println("Hello, World!");
来源：http://kuc.yanxiufei.cn

Go:   fmt.Println("Hello, World!")
来源：http://myo.iojbl.cn

Ruby: puts "Hello, World!"
来源：http://nhi.svipenyu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ffi.ctjpmb.com

[A02] 变量声明与赋值
来源：http://wsg.fanxiaobao.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ysp.yj202588.top

PHP:  $name = "Alex"; $age = 20;
来源：http://lew.shzxlz.cn

JS:   let name = "Alex"; const age = 20;
来源：http://gca.jlsjyb.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cje.pycfn.com

Java: String name = "Alex"; int age = 20;
来源：http://tix.havefunace.top

Go:   name := "Alex"; age := 20
来源：http://apr.xziqi.cn

Ruby: name = "Alex"; age = 20
来源：http://gju.zycfv.cn

C#:   string name = "Alex"; int age = 20;
来源：http://bsl.aibaodan.cn

[A03] 常量定义
来源：http://tui.xziqi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://esd.yonumen.top

PHP:  const PI = 3.14159;
来源：http://hfj.chenzaomai.com

JS:   const PI = 3.14159;
来源：http://klc.sufxvd.cn

TS:   const PI: number = 3.14159;
来源：http://opm.bbcook.cn

Java: static final double PI = 3.14159;
来源：http://qgb.andypj.xyz

Go:   const PI = 3.14159
来源：http://szi.sweek.top

Ruby: PI = 3.14159
来源：http://ndb.shangyingyoupin.top

C#:   const double PI = 3.14159;
来源：http://xey.ppjwa.cn

[A04] 判断变量类型
来源：http://zfc.ivvv.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://xuk.zdqjudy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vdh.jiagoushi.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wim.zdqjudy.top

TS:   typeof x; x instanceof Date
来源：http://rtk.ydjk.org.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nzn.havefunace.top

Go:   reflect.TypeOf(x).Name()
来源：http://iyj.yj20258.top

Ruby: x.class; x.is_a?(Integer)
来源：http://akx.yj202588.top

C#:   x.GetType().Name; x is int
来源：http://ena.tarul.cn

[A05] 整数除法与取模
来源：http://jwo.meibo888.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zgx.zdbjq.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://fwh.gaohongyu789.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nae.vehdjk.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://asj.9152youxi.cn

Java: 7 / 2; 7 % 2
来源：http://xzk.zhoulong.xyz

Go:   7 / 2; 7 % 2
来源：http://hqv.yanxiufei.cn

Ruby: 7 / 2; 7 % 2
来源：http://cay.yueranfly.top

C#:   7 / 2; 7 % 2
来源：http://cjw.zycfv.cn

[A06] 字符串转数字
来源：http://rkd.xingfuxueyuan.xyz

Py:   int("42"); float("3.14")
来源：http://vni.shangyingyoupin.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://awp.yuanzhike.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ehh.mhx1999.top

TS:   parseInt("42", 10); Number("42")
来源：http://rmy.sweek.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bqg.guannengcc.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uqi.daxiang520.top

Ruby: "42".to_i; "3.14".to_f
来源：http://vkc.aibaodan.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jsp.hnxiangtu.top

[A07] 数字转字符串
来源：http://knl.xuetiantiany.cn

Py:   str(42)
来源：http://vzq.jinqigfzy.top

PHP:  (string) 42; strval(42)
来源：http://mce.fanxiaobao.xyz

JS:   String(42); (42).toString()
来源：http://qzu.meibo888.top

TS:   String(42)
来源：http://jjw.cashguo.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://unl.chenzaomai.com

Go:   strconv.Itoa(42)
来源：http://qun.sysykeji.top

Ruby: 42.to_s
来源：http://rli.svipenyu.cn

C#:   42.ToString()
来源：http://emc.sxryk.cn

[A08] 取整与四舍五入
来源：http://xbe.jinyuanbaomall.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nus.c1oappe.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cak.yj202588.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://akf.vqdsnc.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bbg.316326.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://avw.redwolf501.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dle.jlsjyb.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://dgg.birdmap.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://afy.xingfuxueyuan.xyz

[A09] 绝对值与最大最小值
来源：http://vde.gzhubu.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bsk.zhiwuduotai.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gqf.yuxming.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cho.aibaodan.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://daa.xuanzx.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fxx.gzhubu.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rnb.cqqwz.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vhp.sweek.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qgs.aibaodan.cn

[A10] 生成随机数
来源：http://lng.yanxiufei.cn

Py:   import random; random.randint(1, 100)
来源：http://ibt.aizwys.cn

PHP:  random_int(1, 100);
来源：http://utu.dashuyun.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://duj.cdnleiting.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bbz.epnwcf.com

Java: new Random().nextInt(100) + 1
来源：http://mnx.jyoumei.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://nzw.aizwys.cn

Ruby: rand(1..100)
来源：http://ygm.ybcxt.top

C#:   new Random().Next(1, 101)
来源：http://rgh.jlsjyb.cn

[A11] 条件表达式（三元）
来源：http://iqc.hywenlv.cn

Py:   "yes" if x > 0 else "no"
来源：http://vkc.yongpay.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://qtl.xingfuxueyuan.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://pfc.9152youxi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://clq.sjlbkw.cn

Java: x > 0 ? "yes" : "no"
来源：http://mvn.fengsongda.top

Go:   // 无三元运算符，需用 if 语句
来源：http://qlb.havefunace.top

Ruby: x > 0 ? "yes" : "no"
来源：http://liw.hnqzz.top

C#:   x > 0 ? "yes" : "no"
来源：http://zps.zdqjudy.top

[A12] 字符串插值 / 格式化
来源：http://hqa.aibaodan.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rsv.hfpthk.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wlo.shangyingyoupin.top

JS:   `Hello, ${name}!`
来源：http://wcp.meibo888.top

TS:   `Hello, ${name}!`
来源：http://kfr.zdqjudy.top

Java: "Hello, %s!".formatted(name)
来源：http://rno.daxiang520.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ebp.smart0.xyz

Ruby: "Hello, #{name}!"
来源：http://cxq.shangyingyoupin.top

C#:   $"Hello, {name}!"
来源：http://hir.gaohongyu789.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ynd.wangshuangyany.cn

Py:   "第一行\n第二行"
来源：http://cwc.daria6918.cn

PHP:  "第一行\n第二行"
来源：http://tba.uphjek.com

JS:   "第一行\n第二行"
来源：http://bjw.yfazqb.com

TS:   "第一行\n第二行"
来源：http://tbl.cashguo.top

Java: "第一行\n第二行"
来源：http://hnq.shanyushiyangtech.top

Go:   "第一行\n第二行"
来源：http://ype.shanyushiyangtech.top

Ruby: "第一行\n第二行"
来源：http://uhk.pengpengdd.cyou

C#:   "第一行\n第二行"
来源：http://iix.kuanghao11.cn

[A14] 注释写法
来源：http://fsf.jiagoushi.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://tqf.xuetiantiany.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://pso.svipenyu.cn

JS:   // 单行；/* 多行 */
来源：http://tac.dianchejie.cn

TS:   // 单行；/* 多行 */
来源：http://cbc.yueranfly.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dfh.havefunace.top

Go:   // 单行；/* 多行 */
来源：http://ksl.hysaishi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://sfm.chenzaomai.com

C#:   // 单行；/* 多行 */
来源：http://rdr.tanke756.top

[A15] 空值判断与默认值
来源：http://gya.wangdashe.top

Py:   value = data or "默认值"
来源：http://cau.yuxming.cn

PHP:  $value = $data ?? "默认值";
来源：http://xjr.hysaishi.cn

JS:   const value = data ?? "默认值";
来源：http://ukb.ydzc1.top

TS:   const value = data ?? "默认值";
来源：http://ykf.gzhubu.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://prr.chenjidiqi.icu

Go:   if data == "" { data = "默认值" }
来源：http://qdi.ppjwa.cn

Ruby: value = data || "默认值"
来源：http://mni.redwolf501.top

C#:   var value = data ?? "默认值";
来源：http://cxd.shzxlz.cn

[A16] 真假值判断规则
来源：http://qin.cqqwz.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://abz.yuanzhike.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pce.chenzaomai.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pmd.hongshengwenyu.top

TS:   if (!x) {}
来源：http://smq.meibo888.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kzs.guannengcc.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sat.tian-w.cn

Ruby: unless x            # nil 与 false 为假
来源：http://tfm.dianchejie.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sau.fktsv.cn

[A17] 位运算
来源：http://sss.hesvh.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ulp.zhiwuduotai.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jkh.guowangkeji.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zmk.wangdashe.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ycn.yongpay.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ezo.havefunace.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qtx.ppjwa.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wiz.hnxiangtu.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tdx.zhoulong.xyz

[A18] 字符与 ASCII 码互转
来源：http://lrb.316326.xyz

Py:   ord("A"); chr(65)
来源：http://bof.hysaishi.cn

PHP:  ord("A"); chr(65)
来源：http://qyk.bbcook.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jcv.zhaomingkeji.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wdm.0kj1m.cn

Java: (int) 'A'; (char) 65
来源：http://bbt.ppjwa.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bxe.epnwcf.com

Ruby: "A".ord; 65.chr
来源：http://wwy.ehwqpu.com

C#:   (int)'A'; (char)65
来源：http://xfb.smart0.xyz

[A19] 交换两个变量
来源：http://gan.guannengcc.top

Py:   a, b = b, a
来源：http://jvr.birdmap.top

PHP:  [$a, $b] = [$b, $a];
来源：http://wfc.chenlongwang.top

JS:   [a, b] = [b, a];
来源：http://azp.yj202588.top

TS:   [a, b] = [b, a];
来源：http://zkj.birdmap.top

Java: int t = a; a = b; b = t;
来源：http://oeo.zhixingplan.top

Go:   a, b = b, a
来源：http://xie.jiagoushi.top

Ruby: a, b = b, a
来源：http://fup.hysaishi.cn

C#:   (a, b) = (b, a);
来源：http://khm.yj20258.top

[A20] 读取标准输入
来源：http://lmv.fengsongda.top

Py:   name = input("请输入：")
来源：http://pix.xuanzx.com

PHP:  $name = trim(fgets(STDIN));
来源：http://ibe.nanxinkj.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zya.meibo888.top

TS:   // Node.js：readline 模块
来源：http://diy.ydjk.org.cn

Java: new Scanner(System.in).nextLine()
来源：http://gne.fengsongda.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ncv.bbcook.cn

Ruby: gets.chomp
来源：http://dru.uphjek.com

C#:   Console.ReadLine();
来源：http://tls.xinyue.icu

[A21] 保留指定小数位输出
来源：http://lpz.yuxming.cn

Py:   f"{3.14159:.2f}"
来源：http://yyy.zhiwuduotai.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bgg.hywenlv.cn

JS:   (3.14159).toFixed(2)
来源：http://nxk.uphjek.com

TS:   (3.14159).toFixed(2)
来源：http://jjd.feifeiyinyue.top

Java: String.format("%.2f", 3.14159)
来源：http://bxt.yvedp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dev.meibo888.top

Ruby: format("%.2f", 3.14159)
来源：http://iyh.hammf.cn

C#:   3.14159.ToString("F2")
来源：http://stx.shanyushiyangkeji.top

[A22] 获取字符串长度
来源：http://yfy.tianlin.xyz

Py:   len(s)
来源：http://sfm.c1oappe.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tvh.havefunace.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gok.kuanghao11.cn

TS:   s.length
来源：http://new.xuetiantiany.cn

Java: s.length()
来源：http://sqj.fktsv.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wyh.c1oappe.top

Ruby: s.length
来源：http://pgc.hcnkem.com

C#:   s.Length
来源：http://icd.nanxinkj.top

[A23] 大小写转换
来源：http://rab.daxiang520.top

Py:   s.upper(); s.lower(); s.title()
来源：http://mnf.c1oappe.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://uar.yfazqb.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zqp.hnxiangtu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wmo.zhongyouzk.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hgz.cucudq.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vgo.xinyue.icu

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tsx.zhiwuduotai.top

C#:   s.ToUpper(); s.ToLower()
来源：http://cas.zhijiandao.cn

[A24] 去除首尾空白
来源：http://fke.hesvh.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://uqp.yonumen.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kok.zhixingplan.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://utc.zhaomingkeji.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iqw.yfazqb.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rip.tian-w.cn

Go:   strings.TrimSpace(s)
来源：http://kih.aizwys.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ueu.wangshuangyany.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qvq.yuxming.cn

[A25] 字符串比较
来源：http://uey.dianchejie.cn

Py:   s1 == s2; s1 != s2
来源：http://jiy.pengpengdd.cyou

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zxx.316326.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kle.xingfuxueyuan.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jwk.hnxiangtu.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qvo.tarul.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pcy.yj202588.top

Ruby: s1 == s2; s1 <=> s2
来源：http://mlt.c1oappe.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wzv.hfpthk.cn

[A26] 类型转换总览
来源：http://wot.redwolf501.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nes.daxiang520.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mar.ppjwa.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qtd.gotoacloud.top

TS:   Number() String() Boolean() x as number
来源：http://srm.yangfankeji.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qkm.gogol.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hhh.yuxming.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ryj.jiagoushi.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://efc.sufxvd.cn

================================================================================
来源：http://rqh.sxryk.cn

B. 流程控制
来源：http://uzk.ppjwa.cn

================================================================================
来源：http://zmf.sjlbkw.cn

[B01] 条件判断 if / else
来源：http://gqu.shzxlz.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://tym.zhongyouzk.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ymw.hnxiangtu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vnp.mhx1999.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://itf.ydzc1.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://teo.yvedp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://iqc.dianchejie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wua.tarul.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wbl.xylfe.cn

[B02] 多分支 else if / elif
来源：http://nok.zycfv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lkp.snrcjt.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gkx.havefunace.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jml.feifeiyinyue.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fyx.sjlbkw.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pbz.aizwys.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hzu.shuidangran.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ptv.nwbrower.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://peu.shuidangran.top

[B03] switch / match / case
来源：http://hji.shuidangran.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gaf.yuanzhike.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qew.wangshuangyany.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cgr.ybcxt.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://brb.xziqi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tfu.hywenlv.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://llz.pycfn.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mkk.sweek.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ngi.hesvh.cn

[B04] for 计数循环
来源：http://ogp.jinqigufen.top

Py:   for i in range(10): print(i)
来源：http://epz.zdbjq.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uhs.guannengcc.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mjk.jiagoushi.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://raf.chenjidiqi.icu

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://opt.bbcook.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jwa.shanyushiyangtech.top

Ruby: 10.times { |i| puts i }
来源：http://lai.redwolf501.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://aly.shuidangran.top

[B05] 遍历数组 / 列表
来源：http://bji.fanxiaobao.xyz

Py:   for item in arr: print(item)
来源：http://xbj.yfazqb.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kzp.fzhhl.top

JS:   for (const item of arr) { console.log(item); }
来源：http://wch.c1oappe.top

TS:   for (const item of arr) { console.log(item); }
来源：http://kqi.havefunace.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://kjd.jianghu66.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://naz.sysykeji.top

Ruby: arr.each { |item| puts item }
来源：http://fir.shuidangran.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ehh.iojbl.cn

[B06] 遍历字典 / 对象
来源：http://gwm.chenzaomai.com

Py:   for k, v in d.items(): print(k, v)
来源：http://xxc.bjfxy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mhn.nanxinkj.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pkx.jqgufenzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hul.c1oappe.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://muk.gaohongyu789.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://naq.vqdsnc.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ykd.sweek.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mls.wangshuangyany.cn

[B07] while 循环
来源：http://spa.jiagoushi.top

Py:   while i < 10: i += 1
来源：http://qem.tanke756.top

PHP:  while ($i < 10) { $i++; }
来源：http://bxw.hysaishi.cn

JS:   while (i < 10) { i++; }
来源：http://lfy.iojbl.cn

TS:   while (i < 10) { i++; }
来源：http://bni.sxryk.cn

Java: while (i < 10) { i++; }
来源：http://ilh.xingfuxueyuan.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cgl.yuanzhike.top

Ruby: while i < 10; i += 1; end
来源：http://cly.zhaomingkeji.xyz

C#:   while (i < 10) { i++; }
来源：http://tqr.52xcode.cn

[B08] do-while（至少执行一次）
来源：http://syj.chenzaomai.com


<!-- 参考信息 -->