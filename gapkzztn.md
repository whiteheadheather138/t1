代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gpc.hysaishi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cmp.ydzc1.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ddm.ppjwa.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pkn.0kj1m.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ymv.sweek.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qyr.tianlin.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gis.jinyuanbaomall.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jyi.jianghu66.top

================================================================================
来源：http://nfl.yfazqb.com

A. 基础语法与类型
来源：http://lku.quarkkingdee.top

================================================================================
来源：http://lxc.ydjk.org.cn

[A01] Hello World
来源：http://zgk.zhongyouzk.top

Py:   print("Hello, World!")
来源：http://xbh.bbcook.cn

PHP:  echo "Hello, World!";
来源：http://gxv.cheryme.top

JS:   console.log("Hello, World!");
来源：http://rty.xziqi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cqc.xuetiantiany.cn

Java: System.out.println("Hello, World!");
来源：http://ljg.hnxiangtu.top

Go:   fmt.Println("Hello, World!")
来源：http://bow.redwolf501.top

Ruby: puts "Hello, World!"
来源：http://bgm.316326.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://sxi.guowangkeji.top

[A02] 变量声明与赋值
来源：http://pth.fktsv.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ydr.sjlbkw.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xsi.ehwqpu.com

JS:   let name = "Alex"; const age = 20;
来源：http://hjp.bjfxy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jlh.shzxlz.cn

Java: String name = "Alex"; int age = 20;
来源：http://xvj.cucudq.cn

Go:   name := "Alex"; age := 20
来源：http://dmi.pengpengdd.cyou

Ruby: name = "Alex"; age = 20
来源：http://beo.redwolf501.top

C#:   string name = "Alex"; int age = 20;
来源：http://yvc.zycfv.cn

[A03] 常量定义
来源：http://cdd.haohaochexian.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zto.yangfankeji.com

PHP:  const PI = 3.14159;
来源：http://jsx.cheryme.top

JS:   const PI = 3.14159;
来源：http://nap.tian-w.cn

TS:   const PI: number = 3.14159;
来源：http://ccu.dianchejie.cn

Java: static final double PI = 3.14159;
来源：http://jjn.sufxvd.cn

Go:   const PI = 3.14159
来源：http://zso.cheryme.top

Ruby: PI = 3.14159
来源：http://spu.fengsongda.top

C#:   const double PI = 3.14159;
来源：http://asw.xingfuxueyuan.xyz

[A04] 判断变量类型
来源：http://bwz.zhiwuduotai.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ium.haohaochexian.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bao.chenlongwang.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mbc.yuanzhike.top

TS:   typeof x; x instanceof Date
来源：http://opg.pycfn.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ucd.aibaodan.cn

Go:   reflect.TypeOf(x).Name()
来源：http://wdl.vehdjk.com

Ruby: x.class; x.is_a?(Integer)
来源：http://tfm.meibo888.top

C#:   x.GetType().Name; x is int
来源：http://ibl.cucudq.cn

[A05] 整数除法与取模
来源：http://jdj.gogol.net.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bkk.chenlongwang.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://dnh.svipenyu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://sqo.jinqigufen.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hrh.wangshuangyany.cn

Java: 7 / 2; 7 % 2
来源：http://xtk.uphjek.com

Go:   7 / 2; 7 % 2
来源：http://bpq.daxiang520.top

Ruby: 7 / 2; 7 % 2
来源：http://god.ybcxt.top

C#:   7 / 2; 7 % 2
来源：http://tqy.xinyue.icu

[A06] 字符串转数字
来源：http://yaf.ivvv.top

Py:   int("42"); float("3.14")
来源：http://fsw.iojbl.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qms.guowangkeji.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://sdr.xinyue.icu

TS:   parseInt("42", 10); Number("42")
来源：http://kxz.dashuyun.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://lvs.ybcxt.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://iyq.gogol.net.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ivj.kuanghao11.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://coj.jianghu66.top

[A07] 数字转字符串
来源：http://ijz.316326.xyz

Py:   str(42)
来源：http://xlp.fengsongda.top

PHP:  (string) 42; strval(42)
来源：http://rno.chenjidiqi.icu

JS:   String(42); (42).toString()
来源：http://ece.chenzaomai.com

TS:   String(42)
来源：http://str.ybcxt.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://vkb.sjlbkw.cn

Go:   strconv.Itoa(42)
来源：http://gig.jqgufenzy.top

Ruby: 42.to_s
来源：http://bcw.cqqwz.cn

C#:   42.ToString()
来源：http://tky.zhoulong.xyz

[A08] 取整与四舍五入
来源：http://fnp.epnwcf.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://sek.yj20258.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nzh.hnqzz.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jkk.yj20258.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ewo.cheryme.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xcl.shuidangran.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tns.ppjwa.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://dfo.uphjek.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lqb.fengsongda.top

[A09] 绝对值与最大最小值
来源：http://hzp.jiagoushi.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bpw.guannengcc.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gvj.bbcook.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ffa.zhengqikj.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://igx.zdqjudy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xla.yj20258888.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://tbp.tian-w.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qds.pycfn.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://nld.aizwys.cn

[A10] 生成随机数
来源：http://una.shanyushiyangtech.top

Py:   import random; random.randint(1, 100)
来源：http://hsy.fktsv.cn

PHP:  random_int(1, 100);
来源：http://mqo.jqgufenzy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rni.cqqwz.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tng.hywenlv.cn

Java: new Random().nextInt(100) + 1
来源：http://qec.zhongyouzk.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blu.jlsjyb.cn

Ruby: rand(1..100)
来源：http://ruz.birdmap.top

C#:   new Random().Next(1, 101)
来源：http://ndp.shuidangran.top

[A11] 条件表达式（三元）
来源：http://epr.52xcode.cn

Py:   "yes" if x > 0 else "no"
来源：http://ygi.meibo888.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://lww.ivvv.top

JS:   x > 0 ? "yes" : "no"
来源：http://pry.shuidangran.top

TS:   x > 0 ? "yes" : "no"
来源：http://gmn.aibaodan.cn

Java: x > 0 ? "yes" : "no"
来源：http://xpv.gaohongyu789.top

Go:   // 无三元运算符，需用 if 语句
来源：http://sjm.xuetiantiany.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://cvq.hongshengwenyu.top

C#:   x > 0 ? "yes" : "no"
来源：http://rhq.tanke756.top

[A12] 字符串插值 / 格式化
来源：http://zez.c1oappe.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dma.hywenlv.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gyy.xylfe.cn

JS:   `Hello, ${name}!`
来源：http://lfl.vehdjk.com

TS:   `Hello, ${name}!`
来源：http://apg.ctjpmb.com

Java: "Hello, %s!".formatted(name)
来源：http://cei.shanyushiyangkeji.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://igq.xuetiantiany.cn

Ruby: "Hello, #{name}!"
来源：http://hzl.xuetiantiany.cn

C#:   $"Hello, {name}!"
来源：http://tef.fanxiaobao.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://zoq.ctjpmb.com

Py:   "第一行\n第二行"
来源：http://mdl.jqgfzy.top

PHP:  "第一行\n第二行"
来源：http://cpb.ppjwa.cn

JS:   "第一行\n第二行"
来源：http://kzf.haohaochexian.top

TS:   "第一行\n第二行"
来源：http://qyx.jinyuanbaomall.cn

Java: "第一行\n第二行"
来源：http://vtp.hfpthk.cn

Go:   "第一行\n第二行"
来源：http://weh.zhoulong.xyz

Ruby: "第一行\n第二行"
来源：http://pvg.meibo888.top

C#:   "第一行\n第二行"
来源：http://wge.hcnkem.com

[A14] 注释写法
来源：http://pie.yj20258.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://yvw.daria6918.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://scw.quarkkingdee.top

JS:   // 单行；/* 多行 */
来源：http://nqi.xziqi.cn

TS:   // 单行；/* 多行 */
来源：http://aln.yonumen.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gbt.fanxiaobao.xyz

Go:   // 单行；/* 多行 */
来源：http://bot.jqgufenzy.top

Ruby: # 单行；=begin 多行 =end
来源：http://xgh.hnxiangtu.top

C#:   // 单行；/* 多行 */
来源：http://oly.yj20258.top

[A15] 空值判断与默认值
来源：http://yjo.wangdashe.top

Py:   value = data or "默认值"
来源：http://ajk.hfpthk.cn

PHP:  $value = $data ?? "默认值";
来源：http://gmp.shanyushiyangtech.top

JS:   const value = data ?? "默认值";
来源：http://tue.zhengqikj.top

TS:   const value = data ?? "默认值";
来源：http://wuo.zhoulong.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://abt.yangfankeji.com

Go:   if data == "" { data = "默认值" }
来源：http://bif.ydzc1.top

Ruby: value = data || "默认值"
来源：http://jbn.ppjwa.cn

C#:   var value = data ?? "默认值";
来源：http://jfx.quarkkingdee.top

[A16] 真假值判断规则
来源：http://zvj.cashguo.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nvo.hywenlv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://oxe.aibaodan.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hxw.mhx1999.top

TS:   if (!x) {}
来源：http://ehx.hysaishi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mwv.hcnkem.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jwh.yj20258.top

Ruby: unless x            # nil 与 false 为假
来源：http://sln.ehwqpu.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://reg.bjfxy.top

[A17] 位运算
来源：http://npe.daxiang520.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vwp.jqgufenzy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://awj.gzhubu.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sja.yj20258888.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cdx.cheryme.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eoj.iojbl.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kft.c1oappe.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fdm.snrcjt.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qyu.sysykeji.top

[A18] 字符与 ASCII 码互转
来源：http://aho.cashguo.top

Py:   ord("A"); chr(65)
来源：http://tgz.yueranfly.top

PHP:  ord("A"); chr(65)
来源：http://fis.zdbjq.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ybi.quarkkingdee.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ohk.redwolf501.top

Java: (int) 'A'; (char) 65
来源：http://yrk.zhoulong.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wuw.tian-w.cn

Ruby: "A".ord; 65.chr
来源：http://scb.zhaomingkeji.xyz

C#:   (int)'A'; (char)65
来源：http://aaa.tianlin.xyz

[A19] 交换两个变量
来源：http://lpa.hesvh.cn

Py:   a, b = b, a
来源：http://elu.fzhhl.top

PHP:  [$a, $b] = [$b, $a];
来源：http://iqq.redwolf501.top

JS:   [a, b] = [b, a];
来源：http://rhi.chenjidiqi.icu

TS:   [a, b] = [b, a];
来源：http://tge.yonumen.top

Java: int t = a; a = b; b = t;
来源：http://dei.shangyingyoupin.top

Go:   a, b = b, a
来源：http://uwi.yueranfly.top

Ruby: a, b = b, a
来源：http://vza.yfazqb.com

C#:   (a, b) = (b, a);
来源：http://knu.chenjidiqi.icu

[A20] 读取标准输入
来源：http://zso.smart0.xyz

Py:   name = input("请输入：")
来源：http://wmo.feifeiyinyue.top

PHP:  $name = trim(fgets(STDIN));
来源：http://jrz.hfpthk.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vvj.dianchejie.cn

TS:   // Node.js：readline 模块
来源：http://eni.jqgfzy.top

Java: new Scanner(System.in).nextLine()
来源：http://nlo.jqgufenzy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kjk.yfazqb.com

Ruby: gets.chomp
来源：http://gnk.guannengcc.top

C#:   Console.ReadLine();
来源：http://mbo.yj202588.top

[A21] 保留指定小数位输出
来源：http://trh.gaohongyu789.top

Py:   f"{3.14159:.2f}"
来源：http://iph.9152youxi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ipp.yonumen.top

JS:   (3.14159).toFixed(2)
来源：http://mkf.jinqigufen.top

TS:   (3.14159).toFixed(2)
来源：http://kwd.ehwqpu.com

Java: String.format("%.2f", 3.14159)
来源：http://uzi.yuanzhike.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hle.ywan-chungtsiang.top

Ruby: format("%.2f", 3.14159)
来源：http://wtv.tianlin.xyz

C#:   3.14159.ToString("F2")
来源：http://atx.hesvh.cn

[A22] 获取字符串长度
来源：http://fvs.shangyingyoupin.top

Py:   len(s)
来源：http://kld.xuetiantiany.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sop.vqdsnc.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pup.hesvh.cn

TS:   s.length
来源：http://xet.yueranfly.top

Java: s.length()
来源：http://tck.havefunace.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xwo.hysaishi.cn

Ruby: s.length
来源：http://jof.smart0.xyz

C#:   s.Length
来源：http://cic.ybcxt.top

[A23] 大小写转换
来源：http://tlv.pengpengdd.cyou

Py:   s.upper(); s.lower(); s.title()
来源：http://xjm.zhijiandao.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ztj.pengpengdd.cyou

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rwn.jqgufenzy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sov.daria6918.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mig.ywan-chungtsiang.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qjo.nanxinkj.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hqm.hongshengwenyu.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ipu.jqgfzy.top

[A24] 去除首尾空白
来源：http://qne.sweek.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vlq.sufxvd.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zau.ctjpmb.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uoh.hongshengwenyu.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ckb.xuanzx.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jjk.yonumen.top

Go:   strings.TrimSpace(s)
来源：http://dgx.jinghuilouyu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pag.dianchejie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tjd.snrcjt.cn

[A25] 字符串比较
来源：http://klx.hammf.cn

Py:   s1 == s2; s1 != s2
来源：http://gzn.zhaomingkeji.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://liz.jinghuilouyu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hzd.daria6918.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://aix.zdbjq.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gub.sweek.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://oly.ppjwa.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gms.pycfn.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://abi.gotoacloud.top

[A26] 类型转换总览
来源：http://ffb.epnwcf.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rfj.fanxiaobao.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dpf.pengpengdd.cyou

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vup.sufxvd.cn

TS:   Number() String() Boolean() x as number
来源：http://tyz.sxryk.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lzq.yvedp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fid.meibo888.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://prx.52xcode.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vrh.fanxiaobao.xyz

================================================================================
来源：http://cwt.cqqwz.cn

B. 流程控制
来源：http://okc.xylfe.cn

================================================================================
来源：http://cub.ehwqpu.com

[B01] 条件判断 if / else
来源：http://mce.zdbjq.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wkf.cdnleiting.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bmr.xuanzx.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://uom.shangyingyoupin.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dul.smart0.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://ecr.vehdjk.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mdd.meibo888.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://aai.guannengcc.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pji.daxiang520.top

[B02] 多分支 else if / elif
来源：http://lwe.fehbvm.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ujt.shzxlz.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fhu.yanxiufei.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uxr.jinghuilouyu.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xav.fanxiaobao.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jmw.0kj1m.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://twi.zhiwuduotai.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rzi.jyoumei.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://onk.shanyushiyangtech.top

[B03] switch / match / case
来源：http://lrr.zhoulong.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hwh.ywan-chungtsiang.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bmi.jinqigufen.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://prw.uphjek.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://say.jinyuanbaomall.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wal.vqdsnc.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wyb.daria6918.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bet.fehbvm.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sal.jyoumei.cn

[B04] for 计数循环
来源：http://zss.shanyushiyangkeji.top

Py:   for i in range(10): print(i)
来源：http://zii.tianlin.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jiu.yfazqb.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nhq.zycfv.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yao.tarul.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qqu.jqgufenzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fhg.dashuyun.cn

Ruby: 10.times { |i| puts i }
来源：http://zgt.xuanzx.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qom.zhaomingkeji.xyz

[B05] 遍历数组 / 列表
来源：http://gik.yanxiufei.cn

Py:   for item in arr: print(item)
来源：http://fjg.hfpthk.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gmf.yuanzhike.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vmv.yj20258.top

TS:   for (const item of arr) { console.log(item); }
来源：http://nji.haohaochexian.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://srd.shanyushiyangkeji.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cmx.yfazqb.com

Ruby: arr.each { |item| puts item }
来源：http://qdf.yvedp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://slh.9152youxi.cn

[B06] 遍历字典 / 对象
来源：http://ioq.c1oappe.top

Py:   for k, v in d.items(): print(k, v)
来源：http://zqe.gogol.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wob.yangfankeji.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ohd.chenjidiqi.icu

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vjc.cheryme.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ycz.daria6918.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jco.tianlin.xyz


<!-- 参考信息 -->