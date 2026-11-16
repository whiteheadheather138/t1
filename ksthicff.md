代发 wailian999

[A02] 变量声明与赋值
来源：http://tta.pengpengdd.cyou

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dhg.quarkkingdee.top

PHP:  $name = "Alex"; $age = 20;
来源：http://dpl.wangshuangyany.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qoc.hongshengwenyu.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ncu.jinqigfzy.top

Java: String name = "Alex"; int age = 20;
来源：http://pqa.aizwys.cn

Go:   name := "Alex"; age := 20
来源：http://leb.cheryme.top

Ruby: name = "Alex"; age = 20
来源：http://kav.bbcook.cn

C#:   string name = "Alex"; int age = 20;
来源：http://upl.sysykeji.top

[A03] 常量定义
来源：http://rei.dashuyun.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://oph.nwbrower.top

PHP:  const PI = 3.14159;
来源：http://kis.fengsongda.top

JS:   const PI = 3.14159;
来源：http://lmo.pengpengdd.cyou

TS:   const PI: number = 3.14159;
来源：http://iwm.sysykeji.top

Java: static final double PI = 3.14159;
来源：http://jsy.vehdjk.com

Go:   const PI = 3.14159
来源：http://yks.zhengqikj.top

Ruby: PI = 3.14159
来源：http://vsf.zdqjudy.top

C#:   const double PI = 3.14159;
来源：http://jta.tarul.cn

[A04] 判断变量类型
来源：http://dwv.jqgfzy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://pqx.gzhubu.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tnl.yongpay.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://amg.epnwcf.com

TS:   typeof x; x instanceof Date
来源：http://pwk.yanxiufei.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zns.hywenlv.cn

Go:   reflect.TypeOf(x).Name()
来源：http://qac.guannengcc.top

Ruby: x.class; x.is_a?(Integer)
来源：http://haf.yuxming.cn

C#:   x.GetType().Name; x is int
来源：http://tlz.hfpthk.cn

[A05] 整数除法与取模
来源：http://bmm.tian-w.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cww.cucudq.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://hsq.zhengqikj.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://aco.birdmap.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xpn.guannengcc.top

Java: 7 / 2; 7 % 2
来源：http://wjq.yj202588.top

Go:   7 / 2; 7 % 2
来源：http://sqf.aizwys.cn

Ruby: 7 / 2; 7 % 2
来源：http://nyh.zdbjq.cn

C#:   7 / 2; 7 % 2
来源：http://hvz.chenzaomai.com

[A06] 字符串转数字
来源：http://vfb.ctjpmb.com

Py:   int("42"); float("3.14")
来源：http://kgp.shzxlz.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://qfb.fktsv.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://rgv.hnxiangtu.top

TS:   parseInt("42", 10); Number("42")
来源：http://ggf.c1oappe.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wqg.hnqzz.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vef.yonumen.top

Ruby: "42".to_i; "3.14".to_f
来源：http://wtp.kuanghao11.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hsi.iojbl.cn

[A07] 数字转字符串
来源：http://qrl.wangshuangyany.cn

Py:   str(42)
来源：http://nmo.hnqzz.top

PHP:  (string) 42; strval(42)
来源：http://wfa.quarkkingdee.top

JS:   String(42); (42).toString()
来源：http://bmp.jiagoushi.top

TS:   String(42)
来源：http://dep.ivvv.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://oxj.ivvv.top

Go:   strconv.Itoa(42)
来源：http://efe.nanxinkj.top

Ruby: 42.to_s
来源：http://kiy.bbcook.cn

C#:   42.ToString()
来源：http://utb.meibo888.top

[A08] 取整与四舍五入
来源：http://cfs.shanyushiyangtech.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jna.gzhubu.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tgb.snrcjt.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xoc.guannengcc.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wmk.xingfuxueyuan.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tmw.zdqjudy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://iko.tanke756.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://cpx.chenzaomai.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hgj.jinqigufen.top

[A09] 绝对值与最大最小值
来源：http://lit.fehbvm.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pfk.ywan-chungtsiang.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bqa.tianlin.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mku.sxryk.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://uam.svipenyu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lon.cashguo.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zza.meibo888.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wlv.jiagoushi.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://iaz.xuanzx.com

[A10] 生成随机数
来源：http://hdi.yanxiufei.cn

Py:   import random; random.randint(1, 100)
来源：http://jdn.guannengcc.top

PHP:  random_int(1, 100);
来源：http://dwf.feifeiyinyue.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xer.svipenyu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://iwg.jinyuanbaomall.cn

Java: new Random().nextInt(100) + 1
来源：http://rrs.fzhhl.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://chi.tian-w.cn

Ruby: rand(1..100)
来源：http://mct.yueranfly.top

C#:   new Random().Next(1, 101)
来源：http://zzt.hysaishi.cn

[A11] 条件表达式（三元）
来源：http://ltq.hongshengwenyu.top

Py:   "yes" if x > 0 else "no"
来源：http://eyk.pengpengdd.cyou

PHP:  $x > 0 ? "yes" : "no"
来源：http://udv.wangshuangyany.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qfk.sufxvd.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xqk.quarkkingdee.top

Java: x > 0 ? "yes" : "no"
来源：http://tkm.hywenlv.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://cjl.xziqi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://sxw.9152youxi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ftf.nanxuanxn.top

[A12] 字符串插值 / 格式化
来源：http://vog.sjlbkw.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kbz.wangdashe.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lnw.aibaodan.cn

JS:   `Hello, ${name}!`
来源：http://ahv.iojbl.cn

TS:   `Hello, ${name}!`
来源：http://jbu.gaohongyu789.top

Java: "Hello, %s!".formatted(name)
来源：http://nfi.ydjk.org.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xmm.xuetiantiany.cn

Ruby: "Hello, #{name}!"
来源：http://mck.tanke756.top

C#:   $"Hello, {name}!"
来源：http://oqt.zhengqikj.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ocb.hfpthk.cn

Py:   "第一行\n第二行"
来源：http://lne.jqgfzy.top

PHP:  "第一行\n第二行"
来源：http://ghm.vehdjk.com

JS:   "第一行\n第二行"
来源：http://jod.xuanzx.com

TS:   "第一行\n第二行"
来源：http://qiv.zhaomingkeji.xyz

Java: "第一行\n第二行"
来源：http://bsi.havefunace.top

Go:   "第一行\n第二行"
来源：http://oik.nwbrower.top

Ruby: "第一行\n第二行"
来源：http://cnm.hcnkem.com

C#:   "第一行\n第二行"
来源：http://lzt.nanxinkj.top

[A14] 注释写法
来源：http://ewf.xuanzx.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://lvn.zycfv.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://gxg.52xcode.cn

JS:   // 单行；/* 多行 */
来源：http://vyj.sweek.top

TS:   // 单行；/* 多行 */
来源：http://qix.gotoacloud.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yvi.jinqigfzy.top

Go:   // 单行；/* 多行 */
来源：http://yun.jinghuilouyu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://snb.yuanzhike.top

C#:   // 单行；/* 多行 */
来源：http://tuy.kuanghao11.cn

[A15] 空值判断与默认值
来源：http://rpg.pengpengdd.cyou

Py:   value = data or "默认值"
来源：http://mby.sufxvd.cn

PHP:  $value = $data ?? "默认值";
来源：http://tel.dashuyun.cn

JS:   const value = data ?? "默认值";
来源：http://yqz.yuanzhike.top

TS:   const value = data ?? "默认值";
来源：http://ycr.tianlin.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://khp.wangdashe.top

Go:   if data == "" { data = "默认值" }
来源：http://iyq.jqgufenzy.top

Ruby: value = data || "默认值"
来源：http://aks.fktsv.cn

C#:   var value = data ?? "默认值";
来源：http://aju.jiagoushi.top

[A16] 真假值判断规则
来源：http://ukr.feifeiyinyue.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://eqo.zhiwuduotai.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://pup.ywan-chungtsiang.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bio.jqgufenzy.top

TS:   if (!x) {}
来源：http://scr.zhaomingkeji.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ued.zdbjq.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yqn.tian-w.cn

Ruby: unless x            # nil 与 false 为假
来源：http://mxf.zhijiandao.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ubo.aizwys.cn

[A17] 位运算
来源：http://akm.gogol.net.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://beb.zhaomingkeji.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://yqo.gzhubu.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ysj.pengpengdd.cyou

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xmd.zhaomingkeji.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zqw.tanke756.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gad.ydzc1.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mrc.gogol.net.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nvg.aizwys.cn

[A18] 字符与 ASCII 码互转
来源：http://uuj.cheryme.top

Py:   ord("A"); chr(65)
来源：http://zpg.dianchejie.cn

PHP:  ord("A"); chr(65)
来源：http://bvj.hysaishi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://upx.iojbl.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kue.havefunace.top

Java: (int) 'A'; (char) 65
来源：http://ulk.jinyuanbaomall.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zde.fehbvm.com

Ruby: "A".ord; 65.chr
来源：http://vsc.zdqjudy.top

C#:   (int)'A'; (char)65
来源：http://ivb.zhengqikj.top

[A19] 交换两个变量
来源：http://rtu.nanxuanxn.top

Py:   a, b = b, a
来源：http://amt.tian-w.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hrj.hesvh.cn

JS:   [a, b] = [b, a];
来源：http://xws.ivvv.top

TS:   [a, b] = [b, a];
来源：http://dkv.bbcook.cn

Java: int t = a; a = b; b = t;
来源：http://kwt.hammf.cn

Go:   a, b = b, a
来源：http://wnq.ydzc1.top

Ruby: a, b = b, a
来源：http://bxs.ctjpmb.com

C#:   (a, b) = (b, a);
来源：http://nej.ehwqpu.com

[A20] 读取标准输入
来源：http://tiq.yangfankeji.com

Py:   name = input("请输入：")
来源：http://epo.tianlin.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://xwi.xuanzx.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jhs.xylfe.cn

TS:   // Node.js：readline 模块
来源：http://ktv.sufxvd.cn

Java: new Scanner(System.in).nextLine()
来源：http://kuh.nanxinkj.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qsb.yuxming.cn

Ruby: gets.chomp
来源：http://agl.yj20258.top

C#:   Console.ReadLine();
来源：http://rxq.9152youxi.cn

[A21] 保留指定小数位输出
来源：http://cgf.jinqigufen.top

Py:   f"{3.14159:.2f}"
来源：http://gqk.hcnkem.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bso.mhx1999.top

JS:   (3.14159).toFixed(2)
来源：http://wkb.nanxuanxn.top

TS:   (3.14159).toFixed(2)
来源：http://edx.yj202588.top

Java: String.format("%.2f", 3.14159)
来源：http://als.ybcxt.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://asi.shuidangran.top

Ruby: format("%.2f", 3.14159)
来源：http://wqp.gotoacloud.top

C#:   3.14159.ToString("F2")
来源：http://quw.gaohongyu789.top

[A22] 获取字符串长度
来源：http://ayd.jianghu66.top

Py:   len(s)
来源：http://mnx.cdnleiting.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uqm.fktsv.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ggy.cheryme.top

TS:   s.length
来源：http://rqw.hammf.cn

Java: s.length()
来源：http://mem.sjlbkw.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tjt.birdmap.top

Ruby: s.length
来源：http://cwr.bbcook.cn

C#:   s.Length
来源：http://zov.quarkkingdee.top

[A23] 大小写转换
来源：http://czq.meibo888.top

Py:   s.upper(); s.lower(); s.title()
来源：http://lxw.zdbjq.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rmk.daria6918.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tnm.chenjidiqi.icu

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://apr.xziqi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://thm.yuxming.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vpy.fehbvm.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mtn.yongpay.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ntr.zhoulong.xyz

[A24] 去除首尾空白
来源：http://fqb.zhaomingkeji.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://aof.yvedp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cti.quarkkingdee.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qhu.snrcjt.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jtj.sufxvd.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jud.sweek.top

Go:   strings.TrimSpace(s)
来源：http://dgl.yj20258888.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nwe.fzhhl.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jfa.guowangkeji.top

[A25] 字符串比较
来源：http://nwg.fehbvm.com

Py:   s1 == s2; s1 != s2
来源：http://tmx.hongshengwenyu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://upk.52xcode.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vfb.haohaochexian.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qbi.quarkkingdee.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hll.zhengqikj.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://waw.gogol.net.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hhf.uphjek.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://suh.yonumen.top

[A26] 类型转换总览
来源：http://umc.hywenlv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wit.zhaomingkeji.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tbn.andypj.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dux.feifeiyinyue.top

TS:   Number() String() Boolean() x as number
来源：http://zpa.ctjpmb.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://aqb.wangdashe.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fqi.hnxiangtu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://guv.shanyushiyangkeji.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sse.snrcjt.cn

================================================================================
来源：http://oax.vqdsnc.cn

B. 流程控制
来源：http://lbm.mhx1999.top

================================================================================
来源：http://wnt.fengsongda.top

[B01] 条件判断 if / else
来源：http://pcg.gotoacloud.top

Py:   result = "正" if x > 0 else "非正"
来源：http://zsi.cqqwz.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xze.pycfn.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mur.zhixingplan.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hke.ybcxt.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://lqu.wangshuangyany.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bxp.guowangkeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nzz.jqgufenzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qrg.yfazqb.com

[B02] 多分支 else if / elif
来源：http://xyz.yanxiufei.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://djk.svipenyu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zhl.yangfankeji.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yvf.hnqzz.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jgk.dianchejie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lbe.zdqjudy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qlc.bjfxy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://set.zhixingplan.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vrw.ybcxt.top

[B03] switch / match / case
来源：http://ndt.ctjpmb.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kqe.9152youxi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lui.daxiang520.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tzk.9152youxi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iyu.sufxvd.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ecj.svipenyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://agq.jyoumei.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dlx.0kj1m.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://goh.wangshuangyany.cn

[B04] for 计数循环
来源：http://qfi.smart0.xyz

Py:   for i in range(10): print(i)
来源：http://ndi.birdmap.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fmt.shanyushiyangtech.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ypm.jyoumei.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rpg.vqdsnc.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://heu.meibo888.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fyi.shuidangran.top

Ruby: 10.times { |i| puts i }
来源：http://zwb.hfpthk.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kfn.jinghuilouyu.cn

[B05] 遍历数组 / 列表
来源：http://hbk.pengpengdd.cyou

Py:   for item in arr: print(item)
来源：http://dfs.tanke756.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nie.pycfn.com

JS:   for (const item of arr) { console.log(item); }
来源：http://wxk.yj202588.top

TS:   for (const item of arr) { console.log(item); }
来源：http://wzy.52xcode.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pgl.shangyingyoupin.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://oji.0kj1m.cn

Ruby: arr.each { |item| puts item }
来源：http://ivd.nanxuanxn.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ref.ivvv.top

[B06] 遍历字典 / 对象
来源：http://qbd.hammf.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://iwr.yuanzhike.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vpr.gzhubu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mca.jiagoushi.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://png.c1oappe.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ens.bjfxy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://moc.birdmap.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://grr.hesvh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lpb.ppjwa.cn

[B07] while 循环
来源：http://mph.jinqigufen.top

Py:   while i < 10: i += 1
来源：http://inh.dianchejie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ees.zhongyouzk.top

JS:   while (i < 10) { i++; }
来源：http://dab.hammf.cn

TS:   while (i < 10) { i++; }
来源：http://oyq.sufxvd.cn

Java: while (i < 10) { i++; }
来源：http://daa.jyoumei.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mvg.guowangkeji.top

Ruby: while i < 10; i += 1; end
来源：http://phc.jqgufenzy.top

C#:   while (i < 10) { i++; }
来源：http://myd.ivvv.top

[B08] do-while（至少执行一次）
来源：http://ulx.gogol.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://xsy.guannengcc.top

PHP:  do { $i++; } while ($i < 10);
来源：http://pgf.hfpthk.cn

JS:   do { i++; } while (i < 10);
来源：http://zkd.cucudq.cn

TS:   do { i++; } while (i < 10);
来源：http://tog.shzxlz.cn

Java: do { i++; } while (i < 10);
来源：http://yhf.jinghuilouyu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://kns.vehdjk.com

Ruby: begin; i += 1; end while i < 10
来源：http://hbs.tianlin.xyz

C#:   do { i++; } while (i < 10);
来源：http://nkb.ehwqpu.com


<!-- 参考信息 -->