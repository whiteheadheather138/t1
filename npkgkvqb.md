代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://vyg.yueranfly.top

Go:   fmt.Println("Hello, World!")
来源：http://aha.vehdjk.com

Ruby: puts "Hello, World!"
来源：http://sri.jinghuilouyu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://bkg.shanyushiyangkeji.top

[A02] 变量声明与赋值
来源：http://die.daria6918.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://prl.tianlin.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://cby.zycfv.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qup.ivvv.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://djb.wangdashe.top

Java: String name = "Alex"; int age = 20;
来源：http://kjg.yfazqb.com

Go:   name := "Alex"; age := 20
来源：http://oue.fengsongda.top

Ruby: name = "Alex"; age = 20
来源：http://orm.fktsv.cn

C#:   string name = "Alex"; int age = 20;
来源：http://nsk.gaohongyu789.top

[A03] 常量定义
来源：http://zkj.bjfxy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bqy.jqgufenzy.top

PHP:  const PI = 3.14159;
来源：http://zpk.ydjk.org.cn

JS:   const PI = 3.14159;
来源：http://skv.dashuyun.cn

TS:   const PI: number = 3.14159;
来源：http://yvg.zhiwuduotai.top

Java: static final double PI = 3.14159;
来源：http://vml.uphjek.com

Go:   const PI = 3.14159
来源：http://spo.ybcxt.top

Ruby: PI = 3.14159
来源：http://sqg.cucudq.cn

C#:   const double PI = 3.14159;
来源：http://fcb.hnxiangtu.top

[A04] 判断变量类型
来源：http://gfv.andypj.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://avj.havefunace.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://byb.ehwqpu.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://aab.gotoacloud.top

TS:   typeof x; x instanceof Date
来源：http://svd.chenzaomai.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sfw.zhijiandao.cn

Go:   reflect.TypeOf(x).Name()
来源：http://dlp.chenzaomai.com

Ruby: x.class; x.is_a?(Integer)
来源：http://lbn.wangshuangyany.cn

C#:   x.GetType().Name; x is int
来源：http://mso.snrcjt.cn

[A05] 整数除法与取模
来源：http://srq.tanke756.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qqi.sjlbkw.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://awl.tianlin.xyz

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://agj.yanxiufei.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fpd.pengpengdd.cyou

Java: 7 / 2; 7 % 2
来源：http://cfb.zhongyouzk.top

Go:   7 / 2; 7 % 2
来源：http://qfo.zdbjq.cn

Ruby: 7 / 2; 7 % 2
来源：http://egn.feifeiyinyue.top

C#:   7 / 2; 7 % 2
来源：http://hcr.mhx1999.top

[A06] 字符串转数字
来源：http://xji.aibaodan.cn

Py:   int("42"); float("3.14")
来源：http://vix.c1oappe.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://roj.cheryme.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fai.hysaishi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://bac.fzhhl.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://adb.chenjidiqi.icu

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jhz.ivvv.top

Ruby: "42".to_i; "3.14".to_f
来源：http://oiy.shzxlz.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tqx.nwbrower.top

[A07] 数字转字符串
来源：http://uns.cucudq.cn

Py:   str(42)
来源：http://ymf.xingfuxueyuan.xyz

PHP:  (string) 42; strval(42)
来源：http://dbi.haohaochexian.top

JS:   String(42); (42).toString()
来源：http://ggh.c1oappe.top

TS:   String(42)
来源：http://gmx.ywan-chungtsiang.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://zwn.316326.xyz

Go:   strconv.Itoa(42)
来源：http://gwv.shanyushiyangkeji.top

Ruby: 42.to_s
来源：http://apv.dianchejie.cn

C#:   42.ToString()
来源：http://cvu.shanyushiyangkeji.top

[A08] 取整与四舍五入
来源：http://uiv.xingfuxueyuan.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ihb.xuanzx.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ied.cheryme.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://imh.zdqjudy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://nqm.zhengqikj.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://htj.aibaodan.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://kol.gaohongyu789.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://kof.vehdjk.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jze.jianghu66.top

[A09] 绝对值与最大最小值
来源：http://poq.bjfxy.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://oua.redwolf501.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ujx.yj202588.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vdn.sufxvd.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hxd.snrcjt.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://euw.zhaomingkeji.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wmr.jinqigfzy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fui.zdbjq.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://uha.zhiwuduotai.top

[A10] 生成随机数
来源：http://vtz.ydzc1.top

Py:   import random; random.randint(1, 100)
来源：http://xnt.bjfxy.top

PHP:  random_int(1, 100);
来源：http://lrk.jinqigufen.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qei.zhoulong.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://omr.cashguo.top

Java: new Random().nextInt(100) + 1
来源：http://tyg.andypj.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://czp.jlsjyb.cn

Ruby: rand(1..100)
来源：http://vmu.pycfn.com

C#:   new Random().Next(1, 101)
来源：http://txj.wangdashe.top

[A11] 条件表达式（三元）
来源：http://bpa.yj20258.top

Py:   "yes" if x > 0 else "no"
来源：http://lyv.shanyushiyangtech.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://via.cqqwz.cn

JS:   x > 0 ? "yes" : "no"
来源：http://oyz.iojbl.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rcr.hnqzz.top

Java: x > 0 ? "yes" : "no"
来源：http://lzf.yonumen.top

Go:   // 无三元运算符，需用 if 语句
来源：http://hvf.zhongyouzk.top

Ruby: x > 0 ? "yes" : "no"
来源：http://jcw.iojbl.cn

C#:   x > 0 ? "yes" : "no"
来源：http://daa.yongpay.top

[A12] 字符串插值 / 格式化
来源：http://zgl.shanyushiyangtech.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vaj.daria6918.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vad.zhijiandao.cn

JS:   `Hello, ${name}!`
来源：http://eaz.hesvh.cn

TS:   `Hello, ${name}!`
来源：http://wqc.fengsongda.top

Java: "Hello, %s!".formatted(name)
来源：http://mhs.gaohongyu789.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://emy.wangdashe.top

Ruby: "Hello, #{name}!"
来源：http://hqk.cashguo.top

C#:   $"Hello, {name}!"
来源：http://jiq.nanxinkj.top

[A13] 多行字符串（练习 \n 转义）
来源：http://zbm.zhaomingkeji.xyz

Py:   "第一行\n第二行"
来源：http://lkj.hfpthk.cn

PHP:  "第一行\n第二行"
来源：http://xgn.chenjidiqi.icu

JS:   "第一行\n第二行"
来源：http://zut.hysaishi.cn

TS:   "第一行\n第二行"
来源：http://nye.tanke756.top

Java: "第一行\n第二行"
来源：http://pwl.dianchejie.cn

Go:   "第一行\n第二行"
来源：http://gxs.bbcook.cn

Ruby: "第一行\n第二行"
来源：http://ndr.ehwqpu.com

C#:   "第一行\n第二行"
来源：http://fle.nanxinkj.top

[A14] 注释写法
来源：http://ktw.andypj.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://dcn.daria6918.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hze.yfazqb.com

JS:   // 单行；/* 多行 */
来源：http://xdc.fzhhl.top

TS:   // 单行；/* 多行 */
来源：http://oea.yangfankeji.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lga.snrcjt.cn

Go:   // 单行；/* 多行 */
来源：http://opa.snrcjt.cn

Ruby: # 单行；=begin 多行 =end
来源：http://uxk.svipenyu.cn

C#:   // 单行；/* 多行 */
来源：http://lwo.sweek.top

[A15] 空值判断与默认值
来源：http://gld.jyoumei.cn

Py:   value = data or "默认值"
来源：http://srw.ybcxt.top

PHP:  $value = $data ?? "默认值";
来源：http://irn.c1oappe.top

JS:   const value = data ?? "默认值";
来源：http://dds.zhixingplan.top

TS:   const value = data ?? "默认值";
来源：http://soo.snrcjt.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zsh.tanke756.top

Go:   if data == "" { data = "默认值" }
来源：http://cfh.mhx1999.top

Ruby: value = data || "默认值"
来源：http://qjr.fanxiaobao.xyz

C#:   var value = data ?? "默认值";
来源：http://agy.nwbrower.top

[A16] 真假值判断规则
来源：http://wie.epnwcf.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jts.xingfuxueyuan.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://stk.gaohongyu789.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zda.dianchejie.cn

TS:   if (!x) {}
来源：http://dlq.shangyingyoupin.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://que.ydjk.org.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wio.fktsv.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jez.andypj.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fvq.dashuyun.cn

[A17] 位运算
来源：http://pnd.pycfn.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zku.hnxiangtu.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dyb.xuanzx.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rwr.zhiwuduotai.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xpb.jinqigufen.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ani.dianchejie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ytz.ydjk.org.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mwb.yj202588.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://flm.hnxiangtu.top

[A18] 字符与 ASCII 码互转
来源：http://ugk.svipenyu.cn

Py:   ord("A"); chr(65)
来源：http://lxt.zdbjq.cn

PHP:  ord("A"); chr(65)
来源：http://fzi.ivvv.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://czl.sufxvd.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qtr.havefunace.top

Java: (int) 'A'; (char) 65
来源：http://uov.shzxlz.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xgp.meibo888.top

Ruby: "A".ord; 65.chr
来源：http://xfb.vqdsnc.cn

C#:   (int)'A'; (char)65
来源：http://ejm.yj20258888.top

[A19] 交换两个变量
来源：http://alv.yuanzhike.top

Py:   a, b = b, a
来源：http://xzv.andypj.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://tis.zhijiandao.cn

JS:   [a, b] = [b, a];
来源：http://ruq.fengsongda.top

TS:   [a, b] = [b, a];
来源：http://tjr.zhoulong.xyz

Java: int t = a; a = b; b = t;
来源：http://ulr.jyoumei.cn

Go:   a, b = b, a
来源：http://tih.316326.xyz

Ruby: a, b = b, a
来源：http://aly.zhongyouzk.top

C#:   (a, b) = (b, a);
来源：http://trx.tanke756.top

[A20] 读取标准输入
来源：http://lgg.jlsjyb.cn

Py:   name = input("请输入：")
来源：http://qcq.hywenlv.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zpv.yvedp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fer.zhixingplan.top

TS:   // Node.js：readline 模块
来源：http://tjr.zhoulong.xyz

Java: new Scanner(System.in).nextLine()
来源：http://yix.cqqwz.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ldx.0kj1m.cn

Ruby: gets.chomp
来源：http://joq.zhongyouzk.top

C#:   Console.ReadLine();
来源：http://nfd.daxiang520.top

[A21] 保留指定小数位输出
来源：http://exv.316326.xyz

Py:   f"{3.14159:.2f}"
来源：http://faj.ydzc1.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://oto.smart0.xyz

JS:   (3.14159).toFixed(2)
来源：http://agm.havefunace.top

TS:   (3.14159).toFixed(2)
来源：http://pep.fengsongda.top

Java: String.format("%.2f", 3.14159)
来源：http://mbp.hongshengwenyu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pjc.hammf.cn

Ruby: format("%.2f", 3.14159)
来源：http://ops.cdnleiting.top

C#:   3.14159.ToString("F2")
来源：http://buj.chenjidiqi.icu

[A22] 获取字符串长度
来源：http://bwx.vehdjk.com

Py:   len(s)
来源：http://wtl.hongshengwenyu.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qbk.redwolf501.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fth.yuanzhike.top

TS:   s.length
来源：http://yda.chenjidiqi.icu

Java: s.length()
来源：http://ixx.chenzaomai.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://imd.hcnkem.com

Ruby: s.length
来源：http://dnh.fengsongda.top

C#:   s.Length
来源：http://ksb.cashguo.top

[A23] 大小写转换
来源：http://ain.yj202588.top

Py:   s.upper(); s.lower(); s.title()
来源：http://hsy.kuanghao11.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bwk.gogol.net.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ivi.dianchejie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://efj.pengpengdd.cyou

Java: s.toUpperCase(); s.toLowerCase()
来源：http://uzs.zdbjq.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jag.shanyushiyangkeji.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yfh.snrcjt.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fee.iojbl.cn

[A24] 去除首尾空白
来源：http://ymu.zycfv.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pcu.iojbl.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xep.daxiang520.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://udj.havefunace.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lhc.yvedp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xsb.yfazqb.com

Go:   strings.TrimSpace(s)
来源：http://jlq.wangdashe.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blo.fanxiaobao.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rkf.52xcode.cn

[A25] 字符串比较
来源：http://ntu.yfazqb.com

Py:   s1 == s2; s1 != s2
来源：http://arp.yanxiufei.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://spy.jiagoushi.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vhp.feifeiyinyue.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wsb.daria6918.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cwj.hywenlv.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ilq.shuidangran.top

Ruby: s1 == s2; s1 <=> s2
来源：http://wlg.xingfuxueyuan.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bcu.nanxuanxn.top

[A26] 类型转换总览
来源：http://wci.hywenlv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qoo.daxiang520.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pgw.zhoulong.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://upc.ydjk.org.cn

TS:   Number() String() Boolean() x as number
来源：http://cbn.yanxiufei.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tgi.ydjk.org.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cjf.svipenyu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://end.hfpthk.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://esu.vehdjk.com

================================================================================
来源：http://zce.shangyingyoupin.top

B. 流程控制
来源：http://qut.0kj1m.cn

================================================================================
来源：http://efv.bbcook.cn

[B01] 条件判断 if / else
来源：http://mse.birdmap.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ygh.yongpay.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://opp.havefunace.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bzs.guowangkeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tbv.cucudq.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sjk.zhijiandao.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://iwv.shuidangran.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lbn.zdbjq.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wyu.zhoulong.xyz

[B02] 多分支 else if / elif
来源：http://hbt.jlsjyb.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vhu.hnqzz.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fgk.xylfe.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kvs.cucudq.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xpc.zhoulong.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gyy.chenlongwang.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wcv.cheryme.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://haw.ywan-chungtsiang.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hnb.fehbvm.com

[B03] switch / match / case
来源：http://xtv.dashuyun.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kvy.0kj1m.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rsl.xuetiantiany.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jug.jinghuilouyu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://viq.chenlongwang.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kfm.yangfankeji.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lkg.xuetiantiany.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://brv.yanxiufei.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dja.cdnleiting.top

[B04] for 计数循环
来源：http://fqx.tianlin.xyz

Py:   for i in range(10): print(i)
来源：http://gft.jiagoushi.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://icj.nwbrower.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eel.zhiwuduotai.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mpz.ybcxt.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gnt.aibaodan.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://epk.ybcxt.top

Ruby: 10.times { |i| puts i }
来源：http://wmj.nanxuanxn.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lpo.chenjidiqi.icu

[B05] 遍历数组 / 列表
来源：http://xoh.cashguo.top

Py:   for item in arr: print(item)
来源：http://jii.hammf.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dwq.jinyuanbaomall.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://pir.daxiang520.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qyu.yj202588.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://wnw.birdmap.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kxf.zdbjq.cn

Ruby: arr.each { |item| puts item }
来源：http://urs.fzhhl.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ncz.xinyue.icu

[B06] 遍历字典 / 对象
来源：http://qxg.sweek.top

Py:   for k, v in d.items(): print(k, v)
来源：http://kxc.wangshuangyany.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jua.snrcjt.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pao.guowangkeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rgl.cucudq.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ysx.jqgfzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wtm.sjlbkw.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://afi.shanyushiyangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hba.c1oappe.top

[B07] while 循环
来源：http://cjt.aibaodan.cn

Py:   while i < 10: i += 1
来源：http://wzy.fktsv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://eyd.jqgfzy.top

JS:   while (i < 10) { i++; }
来源：http://yrx.jiagoushi.top

TS:   while (i < 10) { i++; }
来源：http://ncb.smart0.xyz

Java: while (i < 10) { i++; }
来源：http://rmb.meibo888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sjq.daria6918.cn

Ruby: while i < 10; i += 1; end
来源：http://cbg.nwbrower.top

C#:   while (i < 10) { i++; }
来源：http://nhe.jinyuanbaomall.cn

[B08] do-while（至少执行一次）
来源：http://qvn.zdqjudy.top

Py:   # 无 do-while：用 while True + break
来源：http://fsf.xinyue.icu

PHP:  do { $i++; } while ($i < 10);
来源：http://lzc.zhongyouzk.top

JS:   do { i++; } while (i < 10);
来源：http://rvj.andypj.xyz

TS:   do { i++; } while (i < 10);
来源：http://tbz.zycfv.cn


<!-- 参考信息 -->