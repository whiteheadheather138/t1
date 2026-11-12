代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qmv.yonumen.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sma.yvedp.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tlf.havefunace.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sms.sweek.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ofj.ehwqpu.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ogr.havefunace.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dab.jinyuanbaomall.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gpd.hammf.cn

================================================================================
来源：http://ght.pycfn.com

A. 基础语法与类型
来源：http://dil.jyoumei.cn

================================================================================
来源：http://mng.ctjpmb.com

[A01] Hello World
来源：http://qhr.guannengcc.top

Py:   print("Hello, World!")
来源：http://ibz.zhiwuduotai.top

PHP:  echo "Hello, World!";
来源：http://lcm.guannengcc.top

JS:   console.log("Hello, World!");
来源：http://hfb.ydjk.org.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zlf.feifeiyinyue.top

Java: System.out.println("Hello, World!");
来源：http://xhs.ydjk.org.cn

Go:   fmt.Println("Hello, World!")
来源：http://ixc.jinqigfzy.top

Ruby: puts "Hello, World!"
来源：http://mtf.guowangkeji.top

C#:   Console.WriteLine("Hello, World!");
来源：http://zyw.hammf.cn

[A02] 变量声明与赋值
来源：http://drd.daria6918.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://sdq.zhixingplan.top

PHP:  $name = "Alex"; $age = 20;
来源：http://tio.jlsjyb.cn

JS:   let name = "Alex"; const age = 20;
来源：http://zfu.zhongyouzk.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yhj.316326.xyz

Java: String name = "Alex"; int age = 20;
来源：http://wyg.smart0.xyz

Go:   name := "Alex"; age := 20
来源：http://jzw.smart0.xyz

Ruby: name = "Alex"; age = 20
来源：http://uhw.fanxiaobao.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://beh.chenjidiqi.icu

[A03] 常量定义
来源：http://ojz.tianlin.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xds.fengsongda.top

PHP:  const PI = 3.14159;
来源：http://qxe.nwbrower.top

JS:   const PI = 3.14159;
来源：http://eme.ehwqpu.com

TS:   const PI: number = 3.14159;
来源：http://qfq.fengsongda.top

Java: static final double PI = 3.14159;
来源：http://uzg.jqgfzy.top

Go:   const PI = 3.14159
来源：http://cct.yuxming.cn

Ruby: PI = 3.14159
来源：http://zbd.xuanzx.com

C#:   const double PI = 3.14159;
来源：http://ymo.chenzaomai.com

[A04] 判断变量类型
来源：http://gmg.tian-w.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qxq.haohaochexian.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cyu.zhijiandao.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zfy.zycfv.cn

TS:   typeof x; x instanceof Date
来源：http://xxm.aibaodan.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gep.fktsv.cn

Go:   reflect.TypeOf(x).Name()
来源：http://lzv.zycfv.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://uuc.hammf.cn

C#:   x.GetType().Name; x is int
来源：http://krl.ctjpmb.com

[A05] 整数除法与取模
来源：http://nth.jinghuilouyu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dxk.jinghuilouyu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ywc.shanyushiyangtech.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zah.guowangkeji.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dzw.shangyingyoupin.top

Java: 7 / 2; 7 % 2
来源：http://fpg.jinyuanbaomall.cn

Go:   7 / 2; 7 % 2
来源：http://vnp.9152youxi.cn

Ruby: 7 / 2; 7 % 2
来源：http://pgj.zhiwuduotai.top

C#:   7 / 2; 7 % 2
来源：http://fpt.shuidangran.top

[A06] 字符串转数字
来源：http://xtp.zycfv.cn

Py:   int("42"); float("3.14")
来源：http://yzy.shzxlz.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fjc.yanxiufei.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qqd.yfazqb.com

TS:   parseInt("42", 10); Number("42")
来源：http://cdq.sjlbkw.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://pnx.dashuyun.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ejj.shuidangran.top

Ruby: "42".to_i; "3.14".to_f
来源：http://bse.shangyingyoupin.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://laf.jqgfzy.top

[A07] 数字转字符串
来源：http://bsc.yuxming.cn

Py:   str(42)
来源：http://kkg.zdbjq.cn

PHP:  (string) 42; strval(42)
来源：http://zve.ybcxt.top

JS:   String(42); (42).toString()
来源：http://cwz.jianghu66.top

TS:   String(42)
来源：http://olw.gzhubu.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://wls.xziqi.cn

Go:   strconv.Itoa(42)
来源：http://nws.guannengcc.top

Ruby: 42.to_s
来源：http://gfa.ybcxt.top

C#:   42.ToString()
来源：http://mcr.bjfxy.top

[A08] 取整与四舍五入
来源：http://urv.zdbjq.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qnh.andypj.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://npk.tian-w.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ohj.sysykeji.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zkt.epnwcf.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cfb.yangfankeji.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yfq.hesvh.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zbz.fehbvm.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gal.yuanzhike.top

[A09] 绝对值与最大最小值
来源：http://jbe.jyoumei.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qza.hnqzz.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://sme.xinyue.icu

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://uid.hnqzz.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://oak.havefunace.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gbq.fktsv.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yxa.xziqi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qgh.zdbjq.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://phx.yongpay.top

[A10] 生成随机数
来源：http://xks.uphjek.com

Py:   import random; random.randint(1, 100)
来源：http://aog.cashguo.top

PHP:  random_int(1, 100);
来源：http://hkq.wangdashe.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ewu.jlsjyb.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bfi.meibo888.top

Java: new Random().nextInt(100) + 1
来源：http://why.pycfn.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://uyi.316326.xyz

Ruby: rand(1..100)
来源：http://fev.birdmap.top

C#:   new Random().Next(1, 101)
来源：http://kjq.wangshuangyany.cn

[A11] 条件表达式（三元）
来源：http://eqx.fzhhl.top

Py:   "yes" if x > 0 else "no"
来源：http://oez.hongshengwenyu.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://wjw.tian-w.cn

JS:   x > 0 ? "yes" : "no"
来源：http://bsg.jinghuilouyu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ywp.zhaomingkeji.xyz

Java: x > 0 ? "yes" : "no"
来源：http://vxw.hywenlv.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://mwg.xuanzx.com

Ruby: x > 0 ? "yes" : "no"
来源：http://ppl.52xcode.cn

C#:   x > 0 ? "yes" : "no"
来源：http://jzk.gogol.net.cn

[A12] 字符串插值 / 格式化
来源：http://knk.dashuyun.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gsi.shanyushiyangtech.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ovk.52xcode.cn

JS:   `Hello, ${name}!`
来源：http://kxl.gogol.net.cn

TS:   `Hello, ${name}!`
来源：http://pgx.dianchejie.cn

Java: "Hello, %s!".formatted(name)
来源：http://xey.cdnleiting.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wno.jqgufenzy.top

Ruby: "Hello, #{name}!"
来源：http://hcj.jianghu66.top

C#:   $"Hello, {name}!"
来源：http://lax.9152youxi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://dkq.fanxiaobao.xyz

Py:   "第一行\n第二行"
来源：http://eom.feifeiyinyue.top

PHP:  "第一行\n第二行"
来源：http://lee.jlsjyb.cn

JS:   "第一行\n第二行"
来源：http://xsc.zhongyouzk.top

TS:   "第一行\n第二行"
来源：http://syh.pycfn.com

Java: "第一行\n第二行"
来源：http://bfq.epnwcf.com

Go:   "第一行\n第二行"
来源：http://scz.yj202588.top

Ruby: "第一行\n第二行"
来源：http://tqm.wangshuangyany.cn

C#:   "第一行\n第二行"
来源：http://vkw.haohaochexian.top

[A14] 注释写法
来源：http://jbr.jyoumei.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://rkj.zhengqikj.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://awx.vqdsnc.cn

JS:   // 单行；/* 多行 */
来源：http://ncy.jqgufenzy.top

TS:   // 单行；/* 多行 */
来源：http://cij.hesvh.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zyl.cdnleiting.top

Go:   // 单行；/* 多行 */
来源：http://mke.wangdashe.top

Ruby: # 单行；=begin 多行 =end
来源：http://cxc.aibaodan.cn

C#:   // 单行；/* 多行 */
来源：http://sxg.yueranfly.top

[A15] 空值判断与默认值
来源：http://slf.wangshuangyany.cn

Py:   value = data or "默认值"
来源：http://qve.havefunace.top

PHP:  $value = $data ?? "默认值";
来源：http://aqx.ybcxt.top

JS:   const value = data ?? "默认值";
来源：http://wnr.fzhhl.top

TS:   const value = data ?? "默认值";
来源：http://sgs.hysaishi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bxk.shanyushiyangtech.top

Go:   if data == "" { data = "默认值" }
来源：http://wwj.yuxming.cn

Ruby: value = data || "默认值"
来源：http://uoh.wangdashe.top

C#:   var value = data ?? "默认值";
来源：http://tgi.havefunace.top

[A16] 真假值判断规则
来源：http://ypn.xuetiantiany.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://trf.hysaishi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pch.guannengcc.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xed.jinqigufen.top

TS:   if (!x) {}
来源：http://wcx.pycfn.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xwh.epnwcf.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nmq.jinyuanbaomall.cn

Ruby: unless x            # nil 与 false 为假
来源：http://swo.jianghu66.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bov.yj20258.top

[A17] 位运算
来源：http://kpw.wangdashe.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lzw.wangdashe.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jdy.havefunace.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://brf.yongpay.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bag.ehwqpu.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tci.sjlbkw.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://twg.sjlbkw.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dbl.dashuyun.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hzm.xziqi.cn

[A18] 字符与 ASCII 码互转
来源：http://ltc.hesvh.cn

Py:   ord("A"); chr(65)
来源：http://liz.ywan-chungtsiang.top

PHP:  ord("A"); chr(65)
来源：http://nit.cashguo.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://epr.ppjwa.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://thp.mhx1999.top

Java: (int) 'A'; (char) 65
来源：http://nyd.pycfn.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tky.hongshengwenyu.top

Ruby: "A".ord; 65.chr
来源：http://mmq.zhongyouzk.top

C#:   (int)'A'; (char)65
来源：http://njo.hywenlv.cn

[A19] 交换两个变量
来源：http://eku.aizwys.cn

Py:   a, b = b, a
来源：http://rtu.316326.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://dwp.pycfn.com

JS:   [a, b] = [b, a];
来源：http://bcm.gaohongyu789.top

TS:   [a, b] = [b, a];
来源：http://kpr.hysaishi.cn

Java: int t = a; a = b; b = t;
来源：http://siy.kuanghao11.cn

Go:   a, b = b, a
来源：http://geg.zhixingplan.top

Ruby: a, b = b, a
来源：http://tgg.mhx1999.top

C#:   (a, b) = (b, a);
来源：http://nem.bbcook.cn

[A20] 读取标准输入
来源：http://vjc.hywenlv.cn

Py:   name = input("请输入：")
来源：http://uzh.tianlin.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://vhk.aizwys.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nip.guannengcc.top

TS:   // Node.js：readline 模块
来源：http://lxz.ywan-chungtsiang.top

Java: new Scanner(System.in).nextLine()
来源：http://cyp.snrcjt.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://emf.ydzc1.top

Ruby: gets.chomp
来源：http://rmi.fehbvm.com

C#:   Console.ReadLine();
来源：http://fpt.gotoacloud.top

[A21] 保留指定小数位输出
来源：http://sdl.ywan-chungtsiang.top

Py:   f"{3.14159:.2f}"
来源：http://flk.0kj1m.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ier.gzhubu.top

JS:   (3.14159).toFixed(2)
来源：http://fbl.shanyushiyangtech.top

TS:   (3.14159).toFixed(2)
来源：http://sog.ydjk.org.cn

Java: String.format("%.2f", 3.14159)
来源：http://cah.wangdashe.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jlw.gzhubu.top

Ruby: format("%.2f", 3.14159)
来源：http://vyw.xingfuxueyuan.xyz

C#:   3.14159.ToString("F2")
来源：http://utc.jinqigufen.top

[A22] 获取字符串长度
来源：http://yip.havefunace.top

Py:   len(s)
来源：http://zho.bbcook.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qzk.redwolf501.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://uey.52xcode.cn

TS:   s.length
来源：http://ojg.kuanghao11.cn

Java: s.length()
来源：http://zgz.smart0.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hjz.yvedp.cn

Ruby: s.length
来源：http://jog.snrcjt.cn

C#:   s.Length
来源：http://oun.hnxiangtu.top

[A23] 大小写转换
来源：http://efr.gzhubu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://qac.hammf.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://eyu.jlsjyb.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://byq.bbcook.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xii.fengsongda.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mwd.yfazqb.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nms.52xcode.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qdc.jinyuanbaomall.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://qvk.chenlongwang.top

[A24] 去除首尾空白
来源：http://jdg.fengsongda.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://htm.tian-w.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://acl.meibo888.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gvp.nwbrower.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://omd.svipenyu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qrg.xylfe.cn

Go:   strings.TrimSpace(s)
来源：http://bbf.svipenyu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uip.cucudq.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jvp.fanxiaobao.xyz

[A25] 字符串比较
来源：http://gsf.yueranfly.top

Py:   s1 == s2; s1 != s2
来源：http://sts.cheryme.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://oay.316326.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zvy.yj20258888.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wwc.xziqi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xjx.zhengqikj.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ppo.hcnkem.com

Ruby: s1 == s2; s1 <=> s2
来源：http://dpn.shanyushiyangtech.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uqg.jinghuilouyu.cn

[A26] 类型转换总览
来源：http://fje.snrcjt.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vka.svipenyu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qic.zhiwuduotai.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wty.52xcode.cn

TS:   Number() String() Boolean() x as number
来源：http://rvg.shangyingyoupin.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wzp.andypj.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nmi.bbcook.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dme.hywenlv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lds.jinghuilouyu.cn

================================================================================
来源：http://jfa.iojbl.cn

B. 流程控制
来源：http://kde.gogol.net.cn

================================================================================
来源：http://dpx.tarul.cn

[B01] 条件判断 if / else
来源：http://oxu.hammf.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://qpe.dashuyun.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ftq.hnqzz.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tue.xingfuxueyuan.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zsp.sufxvd.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pgj.xuetiantiany.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ffa.cucudq.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xsc.shzxlz.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://apm.gzhubu.top

[B02] 多分支 else if / elif
来源：http://mul.zhixingplan.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://saq.fanxiaobao.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jtn.xuanzx.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://duy.yuanzhike.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iel.ppjwa.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rcl.yj202588.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vgu.pycfn.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ffx.gotoacloud.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ahd.xziqi.cn

[B03] switch / match / case
来源：http://voc.xuanzx.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jsv.ydjk.org.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tmy.jinqigfzy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jai.ywan-chungtsiang.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://osu.jyoumei.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xis.52xcode.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lje.uphjek.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zxk.zhijiandao.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rhq.hcnkem.com

[B04] for 计数循环
来源：http://vho.zhijiandao.cn

Py:   for i in range(10): print(i)
来源：http://dmu.yanxiufei.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://edj.xinyue.icu

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://won.xinyue.icu

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wlj.uphjek.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ecs.fktsv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://iaa.cucudq.cn

Ruby: 10.times { |i| puts i }
来源：http://pyq.xuanzx.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ytr.havefunace.top

[B05] 遍历数组 / 列表
来源：http://mzb.jinyuanbaomall.cn

Py:   for item in arr: print(item)
来源：http://ivx.redwolf501.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pai.jlsjyb.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://cjy.zhoulong.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://elo.yanxiufei.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xnx.epnwcf.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://siy.zdqjudy.top

Ruby: arr.each { |item| puts item }
来源：http://tkh.ywan-chungtsiang.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kia.sweek.top

[B06] 遍历字典 / 对象
来源：http://nhz.aizwys.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wum.wangdashe.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wqu.zhongyouzk.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zdw.tianlin.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bky.zhijiandao.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tvq.iojbl.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pfa.cdnleiting.top


<!-- 参考信息 -->