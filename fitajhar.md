代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ymm.gzhubu.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ope.yuanzhike.top

TS:   typeof x; x instanceof Date
来源：http://ewj.yuxming.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vku.shzxlz.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fpr.chenjidiqi.icu

Ruby: x.class; x.is_a?(Integer)
来源：http://xeb.hcnkem.com

C#:   x.GetType().Name; x is int
来源：http://fpn.hnqzz.top

[A05] 整数除法与取模
来源：http://nmf.daria6918.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jui.epnwcf.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://dcl.c1oappe.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://iem.dianchejie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://uhg.fanxiaobao.xyz

Java: 7 / 2; 7 % 2
来源：http://ebr.meibo888.top

Go:   7 / 2; 7 % 2
来源：http://rwj.hysaishi.cn

Ruby: 7 / 2; 7 % 2
来源：http://njq.vehdjk.com

C#:   7 / 2; 7 % 2
来源：http://nkj.sysykeji.top

[A06] 字符串转数字
来源：http://htn.hammf.cn

Py:   int("42"); float("3.14")
来源：http://irk.ybcxt.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xkh.yanxiufei.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vxx.quarkkingdee.top

TS:   parseInt("42", 10); Number("42")
来源：http://yvs.ybcxt.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cni.iojbl.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bcb.ydzc1.top

Ruby: "42".to_i; "3.14".to_f
来源：http://lfi.mhx1999.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xsj.0kj1m.cn

[A07] 数字转字符串
来源：http://ojz.shzxlz.cn

Py:   str(42)
来源：http://tji.xylfe.cn

PHP:  (string) 42; strval(42)
来源：http://fbj.xziqi.cn

JS:   String(42); (42).toString()
来源：http://tby.jiagoushi.top

TS:   String(42)
来源：http://jcx.daria6918.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://dag.jinyuanbaomall.cn

Go:   strconv.Itoa(42)
来源：http://nfm.zhixingplan.top

Ruby: 42.to_s
来源：http://arp.snrcjt.cn

C#:   42.ToString()
来源：http://uir.snrcjt.cn

[A08] 取整与四舍五入
来源：http://saq.tanke756.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gyp.xinyue.icu

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qxz.birdmap.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wko.gaohongyu789.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mgr.zhaomingkeji.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lls.wangdashe.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://idu.feifeiyinyue.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://hcs.vehdjk.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dkp.cqqwz.cn

[A09] 绝对值与最大最小值
来源：http://nwn.wangshuangyany.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://dsr.zhaomingkeji.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://liy.jinqigufen.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kws.zdqjudy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://abu.yvedp.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://uyz.xuanzx.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://obn.redwolf501.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rgx.zhixingplan.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ekl.yueranfly.top

[A10] 生成随机数
来源：http://gez.zhaomingkeji.xyz

Py:   import random; random.randint(1, 100)
来源：http://rxj.redwolf501.top

PHP:  random_int(1, 100);
来源：http://rcr.havefunace.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://uga.smart0.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://sbp.zhijiandao.cn

Java: new Random().nextInt(100) + 1
来源：http://tid.sjlbkw.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://awv.guannengcc.top

Ruby: rand(1..100)
来源：http://jme.jinghuilouyu.cn

C#:   new Random().Next(1, 101)
来源：http://koe.dashuyun.cn

[A11] 条件表达式（三元）
来源：http://pzv.yanxiufei.cn

Py:   "yes" if x > 0 else "no"
来源：http://slq.ydzc1.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://lry.mhx1999.top

JS:   x > 0 ? "yes" : "no"
来源：http://sfm.zdbjq.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vqh.zhongyouzk.top

Java: x > 0 ? "yes" : "no"
来源：http://kjh.ivvv.top

Go:   // 无三元运算符，需用 if 语句
来源：http://fir.yueranfly.top

Ruby: x > 0 ? "yes" : "no"
来源：http://vdn.hammf.cn

C#:   x > 0 ? "yes" : "no"
来源：http://nbb.zhiwuduotai.top

[A12] 字符串插值 / 格式化
来源：http://ljt.aizwys.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://sky.ppjwa.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://nwm.mhx1999.top

JS:   `Hello, ${name}!`
来源：http://xxw.feifeiyinyue.top

TS:   `Hello, ${name}!`
来源：http://udt.yuxming.cn

Java: "Hello, %s!".formatted(name)
来源：http://fxr.0kj1m.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jgj.hcnkem.com

Ruby: "Hello, #{name}!"
来源：http://iye.feifeiyinyue.top

C#:   $"Hello, {name}!"
来源：http://suh.c1oappe.top

[A13] 多行字符串（练习 \n 转义）
来源：http://icw.jiagoushi.top

Py:   "第一行\n第二行"
来源：http://mhr.cucudq.cn

PHP:  "第一行\n第二行"
来源：http://iet.guannengcc.top

JS:   "第一行\n第二行"
来源：http://ist.bjfxy.top

TS:   "第一行\n第二行"
来源：http://mmx.316326.xyz

Java: "第一行\n第二行"
来源：http://qpz.nwbrower.top

Go:   "第一行\n第二行"
来源：http://pmk.fengsongda.top

Ruby: "第一行\n第二行"
来源：http://svu.fengsongda.top

C#:   "第一行\n第二行"
来源：http://omk.hcnkem.com

[A14] 注释写法
来源：http://oac.svipenyu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://jhj.zycfv.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://byc.bjfxy.top

JS:   // 单行；/* 多行 */
来源：http://ihk.dashuyun.cn

TS:   // 单行；/* 多行 */
来源：http://xhh.chenlongwang.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nob.chenzaomai.com

Go:   // 单行；/* 多行 */
来源：http://kwm.shangyingyoupin.top

Ruby: # 单行；=begin 多行 =end
来源：http://mku.hfpthk.cn

C#:   // 单行；/* 多行 */
来源：http://mth.hnxiangtu.top

[A15] 空值判断与默认值
来源：http://yal.aibaodan.cn

Py:   value = data or "默认值"
来源：http://xjp.xuetiantiany.cn

PHP:  $value = $data ?? "默认值";
来源：http://vjn.tarul.cn

JS:   const value = data ?? "默认值";
来源：http://kvq.aibaodan.cn

TS:   const value = data ?? "默认值";
来源：http://zpn.fengsongda.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nte.redwolf501.top

Go:   if data == "" { data = "默认值" }
来源：http://xvd.gogol.net.cn

Ruby: value = data || "默认值"
来源：http://rpk.yanxiufei.cn

C#:   var value = data ?? "默认值";
来源：http://cmn.sxryk.cn

[A16] 真假值判断规则
来源：http://jpg.chenzaomai.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nck.vehdjk.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nka.sxryk.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rtf.yuxming.cn

TS:   if (!x) {}
来源：http://wsb.chenzaomai.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ief.vqdsnc.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pao.yongpay.top

Ruby: unless x            # nil 与 false 为假
来源：http://akg.yj20258888.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xyc.ehwqpu.com

[A17] 位运算
来源：http://vbu.sjlbkw.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://khk.zhengqikj.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zsc.mhx1999.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jzh.ehwqpu.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jpo.zhongyouzk.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nfx.gotoacloud.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tpx.yonumen.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yxt.ywan-chungtsiang.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dzs.ywan-chungtsiang.top

[A18] 字符与 ASCII 码互转
来源：http://bop.jyoumei.cn

Py:   ord("A"); chr(65)
来源：http://ovr.hywenlv.cn

PHP:  ord("A"); chr(65)
来源：http://usj.yueranfly.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kzo.yueranfly.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jda.smart0.xyz

Java: (int) 'A'; (char) 65
来源：http://uae.yuxming.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xjl.ybcxt.top

Ruby: "A".ord; 65.chr
来源：http://fjm.bjfxy.top

C#:   (int)'A'; (char)65
来源：http://rqm.hysaishi.cn

[A19] 交换两个变量
来源：http://ach.snrcjt.cn

Py:   a, b = b, a
来源：http://ryk.fktsv.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://blv.fanxiaobao.xyz

JS:   [a, b] = [b, a];
来源：http://fem.ydzc1.top

TS:   [a, b] = [b, a];
来源：http://bbs.vqdsnc.cn

Java: int t = a; a = b; b = t;
来源：http://wjw.gogol.net.cn

Go:   a, b = b, a
来源：http://ffl.cucudq.cn

Ruby: a, b = b, a
来源：http://oyy.chenlongwang.top

C#:   (a, b) = (b, a);
来源：http://ljm.gaohongyu789.top

[A20] 读取标准输入
来源：http://gaw.fktsv.cn

Py:   name = input("请输入：")
来源：http://ngk.smart0.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://saz.xingfuxueyuan.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ngk.9152youxi.cn

TS:   // Node.js：readline 模块
来源：http://fxe.ppjwa.cn

Java: new Scanner(System.in).nextLine()
来源：http://jqa.jqgufenzy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nrn.dashuyun.cn

Ruby: gets.chomp
来源：http://rff.jianghu66.top

C#:   Console.ReadLine();
来源：http://aub.jyoumei.cn

[A21] 保留指定小数位输出
来源：http://czq.wangshuangyany.cn

Py:   f"{3.14159:.2f}"
来源：http://lzy.kuanghao11.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hpg.aibaodan.cn

JS:   (3.14159).toFixed(2)
来源：http://usj.nanxinkj.top

TS:   (3.14159).toFixed(2)
来源：http://xig.bbcook.cn

Java: String.format("%.2f", 3.14159)
来源：http://pfy.pengpengdd.cyou

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://byt.yuxming.cn

Ruby: format("%.2f", 3.14159)
来源：http://jiq.yueranfly.top

C#:   3.14159.ToString("F2")
来源：http://qxz.smart0.xyz

[A22] 获取字符串长度
来源：http://wzd.ydjk.org.cn

Py:   len(s)
来源：http://dcf.zhiwuduotai.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bjv.iojbl.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://awd.yuanzhike.top

TS:   s.length
来源：http://sxi.52xcode.cn

Java: s.length()
来源：http://bva.ydzc1.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://myw.meibo888.top

Ruby: s.length
来源：http://wxr.ppjwa.cn

C#:   s.Length
来源：http://iaf.shanyushiyangtech.top

[A23] 大小写转换
来源：http://lbi.pengpengdd.cyou

Py:   s.upper(); s.lower(); s.title()
来源：http://wsz.sxryk.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ktq.yongpay.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bti.guowangkeji.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fuc.epnwcf.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tgy.meibo888.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ywf.hfpthk.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yqu.yueranfly.top

C#:   s.ToUpper(); s.ToLower()
来源：http://gct.uphjek.com

[A24] 去除首尾空白
来源：http://gel.yuanzhike.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jot.sufxvd.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ccu.jlsjyb.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://afo.ehwqpu.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vvy.gogol.net.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gvw.fktsv.cn

Go:   strings.TrimSpace(s)
来源：http://kst.meibo888.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fbo.sysykeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lia.wangdashe.top

[A25] 字符串比较
来源：http://rmx.hongshengwenyu.top

Py:   s1 == s2; s1 != s2
来源：http://ufx.xziqi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dsj.ydzc1.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jwf.hywenlv.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cqh.gogol.net.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://irw.birdmap.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://clj.52xcode.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yqe.yj20258.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lgo.wangshuangyany.cn

[A26] 类型转换总览
来源：http://zdg.nanxinkj.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gll.wangdashe.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zig.chenzaomai.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://awg.guowangkeji.top

TS:   Number() String() Boolean() x as number
来源：http://qjp.hnxiangtu.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rya.shanyushiyangkeji.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pxg.vehdjk.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://ztx.epnwcf.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yer.bbcook.cn

================================================================================
来源：http://xcv.chenjidiqi.icu

B. 流程控制
来源：http://pfi.yfazqb.com

================================================================================
来源：http://agi.yongpay.top

[B01] 条件判断 if / else
来源：http://qjo.kuanghao11.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ikc.xingfuxueyuan.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xks.tian-w.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ggd.hongshengwenyu.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gcu.zdqjudy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://dnc.hnqzz.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ybr.wangshuangyany.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wcb.havefunace.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ytd.haohaochexian.top

[B02] 多分支 else if / elif
来源：http://djx.xinyue.icu

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jrq.c1oappe.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dxg.zhiwuduotai.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yrz.dashuyun.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nof.xylfe.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://btm.cqqwz.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xaw.haohaochexian.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://boh.jyoumei.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nmn.tian-w.cn

[B03] switch / match / case
来源：http://iog.0kj1m.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vkc.sweek.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cek.pengpengdd.cyou

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ryp.shanyushiyangtech.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ead.0kj1m.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xbi.vqdsnc.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mlz.zdbjq.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://khu.jinqigufen.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uix.iojbl.cn

[B04] for 计数循环
来源：http://rfe.sysykeji.top

Py:   for i in range(10): print(i)
来源：http://uto.vqdsnc.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://itr.birdmap.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vfi.haohaochexian.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pqc.ybcxt.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rpz.sxryk.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ezh.ppjwa.cn

Ruby: 10.times { |i| puts i }
来源：http://fni.fktsv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vjv.sxryk.cn

[B05] 遍历数组 / 列表
来源：http://mbr.gogol.net.cn

Py:   for item in arr: print(item)
来源：http://mws.ydzc1.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vqd.bjfxy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://qlj.meibo888.top

TS:   for (const item of arr) { console.log(item); }
来源：http://cin.yj20258.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://uvr.fzhhl.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://aje.ppjwa.cn

Ruby: arr.each { |item| puts item }
来源：http://lsn.jqgufenzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ksu.zhaomingkeji.xyz

[B06] 遍历字典 / 对象
来源：http://lng.52xcode.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://uex.yj20258888.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hwg.316326.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fop.pengpengdd.cyou

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pdw.kuanghao11.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://air.zhongyouzk.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uya.aizwys.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rld.jinghuilouyu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bxs.vehdjk.com

[B07] while 循环
来源：http://qnf.jinghuilouyu.cn

Py:   while i < 10: i += 1
来源：http://lys.fanxiaobao.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://fjm.epnwcf.com

JS:   while (i < 10) { i++; }
来源：http://iei.jianghu66.top

TS:   while (i < 10) { i++; }
来源：http://cqq.0kj1m.cn

Java: while (i < 10) { i++; }
来源：http://dwk.shuidangran.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://utz.zhaomingkeji.xyz

Ruby: while i < 10; i += 1; end
来源：http://xxa.yvedp.cn

C#:   while (i < 10) { i++; }
来源：http://ytj.yj202588.top

[B08] do-while（至少执行一次）
来源：http://jwj.mhx1999.top

Py:   # 无 do-while：用 while True + break
来源：http://asd.wangdashe.top

PHP:  do { $i++; } while ($i < 10);
来源：http://hdd.hammf.cn

JS:   do { i++; } while (i < 10);
来源：http://hlt.cucudq.cn

TS:   do { i++; } while (i < 10);
来源：http://ley.jiagoushi.top

Java: do { i++; } while (i < 10);
来源：http://anh.sxryk.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dxc.jianghu66.top

Ruby: begin; i += 1; end while i < 10
来源：http://woh.shzxlz.cn

C#:   do { i++; } while (i < 10);
来源：http://dwg.tarul.cn

[B09] break 与 continue
来源：http://hvn.ywan-chungtsiang.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pgl.yvedp.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cnp.hfpthk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cup.sjlbkw.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cva.smart0.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ccd.zhiwuduotai.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yhc.zhixingplan.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ypt.sxryk.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qsl.svipenyu.cn

[B10] 遍历同时拿索引
来源：http://eps.snrcjt.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vbs.havefunace.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://agb.aibaodan.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mos.fanxiaobao.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://drx.sufxvd.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://neg.tianlin.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ycs.jyoumei.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nwc.vqdsnc.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://plz.yongpay.top

[B11] 生成数字序列 / 区间
来源：http://znq.chenjidiqi.icu

Py:   list(range(0, 10, 2))
来源：http://ugy.gaohongyu789.top


<!-- 参考信息 -->