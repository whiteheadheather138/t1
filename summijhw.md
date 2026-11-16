代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://yzg.hfpthk.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hdl.dianchejie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wxu.birdmap.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yxf.guowangkeji.top

================================================================================
来源：http://iaq.gzhubu.top

A. 基础语法与类型
来源：http://loc.yj202588.top

================================================================================
来源：http://ocw.havefunace.top

[A01] Hello World
来源：http://bey.zhaomingkeji.xyz

Py:   print("Hello, World!")
来源：http://nuq.yonumen.top

PHP:  echo "Hello, World!";
来源：http://ttv.pengpengdd.cyou

JS:   console.log("Hello, World!");
来源：http://eon.hcnkem.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sjx.zhaomingkeji.xyz

Java: System.out.println("Hello, World!");
来源：http://dgg.fengsongda.top

Go:   fmt.Println("Hello, World!")
来源：http://czx.tian-w.cn

Ruby: puts "Hello, World!"
来源：http://kli.aizwys.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fbt.yuanzhike.top

[A02] 变量声明与赋值
来源：http://cvm.c1oappe.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xtj.zhongyouzk.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ukj.yonumen.top

JS:   let name = "Alex"; const age = 20;
来源：http://eyp.epnwcf.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ttr.meibo888.top

Java: String name = "Alex"; int age = 20;
来源：http://gvy.aizwys.cn

Go:   name := "Alex"; age := 20
来源：http://shc.ybcxt.top

Ruby: name = "Alex"; age = 20
来源：http://ask.yongpay.top

C#:   string name = "Alex"; int age = 20;
来源：http://hcc.gogol.net.cn

[A03] 常量定义
来源：http://dxa.hesvh.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hkp.chenjidiqi.icu

PHP:  const PI = 3.14159;
来源：http://eya.jinqigfzy.top

JS:   const PI = 3.14159;
来源：http://uqf.zhongyouzk.top

TS:   const PI: number = 3.14159;
来源：http://lnj.hesvh.cn

Java: static final double PI = 3.14159;
来源：http://kwe.yanxiufei.cn

Go:   const PI = 3.14159
来源：http://yky.yj202588.top

Ruby: PI = 3.14159
来源：http://uhs.jqgufenzy.top

C#:   const double PI = 3.14159;
来源：http://dtw.fengsongda.top

[A04] 判断变量类型
来源：http://daq.cashguo.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://skd.zhixingplan.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wvf.uphjek.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://sul.nanxuanxn.top

TS:   typeof x; x instanceof Date
来源：http://hyo.fehbvm.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hsb.gogol.net.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bks.xylfe.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://sfb.zycfv.cn

C#:   x.GetType().Name; x is int
来源：http://dmp.sjlbkw.cn

[A05] 整数除法与取模
来源：http://pbh.zhiwuduotai.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jbn.hesvh.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://neb.jinqigfzy.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vjj.guannengcc.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rns.fzhhl.top

Java: 7 / 2; 7 % 2
来源：http://gxh.zhixingplan.top

Go:   7 / 2; 7 % 2
来源：http://xws.sufxvd.cn

Ruby: 7 / 2; 7 % 2
来源：http://ehh.zhixingplan.top

C#:   7 / 2; 7 % 2
来源：http://nju.316326.xyz

[A06] 字符串转数字
来源：http://aoj.ppjwa.cn

Py:   int("42"); float("3.14")
来源：http://naq.ivvv.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ezw.hywenlv.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jmn.wangshuangyany.cn

TS:   parseInt("42", 10); Number("42")
来源：http://txh.shzxlz.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://evy.bjfxy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mzj.ybcxt.top

Ruby: "42".to_i; "3.14".to_f
来源：http://jya.yj202588.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pdq.haohaochexian.top

[A07] 数字转字符串
来源：http://qkh.shuidangran.top

Py:   str(42)
来源：http://xwc.iojbl.cn

PHP:  (string) 42; strval(42)
来源：http://avh.snrcjt.cn

JS:   String(42); (42).toString()
来源：http://fek.iojbl.cn

TS:   String(42)
来源：http://ocs.52xcode.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://tve.c1oappe.top

Go:   strconv.Itoa(42)
来源：http://cgd.hcnkem.com

Ruby: 42.to_s
来源：http://ibx.hysaishi.cn

C#:   42.ToString()
来源：http://ujl.yfazqb.com

[A08] 取整与四舍五入
来源：http://gnb.zhiwuduotai.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mth.epnwcf.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ghu.bjfxy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://var.jiagoushi.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://how.meibo888.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nhs.cashguo.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pmr.jinghuilouyu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://spj.meibo888.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yee.gzhubu.top

[A09] 绝对值与最大最小值
来源：http://ije.ywan-chungtsiang.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pnv.52xcode.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yuh.yuxming.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hwh.ehwqpu.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fnq.hcnkem.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pqh.sxryk.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tko.hfpthk.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://csy.jyoumei.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ibo.9152youxi.cn

[A10] 生成随机数
来源：http://rlu.quarkkingdee.top

Py:   import random; random.randint(1, 100)
来源：http://hfz.yj202588.top

PHP:  random_int(1, 100);
来源：http://gxb.nwbrower.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://elt.nwbrower.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gpa.chenlongwang.top

Java: new Random().nextInt(100) + 1
来源：http://nbp.hysaishi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qsz.ivvv.top

Ruby: rand(1..100)
来源：http://mss.jinqigufen.top

C#:   new Random().Next(1, 101)
来源：http://jho.pycfn.com

[A11] 条件表达式（三元）
来源：http://fkq.cucudq.cn

Py:   "yes" if x > 0 else "no"
来源：http://wlk.wangshuangyany.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://hej.quarkkingdee.top

JS:   x > 0 ? "yes" : "no"
来源：http://fzy.gaohongyu789.top

TS:   x > 0 ? "yes" : "no"
来源：http://rad.fzhhl.top

Java: x > 0 ? "yes" : "no"
来源：http://mvb.iojbl.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xxf.hysaishi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://knm.ehwqpu.com

C#:   x > 0 ? "yes" : "no"
来源：http://zpj.tian-w.cn

[A12] 字符串插值 / 格式化
来源：http://kxj.yangfankeji.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://voo.shanyushiyangkeji.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://acd.andypj.xyz

JS:   `Hello, ${name}!`
来源：http://jor.yj20258888.top

TS:   `Hello, ${name}!`
来源：http://hjx.hongshengwenyu.top

Java: "Hello, %s!".formatted(name)
来源：http://gbq.9152youxi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tak.shanyushiyangkeji.top

Ruby: "Hello, #{name}!"
来源：http://viw.jyoumei.cn

C#:   $"Hello, {name}!"
来源：http://zyk.yj20258.top

[A13] 多行字符串（练习 \n 转义）
来源：http://pcd.fanxiaobao.xyz

Py:   "第一行\n第二行"
来源：http://npg.zhiwuduotai.top

PHP:  "第一行\n第二行"
来源：http://oyw.sweek.top

JS:   "第一行\n第二行"
来源：http://zgq.fehbvm.com

TS:   "第一行\n第二行"
来源：http://kww.pengpengdd.cyou

Java: "第一行\n第二行"
来源：http://mxo.nwbrower.top

Go:   "第一行\n第二行"
来源：http://qpj.zhaomingkeji.xyz

Ruby: "第一行\n第二行"
来源：http://bpq.gaohongyu789.top

C#:   "第一行\n第二行"
来源：http://fcu.sysykeji.top

[A14] 注释写法
来源：http://aie.pycfn.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://fam.vehdjk.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://euq.andypj.xyz

JS:   // 单行；/* 多行 */
来源：http://sbp.nanxuanxn.top

TS:   // 单行；/* 多行 */
来源：http://jhs.shanyushiyangtech.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zau.zhoulong.xyz

Go:   // 单行；/* 多行 */
来源：http://cly.52xcode.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wxq.ywan-chungtsiang.top

C#:   // 单行；/* 多行 */
来源：http://jhp.xingfuxueyuan.xyz

[A15] 空值判断与默认值
来源：http://dwl.sysykeji.top

Py:   value = data or "默认值"
来源：http://ozo.pycfn.com

PHP:  $value = $data ?? "默认值";
来源：http://htg.gogol.net.cn

JS:   const value = data ?? "默认值";
来源：http://ngb.yfazqb.com

TS:   const value = data ?? "默认值";
来源：http://ooo.xinyue.icu

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://uxt.guannengcc.top

Go:   if data == "" { data = "默认值" }
来源：http://qkw.ctjpmb.com

Ruby: value = data || "默认值"
来源：http://zme.gogol.net.cn

C#:   var value = data ?? "默认值";
来源：http://xwo.c1oappe.top

[A16] 真假值判断规则
来源：http://sbm.smart0.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gua.guannengcc.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://akx.yuxming.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lxy.nanxinkj.top

TS:   if (!x) {}
来源：http://njh.yuxming.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ukv.yj20258.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://daa.xuanzx.com

Ruby: unless x            # nil 与 false 为假
来源：http://iwl.feifeiyinyue.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zeb.aizwys.cn

[A17] 位运算
来源：http://rwd.hywenlv.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fri.ybcxt.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://com.zhaomingkeji.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fsd.316326.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wam.fanxiaobao.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iwp.sjlbkw.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nmf.ehwqpu.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kej.jianghu66.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nsh.gzhubu.top

[A18] 字符与 ASCII 码互转
来源：http://ado.shangyingyoupin.top

Py:   ord("A"); chr(65)
来源：http://yya.hysaishi.cn

PHP:  ord("A"); chr(65)
来源：http://agd.tanke756.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://usp.redwolf501.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kqr.iojbl.cn

Java: (int) 'A'; (char) 65
来源：http://dzt.dashuyun.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pkj.xuanzx.com

Ruby: "A".ord; 65.chr
来源：http://fmw.aibaodan.cn

C#:   (int)'A'; (char)65
来源：http://jjk.havefunace.top

[A19] 交换两个变量
来源：http://jat.wangdashe.top

Py:   a, b = b, a
来源：http://wvf.yongpay.top

PHP:  [$a, $b] = [$b, $a];
来源：http://koc.jlsjyb.cn

JS:   [a, b] = [b, a];
来源：http://ceg.yueranfly.top

TS:   [a, b] = [b, a];
来源：http://mun.ppjwa.cn

Java: int t = a; a = b; b = t;
来源：http://cdb.zhijiandao.cn

Go:   a, b = b, a
来源：http://mki.yuanzhike.top

Ruby: a, b = b, a
来源：http://xeg.redwolf501.top

C#:   (a, b) = (b, a);
来源：http://qjr.haohaochexian.top

[A20] 读取标准输入
来源：http://sxz.yuanzhike.top

Py:   name = input("请输入：")
来源：http://rwd.fzhhl.top

PHP:  $name = trim(fgets(STDIN));
来源：http://gwq.ybcxt.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qot.hammf.cn

TS:   // Node.js：readline 模块
来源：http://ehf.xylfe.cn

Java: new Scanner(System.in).nextLine()
来源：http://vhq.daria6918.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gly.uphjek.com

Ruby: gets.chomp
来源：http://xnk.gzhubu.top

C#:   Console.ReadLine();
来源：http://xbi.haohaochexian.top

[A21] 保留指定小数位输出
来源：http://min.jinghuilouyu.cn

Py:   f"{3.14159:.2f}"
来源：http://dut.bjfxy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://omr.haohaochexian.top

JS:   (3.14159).toFixed(2)
来源：http://tpc.jinqigfzy.top

TS:   (3.14159).toFixed(2)
来源：http://iqy.cdnleiting.top

Java: String.format("%.2f", 3.14159)
来源：http://wqt.xuetiantiany.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://koh.0kj1m.cn

Ruby: format("%.2f", 3.14159)
来源：http://hwd.ppjwa.cn

C#:   3.14159.ToString("F2")
来源：http://lqx.yvedp.cn

[A22] 获取字符串长度
来源：http://pyx.xuanzx.com

Py:   len(s)
来源：http://pdt.hammf.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yjy.jlsjyb.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nbp.cucudq.cn

TS:   s.length
来源：http://jdn.nanxuanxn.top

Java: s.length()
来源：http://elw.hnqzz.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://saf.jiagoushi.top

Ruby: s.length
来源：http://kds.jiagoushi.top

C#:   s.Length
来源：http://dgu.yj20258.top

[A23] 大小写转换
来源：http://xyj.quarkkingdee.top

Py:   s.upper(); s.lower(); s.title()
来源：http://zey.fanxiaobao.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hrg.hnxiangtu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://euq.xziqi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://idz.aibaodan.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://iib.ybcxt.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://buy.chenlongwang.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lup.hnxiangtu.top

C#:   s.ToUpper(); s.ToLower()
来源：http://fat.hongshengwenyu.top

[A24] 去除首尾空白
来源：http://vwu.meibo888.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jbw.kuanghao11.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mjc.zhixingplan.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ezj.redwolf501.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://veo.dashuyun.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ffj.tarul.cn

Go:   strings.TrimSpace(s)
来源：http://fje.hcnkem.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jop.xylfe.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pfy.uphjek.com

[A25] 字符串比较
来源：http://nae.fehbvm.com

Py:   s1 == s2; s1 != s2
来源：http://qao.xziqi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bgq.xingfuxueyuan.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jls.cheryme.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kdc.c1oappe.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dun.mhx1999.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jsy.yanxiufei.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://maq.fktsv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://oke.guannengcc.top

[A26] 类型转换总览
来源：http://lfd.fengsongda.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kec.zhoulong.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kdd.bbcook.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nvr.yuanzhike.top

TS:   Number() String() Boolean() x as number
来源：http://vhe.nanxinkj.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://psr.wangdashe.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zcz.zhoulong.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://jxz.wangdashe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ywp.smart0.xyz

================================================================================
来源：http://mvy.tanke756.top

B. 流程控制
来源：http://bry.xingfuxueyuan.xyz

================================================================================
来源：http://kds.xingfuxueyuan.xyz

[B01] 条件判断 if / else
来源：http://itf.yfazqb.com

Py:   result = "正" if x > 0 else "非正"
来源：http://amz.snrcjt.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fmk.sysykeji.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pdf.zhijiandao.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xyk.ivvv.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://nmv.yuanzhike.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nhg.yfazqb.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://srd.ivvv.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uah.fanxiaobao.xyz

[B02] 多分支 else if / elif
来源：http://esl.chenlongwang.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://oyd.jinqigfzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pan.svipenyu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wmf.nanxuanxn.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fyx.nanxuanxn.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qbb.fehbvm.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://usv.ybcxt.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bjm.vqdsnc.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xff.aibaodan.cn

[B03] switch / match / case
来源：http://mmj.hongshengwenyu.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wns.yvedp.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fns.hongshengwenyu.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nki.daxiang520.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lle.sufxvd.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wub.ywan-chungtsiang.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gcl.zhengqikj.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lmy.jlsjyb.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uvv.yuxming.cn

[B04] for 计数循环
来源：http://ufe.gaohongyu789.top

Py:   for i in range(10): print(i)
来源：http://ibv.zhixingplan.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kqv.bbcook.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iyq.daxiang520.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gnv.daxiang520.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ugm.yongpay.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pwd.ybcxt.top

Ruby: 10.times { |i| puts i }
来源：http://nml.chenjidiqi.icu

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://erc.jqgfzy.top

[B05] 遍历数组 / 列表
来源：http://jmf.tian-w.cn

Py:   for item in arr: print(item)
来源：http://mwt.zhongyouzk.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pwb.mhx1999.top

JS:   for (const item of arr) { console.log(item); }
来源：http://lor.gogol.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://vbf.sjlbkw.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zgi.ywan-chungtsiang.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tew.zhaomingkeji.xyz

Ruby: arr.each { |item| puts item }
来源：http://ptg.shzxlz.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hqe.yongpay.top

[B06] 遍历字典 / 对象
来源：http://zas.jinqigfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://hiz.xuanzx.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://woi.hnqzz.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hmw.epnwcf.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vox.hfpthk.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://frr.yueranfly.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://iwy.c1oappe.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rsa.cqqwz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ein.yfazqb.com

[B07] while 循环
来源：http://uut.zhaomingkeji.xyz

Py:   while i < 10: i += 1
来源：http://ktf.cashguo.top


<!-- 参考信息 -->