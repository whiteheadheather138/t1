代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://dez.sweek.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yis.zhixingplan.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ntu.redwolf501.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://agb.yuxming.cn

================================================================================
来源：http://rex.aibaodan.cn

A. 基础语法与类型
来源：http://bpa.yonumen.top

================================================================================
来源：http://qap.0kj1m.cn

[A01] Hello World
来源：http://tbq.xingfuxueyuan.xyz

Py:   print("Hello, World!")
来源：http://mfn.jyoumei.cn

PHP:  echo "Hello, World!";
来源：http://ioc.cdnleiting.top

JS:   console.log("Hello, World!");
来源：http://kqo.yj20258888.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://dmt.epnwcf.com

Java: System.out.println("Hello, World!");
来源：http://cgg.nwbrower.top

Go:   fmt.Println("Hello, World!")
来源：http://kic.xingfuxueyuan.xyz

Ruby: puts "Hello, World!"
来源：http://smh.sxryk.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hou.iojbl.cn

[A02] 变量声明与赋值
来源：http://ywq.guannengcc.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pkp.tanke756.top

PHP:  $name = "Alex"; $age = 20;
来源：http://rri.ydzc1.top

JS:   let name = "Alex"; const age = 20;
来源：http://mcj.mhx1999.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tgm.hesvh.cn

Java: String name = "Alex"; int age = 20;
来源：http://kuq.gotoacloud.top

Go:   name := "Alex"; age := 20
来源：http://xsu.aizwys.cn

Ruby: name = "Alex"; age = 20
来源：http://wjv.yanxiufei.cn

C#:   string name = "Alex"; int age = 20;
来源：http://smh.chenjidiqi.icu

[A03] 常量定义
来源：http://hkl.gogol.net.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://scm.xziqi.cn

PHP:  const PI = 3.14159;
来源：http://qil.yuanzhike.top

JS:   const PI = 3.14159;
来源：http://eug.xuetiantiany.cn

TS:   const PI: number = 3.14159;
来源：http://rzg.xinyue.icu

Java: static final double PI = 3.14159;
来源：http://ywq.zhengqikj.top

Go:   const PI = 3.14159
来源：http://nvn.kuanghao11.cn

Ruby: PI = 3.14159
来源：http://fnd.yj202588.top

C#:   const double PI = 3.14159;
来源：http://xda.andypj.xyz

[A04] 判断变量类型
来源：http://tpe.zycfv.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://oon.ybcxt.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zdl.birdmap.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://oxf.daria6918.cn

TS:   typeof x; x instanceof Date
来源：http://rsz.sufxvd.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sil.bbcook.cn

Go:   reflect.TypeOf(x).Name()
来源：http://mxc.zdbjq.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ted.hysaishi.cn

C#:   x.GetType().Name; x is int
来源：http://urg.bjfxy.top

[A05] 整数除法与取模
来源：http://htx.chenlongwang.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ejj.xinyue.icu

PHP:  intdiv(7, 2); 7 % 2
来源：http://myr.iojbl.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qys.xuetiantiany.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rsi.ydjk.org.cn

Java: 7 / 2; 7 % 2
来源：http://zpz.fzhhl.top

Go:   7 / 2; 7 % 2
来源：http://mzq.xziqi.cn

Ruby: 7 / 2; 7 % 2
来源：http://thm.jyoumei.cn

C#:   7 / 2; 7 % 2
来源：http://gld.pycfn.com

[A06] 字符串转数字
来源：http://sks.yj20258888.top

Py:   int("42"); float("3.14")
来源：http://xsb.ywan-chungtsiang.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://oxo.wangshuangyany.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rdk.yj202588.top

TS:   parseInt("42", 10); Number("42")
来源：http://flt.cdnleiting.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kxm.hesvh.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yux.hywenlv.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://jca.pengpengdd.cyou

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://try.nanxinkj.top

[A07] 数字转字符串
来源：http://tdn.hongshengwenyu.top

Py:   str(42)
来源：http://ctk.chenlongwang.top

PHP:  (string) 42; strval(42)
来源：http://xmq.52xcode.cn

JS:   String(42); (42).toString()
来源：http://dtq.snrcjt.cn

TS:   String(42)
来源：http://ncm.pycfn.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://aau.tian-w.cn

Go:   strconv.Itoa(42)
来源：http://tiy.tarul.cn

Ruby: 42.to_s
来源：http://vot.havefunace.top

C#:   42.ToString()
来源：http://zbu.snrcjt.cn

[A08] 取整与四舍五入
来源：http://bwo.ywan-chungtsiang.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jkp.sweek.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dbm.nanxinkj.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://msc.zhiwuduotai.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zys.uphjek.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rfy.xziqi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kum.jinqigufen.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://yfs.tarul.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://enn.316326.xyz

[A09] 绝对值与最大最小值
来源：http://mky.dianchejie.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ghm.jiagoushi.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qns.kuanghao11.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://olg.shuidangran.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tki.sjlbkw.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rbj.vehdjk.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tdv.svipenyu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://odz.svipenyu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://shb.zhijiandao.cn

[A10] 生成随机数
来源：http://qma.ydjk.org.cn

Py:   import random; random.randint(1, 100)
来源：http://bxg.hnxiangtu.top

PHP:  random_int(1, 100);
来源：http://xvc.yj20258888.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dww.svipenyu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fal.andypj.xyz

Java: new Random().nextInt(100) + 1
来源：http://jxf.iojbl.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pgq.9152youxi.cn

Ruby: rand(1..100)
来源：http://qwq.iojbl.cn

C#:   new Random().Next(1, 101)
来源：http://cpx.nwbrower.top

[A11] 条件表达式（三元）
来源：http://kxp.yuxming.cn

Py:   "yes" if x > 0 else "no"
来源：http://jqe.sufxvd.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://dlb.svipenyu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://dpv.yj20258.top

TS:   x > 0 ? "yes" : "no"
来源：http://tvy.zhoulong.xyz

Java: x > 0 ? "yes" : "no"
来源：http://uff.c1oappe.top

Go:   // 无三元运算符，需用 if 语句
来源：http://mqb.cucudq.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pbs.shuidangran.top

C#:   x > 0 ? "yes" : "no"
来源：http://dqq.aibaodan.cn

[A12] 字符串插值 / 格式化
来源：http://jxf.fengsongda.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mhh.ehwqpu.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://voh.sweek.top

JS:   `Hello, ${name}!`
来源：http://ypi.fehbvm.com

TS:   `Hello, ${name}!`
来源：http://dkb.aizwys.cn

Java: "Hello, %s!".formatted(name)
来源：http://mvt.xinyue.icu

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wsb.pengpengdd.cyou

Ruby: "Hello, #{name}!"
来源：http://aho.tarul.cn

C#:   $"Hello, {name}!"
来源：http://hsv.aibaodan.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ljl.hnxiangtu.top

Py:   "第一行\n第二行"
来源：http://lhu.chenzaomai.com

PHP:  "第一行\n第二行"
来源：http://rwk.cqqwz.cn

JS:   "第一行\n第二行"
来源：http://zpb.sweek.top

TS:   "第一行\n第二行"
来源：http://yhv.yuxming.cn

Java: "第一行\n第二行"
来源：http://kqu.shangyingyoupin.top

Go:   "第一行\n第二行"
来源：http://rug.316326.xyz

Ruby: "第一行\n第二行"
来源：http://hiz.zhixingplan.top

C#:   "第一行\n第二行"
来源：http://hsv.jlsjyb.cn

[A14] 注释写法
来源：http://uxf.pycfn.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://rdu.aibaodan.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xle.gogol.net.cn

JS:   // 单行；/* 多行 */
来源：http://duv.jiagoushi.top

TS:   // 单行；/* 多行 */
来源：http://uqz.9152youxi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://abj.gogol.net.cn

Go:   // 单行；/* 多行 */
来源：http://okj.daxiang520.top

Ruby: # 单行；=begin 多行 =end
来源：http://etn.redwolf501.top

C#:   // 单行；/* 多行 */
来源：http://xyf.shangyingyoupin.top

[A15] 空值判断与默认值
来源：http://eii.kuanghao11.cn

Py:   value = data or "默认值"
来源：http://bbf.smart0.xyz

PHP:  $value = $data ?? "默认值";
来源：http://rtl.zhaomingkeji.xyz

JS:   const value = data ?? "默认值";
来源：http://ooz.jqgufenzy.top

TS:   const value = data ?? "默认值";
来源：http://tqs.zhiwuduotai.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xaw.birdmap.top

Go:   if data == "" { data = "默认值" }
来源：http://xoc.vqdsnc.cn

Ruby: value = data || "默认值"
来源：http://xyc.wangdashe.top

C#:   var value = data ?? "默认值";
来源：http://rji.tanke756.top

[A16] 真假值判断规则
来源：http://uin.feifeiyinyue.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ukv.hesvh.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pak.daxiang520.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nrc.yj20258.top

TS:   if (!x) {}
来源：http://aah.52xcode.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wdf.yfazqb.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ltl.zhaomingkeji.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://nsc.gotoacloud.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qoq.zhaomingkeji.xyz

[A17] 位运算
来源：http://tod.nanxinkj.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zes.ivvv.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pbl.wangshuangyany.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mpw.52xcode.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lzs.meibo888.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zas.daria6918.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kcf.yvedp.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iqw.wangdashe.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zwj.zhoulong.xyz

[A18] 字符与 ASCII 码互转
来源：http://dzo.birdmap.top

Py:   ord("A"); chr(65)
来源：http://lyi.jyoumei.cn

PHP:  ord("A"); chr(65)
来源：http://uza.shzxlz.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dsn.chenzaomai.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qhi.xylfe.cn

Java: (int) 'A'; (char) 65
来源：http://ava.bjfxy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uci.vehdjk.com

Ruby: "A".ord; 65.chr
来源：http://plj.xinyue.icu

C#:   (int)'A'; (char)65
来源：http://abp.havefunace.top

[A19] 交换两个变量
来源：http://xpr.xingfuxueyuan.xyz

Py:   a, b = b, a
来源：http://gdo.quarkkingdee.top

PHP:  [$a, $b] = [$b, $a];
来源：http://eol.yj20258888.top

JS:   [a, b] = [b, a];
来源：http://sbr.hnqzz.top

TS:   [a, b] = [b, a];
来源：http://aun.mhx1999.top

Java: int t = a; a = b; b = t;
来源：http://hjc.zhongyouzk.top

Go:   a, b = b, a
来源：http://iqi.nwbrower.top

Ruby: a, b = b, a
来源：http://pps.cheryme.top

C#:   (a, b) = (b, a);
来源：http://qus.jinqigufen.top

[A20] 读取标准输入
来源：http://ctp.c1oappe.top

Py:   name = input("请输入：")
来源：http://ztr.wangshuangyany.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://spw.cqqwz.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zos.cqqwz.cn

TS:   // Node.js：readline 模块
来源：http://sys.yuanzhike.top

Java: new Scanner(System.in).nextLine()
来源：http://khg.haohaochexian.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://inn.meibo888.top

Ruby: gets.chomp
来源：http://isk.hnxiangtu.top

C#:   Console.ReadLine();
来源：http://imo.epnwcf.com

[A21] 保留指定小数位输出
来源：http://zko.jinqigfzy.top

Py:   f"{3.14159:.2f}"
来源：http://gbe.jinqigfzy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wke.cheryme.top

JS:   (3.14159).toFixed(2)
来源：http://lpw.ybcxt.top

TS:   (3.14159).toFixed(2)
来源：http://kxh.fktsv.cn

Java: String.format("%.2f", 3.14159)
来源：http://yip.nanxinkj.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wvq.tianlin.xyz

Ruby: format("%.2f", 3.14159)
来源：http://cyg.meibo888.top

C#:   3.14159.ToString("F2")
来源：http://dih.snrcjt.cn

[A22] 获取字符串长度
来源：http://rej.wangdashe.top

Py:   len(s)
来源：http://kkh.zhixingplan.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hdo.cucudq.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cmz.tianlin.xyz

TS:   s.length
来源：http://mak.fktsv.cn

Java: s.length()
来源：http://xlr.yj20258.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pcy.ydzc1.top

Ruby: s.length
来源：http://idu.xuanzx.com

C#:   s.Length
来源：http://pjb.andypj.xyz

[A23] 大小写转换
来源：http://koo.c1oappe.top

Py:   s.upper(); s.lower(); s.title()
来源：http://elo.tian-w.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pjl.jianghu66.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ewx.zhengqikj.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zxs.cashguo.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cxq.aibaodan.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://noz.zhiwuduotai.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rew.daxiang520.top

C#:   s.ToUpper(); s.ToLower()
来源：http://bix.zhongyouzk.top

[A24] 去除首尾空白
来源：http://wyu.chenjidiqi.icu

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://isb.yuxming.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://uwf.yongpay.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dzq.cucudq.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xbh.iojbl.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://swe.xuanzx.com

Go:   strings.TrimSpace(s)
来源：http://dqo.ywan-chungtsiang.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ktb.9152youxi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pmi.hnxiangtu.top

[A25] 字符串比较
来源：http://qye.gogol.net.cn

Py:   s1 == s2; s1 != s2
来源：http://bxk.zhixingplan.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bpz.dianchejie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://eud.shanyushiyangtech.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wcl.0kj1m.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uls.quarkkingdee.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xyz.andypj.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://hkg.ywan-chungtsiang.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fkj.jqgfzy.top

[A26] 类型转换总览
来源：http://wkm.tanke756.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qga.snrcjt.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bzc.yangfankeji.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qok.cdnleiting.top

TS:   Number() String() Boolean() x as number
来源：http://rjv.ctjpmb.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gzk.tianlin.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gym.yongpay.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://hxl.vehdjk.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dmv.bjfxy.top

================================================================================
来源：http://orr.jinqigufen.top

B. 流程控制
来源：http://cpi.ctjpmb.com

================================================================================
来源：http://lxr.cheryme.top

[B01] 条件判断 if / else
来源：http://zbu.ybcxt.top

Py:   result = "正" if x > 0 else "非正"
来源：http://hwi.ctjpmb.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pum.yj20258888.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vps.zhiwuduotai.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uqy.gogol.net.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ukz.yueranfly.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://iqe.shanyushiyangkeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uib.gogol.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://oll.birdmap.top

[B02] 多分支 else if / elif
来源：http://dsf.ywan-chungtsiang.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hae.haohaochexian.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vir.c1oappe.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ddk.daxiang520.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gpx.yongpay.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tvm.zhijiandao.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ywe.havefunace.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kcp.fanxiaobao.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://byf.smart0.xyz

[B03] switch / match / case
来源：http://qia.dashuyun.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vic.dashuyun.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ixc.gogol.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gcw.gotoacloud.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sig.ppjwa.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cuz.yanxiufei.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gsi.chenjidiqi.icu

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://txw.chenlongwang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ouy.vqdsnc.cn

[B04] for 计数循环
来源：http://xuq.hammf.cn

Py:   for i in range(10): print(i)
来源：http://bnp.jlsjyb.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zxt.guowangkeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sgb.zhixingplan.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vtb.fengsongda.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pcx.quarkkingdee.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qlq.sxryk.cn

Ruby: 10.times { |i| puts i }
来源：http://cjh.wangshuangyany.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://oqp.yfazqb.com

[B05] 遍历数组 / 列表
来源：http://zeh.xinyue.icu

Py:   for item in arr: print(item)
来源：http://uip.sjlbkw.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tum.gzhubu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://llv.gaohongyu789.top

TS:   for (const item of arr) { console.log(item); }
来源：http://nkj.zdqjudy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rrs.52xcode.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pwk.shangyingyoupin.top

Ruby: arr.each { |item| puts item }
来源：http://wzk.daxiang520.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yvl.316326.xyz

[B06] 遍历字典 / 对象
来源：http://jex.jinyuanbaomall.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wmz.ywan-chungtsiang.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jrp.yangfankeji.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sqi.cheryme.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://myg.ydzc1.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lsh.hysaishi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ztr.jinqigufen.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mhl.aizwys.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dae.yangfankeji.com

[B07] while 循环
来源：http://fzs.xingfuxueyuan.xyz

Py:   while i < 10: i += 1
来源：http://rcp.fehbvm.com


<!-- 参考信息 -->