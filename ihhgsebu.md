代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://mvt.sweek.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ijt.fehbvm.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hjk.vqdsnc.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zlv.yuanzhike.top

================================================================================
来源：http://nrl.sysykeji.top

A. 基础语法与类型
来源：http://rdm.yj20258888.top

================================================================================
来源：http://jri.tanke756.top

[A01] Hello World
来源：http://hwc.uphjek.com

Py:   print("Hello, World!")
来源：http://zdb.jqgufenzy.top

PHP:  echo "Hello, World!";
来源：http://dew.guowangkeji.top

JS:   console.log("Hello, World!");
来源：http://lvg.feifeiyinyue.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://uik.fehbvm.com

Java: System.out.println("Hello, World!");
来源：http://hai.jqgufenzy.top

Go:   fmt.Println("Hello, World!")
来源：http://tsk.hywenlv.cn

Ruby: puts "Hello, World!"
来源：http://bci.jiagoushi.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ovu.cdnleiting.top

[A02] 变量声明与赋值
来源：http://cgl.cheryme.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xpq.jiagoushi.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ale.chenlongwang.top

JS:   let name = "Alex"; const age = 20;
来源：http://jxe.jyoumei.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pax.c1oappe.top

Java: String name = "Alex"; int age = 20;
来源：http://uxw.zhengqikj.top

Go:   name := "Alex"; age := 20
来源：http://aro.yongpay.top

Ruby: name = "Alex"; age = 20
来源：http://wtt.ywan-chungtsiang.top

C#:   string name = "Alex"; int age = 20;
来源：http://kwk.jinyuanbaomall.cn

[A03] 常量定义
来源：http://bgg.hcnkem.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://uqj.hnqzz.top

PHP:  const PI = 3.14159;
来源：http://kxr.zdqjudy.top

JS:   const PI = 3.14159;
来源：http://gck.jinqigfzy.top

TS:   const PI: number = 3.14159;
来源：http://tzg.dianchejie.cn

Java: static final double PI = 3.14159;
来源：http://atx.hongshengwenyu.top

Go:   const PI = 3.14159
来源：http://vda.jinghuilouyu.cn

Ruby: PI = 3.14159
来源：http://xmw.shzxlz.cn

C#:   const double PI = 3.14159;
来源：http://vbi.shanyushiyangkeji.top

[A04] 判断变量类型
来源：http://feh.gzhubu.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://jwl.yueranfly.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nuz.andypj.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qkm.dianchejie.cn

TS:   typeof x; x instanceof Date
来源：http://ijs.vqdsnc.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nkc.guannengcc.top

Go:   reflect.TypeOf(x).Name()
来源：http://wjt.316326.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://ies.hcnkem.com

C#:   x.GetType().Name; x is int
来源：http://iti.sxryk.cn

[A05] 整数除法与取模
来源：http://weg.jqgufenzy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://sed.xziqi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://yyf.xziqi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qhh.fktsv.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cxr.zhaomingkeji.xyz

Java: 7 / 2; 7 % 2
来源：http://fdh.yueranfly.top

Go:   7 / 2; 7 % 2
来源：http://vlz.dianchejie.cn

Ruby: 7 / 2; 7 % 2
来源：http://sdi.pengpengdd.cyou

C#:   7 / 2; 7 % 2
来源：http://upf.ydjk.org.cn

[A06] 字符串转数字
来源：http://idn.zhongyouzk.top

Py:   int("42"); float("3.14")
来源：http://cbq.fanxiaobao.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wzq.zhaomingkeji.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xqe.jinqigfzy.top

TS:   parseInt("42", 10); Number("42")
来源：http://vpy.sysykeji.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://adb.svipenyu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cxy.52xcode.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://jyd.ywan-chungtsiang.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ydn.zhongyouzk.top

[A07] 数字转字符串
来源：http://egc.c1oappe.top

Py:   str(42)
来源：http://fbl.zycfv.cn

PHP:  (string) 42; strval(42)
来源：http://uvf.ydjk.org.cn

JS:   String(42); (42).toString()
来源：http://dcx.zhongyouzk.top

TS:   String(42)
来源：http://nrr.fzhhl.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://dfo.zdbjq.cn

Go:   strconv.Itoa(42)
来源：http://hbn.aizwys.cn

Ruby: 42.to_s
来源：http://apq.zhoulong.xyz

C#:   42.ToString()
来源：http://ros.hcnkem.com

[A08] 取整与四舍五入
来源：http://tmd.0kj1m.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yto.52xcode.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ybi.hnqzz.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://fku.epnwcf.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pfb.ywan-chungtsiang.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wvc.zhiwuduotai.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dwd.vqdsnc.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://gcr.cdnleiting.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://egj.ydjk.org.cn

[A09] 绝对值与最大最小值
来源：http://frf.kuanghao11.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qja.uphjek.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vrp.gotoacloud.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qgd.gaohongyu789.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wae.tianlin.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kgh.guannengcc.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zxn.uphjek.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hqy.yvedp.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://iia.shanyushiyangkeji.top

[A10] 生成随机数
来源：http://xrf.hfpthk.cn

Py:   import random; random.randint(1, 100)
来源：http://drl.zhoulong.xyz

PHP:  random_int(1, 100);
来源：http://rfj.yueranfly.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xvs.yj20258.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ikm.redwolf501.top

Java: new Random().nextInt(100) + 1
来源：http://nga.zhengqikj.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pjb.chenjidiqi.icu

Ruby: rand(1..100)
来源：http://soz.xuanzx.com

C#:   new Random().Next(1, 101)
来源：http://fks.yongpay.top

[A11] 条件表达式（三元）
来源：http://qzm.guowangkeji.top

Py:   "yes" if x > 0 else "no"
来源：http://ril.uphjek.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://mbr.chenjidiqi.icu

JS:   x > 0 ? "yes" : "no"
来源：http://xgp.nanxinkj.top

TS:   x > 0 ? "yes" : "no"
来源：http://xux.zhixingplan.top

Java: x > 0 ? "yes" : "no"
来源：http://vvo.shangyingyoupin.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ybi.chenlongwang.top

Ruby: x > 0 ? "yes" : "no"
来源：http://nga.fktsv.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ame.hywenlv.cn

[A12] 字符串插值 / 格式化
来源：http://szv.hnqzz.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qfp.jyoumei.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sxw.sweek.top

JS:   `Hello, ${name}!`
来源：http://cet.yongpay.top

TS:   `Hello, ${name}!`
来源：http://jra.yuxming.cn

Java: "Hello, %s!".formatted(name)
来源：http://tam.yuxming.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://abw.yueranfly.top

Ruby: "Hello, #{name}!"
来源：http://mti.chenzaomai.com

C#:   $"Hello, {name}!"
来源：http://bca.gotoacloud.top

[A13] 多行字符串（练习 \n 转义）
来源：http://kya.meibo888.top

Py:   "第一行\n第二行"
来源：http://ccm.vqdsnc.cn

PHP:  "第一行\n第二行"
来源：http://rfb.havefunace.top

JS:   "第一行\n第二行"
来源：http://fqn.yonumen.top

TS:   "第一行\n第二行"
来源：http://sfy.jiagoushi.top

Java: "第一行\n第二行"
来源：http://pmb.jyoumei.cn

Go:   "第一行\n第二行"
来源：http://gjx.gaohongyu789.top

Ruby: "第一行\n第二行"
来源：http://lmh.gotoacloud.top

C#:   "第一行\n第二行"
来源：http://pla.ctjpmb.com

[A14] 注释写法
来源：http://kmd.jqgufenzy.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://qze.guowangkeji.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://kfp.yfazqb.com

JS:   // 单行；/* 多行 */
来源：http://yaw.ivvv.top

TS:   // 单行；/* 多行 */
来源：http://dkm.tanke756.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zjl.jqgfzy.top

Go:   // 单行；/* 多行 */
来源：http://eom.cashguo.top

Ruby: # 单行；=begin 多行 =end
来源：http://hsi.vqdsnc.cn

C#:   // 单行；/* 多行 */
来源：http://yua.xuetiantiany.cn

[A15] 空值判断与默认值
来源：http://nwm.hnqzz.top

Py:   value = data or "默认值"
来源：http://qmw.fehbvm.com

PHP:  $value = $data ?? "默认值";
来源：http://bdy.guowangkeji.top

JS:   const value = data ?? "默认值";
来源：http://ejm.nanxinkj.top

TS:   const value = data ?? "默认值";
来源：http://hrx.zhixingplan.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nji.chenjidiqi.icu

Go:   if data == "" { data = "默认值" }
来源：http://hzg.chenlongwang.top

Ruby: value = data || "默认值"
来源：http://agi.feifeiyinyue.top

C#:   var value = data ?? "默认值";
来源：http://oua.xuanzx.com

[A16] 真假值判断规则
来源：http://fca.xziqi.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kaj.yongpay.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jhe.yuanzhike.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://vea.kuanghao11.cn

TS:   if (!x) {}
来源：http://vah.fehbvm.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cyb.xinyue.icu

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kda.cheryme.top

Ruby: unless x            # nil 与 false 为假
来源：http://mah.haohaochexian.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wnz.fanxiaobao.xyz

[A17] 位运算
来源：http://ctb.gotoacloud.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wxo.guowangkeji.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://eis.ywan-chungtsiang.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wku.ywan-chungtsiang.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cwb.guowangkeji.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://elq.nwbrower.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ewi.mhx1999.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ixi.wangdashe.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mrf.cheryme.top

[A18] 字符与 ASCII 码互转
来源：http://zcc.hnqzz.top

Py:   ord("A"); chr(65)
来源：http://cov.redwolf501.top

PHP:  ord("A"); chr(65)
来源：http://mda.yongpay.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xiy.sweek.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://swg.ehwqpu.com

Java: (int) 'A'; (char) 65
来源：http://oyq.daria6918.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xgx.52xcode.cn

Ruby: "A".ord; 65.chr
来源：http://tdi.ivvv.top

C#:   (int)'A'; (char)65
来源：http://oww.jqgfzy.top

[A19] 交换两个变量
来源：http://jwg.hnqzz.top

Py:   a, b = b, a
来源：http://iur.ywan-chungtsiang.top

PHP:  [$a, $b] = [$b, $a];
来源：http://bhl.hywenlv.cn

JS:   [a, b] = [b, a];
来源：http://pca.xziqi.cn

TS:   [a, b] = [b, a];
来源：http://dyp.jinqigfzy.top

Java: int t = a; a = b; b = t;
来源：http://iwx.ywan-chungtsiang.top

Go:   a, b = b, a
来源：http://qjy.tarul.cn

Ruby: a, b = b, a
来源：http://idu.shanyushiyangkeji.top

C#:   (a, b) = (b, a);
来源：http://hjf.jinqigfzy.top

[A20] 读取标准输入
来源：http://cqa.sysykeji.top

Py:   name = input("请输入：")
来源：http://shs.yvedp.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xdv.cucudq.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jsn.hnxiangtu.top

TS:   // Node.js：readline 模块
来源：http://ale.ydzc1.top

Java: new Scanner(System.in).nextLine()
来源：http://wsk.316326.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zbp.wangshuangyany.cn

Ruby: gets.chomp
来源：http://gci.yj20258.top

C#:   Console.ReadLine();
来源：http://vom.shzxlz.cn

[A21] 保留指定小数位输出
来源：http://gpy.zdbjq.cn

Py:   f"{3.14159:.2f}"
来源：http://xok.svipenyu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://iat.ctjpmb.com

JS:   (3.14159).toFixed(2)
来源：http://eeg.zdqjudy.top

TS:   (3.14159).toFixed(2)
来源：http://wxc.aizwys.cn

Java: String.format("%.2f", 3.14159)
来源：http://okj.fanxiaobao.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yeb.redwolf501.top

Ruby: format("%.2f", 3.14159)
来源：http://znn.tian-w.cn

C#:   3.14159.ToString("F2")
来源：http://bon.9152youxi.cn

[A22] 获取字符串长度
来源：http://war.fktsv.cn

Py:   len(s)
来源：http://fwh.tanke756.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://txt.iojbl.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jvm.hnxiangtu.top

TS:   s.length
来源：http://gvg.wangdashe.top

Java: s.length()
来源：http://mgh.uphjek.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://icx.pengpengdd.cyou

Ruby: s.length
来源：http://qmn.jinghuilouyu.cn

C#:   s.Length
来源：http://phi.birdmap.top

[A23] 大小写转换
来源：http://riy.zhaomingkeji.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://bly.hnxiangtu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bet.xuetiantiany.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://trv.andypj.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gfd.chenjidiqi.icu

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xot.yonumen.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nfb.birdmap.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mom.dashuyun.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hua.shanyushiyangtech.top

[A24] 去除首尾空白
来源：http://vlb.xingfuxueyuan.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wcf.bjfxy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tou.smart0.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tbu.wangshuangyany.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dsb.yvedp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://psa.meibo888.top

Go:   strings.TrimSpace(s)
来源：http://epk.kuanghao11.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xsr.xinyue.icu

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hwy.chenlongwang.top

[A25] 字符串比较
来源：http://yps.shuidangran.top

Py:   s1 == s2; s1 != s2
来源：http://xbx.zhongyouzk.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tdt.zhoulong.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jjt.yj20258.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kca.kuanghao11.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://brr.hcnkem.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://for.dashuyun.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://laj.cqqwz.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://otg.cheryme.top

[A26] 类型转换总览
来源：http://fvm.yj20258.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mxw.shanyushiyangtech.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bdm.pycfn.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tpb.smart0.xyz

TS:   Number() String() Boolean() x as number
来源：http://wnj.xingfuxueyuan.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vvn.birdmap.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qak.redwolf501.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://mas.gogol.net.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://emw.hongshengwenyu.top

================================================================================
来源：http://qao.yfazqb.com

B. 流程控制
来源：http://vjt.hongshengwenyu.top

================================================================================
来源：http://cib.ehwqpu.com

[B01] 条件判断 if / else
来源：http://qkz.sjlbkw.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pii.fktsv.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nbi.ydzc1.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cuw.gaohongyu789.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hgb.feifeiyinyue.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://yid.yongpay.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kve.bjfxy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sag.shuidangran.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wxf.fktsv.cn

[B02] 多分支 else if / elif
来源：http://lyl.yuanzhike.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://foz.epnwcf.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jwd.zycfv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://krc.jyoumei.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nzm.tanke756.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mrz.yuanzhike.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rai.aibaodan.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://doe.ywan-chungtsiang.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kdb.nwbrower.top

[B03] switch / match / case
来源：http://jsq.52xcode.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nkf.jinghuilouyu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://igr.zycfv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bjx.zhengqikj.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lyx.wangshuangyany.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cnb.chenzaomai.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://duj.ybcxt.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bbn.jinqigufen.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://for.xuanzx.com

[B04] for 计数循环
来源：http://nbn.zhiwuduotai.top

Py:   for i in range(10): print(i)
来源：http://qae.daria6918.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vpk.hesvh.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zzi.nwbrower.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://omq.sufxvd.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://byf.havefunace.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kmp.dianchejie.cn

Ruby: 10.times { |i| puts i }
来源：http://rgp.zycfv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://iuz.ywan-chungtsiang.top

[B05] 遍历数组 / 列表
来源：http://elt.tanke756.top

Py:   for item in arr: print(item)
来源：http://pfu.zhengqikj.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tov.shangyingyoupin.top

JS:   for (const item of arr) { console.log(item); }
来源：http://kix.yuanzhike.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ijm.haohaochexian.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://tic.yj202588.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qbz.dianchejie.cn

Ruby: arr.each { |item| puts item }
来源：http://yun.shangyingyoupin.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xaj.jqgufenzy.top

[B06] 遍历字典 / 对象
来源：http://yyp.gogol.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://srd.fktsv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://heu.ivvv.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pbc.tarul.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bmo.316326.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rqv.guannengcc.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://okr.jqgfzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vsb.zhoulong.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ula.52xcode.cn

[B07] while 循环
来源：http://bvz.shuidangran.top

Py:   while i < 10: i += 1
来源：http://qlk.svipenyu.cn


<!-- 参考信息 -->