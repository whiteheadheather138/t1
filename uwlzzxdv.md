代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://uje.yanxiufei.cn

Go:   fmt.Println("Hello, World!")
来源：http://kzt.jinghuilouyu.cn

Ruby: puts "Hello, World!"
来源：http://qqf.guowangkeji.top

C#:   Console.WriteLine("Hello, World!");
来源：http://mjs.vehdjk.com

[A02] 变量声明与赋值
来源：http://fxl.pycfn.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://epv.shanyushiyangtech.top

PHP:  $name = "Alex"; $age = 20;
来源：http://toy.fengsongda.top

JS:   let name = "Alex"; const age = 20;
来源：http://pfq.shzxlz.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ofy.quarkkingdee.top

Java: String name = "Alex"; int age = 20;
来源：http://gle.andypj.xyz

Go:   name := "Alex"; age := 20
来源：http://nje.ehwqpu.com

Ruby: name = "Alex"; age = 20
来源：http://udk.zhaomingkeji.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://xlb.hesvh.cn

[A03] 常量定义
来源：http://snx.yj20258888.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ids.zdbjq.cn

PHP:  const PI = 3.14159;
来源：http://nly.tarul.cn

JS:   const PI = 3.14159;
来源：http://psp.yj20258888.top

TS:   const PI: number = 3.14159;
来源：http://dsv.chenzaomai.com

Java: static final double PI = 3.14159;
来源：http://cth.fehbvm.com

Go:   const PI = 3.14159
来源：http://zna.gotoacloud.top

Ruby: PI = 3.14159
来源：http://ybm.yangfankeji.com

C#:   const double PI = 3.14159;
来源：http://vli.smart0.xyz

[A04] 判断变量类型
来源：http://tyj.hywenlv.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hhc.yangfankeji.com

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://acg.ydzc1.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tze.hywenlv.cn

TS:   typeof x; x instanceof Date
来源：http://lnv.cheryme.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nkb.sysykeji.top

Go:   reflect.TypeOf(x).Name()
来源：http://bid.svipenyu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ako.zhengqikj.top

C#:   x.GetType().Name; x is int
来源：http://jzd.xingfuxueyuan.xyz

[A05] 整数除法与取模
来源：http://zht.hfpthk.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hzn.jiagoushi.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://zyd.vqdsnc.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://abw.yvedp.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bts.ctjpmb.com

Java: 7 / 2; 7 % 2
来源：http://zxf.yj202588.top

Go:   7 / 2; 7 % 2
来源：http://pix.jiagoushi.top

Ruby: 7 / 2; 7 % 2
来源：http://qzm.zdqjudy.top

C#:   7 / 2; 7 % 2
来源：http://zzx.nanxuanxn.top

[A06] 字符串转数字
来源：http://uwi.jiagoushi.top

Py:   int("42"); float("3.14")
来源：http://mpk.pengpengdd.cyou

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://exq.zhijiandao.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://eyl.xuanzx.com

TS:   parseInt("42", 10); Number("42")
来源：http://jpe.xinyue.icu

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://spu.316326.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ebl.dianchejie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://dmz.nanxinkj.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tsj.jqgfzy.top

[A07] 数字转字符串
来源：http://zxf.xuanzx.com

Py:   str(42)
来源：http://ojl.jlsjyb.cn

PHP:  (string) 42; strval(42)
来源：http://rqh.yonumen.top

JS:   String(42); (42).toString()
来源：http://foi.wangdashe.top

TS:   String(42)
来源：http://ava.sysykeji.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://kiz.fengsongda.top

Go:   strconv.Itoa(42)
来源：http://wky.sysykeji.top

Ruby: 42.to_s
来源：http://zam.gogol.net.cn

C#:   42.ToString()
来源：http://gvu.aizwys.cn

[A08] 取整与四舍五入
来源：http://gqv.mhx1999.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ctk.shuidangran.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rfv.wangdashe.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xnr.shanyushiyangtech.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rzq.yj202588.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dkz.0kj1m.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bnm.sufxvd.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://mlf.chenlongwang.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bys.hcnkem.com

[A09] 绝对值与最大最小值
来源：http://ici.feifeiyinyue.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fzd.hnqzz.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rgv.redwolf501.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://adt.xziqi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zoo.fanxiaobao.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nxa.jyoumei.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dmm.zhongyouzk.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://yvp.tarul.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qmb.jinqigufen.top

[A10] 生成随机数
来源：http://zun.ydjk.org.cn

Py:   import random; random.randint(1, 100)
来源：http://jhr.xinyue.icu

PHP:  random_int(1, 100);
来源：http://rae.ybcxt.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pir.316326.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://owv.cqqwz.cn

Java: new Random().nextInt(100) + 1
来源：http://abo.yvedp.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://biq.jyoumei.cn

Ruby: rand(1..100)
来源：http://qme.smart0.xyz

C#:   new Random().Next(1, 101)
来源：http://jxj.cdnleiting.top

[A11] 条件表达式（三元）
来源：http://vro.hysaishi.cn

Py:   "yes" if x > 0 else "no"
来源：http://rto.zhengqikj.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://hyx.sjlbkw.cn

JS:   x > 0 ? "yes" : "no"
来源：http://kxl.jiagoushi.top

TS:   x > 0 ? "yes" : "no"
来源：http://rbj.yonumen.top

Java: x > 0 ? "yes" : "no"
来源：http://ofn.gogol.net.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://crc.guannengcc.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ngq.quarkkingdee.top

C#:   x > 0 ? "yes" : "no"
来源：http://qif.hammf.cn

[A12] 字符串插值 / 格式化
来源：http://qcj.tanke756.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://aqx.xziqi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://noh.c1oappe.top

JS:   `Hello, ${name}!`
来源：http://pxg.cdnleiting.top

TS:   `Hello, ${name}!`
来源：http://bvv.xuetiantiany.cn

Java: "Hello, %s!".formatted(name)
来源：http://ryp.xinyue.icu

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nnw.yj20258888.top

Ruby: "Hello, #{name}!"
来源：http://pyt.0kj1m.cn

C#:   $"Hello, {name}!"
来源：http://qgl.cashguo.top

[A13] 多行字符串（练习 \n 转义）
来源：http://elr.jinqigufen.top

Py:   "第一行\n第二行"
来源：http://dno.yj20258888.top

PHP:  "第一行\n第二行"
来源：http://xxo.sufxvd.cn

JS:   "第一行\n第二行"
来源：http://jjy.gaohongyu789.top

TS:   "第一行\n第二行"
来源：http://qla.fanxiaobao.xyz

Java: "第一行\n第二行"
来源：http://nnc.haohaochexian.top

Go:   "第一行\n第二行"
来源：http://shy.tianlin.xyz

Ruby: "第一行\n第二行"
来源：http://ynx.chenjidiqi.icu

C#:   "第一行\n第二行"
来源：http://kss.sweek.top

[A14] 注释写法
来源：http://jjr.meibo888.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://wci.dashuyun.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://mgo.zdbjq.cn

JS:   // 单行；/* 多行 */
来源：http://dkf.zycfv.cn

TS:   // 单行；/* 多行 */
来源：http://kws.hfpthk.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pov.jinyuanbaomall.cn

Go:   // 单行；/* 多行 */
来源：http://ule.yj202588.top

Ruby: # 单行；=begin 多行 =end
来源：http://zvy.gotoacloud.top

C#:   // 单行；/* 多行 */
来源：http://xjc.jqgfzy.top

[A15] 空值判断与默认值
来源：http://jzh.gogol.net.cn

Py:   value = data or "默认值"
来源：http://xyq.vehdjk.com

PHP:  $value = $data ?? "默认值";
来源：http://qzg.fehbvm.com

JS:   const value = data ?? "默认值";
来源：http://ftx.cucudq.cn

TS:   const value = data ?? "默认值";
来源：http://vxz.meibo888.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jpw.fktsv.cn

Go:   if data == "" { data = "默认值" }
来源：http://vim.wangdashe.top

Ruby: value = data || "默认值"
来源：http://ypg.ydjk.org.cn

C#:   var value = data ?? "默认值";
来源：http://sob.ydzc1.top

[A16] 真假值判断规则
来源：http://vtt.c1oappe.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cyl.hywenlv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://sgn.redwolf501.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hof.zhixingplan.top

TS:   if (!x) {}
来源：http://dfe.xuanzx.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://oij.zhijiandao.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tfz.zhoulong.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://hkz.hnxiangtu.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lmc.yuxming.cn

[A17] 位运算
来源：http://nnu.fengsongda.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uar.nanxinkj.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tge.nanxuanxn.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ycw.andypj.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fnr.hongshengwenyu.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ufy.pycfn.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://iep.jiagoushi.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ujf.snrcjt.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rmu.316326.xyz

[A18] 字符与 ASCII 码互转
来源：http://zoj.shanyushiyangtech.top

Py:   ord("A"); chr(65)
来源：http://ozf.jianghu66.top

PHP:  ord("A"); chr(65)
来源：http://vaa.hcnkem.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mas.xziqi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gjo.ybcxt.top

Java: (int) 'A'; (char) 65
来源：http://opp.zhengqikj.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cvf.hysaishi.cn

Ruby: "A".ord; 65.chr
来源：http://jhk.xuetiantiany.cn

C#:   (int)'A'; (char)65
来源：http://vok.guowangkeji.top

[A19] 交换两个变量
来源：http://xlp.bbcook.cn

Py:   a, b = b, a
来源：http://lwp.zdbjq.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tdh.smart0.xyz

JS:   [a, b] = [b, a];
来源：http://vld.gaohongyu789.top

TS:   [a, b] = [b, a];
来源：http://tym.xinyue.icu

Java: int t = a; a = b; b = t;
来源：http://izc.jqgfzy.top

Go:   a, b = b, a
来源：http://qua.nwbrower.top

Ruby: a, b = b, a
来源：http://pry.zhongyouzk.top

C#:   (a, b) = (b, a);
来源：http://zsh.yuxming.cn

[A20] 读取标准输入
来源：http://jfp.pycfn.com

Py:   name = input("请输入：")
来源：http://ces.ctjpmb.com

PHP:  $name = trim(fgets(STDIN));
来源：http://nzg.52xcode.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hva.zhongyouzk.top

TS:   // Node.js：readline 模块
来源：http://okb.ydzc1.top

Java: new Scanner(System.in).nextLine()
来源：http://hgn.snrcjt.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fpr.chenzaomai.com

Ruby: gets.chomp
来源：http://zpx.tanke756.top

C#:   Console.ReadLine();
来源：http://icm.nwbrower.top

[A21] 保留指定小数位输出
来源：http://qse.gzhubu.top

Py:   f"{3.14159:.2f}"
来源：http://mgu.zycfv.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://esq.yfazqb.com

JS:   (3.14159).toFixed(2)
来源：http://pve.gotoacloud.top

TS:   (3.14159).toFixed(2)
来源：http://way.shangyingyoupin.top

Java: String.format("%.2f", 3.14159)
来源：http://hhr.cdnleiting.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sug.havefunace.top

Ruby: format("%.2f", 3.14159)
来源：http://puw.yvedp.cn

C#:   3.14159.ToString("F2")
来源：http://xqp.hcnkem.com

[A22] 获取字符串长度
来源：http://ewq.hywenlv.cn

Py:   len(s)
来源：http://ytp.zhongyouzk.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pco.pycfn.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gun.mhx1999.top

TS:   s.length
来源：http://jhd.jinqigfzy.top

Java: s.length()
来源：http://thr.chenzaomai.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://flb.fktsv.cn

Ruby: s.length
来源：http://bhx.fengsongda.top

C#:   s.Length
来源：http://ous.epnwcf.com

[A23] 大小写转换
来源：http://fum.daxiang520.top

Py:   s.upper(); s.lower(); s.title()
来源：http://agd.hnqzz.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hya.feifeiyinyue.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sck.zdqjudy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pks.hammf.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://klt.vqdsnc.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kaf.316326.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rly.ydjk.org.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dyt.hysaishi.cn

[A24] 去除首尾空白
来源：http://bgp.jinqigfzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sim.xuanzx.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://eew.sysykeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zkm.9152youxi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nre.haohaochexian.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://izi.shzxlz.cn

Go:   strings.TrimSpace(s)
来源：http://sop.yj20258888.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://piv.kuanghao11.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://agb.jinghuilouyu.cn

[A25] 字符串比较
来源：http://sqa.c1oappe.top

Py:   s1 == s2; s1 != s2
来源：http://hto.zhoulong.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yrd.hesvh.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jsr.sxryk.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://swn.hammf.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gbv.quarkkingdee.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hex.iojbl.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vlg.xziqi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lky.xuanzx.com

[A26] 类型转换总览
来源：http://yjr.daria6918.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zhg.vehdjk.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://viu.yj20258.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://aba.yj20258888.top

TS:   Number() String() Boolean() x as number
来源：http://urq.hongshengwenyu.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rvz.andypj.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://eik.sufxvd.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://xjg.zhixingplan.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cfy.ctjpmb.com

================================================================================
来源：http://kqn.jinqigufen.top

B. 流程控制
来源：http://cfb.gogol.net.cn

================================================================================
来源：http://gol.jqgfzy.top

[B01] 条件判断 if / else
来源：http://ziy.aibaodan.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://len.hysaishi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tat.cucudq.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dmn.pycfn.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kvb.zhoulong.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://zqj.jyoumei.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://koq.chenjidiqi.icu

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mip.shanyushiyangtech.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gbn.quarkkingdee.top

[B02] 多分支 else if / elif
来源：http://kys.ydzc1.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gdz.hfpthk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://waf.chenjidiqi.icu

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ntn.sysykeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vnz.shzxlz.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fon.jinqigufen.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ats.cdnleiting.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sut.9152youxi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kbz.chenjidiqi.icu

[B03] switch / match / case
来源：http://ywg.fzhhl.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://oyr.quarkkingdee.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cqy.yj202588.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://adn.zhijiandao.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jdy.feifeiyinyue.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pal.andypj.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://avj.yj202588.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zvv.snrcjt.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xfs.tian-w.cn

[B04] for 计数循环
来源：http://oaf.fanxiaobao.xyz

Py:   for i in range(10): print(i)
来源：http://grd.fehbvm.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dhj.52xcode.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wok.gogol.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jpy.cucudq.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wkw.ivvv.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tso.ctjpmb.com

Ruby: 10.times { |i| puts i }
来源：http://caf.sweek.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lui.c1oappe.top

[B05] 遍历数组 / 列表
来源：http://dhq.aibaodan.cn

Py:   for item in arr: print(item)
来源：http://ouu.zhengqikj.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zvf.xziqi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ffz.vqdsnc.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://dsf.jianghu66.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ybd.sysykeji.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wlo.tianlin.xyz

Ruby: arr.each { |item| puts item }
来源：http://upm.shuidangran.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ysd.shanyushiyangtech.top

[B06] 遍历字典 / 对象
来源：http://cpi.epnwcf.com

Py:   for k, v in d.items(): print(k, v)
来源：http://hpt.nanxuanxn.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://udn.birdmap.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gwg.zhijiandao.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oxf.yuanzhike.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vof.nanxinkj.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kgk.ctjpmb.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vrn.52xcode.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blv.sufxvd.cn

[B07] while 循环
来源：http://pyl.bjfxy.top

Py:   while i < 10: i += 1
来源：http://psk.iojbl.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ugl.tian-w.cn

JS:   while (i < 10) { i++; }
来源：http://nwo.xuetiantiany.cn

TS:   while (i < 10) { i++; }
来源：http://atn.xuetiantiany.cn

Java: while (i < 10) { i++; }
来源：http://lth.haohaochexian.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vke.xingfuxueyuan.xyz

Ruby: while i < 10; i += 1; end
来源：http://gbg.yuanzhike.top

C#:   while (i < 10) { i++; }
来源：http://vpk.zhiwuduotai.top

[B08] do-while（至少执行一次）
来源：http://ieu.yvedp.cn

Py:   # 无 do-while：用 while True + break
来源：http://aay.chenjidiqi.icu

PHP:  do { $i++; } while ($i < 10);
来源：http://jrh.gogol.net.cn

JS:   do { i++; } while (i < 10);
来源：http://mdx.iojbl.cn

TS:   do { i++; } while (i < 10);
来源：http://vob.hysaishi.cn


<!-- 参考信息 -->