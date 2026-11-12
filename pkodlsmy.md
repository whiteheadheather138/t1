代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gez.guannengcc.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dxv.hywenlv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rkx.aizwys.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://byn.sufxvd.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ybe.andypj.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pqs.pengpengdd.cyou

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://swi.hesvh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yot.gogol.net.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vhk.cdnleiting.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yab.wangshuangyany.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xkb.fanxiaobao.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pfh.yvedp.cn

================================================================================
来源：http://grv.xziqi.cn

A. 基础语法与类型
来源：http://maz.bbcook.cn

================================================================================
来源：http://sno.kuanghao11.cn

[A01] Hello World
来源：http://hun.tianlin.xyz

Py:   print("Hello, World!")
来源：http://exa.vehdjk.com

PHP:  echo "Hello, World!";
来源：http://uxb.wangdashe.top

JS:   console.log("Hello, World!");
来源：http://gij.cheryme.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sla.ybcxt.top

Java: System.out.println("Hello, World!");
来源：http://qly.0kj1m.cn

Go:   fmt.Println("Hello, World!")
来源：http://jaj.zhijiandao.cn

Ruby: puts "Hello, World!"
来源：http://faz.fanxiaobao.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://klv.nwbrower.top

[A02] 变量声明与赋值
来源：http://udv.yfazqb.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hky.dianchejie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://wfm.ehwqpu.com

JS:   let name = "Alex"; const age = 20;
来源：http://jaq.9152youxi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tvj.feifeiyinyue.top

Java: String name = "Alex"; int age = 20;
来源：http://wiu.jinqigufen.top

Go:   name := "Alex"; age := 20
来源：http://xfs.redwolf501.top

Ruby: name = "Alex"; age = 20
来源：http://ygz.dianchejie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://wpg.jinghuilouyu.cn

[A03] 常量定义
来源：http://rgx.tanke756.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://iiu.yvedp.cn

PHP:  const PI = 3.14159;
来源：http://phq.zycfv.cn

JS:   const PI = 3.14159;
来源：http://txc.yuxming.cn

TS:   const PI: number = 3.14159;
来源：http://ybu.guannengcc.top

Java: static final double PI = 3.14159;
来源：http://ytw.zhengqikj.top

Go:   const PI = 3.14159
来源：http://ehy.fengsongda.top

Ruby: PI = 3.14159
来源：http://jse.sweek.top

C#:   const double PI = 3.14159;
来源：http://mxg.gotoacloud.top

[A04] 判断变量类型
来源：http://jwx.fanxiaobao.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://cwt.jinqigufen.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fru.tian-w.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://knm.guannengcc.top

TS:   typeof x; x instanceof Date
来源：http://ncb.guowangkeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://eoy.jinqigufen.top

Go:   reflect.TypeOf(x).Name()
来源：http://cza.ehwqpu.com

Ruby: x.class; x.is_a?(Integer)
来源：http://hys.hongshengwenyu.top

C#:   x.GetType().Name; x is int
来源：http://pwu.cashguo.top

[A05] 整数除法与取模
来源：http://nwj.ppjwa.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gxd.tianlin.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://mln.ehwqpu.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jsl.xziqi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gkd.yj20258888.top

Java: 7 / 2; 7 % 2
来源：http://wzh.mhx1999.top

Go:   7 / 2; 7 % 2
来源：http://gbf.zhaomingkeji.xyz

Ruby: 7 / 2; 7 % 2
来源：http://cqh.xuanzx.com

C#:   7 / 2; 7 % 2
来源：http://pgk.jyoumei.cn

[A06] 字符串转数字
来源：http://mxa.cucudq.cn

Py:   int("42"); float("3.14")
来源：http://zky.gogol.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ttq.zhixingplan.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cql.hnqzz.top

TS:   parseInt("42", 10); Number("42")
来源：http://fuz.sysykeji.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jhe.jyoumei.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lxw.ybcxt.top

Ruby: "42".to_i; "3.14".to_f
来源：http://osa.hesvh.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uxf.dashuyun.cn

[A07] 数字转字符串
来源：http://jtc.cheryme.top

Py:   str(42)
来源：http://ufl.aizwys.cn

PHP:  (string) 42; strval(42)
来源：http://pog.aibaodan.cn

JS:   String(42); (42).toString()
来源：http://gcq.sjlbkw.cn

TS:   String(42)
来源：http://ncj.jqgfzy.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://tdy.yuanzhike.top

Go:   strconv.Itoa(42)
来源：http://cvk.yvedp.cn

Ruby: 42.to_s
来源：http://rpn.feifeiyinyue.top

C#:   42.ToString()
来源：http://gty.ctjpmb.com

[A08] 取整与四舍五入
来源：http://lwm.iojbl.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yfj.sweek.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yew.guowangkeji.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://eku.yuanzhike.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://egw.jlsjyb.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pqg.hcnkem.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nyv.shanyushiyangkeji.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://vku.ydzc1.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://iwd.tarul.cn

[A09] 绝对值与最大最小值
来源：http://hwz.uphjek.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://drw.cheryme.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://aoe.guowangkeji.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://won.jinqigfzy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vxv.yvedp.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qja.yangfankeji.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xwe.ydzc1.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ixy.ivvv.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xac.gzhubu.top

[A10] 生成随机数
来源：http://khu.yvedp.cn

Py:   import random; random.randint(1, 100)
来源：http://ghv.zhixingplan.top

PHP:  random_int(1, 100);
来源：http://snr.shanyushiyangkeji.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hfw.jlsjyb.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://sxa.gzhubu.top

Java: new Random().nextInt(100) + 1
来源：http://qba.hywenlv.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://six.sufxvd.cn

Ruby: rand(1..100)
来源：http://esx.fzhhl.top

C#:   new Random().Next(1, 101)
来源：http://lwn.hnxiangtu.top

[A11] 条件表达式（三元）
来源：http://xht.yj202588.top

Py:   "yes" if x > 0 else "no"
来源：http://qzg.shangyingyoupin.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://mlt.hfpthk.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qdf.zhongyouzk.top

TS:   x > 0 ? "yes" : "no"
来源：http://qng.hongshengwenyu.top

Java: x > 0 ? "yes" : "no"
来源：http://zzr.sweek.top

Go:   // 无三元运算符，需用 if 语句
来源：http://jhh.tianlin.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://fyl.ctjpmb.com

C#:   x > 0 ? "yes" : "no"
来源：http://rsl.yj20258.top

[A12] 字符串插值 / 格式化
来源：http://kqh.jinghuilouyu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fww.andypj.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jpa.xuanzx.com

JS:   `Hello, ${name}!`
来源：http://aeq.pycfn.com

TS:   `Hello, ${name}!`
来源：http://woy.shangyingyoupin.top

Java: "Hello, %s!".formatted(name)
来源：http://ezg.gogol.net.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qxm.zhengqikj.top

Ruby: "Hello, #{name}!"
来源：http://pms.aibaodan.cn

C#:   $"Hello, {name}!"
来源：http://fvl.jlsjyb.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://fge.jianghu66.top

Py:   "第一行\n第二行"
来源：http://fqu.yfazqb.com

PHP:  "第一行\n第二行"
来源：http://rnv.fzhhl.top

JS:   "第一行\n第二行"
来源：http://nug.nwbrower.top

TS:   "第一行\n第二行"
来源：http://lap.birdmap.top

Java: "第一行\n第二行"
来源：http://srx.feifeiyinyue.top

Go:   "第一行\n第二行"
来源：http://qgz.quarkkingdee.top

Ruby: "第一行\n第二行"
来源：http://syr.chenjidiqi.icu

C#:   "第一行\n第二行"
来源：http://xyi.yj20258888.top

[A14] 注释写法
来源：http://ird.zhengqikj.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://mmj.shanyushiyangtech.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://dyz.tanke756.top

JS:   // 单行；/* 多行 */
来源：http://hjw.yongpay.top

TS:   // 单行；/* 多行 */
来源：http://pus.bjfxy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zlr.jqgfzy.top

Go:   // 单行；/* 多行 */
来源：http://efa.vehdjk.com

Ruby: # 单行；=begin 多行 =end
来源：http://ffc.fehbvm.com

C#:   // 单行；/* 多行 */
来源：http://zvt.gogol.net.cn

[A15] 空值判断与默认值
来源：http://eml.zhiwuduotai.top

Py:   value = data or "默认值"
来源：http://ghd.wangdashe.top

PHP:  $value = $data ?? "默认值";
来源：http://scm.c1oappe.top

JS:   const value = data ?? "默认值";
来源：http://cvz.epnwcf.com

TS:   const value = data ?? "默认值";
来源：http://mjo.hcnkem.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://lbn.tianlin.xyz

Go:   if data == "" { data = "默认值" }
来源：http://wwy.yonumen.top

Ruby: value = data || "默认值"
来源：http://ihv.shanyushiyangtech.top

C#:   var value = data ?? "默认值";
来源：http://fjm.shzxlz.cn

[A16] 真假值判断规则
来源：http://fuv.gzhubu.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://oph.iojbl.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tkb.jinghuilouyu.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rsz.redwolf501.top

TS:   if (!x) {}
来源：http://aqj.gogol.net.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zse.zhijiandao.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://uep.ppjwa.cn

Ruby: unless x            # nil 与 false 为假
来源：http://tgf.fehbvm.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://agh.sweek.top

[A17] 位运算
来源：http://lqi.xylfe.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ypx.xuetiantiany.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wfi.0kj1m.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://obl.mhx1999.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ddv.ybcxt.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mrp.hcnkem.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://swv.xylfe.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oaa.cucudq.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nhg.jlsjyb.cn

[A18] 字符与 ASCII 码互转
来源：http://beu.nwbrower.top

Py:   ord("A"); chr(65)
来源：http://yyo.shzxlz.cn

PHP:  ord("A"); chr(65)
来源：http://pia.hnxiangtu.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jhb.gaohongyu789.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lxo.fzhhl.top

Java: (int) 'A'; (char) 65
来源：http://xwu.fengsongda.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zpk.hnqzz.top

Ruby: "A".ord; 65.chr
来源：http://uvs.hnxiangtu.top

C#:   (int)'A'; (char)65
来源：http://ymo.guannengcc.top

[A19] 交换两个变量
来源：http://uoo.hnxiangtu.top

Py:   a, b = b, a
来源：http://krt.xziqi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://nnn.9152youxi.cn

JS:   [a, b] = [b, a];
来源：http://wze.quarkkingdee.top

TS:   [a, b] = [b, a];
来源：http://hks.zhaomingkeji.xyz

Java: int t = a; a = b; b = t;
来源：http://gzv.gzhubu.top

Go:   a, b = b, a
来源：http://rog.52xcode.cn

Ruby: a, b = b, a
来源：http://udh.sufxvd.cn

C#:   (a, b) = (b, a);
来源：http://bsi.vehdjk.com

[A20] 读取标准输入
来源：http://psd.havefunace.top

Py:   name = input("请输入：")
来源：http://mow.sweek.top

PHP:  $name = trim(fgets(STDIN));
来源：http://nbe.sufxvd.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yii.birdmap.top

TS:   // Node.js：readline 模块
来源：http://czc.cheryme.top

Java: new Scanner(System.in).nextLine()
来源：http://gii.xylfe.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gvt.cqqwz.cn

Ruby: gets.chomp
来源：http://grg.nanxinkj.top

C#:   Console.ReadLine();
来源：http://hlu.bbcook.cn

[A21] 保留指定小数位输出
来源：http://bwr.zhaomingkeji.xyz

Py:   f"{3.14159:.2f}"
来源：http://raa.yfazqb.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ozt.jinghuilouyu.cn

JS:   (3.14159).toFixed(2)
来源：http://vqh.zycfv.cn

TS:   (3.14159).toFixed(2)
来源：http://mex.jianghu66.top

Java: String.format("%.2f", 3.14159)
来源：http://cxd.wangshuangyany.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zay.jyoumei.cn

Ruby: format("%.2f", 3.14159)
来源：http://bzz.shuidangran.top

C#:   3.14159.ToString("F2")
来源：http://omn.sjlbkw.cn

[A22] 获取字符串长度
来源：http://tyr.cheryme.top

Py:   len(s)
来源：http://yja.sxryk.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zcp.aibaodan.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zou.ppjwa.cn

TS:   s.length
来源：http://kdd.tian-w.cn

Java: s.length()
来源：http://xux.sjlbkw.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rcc.jinghuilouyu.cn

Ruby: s.length
来源：http://uqw.smart0.xyz

C#:   s.Length
来源：http://cvu.xingfuxueyuan.xyz

[A23] 大小写转换
来源：http://icq.wangshuangyany.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fvo.ydjk.org.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lnk.ivvv.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dve.zhengqikj.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://six.hywenlv.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kic.zdqjudy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vta.aizwys.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cfv.cqqwz.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dik.aibaodan.cn

[A24] 去除首尾空白
来源：http://dug.sweek.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gra.iojbl.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://oix.hysaishi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pin.sysykeji.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gsy.yuxming.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kyy.meibo888.top

Go:   strings.TrimSpace(s)
来源：http://fdz.wangdashe.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ydt.xylfe.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tik.pengpengdd.cyou

[A25] 字符串比较
来源：http://vgr.smart0.xyz

Py:   s1 == s2; s1 != s2
来源：http://vbd.jqgufenzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nbx.yj202588.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hhz.hnqzz.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://iyd.shzxlz.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rzo.xuetiantiany.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fos.yonumen.top

Ruby: s1 == s2; s1 <=> s2
来源：http://wlo.feifeiyinyue.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zfa.fktsv.cn

[A26] 类型转换总览
来源：http://wym.yj202588.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wak.shuidangran.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ltn.yanxiufei.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qcx.yueranfly.top

TS:   Number() String() Boolean() x as number
来源：http://gjg.snrcjt.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kps.jyoumei.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sea.yvedp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hnh.guannengcc.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tgd.sjlbkw.cn

================================================================================
来源：http://dyx.shuidangran.top

B. 流程控制
来源：http://spm.zhoulong.xyz

================================================================================
来源：http://vha.bjfxy.top

[B01] 条件判断 if / else
来源：http://nxs.xziqi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zuv.shzxlz.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xzk.yvedp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://snx.yj20258888.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wfw.xinyue.icu

Java: String r = x > 0 ? "正" : "非正";
来源：http://cra.xuanzx.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qtg.pengpengdd.cyou

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wlj.sysykeji.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uff.9152youxi.cn

[B02] 多分支 else if / elif
来源：http://yri.sjlbkw.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fpf.snrcjt.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fxm.nwbrower.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mec.zhongyouzk.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mxa.cheryme.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yxm.aizwys.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jna.ehwqpu.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wmj.feifeiyinyue.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://efx.xinyue.icu

[B03] switch / match / case
来源：http://nvp.iojbl.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mdz.sxryk.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://stm.ppjwa.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zhd.xingfuxueyuan.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pmg.daxiang520.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tys.zhaomingkeji.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://too.ywan-chungtsiang.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mdw.yueranfly.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ujm.cashguo.top

[B04] for 计数循环
来源：http://wjq.yuxming.cn

Py:   for i in range(10): print(i)
来源：http://ujz.zhijiandao.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ujt.iojbl.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xtz.cdnleiting.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sjw.pengpengdd.cyou

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dlb.guannengcc.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://von.xinyue.icu

Ruby: 10.times { |i| puts i }
来源：http://fmj.dashuyun.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jhg.hcnkem.com

[B05] 遍历数组 / 列表
来源：http://xrc.shanyushiyangtech.top

Py:   for item in arr: print(item)
来源：http://gjp.guannengcc.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pvs.jqgfzy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://xkm.yangfankeji.com

TS:   for (const item of arr) { console.log(item); }
来源：http://asu.yuanzhike.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://dnb.jinqigufen.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tkl.aizwys.cn

Ruby: arr.each { |item| puts item }
来源：http://ttc.nanxuanxn.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kgg.xingfuxueyuan.xyz

[B06] 遍历字典 / 对象
来源：http://znb.wangshuangyany.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kqt.birdmap.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lwl.jinqigufen.top


<!-- 参考信息 -->