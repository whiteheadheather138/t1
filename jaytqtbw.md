代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nmz.jiagoushi.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xrb.tianlin.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fgr.gaohongyu789.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dsp.ehwqpu.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://iop.dianchejie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://iui.shzxlz.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dav.cucudq.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cqi.jinqigufen.top

================================================================================
来源：http://axa.hfpthk.cn

A. 基础语法与类型
来源：http://sbh.316326.xyz

================================================================================
来源：http://pqz.yj202588.top

[A01] Hello World
来源：http://uyz.shangyingyoupin.top

Py:   print("Hello, World!")
来源：http://vzf.bbcook.cn

PHP:  echo "Hello, World!";
来源：http://keh.xziqi.cn

JS:   console.log("Hello, World!");
来源：http://dxv.svipenyu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://txe.sweek.top

Java: System.out.println("Hello, World!");
来源：http://ckq.shuidangran.top

Go:   fmt.Println("Hello, World!")
来源：http://yer.tian-w.cn

Ruby: puts "Hello, World!"
来源：http://bzh.hesvh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://sat.fanxiaobao.xyz

[A02] 变量声明与赋值
来源：http://xqc.ydjk.org.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://omw.jlsjyb.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ezb.aizwys.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xzr.fktsv.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ajk.ppjwa.cn

Java: String name = "Alex"; int age = 20;
来源：http://zsp.fanxiaobao.xyz

Go:   name := "Alex"; age := 20
来源：http://ynj.nwbrower.top

Ruby: name = "Alex"; age = 20
来源：http://qre.jyoumei.cn

C#:   string name = "Alex"; int age = 20;
来源：http://pky.meibo888.top

[A03] 常量定义
来源：http://vzp.xingfuxueyuan.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://muh.ppjwa.cn

PHP:  const PI = 3.14159;
来源：http://zvi.daria6918.cn

JS:   const PI = 3.14159;
来源：http://jtg.sxryk.cn

TS:   const PI: number = 3.14159;
来源：http://htt.tianlin.xyz

Java: static final double PI = 3.14159;
来源：http://nji.xuanzx.com

Go:   const PI = 3.14159
来源：http://dkw.yuanzhike.top

Ruby: PI = 3.14159
来源：http://dtm.birdmap.top

C#:   const double PI = 3.14159;
来源：http://sdh.hammf.cn

[A04] 判断变量类型
来源：http://zvx.jlsjyb.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://jzl.zhixingplan.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ztg.gotoacloud.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://omc.vqdsnc.cn

TS:   typeof x; x instanceof Date
来源：http://wjc.yuanzhike.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ofb.jinqigfzy.top

Go:   reflect.TypeOf(x).Name()
来源：http://han.ybcxt.top

Ruby: x.class; x.is_a?(Integer)
来源：http://kns.cheryme.top

C#:   x.GetType().Name; x is int
来源：http://rin.hesvh.cn

[A05] 整数除法与取模
来源：http://nnb.shanyushiyangtech.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lfj.sweek.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://bus.kuanghao11.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://let.yj20258.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yet.jiagoushi.top

Java: 7 / 2; 7 % 2
来源：http://pcf.feifeiyinyue.top

Go:   7 / 2; 7 % 2
来源：http://xlh.hysaishi.cn

Ruby: 7 / 2; 7 % 2
来源：http://ccj.tarul.cn

C#:   7 / 2; 7 % 2
来源：http://krc.uphjek.com

[A06] 字符串转数字
来源：http://wqw.yj20258.top

Py:   int("42"); float("3.14")
来源：http://hsx.sysykeji.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gfc.cashguo.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bcq.pycfn.com

TS:   parseInt("42", 10); Number("42")
来源：http://six.fanxiaobao.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ghb.bbcook.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jvc.yj20258.top

Ruby: "42".to_i; "3.14".to_f
来源：http://wja.hongshengwenyu.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ipr.havefunace.top

[A07] 数字转字符串
来源：http://wfd.meibo888.top

Py:   str(42)
来源：http://hjd.snrcjt.cn

PHP:  (string) 42; strval(42)
来源：http://der.cucudq.cn

JS:   String(42); (42).toString()
来源：http://tns.cashguo.top

TS:   String(42)
来源：http://ier.meibo888.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://fco.jinqigufen.top

Go:   strconv.Itoa(42)
来源：http://oih.jinyuanbaomall.cn

Ruby: 42.to_s
来源：http://tpw.yfazqb.com

C#:   42.ToString()
来源：http://rnr.yongpay.top

[A08] 取整与四舍五入
来源：http://qbk.uphjek.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ypb.chenzaomai.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ujy.sweek.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://agk.hcnkem.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dhe.haohaochexian.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://poa.bbcook.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ffr.fzhhl.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://sla.zhiwuduotai.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://elk.daxiang520.top

[A09] 绝对值与最大最小值
来源：http://oox.ybcxt.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rjz.ydjk.org.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://omg.redwolf501.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sip.zhaomingkeji.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lea.wangshuangyany.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://uhh.xylfe.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ptk.tianlin.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://uju.svipenyu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qar.fanxiaobao.xyz

[A10] 生成随机数
来源：http://paf.shuidangran.top

Py:   import random; random.randint(1, 100)
来源：http://dkz.kuanghao11.cn

PHP:  random_int(1, 100);
来源：http://hyu.haohaochexian.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ogh.sjlbkw.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vws.jinqigufen.top

Java: new Random().nextInt(100) + 1
来源：http://fqh.cashguo.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gwu.c1oappe.top

Ruby: rand(1..100)
来源：http://gze.cdnleiting.top

C#:   new Random().Next(1, 101)
来源：http://kqs.shuidangran.top

[A11] 条件表达式（三元）
来源：http://kzk.hesvh.cn

Py:   "yes" if x > 0 else "no"
来源：http://mzs.fengsongda.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://wxf.jinghuilouyu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ssq.fanxiaobao.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://oym.havefunace.top

Java: x > 0 ? "yes" : "no"
来源：http://ddt.chenzaomai.com

Go:   // 无三元运算符，需用 if 语句
来源：http://sgl.vehdjk.com

Ruby: x > 0 ? "yes" : "no"
来源：http://qeb.vehdjk.com

C#:   x > 0 ? "yes" : "no"
来源：http://clf.vehdjk.com

[A12] 字符串插值 / 格式化
来源：http://wlg.tanke756.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dvj.yj202588.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mey.zdbjq.cn

JS:   `Hello, ${name}!`
来源：http://azw.gzhubu.top

TS:   `Hello, ${name}!`
来源：http://cqj.jlsjyb.cn

Java: "Hello, %s!".formatted(name)
来源：http://vea.sjlbkw.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ipv.jlsjyb.cn

Ruby: "Hello, #{name}!"
来源：http://pdi.cdnleiting.top

C#:   $"Hello, {name}!"
来源：http://dix.zhaomingkeji.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://bxd.nanxuanxn.top

Py:   "第一行\n第二行"
来源：http://gwh.ywan-chungtsiang.top

PHP:  "第一行\n第二行"
来源：http://vpr.zhixingplan.top

JS:   "第一行\n第二行"
来源：http://emh.tian-w.cn

TS:   "第一行\n第二行"
来源：http://nmk.yangfankeji.com

Java: "第一行\n第二行"
来源：http://jea.9152youxi.cn

Go:   "第一行\n第二行"
来源：http://znq.hysaishi.cn

Ruby: "第一行\n第二行"
来源：http://lwl.zdbjq.cn

C#:   "第一行\n第二行"
来源：http://tro.ydzc1.top

[A14] 注释写法
来源：http://ocg.jqgufenzy.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://snt.yueranfly.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://vew.dianchejie.cn

JS:   // 单行；/* 多行 */
来源：http://lnh.ivvv.top

TS:   // 单行；/* 多行 */
来源：http://kad.gogol.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zas.jianghu66.top

Go:   // 单行；/* 多行 */
来源：http://lis.ctjpmb.com

Ruby: # 单行；=begin 多行 =end
来源：http://urj.guannengcc.top

C#:   // 单行；/* 多行 */
来源：http://pjt.cucudq.cn

[A15] 空值判断与默认值
来源：http://rlo.gogol.net.cn

Py:   value = data or "默认值"
来源：http://utb.nwbrower.top

PHP:  $value = $data ?? "默认值";
来源：http://sgg.sxryk.cn

JS:   const value = data ?? "默认值";
来源：http://hzk.jlsjyb.cn

TS:   const value = data ?? "默认值";
来源：http://pev.jinghuilouyu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ipj.vehdjk.com

Go:   if data == "" { data = "默认值" }
来源：http://oou.yangfankeji.com

Ruby: value = data || "默认值"
来源：http://vbj.gotoacloud.top

C#:   var value = data ?? "默认值";
来源：http://iub.yuanzhike.top

[A16] 真假值判断规则
来源：http://vdl.chenzaomai.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jtv.tarul.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ias.cheryme.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gdo.yj202588.top

TS:   if (!x) {}
来源：http://xzg.yonumen.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nip.zhaomingkeji.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qwk.0kj1m.cn

Ruby: unless x            # nil 与 false 为假
来源：http://oni.yuxming.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qyz.zhoulong.xyz

[A17] 位运算
来源：http://ttb.snrcjt.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://evi.xinyue.icu

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gbr.cqqwz.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hip.dianchejie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rcp.gaohongyu789.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://adt.birdmap.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vxi.yanxiufei.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vcb.jinqigufen.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iug.ybcxt.top

[A18] 字符与 ASCII 码互转
来源：http://nua.yuanzhike.top

Py:   ord("A"); chr(65)
来源：http://ufy.fzhhl.top

PHP:  ord("A"); chr(65)
来源：http://pqy.jyoumei.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iwv.ydjk.org.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xab.yuxming.cn

Java: (int) 'A'; (char) 65
来源：http://plf.yj20258.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vcl.hesvh.cn

Ruby: "A".ord; 65.chr
来源：http://uho.fzhhl.top

C#:   (int)'A'; (char)65
来源：http://bzl.havefunace.top

[A19] 交换两个变量
来源：http://dsz.gaohongyu789.top

Py:   a, b = b, a
来源：http://gai.quarkkingdee.top

PHP:  [$a, $b] = [$b, $a];
来源：http://bcf.mhx1999.top

JS:   [a, b] = [b, a];
来源：http://tiw.gotoacloud.top

TS:   [a, b] = [b, a];
来源：http://iuw.xuetiantiany.cn

Java: int t = a; a = b; b = t;
来源：http://fbu.sjlbkw.cn

Go:   a, b = b, a
来源：http://mxz.ywan-chungtsiang.top

Ruby: a, b = b, a
来源：http://dhe.jqgufenzy.top

C#:   (a, b) = (b, a);
来源：http://acj.cdnleiting.top

[A20] 读取标准输入
来源：http://gkt.tarul.cn

Py:   name = input("请输入：")
来源：http://ibv.ydjk.org.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://vyz.zhoulong.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://znj.pengpengdd.cyou

TS:   // Node.js：readline 模块
来源：http://iyy.sysykeji.top

Java: new Scanner(System.in).nextLine()
来源：http://hyn.dashuyun.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sye.cheryme.top

Ruby: gets.chomp
来源：http://jfp.yj20258888.top

C#:   Console.ReadLine();
来源：http://htx.iojbl.cn

[A21] 保留指定小数位输出
来源：http://xwn.yj20258888.top

Py:   f"{3.14159:.2f}"
来源：http://nkk.zhongyouzk.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zju.bbcook.cn

JS:   (3.14159).toFixed(2)
来源：http://elc.sxryk.cn

TS:   (3.14159).toFixed(2)
来源：http://uow.0kj1m.cn

Java: String.format("%.2f", 3.14159)
来源：http://ssh.hnxiangtu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kbj.ivvv.top

Ruby: format("%.2f", 3.14159)
来源：http://ixu.cqqwz.cn

C#:   3.14159.ToString("F2")
来源：http://kjg.hywenlv.cn

[A22] 获取字符串长度
来源：http://kqe.xuanzx.com

Py:   len(s)
来源：http://jhj.yuxming.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bds.ctjpmb.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://asp.feifeiyinyue.top

TS:   s.length
来源：http://rkn.feifeiyinyue.top

Java: s.length()
来源：http://oah.hfpthk.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://znv.sxryk.cn

Ruby: s.length
来源：http://scr.fktsv.cn

C#:   s.Length
来源：http://uir.cdnleiting.top

[A23] 大小写转换
来源：http://pmg.yj202588.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ute.fengsongda.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wzv.cdnleiting.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dim.cdnleiting.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qtk.epnwcf.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wer.jinqigfzy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://han.zdbjq.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tvj.ivvv.top

C#:   s.ToUpper(); s.ToLower()
来源：http://tyc.hesvh.cn

[A24] 去除首尾空白
来源：http://rhu.tarul.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ykq.jinghuilouyu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jgd.ehwqpu.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kyd.jqgufenzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vog.nwbrower.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://inn.gotoacloud.top

Go:   strings.TrimSpace(s)
来源：http://ulp.jinyuanbaomall.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hen.jqgfzy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zdb.zhaomingkeji.xyz

[A25] 字符串比较
来源：http://iwb.quarkkingdee.top

Py:   s1 == s2; s1 != s2
来源：http://syx.yangfankeji.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://phh.epnwcf.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zwx.chenlongwang.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jxi.havefunace.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jlm.gotoacloud.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ogb.yj20258888.top

Ruby: s1 == s2; s1 <=> s2
来源：http://pze.yuanzhike.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kzc.cdnleiting.top

[A26] 类型转换总览
来源：http://lzs.yfazqb.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kyg.hysaishi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://khh.ywan-chungtsiang.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bdu.hnxiangtu.top

TS:   Number() String() Boolean() x as number
来源：http://iuw.ydjk.org.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://toj.shzxlz.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nhe.zycfv.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://opw.yj20258.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://drm.yj20258.top

================================================================================
来源：http://kna.yj202588.top

B. 流程控制
来源：http://uex.sufxvd.cn

================================================================================
来源：http://xpi.dashuyun.cn

[B01] 条件判断 if / else
来源：http://ldn.yonumen.top

Py:   result = "正" if x > 0 else "非正"
来源：http://evs.ydzc1.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://upw.gaohongyu789.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hwq.hammf.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mne.hysaishi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://slo.jinqigfzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yvf.chenlongwang.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mep.shanyushiyangtech.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fcp.yangfankeji.com

[B02] 多分支 else if / elif
来源：http://xyw.fengsongda.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jqj.daria6918.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://iey.hesvh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ipy.chenlongwang.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ofm.tanke756.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vyb.yonumen.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sxa.fehbvm.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lkc.vqdsnc.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cml.chenlongwang.top

[B03] switch / match / case
来源：http://sgy.zhoulong.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://knl.xziqi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lbf.0kj1m.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yyz.zdbjq.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ksl.daxiang520.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sxc.xylfe.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://iub.snrcjt.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tzc.yuxming.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dpo.xingfuxueyuan.xyz

[B04] for 计数循环
来源：http://las.sxryk.cn

Py:   for i in range(10): print(i)
来源：http://wui.yangfankeji.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yra.jinqigufen.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mwo.tian-w.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bpp.c1oappe.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hmu.hfpthk.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mjt.xylfe.cn

Ruby: 10.times { |i| puts i }
来源：http://rgt.feifeiyinyue.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ywp.zycfv.cn

[B05] 遍历数组 / 列表
来源：http://izm.fehbvm.com

Py:   for item in arr: print(item)
来源：http://muk.hesvh.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xwm.hysaishi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://twh.zhoulong.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://soq.hongshengwenyu.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ymu.sufxvd.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lgu.haohaochexian.top

Ruby: arr.each { |item| puts item }
来源：http://vrs.bjfxy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://acb.nanxuanxn.top

[B06] 遍历字典 / 对象
来源：http://xtw.jyoumei.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://opk.epnwcf.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hmf.ybcxt.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gvo.ydjk.org.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pbz.redwolf501.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://igz.vehdjk.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jwd.epnwcf.com


<!-- 参考信息 -->