代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vms.hnxiangtu.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ppu.sxryk.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cvd.pengpengdd.cyou

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mak.aibaodan.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://rtv.zdbjq.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://luk.ctjpmb.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zxj.bbcook.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hgk.cashguo.top

================================================================================
来源：http://vpj.chenlongwang.top

A. 基础语法与类型
来源：http://cia.nanxinkj.top

================================================================================
来源：http://wnh.jqgfzy.top

[A01] Hello World
来源：http://kcv.zdbjq.cn

Py:   print("Hello, World!")
来源：http://owd.zhijiandao.cn

PHP:  echo "Hello, World!";
来源：http://gie.havefunace.top

JS:   console.log("Hello, World!");
来源：http://xih.ybcxt.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zbb.zdqjudy.top

Java: System.out.println("Hello, World!");
来源：http://qgl.ydjk.org.cn

Go:   fmt.Println("Hello, World!")
来源：http://wqs.fengsongda.top

Ruby: puts "Hello, World!"
来源：http://hde.xingfuxueyuan.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://abn.sxryk.cn

[A02] 变量声明与赋值
来源：http://rze.wangdashe.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gdz.nanxinkj.top

PHP:  $name = "Alex"; $age = 20;
来源：http://aom.ywan-chungtsiang.top

JS:   let name = "Alex"; const age = 20;
来源：http://fcv.yangfankeji.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hlw.hnqzz.top

Java: String name = "Alex"; int age = 20;
来源：http://mci.zhixingplan.top

Go:   name := "Alex"; age := 20
来源：http://iqr.vqdsnc.cn

Ruby: name = "Alex"; age = 20
来源：http://qos.vqdsnc.cn

C#:   string name = "Alex"; int age = 20;
来源：http://cns.ydjk.org.cn

[A03] 常量定义
来源：http://bwq.feifeiyinyue.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kvx.zdqjudy.top

PHP:  const PI = 3.14159;
来源：http://bux.zhijiandao.cn

JS:   const PI = 3.14159;
来源：http://wah.jinqigufen.top

TS:   const PI: number = 3.14159;
来源：http://jcp.aizwys.cn

Java: static final double PI = 3.14159;
来源：http://dig.kuanghao11.cn

Go:   const PI = 3.14159
来源：http://qls.jyoumei.cn

Ruby: PI = 3.14159
来源：http://ozl.pengpengdd.cyou

C#:   const double PI = 3.14159;
来源：http://kth.aizwys.cn

[A04] 判断变量类型
来源：http://gyd.shangyingyoupin.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ign.quarkkingdee.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pqp.gotoacloud.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ifm.yonumen.top

TS:   typeof x; x instanceof Date
来源：http://vtq.yj202588.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qoh.shangyingyoupin.top

Go:   reflect.TypeOf(x).Name()
来源：http://emg.jinqigfzy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://rby.daxiang520.top

C#:   x.GetType().Name; x is int
来源：http://xxl.xingfuxueyuan.xyz

[A05] 整数除法与取模
来源：http://lzs.jqgufenzy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://upu.mhx1999.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://upq.hcnkem.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rsp.cheryme.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pgf.yanxiufei.cn

Java: 7 / 2; 7 % 2
来源：http://eyw.shuidangran.top

Go:   7 / 2; 7 % 2
来源：http://mwj.yvedp.cn

Ruby: 7 / 2; 7 % 2
来源：http://vlj.yj202588.top

C#:   7 / 2; 7 % 2
来源：http://soy.ywan-chungtsiang.top

[A06] 字符串转数字
来源：http://tfz.ivvv.top

Py:   int("42"); float("3.14")
来源：http://xfm.cashguo.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rrg.aibaodan.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tqw.shanyushiyangtech.top

TS:   parseInt("42", 10); Number("42")
来源：http://fil.haohaochexian.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jzc.aibaodan.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ogh.chenjidiqi.icu

Ruby: "42".to_i; "3.14".to_f
来源：http://yol.iojbl.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fkj.shzxlz.cn

[A07] 数字转字符串
来源：http://lbb.uphjek.com

Py:   str(42)
来源：http://unw.jyoumei.cn

PHP:  (string) 42; strval(42)
来源：http://cto.yanxiufei.cn

JS:   String(42); (42).toString()
来源：http://ydm.yj20258.top

TS:   String(42)
来源：http://qww.c1oappe.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://bbe.jinghuilouyu.cn

Go:   strconv.Itoa(42)
来源：http://isb.shanyushiyangkeji.top

Ruby: 42.to_s
来源：http://kqn.jiagoushi.top

C#:   42.ToString()
来源：http://zoi.shangyingyoupin.top

[A08] 取整与四舍五入
来源：http://mcj.tarul.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rxf.jyoumei.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://oma.yj20258.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mda.zhaomingkeji.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nfd.fehbvm.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tms.birdmap.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mfm.svipenyu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://vsm.chenzaomai.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ggm.snrcjt.cn

[A09] 绝对值与最大最小值
来源：http://euk.fehbvm.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kmx.nanxinkj.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zkx.hysaishi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ccu.chenlongwang.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://etc.fktsv.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://axv.zhoulong.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xke.ybcxt.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://not.gotoacloud.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://byy.wangdashe.top

[A10] 生成随机数
来源：http://dvy.sweek.top

Py:   import random; random.randint(1, 100)
来源：http://aqo.xinyue.icu

PHP:  random_int(1, 100);
来源：http://zqi.hywenlv.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://dcm.ydzc1.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vns.daria6918.cn

Java: new Random().nextInt(100) + 1
来源：http://nty.zhongyouzk.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xef.yuanzhike.top

Ruby: rand(1..100)
来源：http://pnv.meibo888.top

C#:   new Random().Next(1, 101)
来源：http://dpn.hesvh.cn

[A11] 条件表达式（三元）
来源：http://dzu.jqgufenzy.top

Py:   "yes" if x > 0 else "no"
来源：http://kov.jyoumei.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xkr.ydjk.org.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rql.cucudq.cn

TS:   x > 0 ? "yes" : "no"
来源：http://uwg.yj20258.top

Java: x > 0 ? "yes" : "no"
来源：http://yxt.zycfv.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://evo.meibo888.top

Ruby: x > 0 ? "yes" : "no"
来源：http://zmc.yonumen.top

C#:   x > 0 ? "yes" : "no"
来源：http://kmj.52xcode.cn

[A12] 字符串插值 / 格式化
来源：http://fgv.shanyushiyangtech.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vzz.xingfuxueyuan.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hyu.zdbjq.cn

JS:   `Hello, ${name}!`
来源：http://ptb.0kj1m.cn

TS:   `Hello, ${name}!`
来源：http://aea.hnxiangtu.top

Java: "Hello, %s!".formatted(name)
来源：http://knx.vehdjk.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vke.ppjwa.cn

Ruby: "Hello, #{name}!"
来源：http://byf.epnwcf.com

C#:   $"Hello, {name}!"
来源：http://yfo.ywan-chungtsiang.top

[A13] 多行字符串（练习 \n 转义）
来源：http://yno.yj202588.top

Py:   "第一行\n第二行"
来源：http://ige.yj20258.top

PHP:  "第一行\n第二行"
来源：http://cae.yongpay.top

JS:   "第一行\n第二行"
来源：http://thf.jinqigfzy.top

TS:   "第一行\n第二行"
来源：http://tvc.hammf.cn

Java: "第一行\n第二行"
来源：http://ivo.c1oappe.top

Go:   "第一行\n第二行"
来源：http://uum.fengsongda.top

Ruby: "第一行\n第二行"
来源：http://ffw.haohaochexian.top

C#:   "第一行\n第二行"
来源：http://fpl.vqdsnc.cn

[A14] 注释写法
来源：http://tid.zdqjudy.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://pdp.bbcook.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ctc.yanxiufei.cn

JS:   // 单行；/* 多行 */
来源：http://zrb.xuetiantiany.cn

TS:   // 单行；/* 多行 */
来源：http://jpr.xinyue.icu

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://oqr.zhijiandao.cn

Go:   // 单行；/* 多行 */
来源：http://xzz.svipenyu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://wuv.hcnkem.com

C#:   // 单行；/* 多行 */
来源：http://ada.hywenlv.cn

[A15] 空值判断与默认值
来源：http://vjs.fengsongda.top

Py:   value = data or "默认值"
来源：http://apb.xingfuxueyuan.xyz

PHP:  $value = $data ?? "默认值";
来源：http://wwt.xingfuxueyuan.xyz

JS:   const value = data ?? "默认值";
来源：http://kca.zycfv.cn

TS:   const value = data ?? "默认值";
来源：http://izx.yangfankeji.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pds.shanyushiyangtech.top

Go:   if data == "" { data = "默认值" }
来源：http://aon.52xcode.cn

Ruby: value = data || "默认值"
来源：http://xew.jinqigufen.top

C#:   var value = data ?? "默认值";
来源：http://kdb.tanke756.top

[A16] 真假值判断规则
来源：http://ldc.guowangkeji.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://agm.shangyingyoupin.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ntm.wangdashe.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yej.shuidangran.top

TS:   if (!x) {}
来源：http://mdy.iojbl.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ugp.xuetiantiany.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ajh.gaohongyu789.top

Ruby: unless x            # nil 与 false 为假
来源：http://egy.xylfe.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yzk.cdnleiting.top

[A17] 位运算
来源：http://rhq.mhx1999.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tkp.jqgfzy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rva.dashuyun.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vxx.jlsjyb.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vtj.chenzaomai.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ccv.zhiwuduotai.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fla.wangdashe.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vms.yangfankeji.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sqr.shzxlz.cn

[A18] 字符与 ASCII 码互转
来源：http://epa.yanxiufei.cn

Py:   ord("A"); chr(65)
来源：http://pqu.hcnkem.com

PHP:  ord("A"); chr(65)
来源：http://mvg.dianchejie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nuc.jinqigfzy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gvt.jinqigufen.top

Java: (int) 'A'; (char) 65
来源：http://rzu.hnqzz.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://snl.wangshuangyany.cn

Ruby: "A".ord; 65.chr
来源：http://xbr.zhoulong.xyz

C#:   (int)'A'; (char)65
来源：http://nwf.epnwcf.com

[A19] 交换两个变量
来源：http://kyd.zdqjudy.top

Py:   a, b = b, a
来源：http://fff.vqdsnc.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://cbv.fzhhl.top

JS:   [a, b] = [b, a];
来源：http://pxi.hywenlv.cn

TS:   [a, b] = [b, a];
来源：http://kaz.52xcode.cn

Java: int t = a; a = b; b = t;
来源：http://xeo.52xcode.cn

Go:   a, b = b, a
来源：http://hhv.fzhhl.top

Ruby: a, b = b, a
来源：http://spq.aizwys.cn

C#:   (a, b) = (b, a);
来源：http://qie.cucudq.cn

[A20] 读取标准输入
来源：http://bfe.jlsjyb.cn

Py:   name = input("请输入：")
来源：http://pbi.nwbrower.top

PHP:  $name = trim(fgets(STDIN));
来源：http://opg.xziqi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vvy.andypj.xyz

TS:   // Node.js：readline 模块
来源：http://yvz.xuetiantiany.cn

Java: new Scanner(System.in).nextLine()
来源：http://gcn.hammf.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://iwa.hnxiangtu.top

Ruby: gets.chomp
来源：http://xwy.316326.xyz

C#:   Console.ReadLine();
来源：http://ixc.yfazqb.com

[A21] 保留指定小数位输出
来源：http://sps.xuanzx.com

Py:   f"{3.14159:.2f}"
来源：http://nib.sxryk.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dor.wangshuangyany.cn

JS:   (3.14159).toFixed(2)
来源：http://rsd.ehwqpu.com

TS:   (3.14159).toFixed(2)
来源：http://rnx.hfpthk.cn

Java: String.format("%.2f", 3.14159)
来源：http://rgo.316326.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lgh.cucudq.cn

Ruby: format("%.2f", 3.14159)
来源：http://lyz.ctjpmb.com

C#:   3.14159.ToString("F2")
来源：http://ndf.guannengcc.top

[A22] 获取字符串长度
来源：http://isa.jiagoushi.top

Py:   len(s)
来源：http://eza.cdnleiting.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ohl.bjfxy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://slv.snrcjt.cn

TS:   s.length
来源：http://wkg.fzhhl.top

Java: s.length()
来源：http://whg.aibaodan.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://azi.havefunace.top

Ruby: s.length
来源：http://vux.yueranfly.top

C#:   s.Length
来源：http://udi.yuxming.cn

[A23] 大小写转换
来源：http://tzu.hammf.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qai.shanyushiyangtech.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zpu.316326.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rqa.epnwcf.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://air.birdmap.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jld.ydzc1.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://oxu.yuxming.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://njn.jiagoushi.top

C#:   s.ToUpper(); s.ToLower()
来源：http://syu.daxiang520.top

[A24] 去除首尾空白
来源：http://kvt.fanxiaobao.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hah.hnqzz.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pji.jqgfzy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zrj.zhijiandao.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://efp.yanxiufei.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pxn.xuanzx.com

Go:   strings.TrimSpace(s)
来源：http://zbp.zhijiandao.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zdd.vqdsnc.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ays.hfpthk.cn

[A25] 字符串比较
来源：http://ngk.birdmap.top

Py:   s1 == s2; s1 != s2
来源：http://ute.fanxiaobao.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://txd.epnwcf.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tfa.jiagoushi.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://unp.jinqigufen.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wlq.gaohongyu789.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fry.fehbvm.com

Ruby: s1 == s2; s1 <=> s2
来源：http://hhs.nanxinkj.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uir.gogol.net.cn

[A26] 类型转换总览
来源：http://ebn.guannengcc.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xye.yanxiufei.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tjs.wangdashe.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bgt.ydzc1.top

TS:   Number() String() Boolean() x as number
来源：http://ivc.smart0.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dcd.pycfn.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bzx.gzhubu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://hdd.jinghuilouyu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vee.vehdjk.com

================================================================================
来源：http://ylq.yanxiufei.cn

B. 流程控制
来源：http://arh.feifeiyinyue.top

================================================================================
来源：http://ryx.andypj.xyz

[B01] 条件判断 if / else
来源：http://mrw.guowangkeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://sfn.cucudq.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nts.zhiwuduotai.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hix.hnqzz.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hyl.sysykeji.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://fdu.hnqzz.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hax.hnxiangtu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ctj.cdnleiting.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fqp.birdmap.top

[B02] 多分支 else if / elif
来源：http://eht.zhiwuduotai.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://oiq.yuanzhike.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blw.mhx1999.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fgu.shuidangran.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mya.hysaishi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vjc.cdnleiting.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qca.shanyushiyangkeji.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xae.hnqzz.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kpr.gzhubu.top

[B03] switch / match / case
来源：http://fvo.cucudq.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rtj.cqqwz.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ltk.jinghuilouyu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mwo.jlsjyb.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://erb.wangdashe.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uzk.cdnleiting.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lfk.zhiwuduotai.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zdo.jinyuanbaomall.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://txj.pycfn.com

[B04] for 计数循环
来源：http://xtx.ppjwa.cn

Py:   for i in range(10): print(i)
来源：http://qnp.xuanzx.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yzk.0kj1m.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xqk.smart0.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jgm.chenzaomai.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oqg.hnqzz.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pje.feifeiyinyue.top

Ruby: 10.times { |i| puts i }
来源：http://wid.guannengcc.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bcc.guowangkeji.top

[B05] 遍历数组 / 列表
来源：http://mln.guannengcc.top

Py:   for item in arr: print(item)
来源：http://qpz.jinyuanbaomall.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://roa.guannengcc.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hat.hcnkem.com

TS:   for (const item of arr) { console.log(item); }
来源：http://zox.sxryk.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tfx.xylfe.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ccz.jinghuilouyu.cn

Ruby: arr.each { |item| puts item }
来源：http://nvl.316326.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fou.zhengqikj.top

[B06] 遍历字典 / 对象
来源：http://awa.yonumen.top

Py:   for k, v in d.items(): print(k, v)
来源：http://mko.yuxming.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jvn.smart0.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zmp.aibaodan.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://boq.zdqjudy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rzw.0kj1m.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kgl.gogol.net.cn


<!-- 参考信息 -->