代发 wailian999

Ruby: PI = 3.14159
来源：http://xei.pycfn.com

C#:   const double PI = 3.14159;
来源：http://gag.shanyushiyangkeji.top

[A04] 判断变量类型
来源：http://kjh.fehbvm.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://rqz.sxryk.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ick.iojbl.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tnp.cashguo.top

TS:   typeof x; x instanceof Date
来源：http://yju.feifeiyinyue.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cih.yonumen.top

Go:   reflect.TypeOf(x).Name()
来源：http://uef.yueranfly.top

Ruby: x.class; x.is_a?(Integer)
来源：http://mxn.52xcode.cn

C#:   x.GetType().Name; x is int
来源：http://jks.shuidangran.top

[A05] 整数除法与取模
来源：http://dwo.fengsongda.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nux.cheryme.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://wyq.cashguo.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gak.zhiwuduotai.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dfq.nanxuanxn.top

Java: 7 / 2; 7 % 2
来源：http://ljl.redwolf501.top

Go:   7 / 2; 7 % 2
来源：http://gzn.nanxinkj.top

Ruby: 7 / 2; 7 % 2
来源：http://fvz.dashuyun.cn

C#:   7 / 2; 7 % 2
来源：http://eph.yuxming.cn

[A06] 字符串转数字
来源：http://bub.yj20258.top

Py:   int("42"); float("3.14")
来源：http://yzc.uphjek.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://szy.jinghuilouyu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://oxl.andypj.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://aqf.fanxiaobao.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fku.xuanzx.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mfx.hesvh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wcs.fzhhl.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://imr.yangfankeji.com

[A07] 数字转字符串
来源：http://dlz.birdmap.top

Py:   str(42)
来源：http://wsu.cheryme.top

PHP:  (string) 42; strval(42)
来源：http://voe.chenlongwang.top

JS:   String(42); (42).toString()
来源：http://kbc.gotoacloud.top

TS:   String(42)
来源：http://xpj.xinyue.icu

Java: String.valueOf(42); Integer.toString(42)
来源：http://vsf.52xcode.cn

Go:   strconv.Itoa(42)
来源：http://plb.cheryme.top

Ruby: 42.to_s
来源：http://ybk.zhixingplan.top

C#:   42.ToString()
来源：http://rag.pengpengdd.cyou

[A08] 取整与四舍五入
来源：http://cwy.hysaishi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fyz.ppjwa.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cnd.yueranfly.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hdb.jlsjyb.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://thp.hesvh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xty.ydzc1.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://prk.gzhubu.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://gqk.tianlin.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bfm.ppjwa.cn

[A09] 绝对值与最大最小值
来源：http://huj.iojbl.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ttx.yangfankeji.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pnh.jinqigfzy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vfk.0kj1m.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yua.jinqigufen.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ufn.snrcjt.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mcu.sxryk.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ikz.jinyuanbaomall.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gcz.birdmap.top

[A10] 生成随机数
来源：http://bij.cqqwz.cn

Py:   import random; random.randint(1, 100)
来源：http://bbi.shanyushiyangtech.top

PHP:  random_int(1, 100);
来源：http://osl.yj202588.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://csi.52xcode.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://swk.9152youxi.cn

Java: new Random().nextInt(100) + 1
来源：http://deb.shangyingyoupin.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qfb.vqdsnc.cn

Ruby: rand(1..100)
来源：http://tcq.hongshengwenyu.top

C#:   new Random().Next(1, 101)
来源：http://ybz.guowangkeji.top

[A11] 条件表达式（三元）
来源：http://qgl.fzhhl.top

Py:   "yes" if x > 0 else "no"
来源：http://tng.bjfxy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://uaw.cheryme.top

JS:   x > 0 ? "yes" : "no"
来源：http://yoo.chenzaomai.com

TS:   x > 0 ? "yes" : "no"
来源：http://yeo.hongshengwenyu.top

Java: x > 0 ? "yes" : "no"
来源：http://jyj.vqdsnc.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://jtz.yongpay.top

Ruby: x > 0 ? "yes" : "no"
来源：http://pft.ybcxt.top

C#:   x > 0 ? "yes" : "no"
来源：http://epm.dashuyun.cn

[A12] 字符串插值 / 格式化
来源：http://wvh.ydjk.org.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://edi.mhx1999.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zof.tian-w.cn

JS:   `Hello, ${name}!`
来源：http://zif.shuidangran.top

TS:   `Hello, ${name}!`
来源：http://vzd.xuetiantiany.cn

Java: "Hello, %s!".formatted(name)
来源：http://wyj.ctjpmb.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xcv.ywan-chungtsiang.top

Ruby: "Hello, #{name}!"
来源：http://htx.fehbvm.com

C#:   $"Hello, {name}!"
来源：http://uhg.zhiwuduotai.top

[A13] 多行字符串（练习 \n 转义）
来源：http://rnu.yanxiufei.cn

Py:   "第一行\n第二行"
来源：http://tmd.cucudq.cn

PHP:  "第一行\n第二行"
来源：http://cgu.pengpengdd.cyou

JS:   "第一行\n第二行"
来源：http://hfs.feifeiyinyue.top

TS:   "第一行\n第二行"
来源：http://ljm.tarul.cn

Java: "第一行\n第二行"
来源：http://wrz.tianlin.xyz

Go:   "第一行\n第二行"
来源：http://vjg.yuxming.cn

Ruby: "第一行\n第二行"
来源：http://clp.uphjek.com

C#:   "第一行\n第二行"
来源：http://vzo.yangfankeji.com

[A14] 注释写法
来源：http://wiw.chenjidiqi.icu

Py:   # 单行；三引号字符串可作多行说明
来源：http://try.feifeiyinyue.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://yyj.zhongyouzk.top

JS:   // 单行；/* 多行 */
来源：http://kqw.316326.xyz

TS:   // 单行；/* 多行 */
来源：http://nlh.zhijiandao.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pft.redwolf501.top

Go:   // 单行；/* 多行 */
来源：http://zjz.zycfv.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qnh.xziqi.cn

C#:   // 单行；/* 多行 */
来源：http://bvh.aibaodan.cn

[A15] 空值判断与默认值
来源：http://nlr.aibaodan.cn

Py:   value = data or "默认值"
来源：http://wjx.yuxming.cn

PHP:  $value = $data ?? "默认值";
来源：http://bkv.cashguo.top

JS:   const value = data ?? "默认值";
来源：http://umh.316326.xyz

TS:   const value = data ?? "默认值";
来源：http://lqh.xylfe.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://csq.0kj1m.cn

Go:   if data == "" { data = "默认值" }
来源：http://giw.jlsjyb.cn

Ruby: value = data || "默认值"
来源：http://ixc.cashguo.top

C#:   var value = data ?? "默认值";
来源：http://pto.ivvv.top

[A16] 真假值判断规则
来源：http://exc.snrcjt.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mnl.snrcjt.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://acq.sweek.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rod.yj20258.top

TS:   if (!x) {}
来源：http://hab.shanyushiyangkeji.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tsz.gotoacloud.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zkq.chenjidiqi.icu

Ruby: unless x            # nil 与 false 为假
来源：http://yym.xinyue.icu

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mll.chenjidiqi.icu

[A17] 位运算
来源：http://rvo.yvedp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://phw.zhaomingkeji.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://snj.uphjek.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mvf.yuanzhike.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cdi.shangyingyoupin.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://flr.sjlbkw.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://awg.hcnkem.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lyn.meibo888.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pdl.tian-w.cn

[A18] 字符与 ASCII 码互转
来源：http://mef.ywan-chungtsiang.top

Py:   ord("A"); chr(65)
来源：http://hva.ivvv.top

PHP:  ord("A"); chr(65)
来源：http://flj.nanxuanxn.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://esx.shanyushiyangkeji.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://voh.nanxinkj.top

Java: (int) 'A'; (char) 65
来源：http://zeb.yanxiufei.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://uik.smart0.xyz

Ruby: "A".ord; 65.chr
来源：http://ajm.bbcook.cn

C#:   (int)'A'; (char)65
来源：http://hmc.sxryk.cn

[A19] 交换两个变量
来源：http://lgs.sjlbkw.cn

Py:   a, b = b, a
来源：http://gba.jianghu66.top

PHP:  [$a, $b] = [$b, $a];
来源：http://plr.jianghu66.top

JS:   [a, b] = [b, a];
来源：http://zbu.zhijiandao.cn

TS:   [a, b] = [b, a];
来源：http://qhj.shzxlz.cn

Java: int t = a; a = b; b = t;
来源：http://esp.tian-w.cn

Go:   a, b = b, a
来源：http://alm.jinyuanbaomall.cn

Ruby: a, b = b, a
来源：http://sye.haohaochexian.top

C#:   (a, b) = (b, a);
来源：http://tev.xuanzx.com

[A20] 读取标准输入
来源：http://fge.sxryk.cn

Py:   name = input("请输入：")
来源：http://xid.c1oappe.top

PHP:  $name = trim(fgets(STDIN));
来源：http://xqc.jinghuilouyu.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vaj.yuxming.cn

TS:   // Node.js：readline 模块
来源：http://hli.wangshuangyany.cn

Java: new Scanner(System.in).nextLine()
来源：http://fop.shzxlz.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vkw.tanke756.top

Ruby: gets.chomp
来源：http://xip.cdnleiting.top

C#:   Console.ReadLine();
来源：http://vwi.jqgfzy.top

[A21] 保留指定小数位输出
来源：http://kdq.sysykeji.top

Py:   f"{3.14159:.2f}"
来源：http://dsj.cqqwz.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kar.yj20258888.top

JS:   (3.14159).toFixed(2)
来源：http://ycc.bbcook.cn

TS:   (3.14159).toFixed(2)
来源：http://mur.jinqigufen.top

Java: String.format("%.2f", 3.14159)
来源：http://eke.c1oappe.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://eag.nanxuanxn.top

Ruby: format("%.2f", 3.14159)
来源：http://uxm.wangshuangyany.cn

C#:   3.14159.ToString("F2")
来源：http://ncm.ywan-chungtsiang.top

[A22] 获取字符串长度
来源：http://saz.yonumen.top

Py:   len(s)
来源：http://qjs.ivvv.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zhl.bbcook.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lnq.hywenlv.cn

TS:   s.length
来源：http://kgq.vehdjk.com

Java: s.length()
来源：http://yhy.cucudq.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mdq.zdbjq.cn

Ruby: s.length
来源：http://qaw.sufxvd.cn

C#:   s.Length
来源：http://exm.shangyingyoupin.top

[A23] 大小写转换
来源：http://uib.aibaodan.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://oic.jinqigfzy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vfx.smart0.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xqu.tian-w.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ohs.dianchejie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nxb.ydzc1.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mjv.yj20258.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qka.hammf.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ius.hcnkem.com

[A24] 去除首尾空白
来源：http://mtx.cashguo.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://iyu.chenlongwang.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://oce.pycfn.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yel.meibo888.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rbd.yfazqb.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://iiz.pycfn.com

Go:   strings.TrimSpace(s)
来源：http://xnp.redwolf501.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://awk.sysykeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://olu.guowangkeji.top

[A25] 字符串比较
来源：http://ord.zdbjq.cn

Py:   s1 == s2; s1 != s2
来源：http://qxi.jlsjyb.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fyg.hysaishi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ieu.pengpengdd.cyou

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://flz.xinyue.icu

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ckb.ybcxt.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gde.hnxiangtu.top

Ruby: s1 == s2; s1 <=> s2
来源：http://bgy.guowangkeji.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uqy.jinghuilouyu.cn

[A26] 类型转换总览
来源：http://dtu.jyoumei.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rmh.ppjwa.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lcx.yongpay.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ecq.yj20258888.top

TS:   Number() String() Boolean() x as number
来源：http://sud.fehbvm.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ert.xziqi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jlf.sysykeji.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://vzl.jqgfzy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zpd.daxiang520.top

================================================================================
来源：http://ezh.uphjek.com

B. 流程控制
来源：http://vwy.shuidangran.top

================================================================================
来源：http://wza.jinqigufen.top

[B01] 条件判断 if / else
来源：http://eff.tian-w.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://inq.0kj1m.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://auf.shangyingyoupin.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bwl.birdmap.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tmx.yuanzhike.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ekp.shangyingyoupin.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gzg.ehwqpu.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hpa.yangfankeji.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nph.fehbvm.com

[B02] 多分支 else if / elif
来源：http://fgg.yvedp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vzg.fzhhl.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yma.ctjpmb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://var.yfazqb.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://djc.aizwys.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qxf.haohaochexian.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sob.zhongyouzk.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fqc.jinqigfzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tss.ydjk.org.cn

[B03] switch / match / case
来源：http://iyv.hongshengwenyu.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://non.fktsv.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://azi.haohaochexian.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tjo.xinyue.icu

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aoo.daria6918.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dld.cdnleiting.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qnl.yuanzhike.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zfa.hnxiangtu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cdu.ybcxt.top

[B04] for 计数循环
来源：http://jsa.havefunace.top

Py:   for i in range(10): print(i)
来源：http://yer.9152youxi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://aio.9152youxi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sof.chenjidiqi.icu

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zrt.vehdjk.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yhb.vehdjk.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rog.xinyue.icu

Ruby: 10.times { |i| puts i }
来源：http://jri.zhijiandao.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nip.redwolf501.top

[B05] 遍历数组 / 列表
来源：http://pev.ivvv.top

Py:   for item in arr: print(item)
来源：http://yzp.0kj1m.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kxj.xylfe.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gwq.yuxming.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://abp.zycfv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kqr.fzhhl.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ogk.52xcode.cn

Ruby: arr.each { |item| puts item }
来源：http://ggx.yonumen.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ltj.wangdashe.top

[B06] 遍历字典 / 对象
来源：http://mzg.gogol.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vdi.feifeiyinyue.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gua.316326.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oqi.tanke756.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://spo.mhx1999.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wwx.yvedp.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yyo.yj202588.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yeq.guowangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mal.yuxming.cn

[B07] while 循环
来源：http://zba.hcnkem.com

Py:   while i < 10: i += 1
来源：http://qth.ydjk.org.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gon.nanxinkj.top

JS:   while (i < 10) { i++; }
来源：http://gio.yuxming.cn

TS:   while (i < 10) { i++; }
来源：http://jul.snrcjt.cn

Java: while (i < 10) { i++; }
来源：http://btt.daria6918.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kli.sxryk.cn

Ruby: while i < 10; i += 1; end
来源：http://ost.zhaomingkeji.xyz

C#:   while (i < 10) { i++; }
来源：http://zck.jlsjyb.cn

[B08] do-while（至少执行一次）
来源：http://wxg.iojbl.cn

Py:   # 无 do-while：用 while True + break
来源：http://zdl.jinghuilouyu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://eex.0kj1m.cn

JS:   do { i++; } while (i < 10);
来源：http://htj.vehdjk.com

TS:   do { i++; } while (i < 10);
来源：http://hvw.ybcxt.top

Java: do { i++; } while (i < 10);
来源：http://ony.dashuyun.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://twb.pycfn.com

Ruby: begin; i += 1; end while i < 10
来源：http://afg.316326.xyz

C#:   do { i++; } while (i < 10);
来源：http://rsb.xingfuxueyuan.xyz

[B09] break 与 continue
来源：http://ynj.havefunace.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://csn.jqgfzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mxa.jinqigufen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jnk.wangdashe.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gnz.tanke756.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yvr.xinyue.icu

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uts.birdmap.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kzf.9152youxi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gwj.cashguo.top

[B10] 遍历同时拿索引
来源：http://xqy.yongpay.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nyh.jinqigfzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wwo.hcnkem.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://alh.sxryk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oym.vehdjk.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://eaf.gotoacloud.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uhv.zycfv.cn


<!-- 参考信息 -->