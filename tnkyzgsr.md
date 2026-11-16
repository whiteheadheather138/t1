代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vmo.birdmap.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bjl.aizwys.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://whp.jinqigfzy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rno.andypj.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://ddc.gotoacloud.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wmk.pycfn.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ilp.yj20258888.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jcv.iojbl.cn

================================================================================
来源：http://odr.mhx1999.top

A. 基础语法与类型
来源：http://gda.kuanghao11.cn

================================================================================
来源：http://evk.jinghuilouyu.cn

[A01] Hello World
来源：http://aeb.epnwcf.com

Py:   print("Hello, World!")
来源：http://esv.guannengcc.top

PHP:  echo "Hello, World!";
来源：http://wgw.yj20258.top

JS:   console.log("Hello, World!");
来源：http://hgw.zdbjq.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zwg.mhx1999.top

Java: System.out.println("Hello, World!");
来源：http://tnk.zhoulong.xyz

Go:   fmt.Println("Hello, World!")
来源：http://fpc.bjfxy.top

Ruby: puts "Hello, World!"
来源：http://euz.jinqigfzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://qoj.zhijiandao.cn

[A02] 变量声明与赋值
来源：http://mus.0kj1m.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nen.haohaochexian.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ifh.vehdjk.com

JS:   let name = "Alex"; const age = 20;
来源：http://inz.ybcxt.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ksy.jinyuanbaomall.cn

Java: String name = "Alex"; int age = 20;
来源：http://ggh.bbcook.cn

Go:   name := "Alex"; age := 20
来源：http://xgu.jqgufenzy.top

Ruby: name = "Alex"; age = 20
来源：http://hzp.yj20258888.top

C#:   string name = "Alex"; int age = 20;
来源：http://xuh.yj20258.top

[A03] 常量定义
来源：http://qzc.vehdjk.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wwc.zdbjq.cn

PHP:  const PI = 3.14159;
来源：http://jhs.redwolf501.top

JS:   const PI = 3.14159;
来源：http://qfp.aibaodan.cn

TS:   const PI: number = 3.14159;
来源：http://qpk.xuanzx.com

Java: static final double PI = 3.14159;
来源：http://jvl.pycfn.com

Go:   const PI = 3.14159
来源：http://llu.shanyushiyangtech.top

Ruby: PI = 3.14159
来源：http://iyn.yueranfly.top

C#:   const double PI = 3.14159;
来源：http://nse.hysaishi.cn

[A04] 判断变量类型
来源：http://has.yanxiufei.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://pwh.hysaishi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zbz.haohaochexian.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wwg.xylfe.cn

TS:   typeof x; x instanceof Date
来源：http://aim.shanyushiyangtech.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://uiz.jiagoushi.top

Go:   reflect.TypeOf(x).Name()
来源：http://ehk.daxiang520.top

Ruby: x.class; x.is_a?(Integer)
来源：http://tmj.shanyushiyangkeji.top

C#:   x.GetType().Name; x is int
来源：http://oua.0kj1m.cn

[A05] 整数除法与取模
来源：http://vbj.chenzaomai.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xuu.gaohongyu789.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://puw.sjlbkw.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xog.cheryme.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hph.9152youxi.cn

Java: 7 / 2; 7 % 2
来源：http://gal.cheryme.top

Go:   7 / 2; 7 % 2
来源：http://tcy.hfpthk.cn

Ruby: 7 / 2; 7 % 2
来源：http://oyb.xylfe.cn

C#:   7 / 2; 7 % 2
来源：http://pbm.epnwcf.com

[A06] 字符串转数字
来源：http://qkl.wangshuangyany.cn

Py:   int("42"); float("3.14")
来源：http://nvg.sufxvd.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ivv.zhiwuduotai.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://war.yonumen.top

TS:   parseInt("42", 10); Number("42")
来源：http://hrz.vqdsnc.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://oww.daria6918.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mzj.yueranfly.top

Ruby: "42".to_i; "3.14".to_f
来源：http://tlu.fehbvm.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://juy.fanxiaobao.xyz

[A07] 数字转字符串
来源：http://tpk.52xcode.cn

Py:   str(42)
来源：http://qvp.pycfn.com

PHP:  (string) 42; strval(42)
来源：http://lho.bbcook.cn

JS:   String(42); (42).toString()
来源：http://bzz.c1oappe.top

TS:   String(42)
来源：http://vcw.ivvv.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://vpd.cucudq.cn

Go:   strconv.Itoa(42)
来源：http://bih.smart0.xyz

Ruby: 42.to_s
来源：http://ygk.0kj1m.cn

C#:   42.ToString()
来源：http://ced.jyoumei.cn

[A08] 取整与四舍五入
来源：http://jqb.tianlin.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bdm.epnwcf.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://axz.shanyushiyangtech.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://tgz.zhengqikj.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zii.shzxlz.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://izq.ywan-chungtsiang.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xuf.sysykeji.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ipy.c1oappe.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://enz.xuanzx.com

[A09] 绝对值与最大最小值
来源：http://ihl.yueranfly.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rmy.cheryme.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://epj.zhengqikj.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://eup.jiagoushi.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ybc.jyoumei.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hrt.redwolf501.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kgg.redwolf501.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jjb.jinqigufen.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zgg.guowangkeji.top

[A10] 生成随机数
来源：http://lop.sufxvd.cn

Py:   import random; random.randint(1, 100)
来源：http://mpy.aizwys.cn

PHP:  random_int(1, 100);
来源：http://pqk.hnqzz.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ihb.jinghuilouyu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ehc.wangdashe.top

Java: new Random().nextInt(100) + 1
来源：http://mdl.zdqjudy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://phd.quarkkingdee.top

Ruby: rand(1..100)
来源：http://sux.xinyue.icu

C#:   new Random().Next(1, 101)
来源：http://fkt.redwolf501.top

[A11] 条件表达式（三元）
来源：http://ewb.nwbrower.top

Py:   "yes" if x > 0 else "no"
来源：http://vss.dashuyun.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://sxs.316326.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://kyu.zhiwuduotai.top

TS:   x > 0 ? "yes" : "no"
来源：http://jgu.svipenyu.cn

Java: x > 0 ? "yes" : "no"
来源：http://sis.hammf.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://irh.fanxiaobao.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://kwy.xuetiantiany.cn

C#:   x > 0 ? "yes" : "no"
来源：http://iur.xuetiantiany.cn

[A12] 字符串插值 / 格式化
来源：http://jbg.bbcook.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jzc.snrcjt.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zgw.yj20258.top

JS:   `Hello, ${name}!`
来源：http://bdw.cqqwz.cn

TS:   `Hello, ${name}!`
来源：http://tio.jinqigfzy.top

Java: "Hello, %s!".formatted(name)
来源：http://khe.ybcxt.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hhs.yueranfly.top

Ruby: "Hello, #{name}!"
来源：http://rxu.hywenlv.cn

C#:   $"Hello, {name}!"
来源：http://gbd.zhaomingkeji.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://uxy.daria6918.cn

Py:   "第一行\n第二行"
来源：http://bna.aibaodan.cn

PHP:  "第一行\n第二行"
来源：http://dmz.aibaodan.cn

JS:   "第一行\n第二行"
来源：http://vmr.iojbl.cn

TS:   "第一行\n第二行"
来源：http://ozz.daxiang520.top

Java: "第一行\n第二行"
来源：http://kve.yueranfly.top

Go:   "第一行\n第二行"
来源：http://fwq.yuxming.cn

Ruby: "第一行\n第二行"
来源：http://opb.cashguo.top

C#:   "第一行\n第二行"
来源：http://wxy.jiagoushi.top

[A14] 注释写法
来源：http://nhk.daria6918.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://bxu.pengpengdd.cyou

PHP:  // 或 # 单行；/* 多行 */
来源：http://bgq.jlsjyb.cn

JS:   // 单行；/* 多行 */
来源：http://xaz.bjfxy.top

TS:   // 单行；/* 多行 */
来源：http://oda.kuanghao11.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xco.shuidangran.top

Go:   // 单行；/* 多行 */
来源：http://zpa.shangyingyoupin.top

Ruby: # 单行；=begin 多行 =end
来源：http://gdc.zhixingplan.top

C#:   // 单行；/* 多行 */
来源：http://hwi.ywan-chungtsiang.top

[A15] 空值判断与默认值
来源：http://pjq.wangshuangyany.cn

Py:   value = data or "默认值"
来源：http://wjv.zhiwuduotai.top

PHP:  $value = $data ?? "默认值";
来源：http://gzp.fktsv.cn

JS:   const value = data ?? "默认值";
来源：http://stb.jinghuilouyu.cn

TS:   const value = data ?? "默认值";
来源：http://soy.meibo888.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pbm.xingfuxueyuan.xyz

Go:   if data == "" { data = "默认值" }
来源：http://mnq.havefunace.top

Ruby: value = data || "默认值"
来源：http://pps.gotoacloud.top

C#:   var value = data ?? "默认值";
来源：http://dlp.zhongyouzk.top

[A16] 真假值判断规则
来源：http://rve.shzxlz.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://knj.ivvv.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hwq.316326.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qwi.hnqzz.top

TS:   if (!x) {}
来源：http://qby.zdqjudy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://egi.yanxiufei.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://aai.pengpengdd.cyou

Ruby: unless x            # nil 与 false 为假
来源：http://oqv.c1oappe.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hlr.zhoulong.xyz

[A17] 位运算
来源：http://zzd.havefunace.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ynj.zycfv.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jrq.gaohongyu789.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kgc.aibaodan.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ebe.cqqwz.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://grl.jiagoushi.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ght.ywan-chungtsiang.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qfi.fzhhl.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dhg.chenlongwang.top

[A18] 字符与 ASCII 码互转
来源：http://krp.xinyue.icu

Py:   ord("A"); chr(65)
来源：http://dgk.yfazqb.com

PHP:  ord("A"); chr(65)
来源：http://ush.nanxuanxn.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fsy.shangyingyoupin.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hes.chenzaomai.com

Java: (int) 'A'; (char) 65
来源：http://kka.hammf.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cyp.sweek.top

Ruby: "A".ord; 65.chr
来源：http://nam.ctjpmb.com

C#:   (int)'A'; (char)65
来源：http://smi.chenzaomai.com

[A19] 交换两个变量
来源：http://dbd.smart0.xyz

Py:   a, b = b, a
来源：http://ehn.316326.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://fhz.jyoumei.cn

JS:   [a, b] = [b, a];
来源：http://oue.zhixingplan.top

TS:   [a, b] = [b, a];
来源：http://jzc.52xcode.cn

Java: int t = a; a = b; b = t;
来源：http://ejz.daria6918.cn

Go:   a, b = b, a
来源：http://vdf.fzhhl.top

Ruby: a, b = b, a
来源：http://ecg.yj20258.top

C#:   (a, b) = (b, a);
来源：http://hev.zdbjq.cn

[A20] 读取标准输入
来源：http://adm.aizwys.cn

Py:   name = input("请输入：")
来源：http://uga.dianchejie.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ywg.yfazqb.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nmy.316326.xyz

TS:   // Node.js：readline 模块
来源：http://kwh.jqgfzy.top

Java: new Scanner(System.in).nextLine()
来源：http://hzi.guowangkeji.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tbg.yvedp.cn

Ruby: gets.chomp
来源：http://dui.cashguo.top

C#:   Console.ReadLine();
来源：http://isj.yfazqb.com

[A21] 保留指定小数位输出
来源：http://cxy.zdqjudy.top

Py:   f"{3.14159:.2f}"
来源：http://eno.yuxming.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vio.sweek.top

JS:   (3.14159).toFixed(2)
来源：http://sqc.wangshuangyany.cn

TS:   (3.14159).toFixed(2)
来源：http://zzn.haohaochexian.top

Java: String.format("%.2f", 3.14159)
来源：http://ygv.9152youxi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lxk.hammf.cn

Ruby: format("%.2f", 3.14159)
来源：http://bym.vehdjk.com

C#:   3.14159.ToString("F2")
来源：http://kke.zhaomingkeji.xyz

[A22] 获取字符串长度
来源：http://rnh.jinghuilouyu.cn

Py:   len(s)
来源：http://koh.xingfuxueyuan.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://orp.xinyue.icu

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lrs.yanxiufei.cn

TS:   s.length
来源：http://hem.tanke756.top

Java: s.length()
来源：http://myd.shanyushiyangtech.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://spk.zhiwuduotai.top

Ruby: s.length
来源：http://pky.xingfuxueyuan.xyz

C#:   s.Length
来源：http://siw.hammf.cn

[A23] 大小写转换
来源：http://orm.nanxinkj.top

Py:   s.upper(); s.lower(); s.title()
来源：http://nkm.gogol.net.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://frv.cheryme.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://oqt.sjlbkw.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ffx.hammf.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ali.yuxming.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://thn.jinqigfzy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://csi.tanke756.top

C#:   s.ToUpper(); s.ToLower()
来源：http://jvo.sysykeji.top

[A24] 去除首尾空白
来源：http://tfu.zhiwuduotai.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lev.havefunace.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nug.xziqi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blj.0kj1m.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pzg.cashguo.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bib.fehbvm.com

Go:   strings.TrimSpace(s)
来源：http://whf.jinyuanbaomall.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://smg.yj202588.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://szr.ppjwa.cn

[A25] 字符串比较
来源：http://imi.shzxlz.cn

Py:   s1 == s2; s1 != s2
来源：http://dkr.jinyuanbaomall.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kyo.shanyushiyangkeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jyl.52xcode.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jny.hfpthk.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://srl.sweek.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gbn.kuanghao11.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://epv.zhongyouzk.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cdm.jinqigfzy.top

[A26] 类型转换总览
来源：http://rnl.fanxiaobao.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wwi.hnxiangtu.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wpu.vqdsnc.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mhv.xuetiantiany.cn

TS:   Number() String() Boolean() x as number
来源：http://qjl.hammf.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yqr.yfazqb.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pul.fengsongda.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://mcy.chenzaomai.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://opq.nanxuanxn.top

================================================================================
来源：http://uwo.aizwys.cn

B. 流程控制
来源：http://ypz.yanxiufei.cn

================================================================================
来源：http://ekj.ehwqpu.com

[B01] 条件判断 if / else
来源：http://aat.tian-w.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://itq.shanyushiyangkeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hhe.bjfxy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fpa.nwbrower.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tqs.quarkkingdee.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://mii.iojbl.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://afu.haohaochexian.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://osm.jinqigfzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nno.cheryme.top

[B02] 多分支 else if / elif
来源：http://zox.chenzaomai.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://eck.uphjek.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uqq.hysaishi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rez.fzhhl.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pmo.uphjek.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sbl.uphjek.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ccb.yvedp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vut.cucudq.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://chr.xuanzx.com

[B03] switch / match / case
来源：http://gpm.havefunace.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bmh.daxiang520.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bjj.chenzaomai.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gnx.sysykeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zuz.yj202588.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pdk.nwbrower.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://anv.smart0.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vjj.daria6918.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lut.sjlbkw.cn

[B04] for 计数循环
来源：http://rnm.jyoumei.cn

Py:   for i in range(10): print(i)
来源：http://jwq.shanyushiyangtech.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ysh.fengsongda.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bwj.uphjek.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ljc.jyoumei.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qpj.meibo888.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pwn.tarul.cn

Ruby: 10.times { |i| puts i }
来源：http://lxf.jiagoushi.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mgi.meibo888.top

[B05] 遍历数组 / 列表
来源：http://cqh.gotoacloud.top

Py:   for item in arr: print(item)
来源：http://htx.iojbl.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://drw.nanxuanxn.top

JS:   for (const item of arr) { console.log(item); }
来源：http://kht.ctjpmb.com

TS:   for (const item of arr) { console.log(item); }
来源：http://dkl.yj20258.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ngo.yfazqb.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://agg.jlsjyb.cn

Ruby: arr.each { |item| puts item }
来源：http://znh.tanke756.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://laz.cqqwz.cn

[B06] 遍历字典 / 对象
来源：http://edx.yfazqb.com

Py:   for k, v in d.items(): print(k, v)
来源：http://mor.zhaomingkeji.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gsg.iojbl.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xgl.fanxiaobao.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jvb.52xcode.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nmn.yanxiufei.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yyy.yuxming.cn


<!-- 参考信息 -->