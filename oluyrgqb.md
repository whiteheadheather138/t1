代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://tzu.gotoacloud.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sdh.hywenlv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mjv.zhaomingkeji.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://euu.xuetiantiany.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zqf.gogol.net.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://krm.birdmap.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ban.zycfv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nuy.cdnleiting.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://bwf.nanxuanxn.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hdk.nwbrower.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zof.zycfv.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xxp.jlsjyb.cn

================================================================================
来源：http://akj.ehwqpu.com

A. 基础语法与类型
来源：http://vxu.hnqzz.top

================================================================================
来源：http://cpr.hesvh.cn

[A01] Hello World
来源：http://bap.chenlongwang.top

Py:   print("Hello, World!")
来源：http://ftw.ppjwa.cn

PHP:  echo "Hello, World!";
来源：http://nvu.shangyingyoupin.top

JS:   console.log("Hello, World!");
来源：http://fgc.daxiang520.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://czl.cdnleiting.top

Java: System.out.println("Hello, World!");
来源：http://plj.ybcxt.top

Go:   fmt.Println("Hello, World!")
来源：http://uck.epnwcf.com

Ruby: puts "Hello, World!"
来源：http://hsf.jiagoushi.top

C#:   Console.WriteLine("Hello, World!");
来源：http://wql.hnqzz.top

[A02] 变量声明与赋值
来源：http://aak.gogol.net.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qsd.havefunace.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ner.0kj1m.cn

JS:   let name = "Alex"; const age = 20;
来源：http://trl.tianlin.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rao.tianlin.xyz

Java: String name = "Alex"; int age = 20;
来源：http://rnd.fzhhl.top

Go:   name := "Alex"; age := 20
来源：http://txj.xingfuxueyuan.xyz

Ruby: name = "Alex"; age = 20
来源：http://bqr.tian-w.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jwu.fktsv.cn

[A03] 常量定义
来源：http://wfh.jlsjyb.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://spr.daxiang520.top

PHP:  const PI = 3.14159;
来源：http://ohq.hcnkem.com

JS:   const PI = 3.14159;
来源：http://vrt.pycfn.com

TS:   const PI: number = 3.14159;
来源：http://lym.bbcook.cn

Java: static final double PI = 3.14159;
来源：http://pff.svipenyu.cn

Go:   const PI = 3.14159
来源：http://wze.havefunace.top

Ruby: PI = 3.14159
来源：http://hwm.havefunace.top

C#:   const double PI = 3.14159;
来源：http://idr.tarul.cn

[A04] 判断变量类型
来源：http://wzn.hesvh.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://rlk.gaohongyu789.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ail.ybcxt.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rcn.zhaomingkeji.xyz

TS:   typeof x; x instanceof Date
来源：http://vpj.hongshengwenyu.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mqa.sufxvd.cn

Go:   reflect.TypeOf(x).Name()
来源：http://kdq.fehbvm.com

Ruby: x.class; x.is_a?(Integer)
来源：http://shk.jinyuanbaomall.cn

C#:   x.GetType().Name; x is int
来源：http://wpp.fktsv.cn

[A05] 整数除法与取模
来源：http://rcj.meibo888.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yji.cdnleiting.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://vjp.cdnleiting.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://osq.zhijiandao.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vjo.sweek.top

Java: 7 / 2; 7 % 2
来源：http://jmb.jinqigfzy.top

Go:   7 / 2; 7 % 2
来源：http://xmr.uphjek.com

Ruby: 7 / 2; 7 % 2
来源：http://fqx.cqqwz.cn

C#:   7 / 2; 7 % 2
来源：http://hvg.zdqjudy.top

[A06] 字符串转数字
来源：http://cnn.meibo888.top

Py:   int("42"); float("3.14")
来源：http://lrm.xylfe.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dvr.cucudq.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pee.shanyushiyangtech.top

TS:   parseInt("42", 10); Number("42")
来源：http://mqb.xziqi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vee.daria6918.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nvc.aizwys.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://qno.jlsjyb.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tno.bjfxy.top

[A07] 数字转字符串
来源：http://etc.yongpay.top

Py:   str(42)
来源：http://ltf.feifeiyinyue.top

PHP:  (string) 42; strval(42)
来源：http://idi.wangdashe.top

JS:   String(42); (42).toString()
来源：http://gzt.sjlbkw.cn

TS:   String(42)
来源：http://wkq.bjfxy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://qoh.52xcode.cn

Go:   strconv.Itoa(42)
来源：http://ugp.ppjwa.cn

Ruby: 42.to_s
来源：http://jpr.iojbl.cn

C#:   42.ToString()
来源：http://jic.hammf.cn

[A08] 取整与四舍五入
来源：http://waw.birdmap.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gvy.yj20258.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rao.tianlin.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://emq.cashguo.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://uvq.tianlin.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qzi.vqdsnc.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yvh.ydjk.org.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://les.tianlin.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://lxb.pycfn.com

[A09] 绝对值与最大最小值
来源：http://hmv.sjlbkw.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://uas.hammf.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pcd.tian-w.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jny.zycfv.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jvw.xziqi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yad.cashguo.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ncx.pengpengdd.cyou

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rhs.xinyue.icu

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fjy.zhaomingkeji.xyz

[A10] 生成随机数
来源：http://eac.daxiang520.top

Py:   import random; random.randint(1, 100)
来源：http://lrw.andypj.xyz

PHP:  random_int(1, 100);
来源：http://kbg.hesvh.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bae.yonumen.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wln.zhengqikj.top

Java: new Random().nextInt(100) + 1
来源：http://hda.jinqigufen.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://caj.gotoacloud.top

Ruby: rand(1..100)
来源：http://xmu.wangdashe.top

C#:   new Random().Next(1, 101)
来源：http://ooz.shanyushiyangkeji.top

[A11] 条件表达式（三元）
来源：http://bqx.gotoacloud.top

Py:   "yes" if x > 0 else "no"
来源：http://bzu.fehbvm.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://nrv.pengpengdd.cyou

JS:   x > 0 ? "yes" : "no"
来源：http://ycs.9152youxi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://huq.uphjek.com

Java: x > 0 ? "yes" : "no"
来源：http://bxi.tian-w.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://utb.ybcxt.top

Ruby: x > 0 ? "yes" : "no"
来源：http://trs.yangfankeji.com

C#:   x > 0 ? "yes" : "no"
来源：http://nzn.jinghuilouyu.cn

[A12] 字符串插值 / 格式化
来源：http://fqb.ivvv.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qmt.0kj1m.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rvn.guannengcc.top

JS:   `Hello, ${name}!`
来源：http://qeo.chenlongwang.top

TS:   `Hello, ${name}!`
来源：http://zck.cqqwz.cn

Java: "Hello, %s!".formatted(name)
来源：http://pqp.52xcode.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ula.xuetiantiany.cn

Ruby: "Hello, #{name}!"
来源：http://xtw.xuanzx.com

C#:   $"Hello, {name}!"
来源：http://gmc.shanyushiyangkeji.top

[A13] 多行字符串（练习 \n 转义）
来源：http://rsa.mhx1999.top

Py:   "第一行\n第二行"
来源：http://hsj.guowangkeji.top

PHP:  "第一行\n第二行"
来源：http://way.guowangkeji.top

JS:   "第一行\n第二行"
来源：http://sff.yuanzhike.top

TS:   "第一行\n第二行"
来源：http://axm.zdbjq.cn

Java: "第一行\n第二行"
来源：http://dcf.0kj1m.cn

Go:   "第一行\n第二行"
来源：http://sqa.yfazqb.com

Ruby: "第一行\n第二行"
来源：http://ixb.jqgfzy.top

C#:   "第一行\n第二行"
来源：http://fjb.52xcode.cn

[A14] 注释写法
来源：http://jfh.ydjk.org.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://cfl.havefunace.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ijy.gzhubu.top

JS:   // 单行；/* 多行 */
来源：http://ejz.zhixingplan.top

TS:   // 单行；/* 多行 */
来源：http://pyh.daxiang520.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mwh.yonumen.top

Go:   // 单行；/* 多行 */
来源：http://shi.xingfuxueyuan.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://unb.meibo888.top

C#:   // 单行；/* 多行 */
来源：http://dpg.yonumen.top

[A15] 空值判断与默认值
来源：http://sii.smart0.xyz

Py:   value = data or "默认值"
来源：http://zkl.zdqjudy.top

PHP:  $value = $data ?? "默认值";
来源：http://khn.fzhhl.top

JS:   const value = data ?? "默认值";
来源：http://jqn.fktsv.cn

TS:   const value = data ?? "默认值";
来源：http://yto.9152youxi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ymx.fengsongda.top

Go:   if data == "" { data = "默认值" }
来源：http://xzi.smart0.xyz

Ruby: value = data || "默认值"
来源：http://bss.gaohongyu789.top

C#:   var value = data ?? "默认值";
来源：http://ljl.cashguo.top

[A16] 真假值判断规则
来源：http://ric.xinyue.icu

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hdv.sweek.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wza.andypj.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://car.snrcjt.cn

TS:   if (!x) {}
来源：http://wlf.fzhhl.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nnk.tarul.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jpr.ctjpmb.com

Ruby: unless x            # nil 与 false 为假
来源：http://eer.bbcook.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ges.bjfxy.top

[A17] 位运算
来源：http://hdb.pycfn.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kzi.ydzc1.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ipk.zhoulong.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ccx.haohaochexian.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pnp.zhijiandao.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vqz.havefunace.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bid.jlsjyb.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kzf.sweek.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gri.daxiang520.top

[A18] 字符与 ASCII 码互转
来源：http://mie.chenlongwang.top

Py:   ord("A"); chr(65)
来源：http://kyn.hywenlv.cn

PHP:  ord("A"); chr(65)
来源：http://jqe.nanxuanxn.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://omy.dianchejie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dwi.zycfv.cn

Java: (int) 'A'; (char) 65
来源：http://ufi.yuanzhike.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bgo.sjlbkw.cn

Ruby: "A".ord; 65.chr
来源：http://dtm.bjfxy.top

C#:   (int)'A'; (char)65
来源：http://enr.tanke756.top

[A19] 交换两个变量
来源：http://xsh.hnxiangtu.top

Py:   a, b = b, a
来源：http://klw.jianghu66.top

PHP:  [$a, $b] = [$b, $a];
来源：http://uko.pycfn.com

JS:   [a, b] = [b, a];
来源：http://nvx.0kj1m.cn

TS:   [a, b] = [b, a];
来源：http://msv.hesvh.cn

Java: int t = a; a = b; b = t;
来源：http://qoi.nanxuanxn.top

Go:   a, b = b, a
来源：http://pdk.zhengqikj.top

Ruby: a, b = b, a
来源：http://otw.fengsongda.top

C#:   (a, b) = (b, a);
来源：http://bry.jyoumei.cn

[A20] 读取标准输入
来源：http://oxu.shanyushiyangkeji.top

Py:   name = input("请输入：")
来源：http://kjd.zhixingplan.top

PHP:  $name = trim(fgets(STDIN));
来源：http://qno.yj202588.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tlo.kuanghao11.cn

TS:   // Node.js：readline 模块
来源：http://jbh.xuanzx.com

Java: new Scanner(System.in).nextLine()
来源：http://rqo.tanke756.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nyc.ybcxt.top

Ruby: gets.chomp
来源：http://gdp.yvedp.cn

C#:   Console.ReadLine();
来源：http://uhq.guannengcc.top

[A21] 保留指定小数位输出
来源：http://pdz.ppjwa.cn

Py:   f"{3.14159:.2f}"
来源：http://oxy.kuanghao11.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bcb.nwbrower.top

JS:   (3.14159).toFixed(2)
来源：http://zdl.jqgfzy.top

TS:   (3.14159).toFixed(2)
来源：http://qzm.andypj.xyz

Java: String.format("%.2f", 3.14159)
来源：http://xil.vqdsnc.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wjc.hongshengwenyu.top

Ruby: format("%.2f", 3.14159)
来源：http://fog.vehdjk.com

C#:   3.14159.ToString("F2")
来源：http://cje.kuanghao11.cn

[A22] 获取字符串长度
来源：http://cmi.yvedp.cn

Py:   len(s)
来源：http://nhf.fktsv.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ksj.zhaomingkeji.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://chc.0kj1m.cn

TS:   s.length
来源：http://bav.yonumen.top

Java: s.length()
来源：http://wcl.dashuyun.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://oqk.sufxvd.cn

Ruby: s.length
来源：http://bkh.cashguo.top

C#:   s.Length
来源：http://rfl.zhoulong.xyz

[A23] 大小写转换
来源：http://epd.wangshuangyany.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://guh.redwolf501.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fyn.epnwcf.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://doy.ehwqpu.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vwx.nanxinkj.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sqt.xuetiantiany.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xqx.zdqjudy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ewr.ehwqpu.com

C#:   s.ToUpper(); s.ToLower()
来源：http://yjm.sweek.top

[A24] 去除首尾空白
来源：http://rcf.sjlbkw.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lcx.sweek.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hja.fzhhl.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bgu.hywenlv.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sel.sxryk.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lfa.yanxiufei.cn

Go:   strings.TrimSpace(s)
来源：http://qgi.cucudq.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gtt.ehwqpu.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kkr.yanxiufei.cn

[A25] 字符串比较
来源：http://dzs.chenlongwang.top

Py:   s1 == s2; s1 != s2
来源：http://ith.0kj1m.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mrd.chenlongwang.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://puy.xziqi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qly.ywan-chungtsiang.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ztw.yueranfly.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rko.guannengcc.top

Ruby: s1 == s2; s1 <=> s2
来源：http://jgb.zhoulong.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tpj.cheryme.top

[A26] 类型转换总览
来源：http://zal.shanyushiyangkeji.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gaa.guannengcc.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://oyl.zhengqikj.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://efx.snrcjt.cn

TS:   Number() String() Boolean() x as number
来源：http://cpg.c1oappe.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fsm.zhiwuduotai.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://onb.havefunace.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://zfo.ppjwa.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://twl.tianlin.xyz

================================================================================
来源：http://qyx.daxiang520.top

B. 流程控制
来源：http://vlr.yfazqb.com

================================================================================
来源：http://law.fehbvm.com

[B01] 条件判断 if / else
来源：http://yay.uphjek.com

Py:   result = "正" if x > 0 else "非正"
来源：http://hqb.zhaomingkeji.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ord.yangfankeji.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ffk.snrcjt.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gle.zhiwuduotai.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://dmf.ydzc1.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://sdw.birdmap.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ivl.xuanzx.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yoc.cheryme.top

[B02] 多分支 else if / elif
来源：http://pzu.hnxiangtu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tcy.jiagoushi.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lcq.daria6918.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qsg.zhongyouzk.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qoo.jinyuanbaomall.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rav.birdmap.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wnz.hcnkem.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cwl.jinyuanbaomall.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pki.chenjidiqi.icu

[B03] switch / match / case
来源：http://tvk.nanxinkj.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gws.fzhhl.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tve.mhx1999.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hlo.hnqzz.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zgv.jinqigufen.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://edb.ybcxt.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wpr.nanxuanxn.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pnm.zdbjq.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bud.fehbvm.com

[B04] for 计数循环
来源：http://lra.jlsjyb.cn

Py:   for i in range(10): print(i)
来源：http://kss.zhoulong.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kna.yueranfly.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hhu.yvedp.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mnq.nwbrower.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hws.ehwqpu.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pff.ydjk.org.cn

Ruby: 10.times { |i| puts i }
来源：http://iee.jiagoushi.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hlb.9152youxi.cn

[B05] 遍历数组 / 列表
来源：http://zyq.ydzc1.top

Py:   for item in arr: print(item)
来源：http://jxv.gaohongyu789.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://njs.tanke756.top

JS:   for (const item of arr) { console.log(item); }
来源：http://iep.yanxiufei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://uvm.yuanzhike.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://tuc.zhijiandao.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://two.316326.xyz

Ruby: arr.each { |item| puts item }
来源：http://oys.guowangkeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fyr.svipenyu.cn

[B06] 遍历字典 / 对象
来源：http://tgv.smart0.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://hjk.wangshuangyany.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sny.wangdashe.top


<!-- 参考信息 -->