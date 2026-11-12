代发 wailian999

Ruby: PI = 3.14159
来源：http://sny.ppjwa.cn

C#:   const double PI = 3.14159;
来源：http://idd.mhx1999.top

[A04] 判断变量类型
来源：http://vua.0kj1m.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://lhk.snrcjt.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zqs.yj20258.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ygc.nanxuanxn.top

TS:   typeof x; x instanceof Date
来源：http://yoi.hesvh.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jsa.gotoacloud.top

Go:   reflect.TypeOf(x).Name()
来源：http://ike.zdqjudy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ryv.xziqi.cn

C#:   x.GetType().Name; x is int
来源：http://hld.zhiwuduotai.top

[A05] 整数除法与取模
来源：http://hrl.svipenyu.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rdp.zhixingplan.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://whm.wangshuangyany.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lau.hammf.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://avg.yueranfly.top

Java: 7 / 2; 7 % 2
来源：http://wsy.yj202588.top

Go:   7 / 2; 7 % 2
来源：http://zfa.tianlin.xyz

Ruby: 7 / 2; 7 % 2
来源：http://iki.redwolf501.top

C#:   7 / 2; 7 % 2
来源：http://yue.zhaomingkeji.xyz

[A06] 字符串转数字
来源：http://hng.tian-w.cn

Py:   int("42"); float("3.14")
来源：http://var.pengpengdd.cyou

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rmz.fktsv.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://chp.yfazqb.com

TS:   parseInt("42", 10); Number("42")
来源：http://jin.jinqigfzy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://giv.chenjidiqi.icu

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ikt.fehbvm.com

Ruby: "42".to_i; "3.14".to_f
来源：http://vos.feifeiyinyue.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://diq.fanxiaobao.xyz

[A07] 数字转字符串
来源：http://hiw.xuanzx.com

Py:   str(42)
来源：http://fjc.zhijiandao.cn

PHP:  (string) 42; strval(42)
来源：http://krt.meibo888.top

JS:   String(42); (42).toString()
来源：http://dtl.yuxming.cn

TS:   String(42)
来源：http://pbo.zhongyouzk.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://iod.yvedp.cn

Go:   strconv.Itoa(42)
来源：http://krj.jlsjyb.cn

Ruby: 42.to_s
来源：http://rpt.guannengcc.top

C#:   42.ToString()
来源：http://krg.hnqzz.top

[A08] 取整与四舍五入
来源：http://fae.shangyingyoupin.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qkr.hysaishi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wmp.zhaomingkeji.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ykf.hywenlv.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://smz.cucudq.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yoq.smart0.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fpo.andypj.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://vmw.xingfuxueyuan.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fht.jlsjyb.cn

[A09] 绝对值与最大最小值
来源：http://qep.bbcook.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://evn.yuanzhike.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://slq.jinyuanbaomall.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://exm.mhx1999.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ulb.hammf.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rcl.gogol.net.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hga.xziqi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kom.sjlbkw.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wem.ywan-chungtsiang.top

[A10] 生成随机数
来源：http://hve.ivvv.top

Py:   import random; random.randint(1, 100)
来源：http://iab.xylfe.cn

PHP:  random_int(1, 100);
来源：http://ttg.aizwys.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://swo.zhaomingkeji.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tyq.yj20258888.top

Java: new Random().nextInt(100) + 1
来源：http://hhe.shuidangran.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gei.nwbrower.top

Ruby: rand(1..100)
来源：http://qjj.yangfankeji.com

C#:   new Random().Next(1, 101)
来源：http://hcl.jianghu66.top

[A11] 条件表达式（三元）
来源：http://dwx.yuxming.cn

Py:   "yes" if x > 0 else "no"
来源：http://jng.shanyushiyangtech.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://uvr.guowangkeji.top

JS:   x > 0 ? "yes" : "no"
来源：http://hkk.shanyushiyangkeji.top

TS:   x > 0 ? "yes" : "no"
来源：http://nyj.hfpthk.cn

Java: x > 0 ? "yes" : "no"
来源：http://eri.daxiang520.top

Go:   // 无三元运算符，需用 if 语句
来源：http://dkh.bbcook.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jco.vqdsnc.cn

C#:   x > 0 ? "yes" : "no"
来源：http://tws.meibo888.top

[A12] 字符串插值 / 格式化
来源：http://jfs.svipenyu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pzn.wangshuangyany.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vcc.tianlin.xyz

JS:   `Hello, ${name}!`
来源：http://waf.c1oappe.top

TS:   `Hello, ${name}!`
来源：http://pwz.chenlongwang.top

Java: "Hello, %s!".formatted(name)
来源：http://had.zhixingplan.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ahj.bbcook.cn

Ruby: "Hello, #{name}!"
来源：http://xik.jiagoushi.top

C#:   $"Hello, {name}!"
来源：http://sea.316326.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://mhw.birdmap.top

Py:   "第一行\n第二行"
来源：http://xgm.cashguo.top

PHP:  "第一行\n第二行"
来源：http://vnw.zhijiandao.cn

JS:   "第一行\n第二行"
来源：http://vsg.jiagoushi.top

TS:   "第一行\n第二行"
来源：http://mlc.zhongyouzk.top

Java: "第一行\n第二行"
来源：http://mtk.zhengqikj.top

Go:   "第一行\n第二行"
来源：http://hsa.birdmap.top

Ruby: "第一行\n第二行"
来源：http://zgp.chenjidiqi.icu

C#:   "第一行\n第二行"
来源：http://dyf.jinyuanbaomall.cn

[A14] 注释写法
来源：http://cwc.nwbrower.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://waw.yj20258.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ngf.jianghu66.top

JS:   // 单行；/* 多行 */
来源：http://bdn.dashuyun.cn

TS:   // 单行；/* 多行 */
来源：http://fzt.aizwys.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ywt.ctjpmb.com

Go:   // 单行；/* 多行 */
来源：http://pgz.shanyushiyangkeji.top

Ruby: # 单行；=begin 多行 =end
来源：http://rot.daxiang520.top

C#:   // 单行；/* 多行 */
来源：http://wnd.gotoacloud.top

[A15] 空值判断与默认值
来源：http://euk.yuanzhike.top

Py:   value = data or "默认值"
来源：http://unb.yangfankeji.com

PHP:  $value = $data ?? "默认值";
来源：http://iqt.wangdashe.top

JS:   const value = data ?? "默认值";
来源：http://nhr.zhiwuduotai.top

TS:   const value = data ?? "默认值";
来源：http://fzn.jinghuilouyu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://duk.tanke756.top

Go:   if data == "" { data = "默认值" }
来源：http://ari.vqdsnc.cn

Ruby: value = data || "默认值"
来源：http://dew.52xcode.cn

C#:   var value = data ?? "默认值";
来源：http://osy.kuanghao11.cn

[A16] 真假值判断规则
来源：http://ptb.haohaochexian.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cla.zdqjudy.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://uap.zhixingplan.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dwh.ybcxt.top

TS:   if (!x) {}
来源：http://bdf.jinyuanbaomall.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://efw.xinyue.icu

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lib.316326.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://ugx.birdmap.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mia.guowangkeji.top

[A17] 位运算
来源：http://wue.nanxuanxn.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ory.kuanghao11.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rny.meibo888.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xvf.chenlongwang.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gab.wangshuangyany.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qwm.cdnleiting.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://twq.zhaomingkeji.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jvk.zycfv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gil.ppjwa.cn

[A18] 字符与 ASCII 码互转
来源：http://nst.hfpthk.cn

Py:   ord("A"); chr(65)
来源：http://wtr.guannengcc.top

PHP:  ord("A"); chr(65)
来源：http://tsa.cqqwz.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jpt.zhengqikj.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bjn.ivvv.top

Java: (int) 'A'; (char) 65
来源：http://rsg.fzhhl.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uqx.hcnkem.com

Ruby: "A".ord; 65.chr
来源：http://kxp.yueranfly.top

C#:   (int)'A'; (char)65
来源：http://tnb.gotoacloud.top

[A19] 交换两个变量
来源：http://znb.jianghu66.top

Py:   a, b = b, a
来源：http://itu.zhijiandao.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://cno.ppjwa.cn

JS:   [a, b] = [b, a];
来源：http://jni.mhx1999.top

TS:   [a, b] = [b, a];
来源：http://emb.ydjk.org.cn

Java: int t = a; a = b; b = t;
来源：http://biq.ydjk.org.cn

Go:   a, b = b, a
来源：http://yhy.cucudq.cn

Ruby: a, b = b, a
来源：http://qte.yonumen.top

C#:   (a, b) = (b, a);
来源：http://glu.yj20258.top

[A20] 读取标准输入
来源：http://igr.guannengcc.top

Py:   name = input("请输入：")
来源：http://nec.ywan-chungtsiang.top

PHP:  $name = trim(fgets(STDIN));
来源：http://jtk.chenlongwang.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://red.cheryme.top

TS:   // Node.js：readline 模块
来源：http://lsa.zhongyouzk.top

Java: new Scanner(System.in).nextLine()
来源：http://old.bjfxy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fdo.yj202588.top

Ruby: gets.chomp
来源：http://izd.jianghu66.top

C#:   Console.ReadLine();
来源：http://rxk.sjlbkw.cn

[A21] 保留指定小数位输出
来源：http://mkc.birdmap.top

Py:   f"{3.14159:.2f}"
来源：http://uwy.zhaomingkeji.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gnn.guannengcc.top

JS:   (3.14159).toFixed(2)
来源：http://xpw.yuxming.cn

TS:   (3.14159).toFixed(2)
来源：http://xac.birdmap.top

Java: String.format("%.2f", 3.14159)
来源：http://lto.redwolf501.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://orn.fzhhl.top

Ruby: format("%.2f", 3.14159)
来源：http://mgt.snrcjt.cn

C#:   3.14159.ToString("F2")
来源：http://bqz.gzhubu.top

[A22] 获取字符串长度
来源：http://ioz.snrcjt.cn

Py:   len(s)
来源：http://kyy.dianchejie.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pao.jyoumei.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lnh.tian-w.cn

TS:   s.length
来源：http://hcx.zhaomingkeji.xyz

Java: s.length()
来源：http://dzw.dashuyun.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lux.ehwqpu.com

Ruby: s.length
来源：http://upv.pengpengdd.cyou

C#:   s.Length
来源：http://jcu.shuidangran.top

[A23] 大小写转换
来源：http://lir.cheryme.top

Py:   s.upper(); s.lower(); s.title()
来源：http://aum.iojbl.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dtw.jqgufenzy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zqn.vehdjk.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ozc.daxiang520.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ggb.chenzaomai.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dlm.hysaishi.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://otm.yonumen.top

C#:   s.ToUpper(); s.ToLower()
来源：http://pfh.yj202588.top

[A24] 去除首尾空白
来源：http://odz.chenjidiqi.icu

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nrl.52xcode.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zjk.zhiwuduotai.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gxq.zdqjudy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://knv.quarkkingdee.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dav.c1oappe.top

Go:   strings.TrimSpace(s)
来源：http://gil.yuxming.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://way.zhoulong.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cuu.dianchejie.cn

[A25] 字符串比较
来源：http://uhe.wangdashe.top

Py:   s1 == s2; s1 != s2
来源：http://fzj.cashguo.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zei.vehdjk.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ftc.havefunace.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zxf.cdnleiting.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://whw.yuxming.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ynf.gogol.net.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://dbn.svipenyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ffd.sysykeji.top

[A26] 类型转换总览
来源：http://mmf.sysykeji.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ory.jinghuilouyu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hiq.xinyue.icu

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xgk.cdnleiting.top

TS:   Number() String() Boolean() x as number
来源：http://rrz.fzhhl.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mlq.ydzc1.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lnd.zdbjq.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mib.dianchejie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://grg.ywan-chungtsiang.top

================================================================================
来源：http://tqz.guannengcc.top

B. 流程控制
来源：http://ddw.xylfe.cn

================================================================================
来源：http://xte.chenjidiqi.icu

[B01] 条件判断 if / else
来源：http://ktq.9152youxi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://elo.chenjidiqi.icu

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://muj.yj20258888.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://flz.vqdsnc.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wlb.aibaodan.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fvc.sweek.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://udc.chenlongwang.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dbm.ctjpmb.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fim.jinqigfzy.top

[B02] 多分支 else if / elif
来源：http://ltj.gzhubu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zmd.vehdjk.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lwo.zhongyouzk.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://icz.gzhubu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://spd.hnxiangtu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zhq.zhiwuduotai.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://oke.quarkkingdee.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nox.cdnleiting.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mvx.yueranfly.top

[B03] switch / match / case
来源：http://qhs.vehdjk.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dmg.guowangkeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://chi.9152youxi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ljw.hongshengwenyu.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sxb.hywenlv.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lps.shangyingyoupin.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fyn.hesvh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ouk.shuidangran.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ahu.fzhhl.top

[B04] for 计数循环
来源：http://koe.tian-w.cn

Py:   for i in range(10): print(i)
来源：http://hxq.daria6918.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fyl.ybcxt.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yuz.uphjek.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ftd.xylfe.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bdq.jinqigufen.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yqy.zdqjudy.top

Ruby: 10.times { |i| puts i }
来源：http://xno.bbcook.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lgv.nwbrower.top

[B05] 遍历数组 / 列表
来源：http://lgu.nanxuanxn.top

Py:   for item in arr: print(item)
来源：http://keh.jiagoushi.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dap.hfpthk.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://eob.hongshengwenyu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://cdn.sxryk.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://feq.svipenyu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ubh.ydjk.org.cn

Ruby: arr.each { |item| puts item }
来源：http://kok.yvedp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dmx.xingfuxueyuan.xyz

[B06] 遍历字典 / 对象
来源：http://fad.316326.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://tre.zhoulong.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mae.xylfe.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fsn.redwolf501.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aeb.gogol.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sfl.hfpthk.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wkd.ivvv.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ekd.jinyuanbaomall.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ybp.yj202588.top

[B07] while 循环
来源：http://ign.316326.xyz

Py:   while i < 10: i += 1
来源：http://uxu.zhengqikj.top

PHP:  while ($i < 10) { $i++; }
来源：http://lcl.chenlongwang.top

JS:   while (i < 10) { i++; }
来源：http://lwd.yueranfly.top

TS:   while (i < 10) { i++; }
来源：http://hlc.ybcxt.top

Java: while (i < 10) { i++; }
来源：http://hot.zhiwuduotai.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://drr.52xcode.cn

Ruby: while i < 10; i += 1; end
来源：http://kis.jlsjyb.cn

C#:   while (i < 10) { i++; }
来源：http://oha.epnwcf.com

[B08] do-while（至少执行一次）
来源：http://hgn.c1oappe.top

Py:   # 无 do-while：用 while True + break
来源：http://upb.xinyue.icu

PHP:  do { $i++; } while ($i < 10);
来源：http://imy.guowangkeji.top

JS:   do { i++; } while (i < 10);
来源：http://rig.gzhubu.top

TS:   do { i++; } while (i < 10);
来源：http://dua.jinghuilouyu.cn

Java: do { i++; } while (i < 10);
来源：http://ffo.shzxlz.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dln.jiagoushi.top

Ruby: begin; i += 1; end while i < 10
来源：http://ysf.jinqigfzy.top

C#:   do { i++; } while (i < 10);
来源：http://jkq.yangfankeji.com

[B09] break 与 continue
来源：http://fbx.sufxvd.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ykp.jlsjyb.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xjh.ywan-chungtsiang.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zbp.sweek.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://exe.jiagoushi.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hdu.sufxvd.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ajo.zhaomingkeji.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fie.wangdashe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xod.jinyuanbaomall.cn

[B10] 遍历同时拿索引
来源：http://sql.jinqigufen.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bdo.gogol.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ujc.daria6918.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zlr.yj20258888.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dmr.316326.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gnf.vqdsnc.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gcv.cheryme.top


<!-- 参考信息 -->