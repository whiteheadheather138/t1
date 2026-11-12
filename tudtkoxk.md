代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mad.zhaomingkeji.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yir.sufxvd.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://eha.yvedp.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zsi.aizwys.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cdq.zdbjq.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uiu.zhoulong.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ybl.zdqjudy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gsr.guowangkeji.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://npx.fzhhl.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jwu.sufxvd.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lbs.jqgfzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://otp.hywenlv.cn

================================================================================
来源：http://stl.ydzc1.top

A. 基础语法与类型
来源：http://hhx.mhx1999.top

================================================================================
来源：http://xjn.mhx1999.top

[A01] Hello World
来源：http://bpf.fktsv.cn

Py:   print("Hello, World!")
来源：http://czm.zhaomingkeji.xyz

PHP:  echo "Hello, World!";
来源：http://zki.xziqi.cn

JS:   console.log("Hello, World!");
来源：http://ieh.iojbl.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ixd.yfazqb.com

Java: System.out.println("Hello, World!");
来源：http://yni.zhengqikj.top

Go:   fmt.Println("Hello, World!")
来源：http://hth.chenlongwang.top

Ruby: puts "Hello, World!"
来源：http://qdt.fanxiaobao.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://loe.bbcook.cn

[A02] 变量声明与赋值
来源：http://kvu.chenlongwang.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ujy.gzhubu.top

PHP:  $name = "Alex"; $age = 20;
来源：http://lnh.cucudq.cn

JS:   let name = "Alex"; const age = 20;
来源：http://uhd.yangfankeji.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qkb.pengpengdd.cyou

Java: String name = "Alex"; int age = 20;
来源：http://eoc.aizwys.cn

Go:   name := "Alex"; age := 20
来源：http://kbl.zdbjq.cn

Ruby: name = "Alex"; age = 20
来源：http://ryk.cdnleiting.top

C#:   string name = "Alex"; int age = 20;
来源：http://xtg.zdbjq.cn

[A03] 常量定义
来源：http://qxx.xuetiantiany.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ovn.kuanghao11.cn

PHP:  const PI = 3.14159;
来源：http://rem.hnxiangtu.top

JS:   const PI = 3.14159;
来源：http://fcb.sufxvd.cn

TS:   const PI: number = 3.14159;
来源：http://jlq.mhx1999.top

Java: static final double PI = 3.14159;
来源：http://oet.sufxvd.cn

Go:   const PI = 3.14159
来源：http://mvh.zdbjq.cn

Ruby: PI = 3.14159
来源：http://opz.zdbjq.cn

C#:   const double PI = 3.14159;
来源：http://cuf.yonumen.top

[A04] 判断变量类型
来源：http://vxa.shangyingyoupin.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://mqm.hammf.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wnu.jiagoushi.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://lke.cucudq.cn

TS:   typeof x; x instanceof Date
来源：http://qfl.snrcjt.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qmk.shanyushiyangkeji.top

Go:   reflect.TypeOf(x).Name()
来源：http://rzb.pycfn.com

Ruby: x.class; x.is_a?(Integer)
来源：http://pwk.zycfv.cn

C#:   x.GetType().Name; x is int
来源：http://avc.xuanzx.com

[A05] 整数除法与取模
来源：http://ram.52xcode.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zay.tarul.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://wcp.yueranfly.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ikp.svipenyu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tyh.yj20258.top

Java: 7 / 2; 7 % 2
来源：http://rpp.fehbvm.com

Go:   7 / 2; 7 % 2
来源：http://mxb.zhixingplan.top

Ruby: 7 / 2; 7 % 2
来源：http://tky.zhoulong.xyz

C#:   7 / 2; 7 % 2
来源：http://wnq.ydjk.org.cn

[A06] 字符串转数字
来源：http://dfc.9152youxi.cn

Py:   int("42"); float("3.14")
来源：http://ihi.shanyushiyangkeji.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xqk.cdnleiting.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tld.tianlin.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://dwx.havefunace.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nsz.snrcjt.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bvq.gogol.net.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://xpi.zhaomingkeji.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bmq.sysykeji.top

[A07] 数字转字符串
来源：http://xgc.yanxiufei.cn

Py:   str(42)
来源：http://ifa.epnwcf.com

PHP:  (string) 42; strval(42)
来源：http://qxy.yonumen.top

JS:   String(42); (42).toString()
来源：http://fwl.yj20258888.top

TS:   String(42)
来源：http://tor.fzhhl.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://oqr.ybcxt.top

Go:   strconv.Itoa(42)
来源：http://ram.tianlin.xyz

Ruby: 42.to_s
来源：http://cwy.52xcode.cn

C#:   42.ToString()
来源：http://mpa.hnqzz.top

[A08] 取整与四舍五入
来源：http://snz.xuetiantiany.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bhg.snrcjt.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vmx.hongshengwenyu.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fje.epnwcf.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://axk.yangfankeji.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hvj.ywan-chungtsiang.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ayv.sweek.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://omv.zhoulong.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jvq.shzxlz.cn

[A09] 绝对值与最大最小值
来源：http://mdt.yj20258.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qbp.pycfn.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qap.gzhubu.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dhw.sufxvd.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://srr.ehwqpu.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://git.zhoulong.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fak.fanxiaobao.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hns.wangdashe.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://sdz.jqgfzy.top

[A10] 生成随机数
来源：http://brv.sjlbkw.cn

Py:   import random; random.randint(1, 100)
来源：http://svj.wangshuangyany.cn

PHP:  random_int(1, 100);
来源：http://woi.jinyuanbaomall.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fbn.316326.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://eeu.0kj1m.cn

Java: new Random().nextInt(100) + 1
来源：http://xtb.zhoulong.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ucx.xuetiantiany.cn

Ruby: rand(1..100)
来源：http://uip.gotoacloud.top

C#:   new Random().Next(1, 101)
来源：http://jko.9152youxi.cn

[A11] 条件表达式（三元）
来源：http://djf.chenzaomai.com

Py:   "yes" if x > 0 else "no"
来源：http://wbw.shuidangran.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://lqr.316326.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://wpk.yanxiufei.cn

TS:   x > 0 ? "yes" : "no"
来源：http://sht.cashguo.top

Java: x > 0 ? "yes" : "no"
来源：http://qqi.jqgfzy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://zhj.sufxvd.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vrn.dashuyun.cn

C#:   x > 0 ? "yes" : "no"
来源：http://uqj.guannengcc.top

[A12] 字符串插值 / 格式化
来源：http://yoy.cashguo.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gdb.sjlbkw.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://iuu.hcnkem.com

JS:   `Hello, ${name}!`
来源：http://plv.fanxiaobao.xyz

TS:   `Hello, ${name}!`
来源：http://ilw.xinyue.icu

Java: "Hello, %s!".formatted(name)
来源：http://ejy.hnqzz.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mug.shanyushiyangkeji.top

Ruby: "Hello, #{name}!"
来源：http://jyu.ybcxt.top

C#:   $"Hello, {name}!"
来源：http://kyx.chenlongwang.top

[A13] 多行字符串（练习 \n 转义）
来源：http://tdw.yueranfly.top

Py:   "第一行\n第二行"
来源：http://grf.svipenyu.cn

PHP:  "第一行\n第二行"
来源：http://abv.shangyingyoupin.top

JS:   "第一行\n第二行"
来源：http://dcr.aizwys.cn

TS:   "第一行\n第二行"
来源：http://ikr.zhixingplan.top

Java: "第一行\n第二行"
来源：http://lwu.fktsv.cn

Go:   "第一行\n第二行"
来源：http://xkk.zdqjudy.top

Ruby: "第一行\n第二行"
来源：http://qqy.kuanghao11.cn

C#:   "第一行\n第二行"
来源：http://spy.haohaochexian.top

[A14] 注释写法
来源：http://nsq.pengpengdd.cyou

Py:   # 单行；三引号字符串可作多行说明
来源：http://nkl.ehwqpu.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://pwa.meibo888.top

JS:   // 单行；/* 多行 */
来源：http://esp.316326.xyz

TS:   // 单行；/* 多行 */
来源：http://viv.shuidangran.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ezo.hysaishi.cn

Go:   // 单行；/* 多行 */
来源：http://bll.cashguo.top

Ruby: # 单行；=begin 多行 =end
来源：http://avb.sweek.top

C#:   // 单行；/* 多行 */
来源：http://xjs.guannengcc.top

[A15] 空值判断与默认值
来源：http://vgv.yj20258888.top

Py:   value = data or "默认值"
来源：http://aak.epnwcf.com

PHP:  $value = $data ?? "默认值";
来源：http://zyk.hcnkem.com

JS:   const value = data ?? "默认值";
来源：http://vut.sxryk.cn

TS:   const value = data ?? "默认值";
来源：http://lla.aibaodan.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://aja.0kj1m.cn

Go:   if data == "" { data = "默认值" }
来源：http://wsm.nwbrower.top

Ruby: value = data || "默认值"
来源：http://bqi.havefunace.top

C#:   var value = data ?? "默认值";
来源：http://cac.fengsongda.top

[A16] 真假值判断规则
来源：http://gcq.hywenlv.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nmo.xuanzx.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rrm.cheryme.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kuv.gaohongyu789.top

TS:   if (!x) {}
来源：http://yly.fzhhl.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lzp.fzhhl.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://njp.vqdsnc.cn

Ruby: unless x            # nil 与 false 为假
来源：http://chh.nanxinkj.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pmn.chenlongwang.top

[A17] 位运算
来源：http://lfe.yuanzhike.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bxg.yuanzhike.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ucn.jyoumei.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cox.nwbrower.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://izp.hcnkem.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nlg.zhijiandao.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://aeo.shanyushiyangtech.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tgy.zhijiandao.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gfz.yonumen.top

[A18] 字符与 ASCII 码互转
来源：http://ole.9152youxi.cn

Py:   ord("A"); chr(65)
来源：http://xkl.hnqzz.top

PHP:  ord("A"); chr(65)
来源：http://amm.jinqigfzy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jdx.ehwqpu.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jhf.ehwqpu.com

Java: (int) 'A'; (char) 65
来源：http://zma.shanyushiyangkeji.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mwu.chenlongwang.top

Ruby: "A".ord; 65.chr
来源：http://lkq.shangyingyoupin.top

C#:   (int)'A'; (char)65
来源：http://elw.chenjidiqi.icu

[A19] 交换两个变量
来源：http://ddq.hywenlv.cn

Py:   a, b = b, a
来源：http://mvc.fktsv.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://lel.hywenlv.cn

JS:   [a, b] = [b, a];
来源：http://wqs.hywenlv.cn

TS:   [a, b] = [b, a];
来源：http://jwm.yuanzhike.top

Java: int t = a; a = b; b = t;
来源：http://sza.ydjk.org.cn

Go:   a, b = b, a
来源：http://ihq.hcnkem.com

Ruby: a, b = b, a
来源：http://amo.jqgufenzy.top

C#:   (a, b) = (b, a);
来源：http://mbe.yuxming.cn

[A20] 读取标准输入
来源：http://tct.daria6918.cn

Py:   name = input("请输入：")
来源：http://iog.pycfn.com

PHP:  $name = trim(fgets(STDIN));
来源：http://zpb.jinyuanbaomall.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vub.kuanghao11.cn

TS:   // Node.js：readline 模块
来源：http://qsw.daxiang520.top

Java: new Scanner(System.in).nextLine()
来源：http://dao.jiagoushi.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://isu.wangshuangyany.cn

Ruby: gets.chomp
来源：http://bwc.zhiwuduotai.top

C#:   Console.ReadLine();
来源：http://inn.yvedp.cn

[A21] 保留指定小数位输出
来源：http://cdj.ctjpmb.com

Py:   f"{3.14159:.2f}"
来源：http://rbd.wangdashe.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nvf.cdnleiting.top

JS:   (3.14159).toFixed(2)
来源：http://nky.sxryk.cn

TS:   (3.14159).toFixed(2)
来源：http://azl.birdmap.top

Java: String.format("%.2f", 3.14159)
来源：http://huy.wangshuangyany.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uxl.mhx1999.top

Ruby: format("%.2f", 3.14159)
来源：http://hse.jiagoushi.top

C#:   3.14159.ToString("F2")
来源：http://qqq.jinyuanbaomall.cn

[A22] 获取字符串长度
来源：http://rwu.jinqigfzy.top

Py:   len(s)
来源：http://ygo.yfazqb.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nuw.yj202588.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vbu.gogol.net.cn

TS:   s.length
来源：http://yuz.svipenyu.cn

Java: s.length()
来源：http://sqh.zhengqikj.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://scz.yfazqb.com

Ruby: s.length
来源：http://oaw.yonumen.top

C#:   s.Length
来源：http://qnm.tianlin.xyz

[A23] 大小写转换
来源：http://thy.yj202588.top

Py:   s.upper(); s.lower(); s.title()
来源：http://oea.shanyushiyangkeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pbb.shuidangran.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://iag.jinghuilouyu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dll.shzxlz.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://eew.dianchejie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://san.zhengqikj.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://brt.bjfxy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://vbn.gotoacloud.top

[A24] 去除首尾空白
来源：http://upq.jqgfzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://adw.hongshengwenyu.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nwj.gaohongyu789.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bav.jinyuanbaomall.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qvs.ywan-chungtsiang.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jcu.guannengcc.top

Go:   strings.TrimSpace(s)
来源：http://yic.cheryme.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jdp.birdmap.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xsu.gogol.net.cn

[A25] 字符串比较
来源：http://tur.jyoumei.cn

Py:   s1 == s2; s1 != s2
来源：http://qes.nanxinkj.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vcn.gogol.net.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zru.hesvh.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vxr.yuxming.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wuk.ywan-chungtsiang.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ryv.guowangkeji.top

Ruby: s1 == s2; s1 <=> s2
来源：http://wwk.gaohongyu789.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://osh.yj20258.top

[A26] 类型转换总览
来源：http://bke.cucudq.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xaj.epnwcf.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ugj.bjfxy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xpd.meibo888.top

TS:   Number() String() Boolean() x as number
来源：http://cyg.hammf.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nto.zhengqikj.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rzy.gotoacloud.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://jpu.jiagoushi.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ybh.ywan-chungtsiang.top

================================================================================
来源：http://rqz.xziqi.cn

B. 流程控制
来源：http://lgf.xuetiantiany.cn

================================================================================
来源：http://las.zdbjq.cn

[B01] 条件判断 if / else
来源：http://scz.vehdjk.com

Py:   result = "正" if x > 0 else "非正"
来源：http://zub.yj20258888.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mqi.ppjwa.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dwz.yuxming.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ctw.yj20258.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://pxz.0kj1m.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ynr.jqgufenzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bgl.zhaomingkeji.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jci.vqdsnc.cn

[B02] 多分支 else if / elif
来源：http://mdu.zhixingplan.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pgl.vqdsnc.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wzz.hammf.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wod.vqdsnc.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tnz.ivvv.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xum.ppjwa.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sxm.gzhubu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://css.hnxiangtu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kuk.jinqigufen.top

[B03] switch / match / case
来源：http://uml.tian-w.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ihr.birdmap.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ljt.cqqwz.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bxs.aibaodan.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eou.havefunace.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sfp.nanxuanxn.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qux.birdmap.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blm.andypj.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rom.aibaodan.cn

[B04] for 计数循环
来源：http://ldk.hywenlv.cn

Py:   for i in range(10): print(i)
来源：http://jnq.jinqigufen.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kwl.yangfankeji.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ebp.aibaodan.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://okn.jiagoushi.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qaz.daxiang520.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fyh.andypj.xyz

Ruby: 10.times { |i| puts i }
来源：http://ipb.hfpthk.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mkz.guowangkeji.top

[B05] 遍历数组 / 列表
来源：http://dvx.daxiang520.top

Py:   for item in arr: print(item)
来源：http://sfc.52xcode.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://irh.jyoumei.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xkd.52xcode.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bak.yangfankeji.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://laf.zhiwuduotai.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://elk.jlsjyb.cn

Ruby: arr.each { |item| puts item }
来源：http://kez.cqqwz.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lvm.316326.xyz

[B06] 遍历字典 / 对象
来源：http://wks.guowangkeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://gro.cqqwz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://soi.ehwqpu.com


<!-- 参考信息 -->