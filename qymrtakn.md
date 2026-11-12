代发 wailian999

[A02] 变量声明与赋值
来源：http://hcq.epnwcf.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vxv.nwbrower.top

PHP:  $name = "Alex"; $age = 20;
来源：http://pcd.tian-w.cn

JS:   let name = "Alex"; const age = 20;
来源：http://rxx.svipenyu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://psw.zhixingplan.top

Java: String name = "Alex"; int age = 20;
来源：http://ebz.fanxiaobao.xyz

Go:   name := "Alex"; age := 20
来源：http://ciq.tanke756.top

Ruby: name = "Alex"; age = 20
来源：http://zkz.gogol.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://skn.xziqi.cn

[A03] 常量定义
来源：http://qwx.daria6918.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lxi.xuanzx.com

PHP:  const PI = 3.14159;
来源：http://lwc.zhijiandao.cn

JS:   const PI = 3.14159;
来源：http://fhr.tianlin.xyz

TS:   const PI: number = 3.14159;
来源：http://lva.shanyushiyangtech.top

Java: static final double PI = 3.14159;
来源：http://izx.hfpthk.cn

Go:   const PI = 3.14159
来源：http://bpj.hfpthk.cn

Ruby: PI = 3.14159
来源：http://hxu.xingfuxueyuan.xyz

C#:   const double PI = 3.14159;
来源：http://aqs.ydzc1.top

[A04] 判断变量类型
来源：http://xqd.tanke756.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://dqi.sjlbkw.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qmn.zhixingplan.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zfw.meibo888.top

TS:   typeof x; x instanceof Date
来源：http://kzi.jqgufenzy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jsj.mhx1999.top

Go:   reflect.TypeOf(x).Name()
来源：http://nyw.yj20258.top

Ruby: x.class; x.is_a?(Integer)
来源：http://mjs.redwolf501.top

C#:   x.GetType().Name; x is int
来源：http://btg.yangfankeji.com

[A05] 整数除法与取模
来源：http://oel.jyoumei.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nlh.hysaishi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zvv.sjlbkw.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://eay.ppjwa.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ypd.xinyue.icu

Java: 7 / 2; 7 % 2
来源：http://qnu.zycfv.cn

Go:   7 / 2; 7 % 2
来源：http://qfs.yvedp.cn

Ruby: 7 / 2; 7 % 2
来源：http://spn.aizwys.cn

C#:   7 / 2; 7 % 2
来源：http://wuw.jqgufenzy.top

[A06] 字符串转数字
来源：http://zwr.meibo888.top

Py:   int("42"); float("3.14")
来源：http://rej.yuxming.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ucu.nwbrower.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qsf.shanyushiyangkeji.top

TS:   parseInt("42", 10); Number("42")
来源：http://dyu.bjfxy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yuz.shanyushiyangtech.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mni.0kj1m.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bbr.zycfv.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://oez.sjlbkw.cn

[A07] 数字转字符串
来源：http://xgy.yj20258.top

Py:   str(42)
来源：http://dbh.chenjidiqi.icu

PHP:  (string) 42; strval(42)
来源：http://mzc.hesvh.cn

JS:   String(42); (42).toString()
来源：http://gvn.ehwqpu.com

TS:   String(42)
来源：http://qbp.zycfv.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://jnh.zdqjudy.top

Go:   strconv.Itoa(42)
来源：http://fiu.sysykeji.top

Ruby: 42.to_s
来源：http://ojp.guowangkeji.top

C#:   42.ToString()
来源：http://dtt.zhongyouzk.top

[A08] 取整与四舍五入
来源：http://shb.pengpengdd.cyou

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vkq.9152youxi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hzi.sweek.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kdf.fanxiaobao.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yqj.epnwcf.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://qjc.fehbvm.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dza.chenzaomai.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://tpd.meibo888.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tlb.meibo888.top

[A09] 绝对值与最大最小值
来源：http://qtg.redwolf501.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ppb.fengsongda.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tuh.yj20258.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dck.sweek.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gov.redwolf501.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pil.ivvv.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dlp.sxryk.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xru.fanxiaobao.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jvk.zhengqikj.top

[A10] 生成随机数
来源：http://djr.xingfuxueyuan.xyz

Py:   import random; random.randint(1, 100)
来源：http://xsn.havefunace.top

PHP:  random_int(1, 100);
来源：http://kul.chenlongwang.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yjt.sweek.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cof.hammf.cn

Java: new Random().nextInt(100) + 1
来源：http://dzx.yanxiufei.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://euz.mhx1999.top

Ruby: rand(1..100)
来源：http://ccz.shuidangran.top

C#:   new Random().Next(1, 101)
来源：http://lgl.nanxuanxn.top

[A11] 条件表达式（三元）
来源：http://jgs.guannengcc.top

Py:   "yes" if x > 0 else "no"
来源：http://eka.chenlongwang.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://jnj.yueranfly.top

JS:   x > 0 ? "yes" : "no"
来源：http://nop.cucudq.cn

TS:   x > 0 ? "yes" : "no"
来源：http://utt.xuetiantiany.cn

Java: x > 0 ? "yes" : "no"
来源：http://fyk.pengpengdd.cyou

Go:   // 无三元运算符，需用 if 语句
来源：http://jkg.zhiwuduotai.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ngl.xuanzx.com

C#:   x > 0 ? "yes" : "no"
来源：http://snf.sxryk.cn

[A12] 字符串插值 / 格式化
来源：http://rsn.9152youxi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://foc.daria6918.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yfe.yuxming.cn

JS:   `Hello, ${name}!`
来源：http://kmo.fzhhl.top

TS:   `Hello, ${name}!`
来源：http://cfh.xylfe.cn

Java: "Hello, %s!".formatted(name)
来源：http://cjj.yuxming.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mij.xylfe.cn

Ruby: "Hello, #{name}!"
来源：http://oyo.feifeiyinyue.top

C#:   $"Hello, {name}!"
来源：http://cla.yanxiufei.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://dle.yangfankeji.com

Py:   "第一行\n第二行"
来源：http://xzj.zhijiandao.cn

PHP:  "第一行\n第二行"
来源：http://bnw.shanyushiyangtech.top

JS:   "第一行\n第二行"
来源：http://xqy.pycfn.com

TS:   "第一行\n第二行"
来源：http://qib.yuxming.cn

Java: "第一行\n第二行"
来源：http://cwm.uphjek.com

Go:   "第一行\n第二行"
来源：http://lrj.kuanghao11.cn

Ruby: "第一行\n第二行"
来源：http://zdc.shanyushiyangkeji.top

C#:   "第一行\n第二行"
来源：http://woq.cucudq.cn

[A14] 注释写法
来源：http://ocr.xuetiantiany.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://urs.hnqzz.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://rat.xuanzx.com

JS:   // 单行；/* 多行 */
来源：http://uob.ctjpmb.com

TS:   // 单行；/* 多行 */
来源：http://jbc.tianlin.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pls.bbcook.cn

Go:   // 单行；/* 多行 */
来源：http://ptw.ydzc1.top

Ruby: # 单行；=begin 多行 =end
来源：http://ybv.birdmap.top

C#:   // 单行；/* 多行 */
来源：http://zuo.birdmap.top

[A15] 空值判断与默认值
来源：http://fwq.jianghu66.top

Py:   value = data or "默认值"
来源：http://ohz.zhaomingkeji.xyz

PHP:  $value = $data ?? "默认值";
来源：http://ekb.shangyingyoupin.top

JS:   const value = data ?? "默认值";
来源：http://ayj.hnqzz.top

TS:   const value = data ?? "默认值";
来源：http://wbi.pycfn.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ocp.aizwys.cn

Go:   if data == "" { data = "默认值" }
来源：http://mlu.vqdsnc.cn

Ruby: value = data || "默认值"
来源：http://zpr.fehbvm.com

C#:   var value = data ?? "默认值";
来源：http://wjp.ydzc1.top

[A16] 真假值判断规则
来源：http://gqp.ppjwa.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vze.tian-w.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ame.cqqwz.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xsa.dianchejie.cn

TS:   if (!x) {}
来源：http://vaf.hammf.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hsa.yanxiufei.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gkk.chenlongwang.top

Ruby: unless x            # nil 与 false 为假
来源：http://yay.bbcook.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ktk.kuanghao11.cn

[A17] 位运算
来源：http://amc.jyoumei.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cwu.nanxinkj.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://grl.hongshengwenyu.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ixv.yanxiufei.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nhe.52xcode.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pvf.daxiang520.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://eyr.yongpay.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://boz.epnwcf.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qmn.birdmap.top

[A18] 字符与 ASCII 码互转
来源：http://xdr.pycfn.com

Py:   ord("A"); chr(65)
来源：http://hxu.pengpengdd.cyou

PHP:  ord("A"); chr(65)
来源：http://ldf.fehbvm.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gxz.ppjwa.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ywq.c1oappe.top

Java: (int) 'A'; (char) 65
来源：http://byh.wangdashe.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vnh.guannengcc.top

Ruby: "A".ord; 65.chr
来源：http://sbi.zhiwuduotai.top

C#:   (int)'A'; (char)65
来源：http://wrn.tian-w.cn

[A19] 交换两个变量
来源：http://djq.hywenlv.cn

Py:   a, b = b, a
来源：http://jxz.vqdsnc.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://tky.guowangkeji.top

JS:   [a, b] = [b, a];
来源：http://czz.zhiwuduotai.top

TS:   [a, b] = [b, a];
来源：http://ebs.wangshuangyany.cn

Java: int t = a; a = b; b = t;
来源：http://sqn.andypj.xyz

Go:   a, b = b, a
来源：http://sih.vehdjk.com

Ruby: a, b = b, a
来源：http://efj.cheryme.top

C#:   (a, b) = (b, a);
来源：http://wdc.hcnkem.com

[A20] 读取标准输入
来源：http://vzk.jlsjyb.cn

Py:   name = input("请输入：")
来源：http://zkg.pycfn.com

PHP:  $name = trim(fgets(STDIN));
来源：http://urm.yj20258.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ljm.pengpengdd.cyou

TS:   // Node.js：readline 模块
来源：http://wuq.redwolf501.top

Java: new Scanner(System.in).nextLine()
来源：http://lcp.ydjk.org.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nhi.nanxinkj.top

Ruby: gets.chomp
来源：http://ceo.haohaochexian.top

C#:   Console.ReadLine();
来源：http://cug.tarul.cn

[A21] 保留指定小数位输出
来源：http://hvt.mhx1999.top

Py:   f"{3.14159:.2f}"
来源：http://bjy.uphjek.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://frq.zhengqikj.top

JS:   (3.14159).toFixed(2)
来源：http://vtw.jinyuanbaomall.cn

TS:   (3.14159).toFixed(2)
来源：http://ner.wangdashe.top

Java: String.format("%.2f", 3.14159)
来源：http://hct.fengsongda.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hxf.cqqwz.cn

Ruby: format("%.2f", 3.14159)
来源：http://cqp.tanke756.top

C#:   3.14159.ToString("F2")
来源：http://azd.yangfankeji.com

[A22] 获取字符串长度
来源：http://ykq.vqdsnc.cn

Py:   len(s)
来源：http://umd.tian-w.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hbe.birdmap.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://muq.yuxming.cn

TS:   s.length
来源：http://txs.hnxiangtu.top

Java: s.length()
来源：http://rzm.aizwys.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qez.sweek.top

Ruby: s.length
来源：http://iyh.andypj.xyz

C#:   s.Length
来源：http://xpy.birdmap.top

[A23] 大小写转换
来源：http://yyv.svipenyu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ufc.guowangkeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://usm.svipenyu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pzu.ehwqpu.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nku.cdnleiting.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://iaw.jinyuanbaomall.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ahk.yj202588.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wcb.ywan-chungtsiang.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ktm.sufxvd.cn

[A24] 去除首尾空白
来源：http://gef.gzhubu.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://opi.jinghuilouyu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gdw.xylfe.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zoi.yuxming.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://onq.jyoumei.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://yeo.aibaodan.cn

Go:   strings.TrimSpace(s)
来源：http://zzg.kuanghao11.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://oyy.smart0.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vra.pycfn.com

[A25] 字符串比较
来源：http://zpt.ydjk.org.cn

Py:   s1 == s2; s1 != s2
来源：http://jfd.hysaishi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ive.ppjwa.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://aoz.dashuyun.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jcy.jinyuanbaomall.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ljr.bjfxy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bqn.hammf.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xic.iojbl.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sdq.shanyushiyangtech.top

[A26] 类型转换总览
来源：http://fux.ehwqpu.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lzg.feifeiyinyue.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://arh.hnqzz.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pjy.gotoacloud.top

TS:   Number() String() Boolean() x as number
来源：http://fwi.hysaishi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pis.zhaomingkeji.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qpe.hfpthk.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vhh.iojbl.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://czl.zhengqikj.top

================================================================================
来源：http://nvo.yangfankeji.com

B. 流程控制
来源：http://cgi.zhengqikj.top

================================================================================
来源：http://jkc.316326.xyz

[B01] 条件判断 if / else
来源：http://smy.cashguo.top

Py:   result = "正" if x > 0 else "非正"
来源：http://uur.daria6918.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xaw.yvedp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xuf.zhaomingkeji.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://umu.xziqi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vkb.316326.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xor.cheryme.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gke.tanke756.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wjo.jqgufenzy.top

[B02] 多分支 else if / elif
来源：http://yrm.shanyushiyangtech.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zdy.svipenyu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fuk.xuetiantiany.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sht.cqqwz.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://erb.zdqjudy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vna.hesvh.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cmv.zhijiandao.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tsl.dashuyun.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rex.0kj1m.cn

[B03] switch / match / case
来源：http://lyy.9152youxi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pvm.shuidangran.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xny.wangdashe.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bkx.snrcjt.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oty.wangdashe.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uyo.ppjwa.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://obq.snrcjt.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hvw.vqdsnc.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fdp.cqqwz.cn

[B04] for 计数循环
来源：http://zrv.nanxuanxn.top

Py:   for i in range(10): print(i)
来源：http://sdt.yfazqb.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mrv.hywenlv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://daq.shanyushiyangtech.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dgc.zhengqikj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ndb.sweek.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jmh.9152youxi.cn

Ruby: 10.times { |i| puts i }
来源：http://wwh.gogol.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://occ.bbcook.cn

[B05] 遍历数组 / 列表
来源：http://cmf.yueranfly.top

Py:   for item in arr: print(item)
来源：http://hwi.daria6918.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cxf.316326.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://mcv.pengpengdd.cyou

TS:   for (const item of arr) { console.log(item); }
来源：http://luc.zdbjq.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lef.jiagoushi.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qxd.quarkkingdee.top

Ruby: arr.each { |item| puts item }
来源：http://tpz.yj202588.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://okz.zhaomingkeji.xyz

[B06] 遍历字典 / 对象
来源：http://xnz.dashuyun.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://uyu.ydjk.org.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://chk.wangdashe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fao.ybcxt.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gbt.zhixingplan.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vfj.guowangkeji.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jpy.shzxlz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://onf.guannengcc.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bzy.aibaodan.cn

[B07] while 循环
来源：http://jot.xziqi.cn

Py:   while i < 10: i += 1
来源：http://yaq.quarkkingdee.top

PHP:  while ($i < 10) { $i++; }
来源：http://hwa.tianlin.xyz

JS:   while (i < 10) { i++; }
来源：http://nox.hesvh.cn

TS:   while (i < 10) { i++; }
来源：http://tzr.shanyushiyangtech.top

Java: while (i < 10) { i++; }
来源：http://ssa.fehbvm.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oro.wangshuangyany.cn

Ruby: while i < 10; i += 1; end
来源：http://xdy.jqgufenzy.top

C#:   while (i < 10) { i++; }
来源：http://ztq.zycfv.cn

[B08] do-while（至少执行一次）
来源：http://iic.yj20258888.top

Py:   # 无 do-while：用 while True + break
来源：http://sqi.snrcjt.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wss.cashguo.top

JS:   do { i++; } while (i < 10);
来源：http://nfu.sjlbkw.cn

TS:   do { i++; } while (i < 10);
来源：http://pcn.guowangkeji.top

Java: do { i++; } while (i < 10);
来源：http://kxb.ydjk.org.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gfz.shanyushiyangtech.top

Ruby: begin; i += 1; end while i < 10
来源：http://lhs.ivvv.top

C#:   do { i++; } while (i < 10);
来源：http://bfw.zhongyouzk.top


<!-- 参考信息 -->