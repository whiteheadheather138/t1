代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tbn.fengsongda.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sjh.wangshuangyany.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wsx.zhaomingkeji.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cyv.tian-w.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://lyq.uphjek.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xyf.pycfn.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://syq.jinyuanbaomall.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qvk.jyoumei.cn

================================================================================
来源：http://wcf.chenzaomai.com

A. 基础语法与类型
来源：http://nkw.fengsongda.top

================================================================================
来源：http://hbh.ehwqpu.com

[A01] Hello World
来源：http://owk.zdqjudy.top

Py:   print("Hello, World!")
来源：http://uox.cqqwz.cn

PHP:  echo "Hello, World!";
来源：http://wqj.zhoulong.xyz

JS:   console.log("Hello, World!");
来源：http://knz.xinyue.icu

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://csi.xingfuxueyuan.xyz

Java: System.out.println("Hello, World!");
来源：http://hke.tianlin.xyz

Go:   fmt.Println("Hello, World!")
来源：http://pnt.smart0.xyz

Ruby: puts "Hello, World!"
来源：http://uab.hcnkem.com

C#:   Console.WriteLine("Hello, World!");
来源：http://usl.xuanzx.com

[A02] 变量声明与赋值
来源：http://wob.havefunace.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vfo.cdnleiting.top

PHP:  $name = "Alex"; $age = 20;
来源：http://uur.yfazqb.com

JS:   let name = "Alex"; const age = 20;
来源：http://dsa.316326.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hdz.epnwcf.com

Java: String name = "Alex"; int age = 20;
来源：http://jty.feifeiyinyue.top

Go:   name := "Alex"; age := 20
来源：http://emd.yj202588.top

Ruby: name = "Alex"; age = 20
来源：http://wfn.tianlin.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://tzg.jinghuilouyu.cn

[A03] 常量定义
来源：http://cwn.zdqjudy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gki.quarkkingdee.top

PHP:  const PI = 3.14159;
来源：http://rem.daxiang520.top

JS:   const PI = 3.14159;
来源：http://emb.tianlin.xyz

TS:   const PI: number = 3.14159;
来源：http://zbv.cashguo.top

Java: static final double PI = 3.14159;
来源：http://gpc.birdmap.top

Go:   const PI = 3.14159
来源：http://miq.yfazqb.com

Ruby: PI = 3.14159
来源：http://thi.hnxiangtu.top

C#:   const double PI = 3.14159;
来源：http://fel.haohaochexian.top

[A04] 判断变量类型
来源：http://mbk.nanxinkj.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://qbh.shzxlz.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ait.pycfn.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://etp.kuanghao11.cn

TS:   typeof x; x instanceof Date
来源：http://hfb.ydjk.org.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dty.yvedp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ggk.haohaochexian.top

Ruby: x.class; x.is_a?(Integer)
来源：http://fdp.sjlbkw.cn

C#:   x.GetType().Name; x is int
来源：http://aas.tian-w.cn

[A05] 整数除法与取模
来源：http://rij.hysaishi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yfy.xylfe.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://wfh.cashguo.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qgt.shuidangran.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vdt.hnxiangtu.top

Java: 7 / 2; 7 % 2
来源：http://kcr.redwolf501.top

Go:   7 / 2; 7 % 2
来源：http://yre.jinghuilouyu.cn

Ruby: 7 / 2; 7 % 2
来源：http://jwp.zhiwuduotai.top

C#:   7 / 2; 7 % 2
来源：http://hpy.cqqwz.cn

[A06] 字符串转数字
来源：http://hus.hnqzz.top

Py:   int("42"); float("3.14")
来源：http://dwv.chenlongwang.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://csl.hammf.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://khx.yanxiufei.cn

TS:   parseInt("42", 10); Number("42")
来源：http://mex.sysykeji.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://oet.nanxinkj.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://oes.jinqigfzy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://slm.tian-w.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mub.tanke756.top

[A07] 数字转字符串
来源：http://nzx.jqgfzy.top

Py:   str(42)
来源：http://yub.zhengqikj.top

PHP:  (string) 42; strval(42)
来源：http://hwr.jlsjyb.cn

JS:   String(42); (42).toString()
来源：http://rij.52xcode.cn

TS:   String(42)
来源：http://kvj.aizwys.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://kyz.cucudq.cn

Go:   strconv.Itoa(42)
来源：http://owv.zhongyouzk.top

Ruby: 42.to_s
来源：http://hlg.gaohongyu789.top

C#:   42.ToString()
来源：http://elx.epnwcf.com

[A08] 取整与四舍五入
来源：http://glg.guannengcc.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vjo.ywan-chungtsiang.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xhd.316326.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ztp.jiagoushi.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://axl.snrcjt.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kvb.0kj1m.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tmw.yangfankeji.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://dsf.cucudq.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jpi.quarkkingdee.top

[A09] 绝对值与最大最小值
来源：http://hvu.zhongyouzk.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fii.kuanghao11.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nxl.quarkkingdee.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xdi.yj20258888.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ahw.jianghu66.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://uff.quarkkingdee.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mge.fengsongda.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rtw.chenlongwang.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mon.jqgfzy.top

[A10] 生成随机数
来源：http://mgc.tian-w.cn

Py:   import random; random.randint(1, 100)
来源：http://xld.tian-w.cn

PHP:  random_int(1, 100);
来源：http://mki.redwolf501.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rrm.gotoacloud.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tfr.xingfuxueyuan.xyz

Java: new Random().nextInt(100) + 1
来源：http://lnr.jqgfzy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rua.zhijiandao.cn

Ruby: rand(1..100)
来源：http://ugg.ivvv.top

C#:   new Random().Next(1, 101)
来源：http://jch.cqqwz.cn

[A11] 条件表达式（三元）
来源：http://zlo.hnxiangtu.top

Py:   "yes" if x > 0 else "no"
来源：http://mbd.dashuyun.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://lxw.hysaishi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://nnv.zhiwuduotai.top

TS:   x > 0 ? "yes" : "no"
来源：http://tth.52xcode.cn

Java: x > 0 ? "yes" : "no"
来源：http://din.ybcxt.top

Go:   // 无三元运算符，需用 if 语句
来源：http://bdj.daxiang520.top

Ruby: x > 0 ? "yes" : "no"
来源：http://hyd.jiagoushi.top

C#:   x > 0 ? "yes" : "no"
来源：http://mpi.vqdsnc.cn

[A12] 字符串插值 / 格式化
来源：http://rxf.fktsv.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dcl.bjfxy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sqq.epnwcf.com

JS:   `Hello, ${name}!`
来源：http://wjm.yongpay.top

TS:   `Hello, ${name}!`
来源：http://knf.gotoacloud.top

Java: "Hello, %s!".formatted(name)
来源：http://nbi.xziqi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ktn.sxryk.cn

Ruby: "Hello, #{name}!"
来源：http://axq.hysaishi.cn

C#:   $"Hello, {name}!"
来源：http://ram.nanxinkj.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ong.cdnleiting.top

Py:   "第一行\n第二行"
来源：http://jqo.fzhhl.top

PHP:  "第一行\n第二行"
来源：http://lww.mhx1999.top

JS:   "第一行\n第二行"
来源：http://bnz.fzhhl.top

TS:   "第一行\n第二行"
来源：http://gnp.zhengqikj.top

Java: "第一行\n第二行"
来源：http://hiy.havefunace.top

Go:   "第一行\n第二行"
来源：http://nzs.jinqigfzy.top

Ruby: "第一行\n第二行"
来源：http://aed.jqgfzy.top

C#:   "第一行\n第二行"
来源：http://hnj.ppjwa.cn

[A14] 注释写法
来源：http://ciw.ppjwa.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://hke.xingfuxueyuan.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://mct.ywan-chungtsiang.top

JS:   // 单行；/* 多行 */
来源：http://jwj.jinqigfzy.top

TS:   // 单行；/* 多行 */
来源：http://kap.yuanzhike.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://han.ehwqpu.com

Go:   // 单行；/* 多行 */
来源：http://pyw.316326.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://lbe.ybcxt.top

C#:   // 单行；/* 多行 */
来源：http://ryl.yj20258.top

[A15] 空值判断与默认值
来源：http://clp.ppjwa.cn

Py:   value = data or "默认值"
来源：http://knj.meibo888.top

PHP:  $value = $data ?? "默认值";
来源：http://mwt.jqgufenzy.top

JS:   const value = data ?? "默认值";
来源：http://awk.svipenyu.cn

TS:   const value = data ?? "默认值";
来源：http://rpa.tanke756.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://lmh.meibo888.top

Go:   if data == "" { data = "默认值" }
来源：http://rwh.cucudq.cn

Ruby: value = data || "默认值"
来源：http://gsk.jiagoushi.top

C#:   var value = data ?? "默认值";
来源：http://sos.ctjpmb.com

[A16] 真假值判断规则
来源：http://eqi.hammf.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pnm.yueranfly.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wjp.xuanzx.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qbi.c1oappe.top

TS:   if (!x) {}
来源：http://wic.xinyue.icu

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ser.fktsv.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lwu.xingfuxueyuan.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://jcj.tianlin.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://okp.iojbl.cn

[A17] 位运算
来源：http://wjc.52xcode.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pau.hongshengwenyu.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hsl.dianchejie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dey.zhaomingkeji.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uwq.pengpengdd.cyou

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pxt.gzhubu.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kjs.birdmap.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rtj.hesvh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fts.hnxiangtu.top

[A18] 字符与 ASCII 码互转
来源：http://wzd.zhoulong.xyz

Py:   ord("A"); chr(65)
来源：http://rae.jyoumei.cn

PHP:  ord("A"); chr(65)
来源：http://nbl.tarul.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://npc.ehwqpu.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://glt.nanxinkj.top

Java: (int) 'A'; (char) 65
来源：http://iki.wangdashe.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://sgq.xuanzx.com

Ruby: "A".ord; 65.chr
来源：http://ake.52xcode.cn

C#:   (int)'A'; (char)65
来源：http://ubn.daria6918.cn

[A19] 交换两个变量
来源：http://lir.pengpengdd.cyou

Py:   a, b = b, a
来源：http://met.ydzc1.top

PHP:  [$a, $b] = [$b, $a];
来源：http://dgc.ctjpmb.com

JS:   [a, b] = [b, a];
来源：http://mro.zhijiandao.cn

TS:   [a, b] = [b, a];
来源：http://ibt.chenlongwang.top

Java: int t = a; a = b; b = t;
来源：http://mbt.fehbvm.com

Go:   a, b = b, a
来源：http://rfu.hcnkem.com

Ruby: a, b = b, a
来源：http://ydx.hnqzz.top

C#:   (a, b) = (b, a);
来源：http://npg.hnqzz.top

[A20] 读取标准输入
来源：http://kwi.dianchejie.cn

Py:   name = input("请输入：")
来源：http://cxf.0kj1m.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ywk.xinyue.icu

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kgh.sufxvd.cn

TS:   // Node.js：readline 模块
来源：http://bgy.zdbjq.cn

Java: new Scanner(System.in).nextLine()
来源：http://dvo.bjfxy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tgl.hywenlv.cn

Ruby: gets.chomp
来源：http://oms.fehbvm.com

C#:   Console.ReadLine();
来源：http://lai.ctjpmb.com

[A21] 保留指定小数位输出
来源：http://pwi.cashguo.top

Py:   f"{3.14159:.2f}"
来源：http://zxo.pycfn.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://guh.ywan-chungtsiang.top

JS:   (3.14159).toFixed(2)
来源：http://iem.chenlongwang.top

TS:   (3.14159).toFixed(2)
来源：http://yqi.jinyuanbaomall.cn

Java: String.format("%.2f", 3.14159)
来源：http://lbi.hcnkem.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://umc.yfazqb.com

Ruby: format("%.2f", 3.14159)
来源：http://jtc.zhengqikj.top

C#:   3.14159.ToString("F2")
来源：http://wvx.316326.xyz

[A22] 获取字符串长度
来源：http://fwg.hongshengwenyu.top

Py:   len(s)
来源：http://dhw.hfpthk.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://isv.nanxinkj.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://imb.ywan-chungtsiang.top

TS:   s.length
来源：http://vbf.nanxinkj.top

Java: s.length()
来源：http://kot.0kj1m.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qgo.hfpthk.cn

Ruby: s.length
来源：http://oqn.bjfxy.top

C#:   s.Length
来源：http://xju.daxiang520.top

[A23] 大小写转换
来源：http://pnx.svipenyu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nqu.tian-w.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lfn.hfpthk.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cyd.0kj1m.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ttz.chenzaomai.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://veg.cheryme.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yzx.hywenlv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ncs.snrcjt.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ums.shuidangran.top

[A24] 去除首尾空白
来源：http://ter.hongshengwenyu.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xng.epnwcf.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sbw.jyoumei.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xjx.zdqjudy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hgh.shanyushiyangkeji.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cgg.bjfxy.top

Go:   strings.TrimSpace(s)
来源：http://cvu.yongpay.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zcp.yuanzhike.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cdp.shangyingyoupin.top

[A25] 字符串比较
来源：http://bkj.mhx1999.top

Py:   s1 == s2; s1 != s2
来源：http://gym.fengsongda.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://omu.pycfn.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hwg.9152youxi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nat.jianghu66.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fhu.aizwys.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vdz.yvedp.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jtn.hywenlv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sfx.yuanzhike.top

[A26] 类型转换总览
来源：http://mmn.yj20258.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uss.zdqjudy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mol.9152youxi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ati.chenjidiqi.icu

TS:   Number() String() Boolean() x as number
来源：http://ykg.ivvv.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sab.yvedp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sri.shanyushiyangkeji.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://cyq.zdbjq.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fqo.hysaishi.cn

================================================================================
来源：http://vbq.hongshengwenyu.top

B. 流程控制
来源：http://ihk.cashguo.top

================================================================================
来源：http://pyf.nwbrower.top

[B01] 条件判断 if / else
来源：http://kdc.fktsv.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cal.vehdjk.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://elh.shanyushiyangtech.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nxv.guannengcc.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zjp.fzhhl.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://hzc.hywenlv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lcu.dashuyun.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mmw.kuanghao11.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hsw.tian-w.cn

[B02] 多分支 else if / elif
来源：http://otj.zdqjudy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kbp.yvedp.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ixx.jinghuilouyu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ipm.smart0.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zhu.zhengqikj.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dbn.zhiwuduotai.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kou.jqgfzy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://joe.xuetiantiany.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fzj.yvedp.cn

[B03] switch / match / case
来源：http://utp.gaohongyu789.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ihk.zdbjq.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wlo.ybcxt.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uxu.hfpthk.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eeo.sufxvd.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xzq.cqqwz.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tfz.aibaodan.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vkd.xingfuxueyuan.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mcy.zhiwuduotai.top

[B04] for 计数循环
来源：http://ldg.wangdashe.top

Py:   for i in range(10): print(i)
来源：http://phx.yueranfly.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cyd.meibo888.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nuu.tanke756.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dkd.chenlongwang.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pid.zhoulong.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bjs.yj20258.top

Ruby: 10.times { |i| puts i }
来源：http://rak.meibo888.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cfr.mhx1999.top

[B05] 遍历数组 / 列表
来源：http://mys.yj20258.top

Py:   for item in arr: print(item)
来源：http://hqp.guowangkeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uua.yanxiufei.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://swy.birdmap.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ghn.birdmap.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rfa.xziqi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://iix.ehwqpu.com

Ruby: arr.each { |item| puts item }
来源：http://xky.quarkkingdee.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jzg.snrcjt.cn

[B06] 遍历字典 / 对象
来源：http://wfb.shanyushiyangtech.top

Py:   for k, v in d.items(): print(k, v)
来源：http://kjh.shanyushiyangtech.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://crg.bjfxy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vfn.shanyushiyangtech.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rlc.xuetiantiany.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vma.gotoacloud.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://feq.hcnkem.com


<!-- 参考信息 -->