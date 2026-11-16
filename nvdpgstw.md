代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rqt.tianlin.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://her.cqqwz.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yyv.pengpengdd.cyou

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yya.sweek.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://qvj.fzhhl.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bsa.jianghu66.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lse.zycfv.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://num.wangshuangyany.cn

================================================================================
来源：http://oty.zhixingplan.top

A. 基础语法与类型
来源：http://dls.bjfxy.top

================================================================================
来源：http://lab.hfpthk.cn

[A01] Hello World
来源：http://gpz.vehdjk.com

Py:   print("Hello, World!")
来源：http://bzq.52xcode.cn

PHP:  echo "Hello, World!";
来源：http://yzj.yuxming.cn

JS:   console.log("Hello, World!");
来源：http://psk.ctjpmb.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://kgw.sjlbkw.cn

Java: System.out.println("Hello, World!");
来源：http://nuw.pengpengdd.cyou

Go:   fmt.Println("Hello, World!")
来源：http://qzd.zdqjudy.top

Ruby: puts "Hello, World!"
来源：http://iub.gzhubu.top

C#:   Console.WriteLine("Hello, World!");
来源：http://jwh.chenjidiqi.icu

[A02] 变量声明与赋值
来源：http://rdc.zycfv.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vfn.jiagoushi.top

PHP:  $name = "Alex"; $age = 20;
来源：http://yje.ivvv.top

JS:   let name = "Alex"; const age = 20;
来源：http://amf.zdbjq.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ado.hnqzz.top

Java: String name = "Alex"; int age = 20;
来源：http://xaa.meibo888.top

Go:   name := "Alex"; age := 20
来源：http://teu.iojbl.cn

Ruby: name = "Alex"; age = 20
来源：http://mfr.quarkkingdee.top

C#:   string name = "Alex"; int age = 20;
来源：http://qhy.feifeiyinyue.top

[A03] 常量定义
来源：http://cit.bjfxy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tpi.andypj.xyz

PHP:  const PI = 3.14159;
来源：http://kmw.yj20258888.top

JS:   const PI = 3.14159;
来源：http://mat.daxiang520.top

TS:   const PI: number = 3.14159;
来源：http://maa.ivvv.top

Java: static final double PI = 3.14159;
来源：http://ycp.chenlongwang.top

Go:   const PI = 3.14159
来源：http://pho.ydzc1.top

Ruby: PI = 3.14159
来源：http://ulk.pycfn.com

C#:   const double PI = 3.14159;
来源：http://zpa.cqqwz.cn

[A04] 判断变量类型
来源：http://exv.316326.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://skg.sweek.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qxo.hnqzz.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qbi.c1oappe.top

TS:   typeof x; x instanceof Date
来源：http://bgt.cheryme.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xph.52xcode.cn

Go:   reflect.TypeOf(x).Name()
来源：http://cnb.hnqzz.top

Ruby: x.class; x.is_a?(Integer)
来源：http://bwp.hysaishi.cn

C#:   x.GetType().Name; x is int
来源：http://xur.wangdashe.top

[A05] 整数除法与取模
来源：http://cqm.zhiwuduotai.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gat.uphjek.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://tox.ehwqpu.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://uou.ctjpmb.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ydi.ppjwa.cn

Java: 7 / 2; 7 % 2
来源：http://bmh.chenlongwang.top

Go:   7 / 2; 7 % 2
来源：http://ngt.kuanghao11.cn

Ruby: 7 / 2; 7 % 2
来源：http://sfb.jinghuilouyu.cn

C#:   7 / 2; 7 % 2
来源：http://oqf.cheryme.top

[A06] 字符串转数字
来源：http://vwr.redwolf501.top

Py:   int("42"); float("3.14")
来源：http://yru.vqdsnc.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hvn.feifeiyinyue.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nlm.pengpengdd.cyou

TS:   parseInt("42", 10); Number("42")
来源：http://oat.guowangkeji.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://luj.aizwys.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bnq.shanyushiyangkeji.top

Ruby: "42".to_i; "3.14".to_f
来源：http://aaq.pengpengdd.cyou

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sgj.bbcook.cn

[A07] 数字转字符串
来源：http://bfh.cdnleiting.top

Py:   str(42)
来源：http://prp.zhongyouzk.top

PHP:  (string) 42; strval(42)
来源：http://yul.chenzaomai.com

JS:   String(42); (42).toString()
来源：http://hnr.hongshengwenyu.top

TS:   String(42)
来源：http://dtk.gotoacloud.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://wgj.epnwcf.com

Go:   strconv.Itoa(42)
来源：http://wnh.tanke756.top

Ruby: 42.to_s
来源：http://vzx.xziqi.cn

C#:   42.ToString()
来源：http://mzm.52xcode.cn

[A08] 取整与四舍五入
来源：http://fmg.redwolf501.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pse.chenzaomai.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fmc.hnqzz.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ekz.jiagoushi.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://asv.ivvv.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://oue.shanyushiyangtech.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rdc.gzhubu.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://kmt.yj20258888.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ejo.hammf.cn

[A09] 绝对值与最大最小值
来源：http://qrt.jyoumei.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wun.nanxuanxn.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tnf.bjfxy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gkk.havefunace.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tdv.hnqzz.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cid.yangfankeji.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://orp.cucudq.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://iju.jinyuanbaomall.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zhq.ehwqpu.com

[A10] 生成随机数
来源：http://umi.daxiang520.top

Py:   import random; random.randint(1, 100)
来源：http://ttp.ydjk.org.cn

PHP:  random_int(1, 100);
来源：http://cxd.jiagoushi.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://auq.zdqjudy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nyw.zhaomingkeji.xyz

Java: new Random().nextInt(100) + 1
来源：http://bjz.xingfuxueyuan.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bvn.sysykeji.top

Ruby: rand(1..100)
来源：http://jwn.daria6918.cn

C#:   new Random().Next(1, 101)
来源：http://hby.ydzc1.top

[A11] 条件表达式（三元）
来源：http://iwe.zdbjq.cn

Py:   "yes" if x > 0 else "no"
来源：http://rcj.fzhhl.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://yti.dianchejie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ndd.gogol.net.cn

TS:   x > 0 ? "yes" : "no"
来源：http://kpg.zdqjudy.top

Java: x > 0 ? "yes" : "no"
来源：http://grt.sxryk.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ubq.vehdjk.com

Ruby: x > 0 ? "yes" : "no"
来源：http://gkz.zycfv.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fyt.feifeiyinyue.top

[A12] 字符串插值 / 格式化
来源：http://gdi.cucudq.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tsg.yj202588.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bqc.zhaomingkeji.xyz

JS:   `Hello, ${name}!`
来源：http://hed.sufxvd.cn

TS:   `Hello, ${name}!`
来源：http://pri.shzxlz.cn

Java: "Hello, %s!".formatted(name)
来源：http://omb.zdbjq.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qwu.hysaishi.cn

Ruby: "Hello, #{name}!"
来源：http://wnj.yfazqb.com

C#:   $"Hello, {name}!"
来源：http://wfw.hysaishi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://qka.meibo888.top

Py:   "第一行\n第二行"
来源：http://vqf.tian-w.cn

PHP:  "第一行\n第二行"
来源：http://frv.epnwcf.com

JS:   "第一行\n第二行"
来源：http://fmd.zhengqikj.top

TS:   "第一行\n第二行"
来源：http://gml.316326.xyz

Java: "第一行\n第二行"
来源：http://axb.ywan-chungtsiang.top

Go:   "第一行\n第二行"
来源：http://gbq.redwolf501.top

Ruby: "第一行\n第二行"
来源：http://yps.jlsjyb.cn

C#:   "第一行\n第二行"
来源：http://xxw.hesvh.cn

[A14] 注释写法
来源：http://xuq.kuanghao11.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://aih.gogol.net.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vsp.yueranfly.top

JS:   // 单行；/* 多行 */
来源：http://tyn.zycfv.cn

TS:   // 单行；/* 多行 */
来源：http://dip.fanxiaobao.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xwd.yanxiufei.cn

Go:   // 单行；/* 多行 */
来源：http://gzy.hysaishi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ilu.cashguo.top

C#:   // 单行；/* 多行 */
来源：http://lou.havefunace.top

[A15] 空值判断与默认值
来源：http://bxa.yuanzhike.top

Py:   value = data or "默认值"
来源：http://hyz.smart0.xyz

PHP:  $value = $data ?? "默认值";
来源：http://joc.smart0.xyz

JS:   const value = data ?? "默认值";
来源：http://fzi.quarkkingdee.top

TS:   const value = data ?? "默认值";
来源：http://wdq.tianlin.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://led.chenjidiqi.icu

Go:   if data == "" { data = "默认值" }
来源：http://txf.chenjidiqi.icu

Ruby: value = data || "默认值"
来源：http://nat.shanyushiyangkeji.top

C#:   var value = data ?? "默认值";
来源：http://wze.aizwys.cn

[A16] 真假值判断规则
来源：http://keg.quarkkingdee.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zct.tarul.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xyv.ehwqpu.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wud.cheryme.top

TS:   if (!x) {}
来源：http://tgz.fehbvm.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rxv.jinqigufen.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://paf.meibo888.top

Ruby: unless x            # nil 与 false 为假
来源：http://jls.zdbjq.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://abd.xylfe.cn

[A17] 位运算
来源：http://gcf.zdbjq.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cpu.vqdsnc.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://goe.zdbjq.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iep.guannengcc.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hem.aizwys.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ixo.feifeiyinyue.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jdn.jinyuanbaomall.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eln.gaohongyu789.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nrn.jqgufenzy.top

[A18] 字符与 ASCII 码互转
来源：http://hsi.iojbl.cn

Py:   ord("A"); chr(65)
来源：http://jef.jinqigfzy.top

PHP:  ord("A"); chr(65)
来源：http://vwq.jinyuanbaomall.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cdj.epnwcf.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ejo.aibaodan.cn

Java: (int) 'A'; (char) 65
来源：http://vdt.pengpengdd.cyou

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vno.bbcook.cn

Ruby: "A".ord; 65.chr
来源：http://yvh.ydjk.org.cn

C#:   (int)'A'; (char)65
来源：http://orj.hnxiangtu.top

[A19] 交换两个变量
来源：http://xcn.xinyue.icu

Py:   a, b = b, a
来源：http://ppe.snrcjt.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://cnw.jianghu66.top

JS:   [a, b] = [b, a];
来源：http://tcz.mhx1999.top

TS:   [a, b] = [b, a];
来源：http://xwx.epnwcf.com

Java: int t = a; a = b; b = t;
来源：http://pct.zdbjq.cn

Go:   a, b = b, a
来源：http://xkp.nwbrower.top

Ruby: a, b = b, a
来源：http://iaz.shanyushiyangkeji.top

C#:   (a, b) = (b, a);
来源：http://wmp.yongpay.top

[A20] 读取标准输入
来源：http://qwb.epnwcf.com

Py:   name = input("请输入：")
来源：http://naw.jinyuanbaomall.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rkp.tarul.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wip.jqgfzy.top

TS:   // Node.js：readline 模块
来源：http://boq.jiagoushi.top

Java: new Scanner(System.in).nextLine()
来源：http://jpk.chenzaomai.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gcu.ydzc1.top

Ruby: gets.chomp
来源：http://hpt.zhiwuduotai.top

C#:   Console.ReadLine();
来源：http://pgx.jqgfzy.top

[A21] 保留指定小数位输出
来源：http://ocz.yueranfly.top

Py:   f"{3.14159:.2f}"
来源：http://kxc.shzxlz.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://caw.feifeiyinyue.top

JS:   (3.14159).toFixed(2)
来源：http://drm.quarkkingdee.top

TS:   (3.14159).toFixed(2)
来源：http://dzg.yj20258.top

Java: String.format("%.2f", 3.14159)
来源：http://tts.hfpthk.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ctr.hnxiangtu.top

Ruby: format("%.2f", 3.14159)
来源：http://uid.snrcjt.cn

C#:   3.14159.ToString("F2")
来源：http://wly.yj202588.top

[A22] 获取字符串长度
来源：http://hti.shanyushiyangtech.top

Py:   len(s)
来源：http://vcy.jianghu66.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://aoj.316326.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ljt.sufxvd.cn

TS:   s.length
来源：http://fjo.ivvv.top

Java: s.length()
来源：http://jpy.zhoulong.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gyc.bbcook.cn

Ruby: s.length
来源：http://iaw.jianghu66.top

C#:   s.Length
来源：http://iyd.fengsongda.top

[A23] 大小写转换
来源：http://hpc.vqdsnc.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://myq.uphjek.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wbd.redwolf501.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yuw.hnxiangtu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://iyy.shzxlz.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://iqb.sjlbkw.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mrx.iojbl.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://aut.sysykeji.top

C#:   s.ToUpper(); s.ToLower()
来源：http://eva.fehbvm.com

[A24] 去除首尾空白
来源：http://gwj.shangyingyoupin.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wus.hywenlv.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://puf.shangyingyoupin.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ocl.xuanzx.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://amx.ybcxt.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://azw.zdqjudy.top

Go:   strings.TrimSpace(s)
来源：http://qya.316326.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://aay.ydjk.org.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cky.sufxvd.cn

[A25] 字符串比较
来源：http://coz.ctjpmb.com

Py:   s1 == s2; s1 != s2
来源：http://mld.52xcode.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xtr.hywenlv.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bzk.chenjidiqi.icu

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cio.tanke756.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dvn.0kj1m.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wia.c1oappe.top

Ruby: s1 == s2; s1 <=> s2
来源：http://unx.9152youxi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://clk.jyoumei.cn

[A26] 类型转换总览
来源：http://jnz.yuxming.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ayg.0kj1m.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://waa.mhx1999.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kwc.zycfv.cn

TS:   Number() String() Boolean() x as number
来源：http://knz.jinyuanbaomall.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://urt.vqdsnc.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://eqa.xylfe.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mvz.zycfv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qyo.uphjek.com

================================================================================
来源：http://oyz.zhijiandao.cn

B. 流程控制
来源：http://cfn.zhixingplan.top

================================================================================
来源：http://dwx.xuanzx.com

[B01] 条件判断 if / else
来源：http://qhn.0kj1m.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://fis.zhijiandao.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rny.cheryme.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yhz.shangyingyoupin.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ydj.sjlbkw.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dix.tarul.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://see.yj20258888.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ced.shanyushiyangkeji.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xdt.yj202588.top

[B02] 多分支 else if / elif
来源：http://jal.tian-w.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://iyp.chenzaomai.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://flc.ywan-chungtsiang.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fya.yfazqb.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aau.sweek.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tbm.ehwqpu.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kfr.chenzaomai.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xhh.snrcjt.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://edr.shangyingyoupin.top

[B03] switch / match / case
来源：http://gnw.hysaishi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tqn.guannengcc.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sdu.havefunace.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://txm.guowangkeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rei.ivvv.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dtl.fzhhl.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fmv.jlsjyb.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sud.yj20258.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jeb.shanyushiyangtech.top

[B04] for 计数循环
来源：http://umg.wangdashe.top

Py:   for i in range(10): print(i)
来源：http://nyv.shangyingyoupin.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yrg.sweek.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mhh.zdqjudy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://stb.jinghuilouyu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ukl.zhiwuduotai.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fwv.haohaochexian.top

Ruby: 10.times { |i| puts i }
来源：http://jos.ybcxt.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uef.ydzc1.top

[B05] 遍历数组 / 列表
来源：http://zmq.quarkkingdee.top

Py:   for item in arr: print(item)
来源：http://lhg.0kj1m.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mlp.jinyuanbaomall.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://avu.gaohongyu789.top

TS:   for (const item of arr) { console.log(item); }
来源：http://wyd.hammf.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vwm.nwbrower.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xon.hesvh.cn

Ruby: arr.each { |item| puts item }
来源：http://igg.quarkkingdee.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cfd.yj20258.top

[B06] 遍历字典 / 对象
来源：http://zui.dashuyun.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://cfu.kuanghao11.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cfq.zhiwuduotai.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ipw.hysaishi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dxk.yangfankeji.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sxt.andypj.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://slw.kuanghao11.cn


<!-- 参考信息 -->