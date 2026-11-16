代发 wailian999

Ruby: PI = 3.14159
来源：http://htx.redwolf501.top

C#:   const double PI = 3.14159;
来源：http://utv.zhengqikj.top

[A04] 判断变量类型
来源：http://yxg.zhixingplan.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://ttg.jqgufenzy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://eyy.yanxiufei.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://yux.shzxlz.cn

TS:   typeof x; x instanceof Date
来源：http://cvd.hcnkem.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fvs.ivvv.top

Go:   reflect.TypeOf(x).Name()
来源：http://zcj.yvedp.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hbx.sweek.top

C#:   x.GetType().Name; x is int
来源：http://ihu.daxiang520.top

[A05] 整数除法与取模
来源：http://mfz.redwolf501.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bpt.jlsjyb.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zuj.chenjidiqi.icu

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nia.shanyushiyangkeji.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bfk.gaohongyu789.top

Java: 7 / 2; 7 % 2
来源：http://hcd.haohaochexian.top

Go:   7 / 2; 7 % 2
来源：http://cas.bbcook.cn

Ruby: 7 / 2; 7 % 2
来源：http://wms.cdnleiting.top

C#:   7 / 2; 7 % 2
来源：http://cuu.yfazqb.com

[A06] 字符串转数字
来源：http://fkh.yonumen.top

Py:   int("42"); float("3.14")
来源：http://hav.ydzc1.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bhe.cheryme.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zox.iojbl.cn

TS:   parseInt("42", 10); Number("42")
来源：http://rci.vehdjk.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://szn.jqgufenzy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://vwn.smart0.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://cny.zhixingplan.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zad.yvedp.cn

[A07] 数字转字符串
来源：http://gqt.birdmap.top

Py:   str(42)
来源：http://bdf.cashguo.top

PHP:  (string) 42; strval(42)
来源：http://wgz.pengpengdd.cyou

JS:   String(42); (42).toString()
来源：http://ahc.jinyuanbaomall.cn

TS:   String(42)
来源：http://lwk.iojbl.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://unv.ybcxt.top

Go:   strconv.Itoa(42)
来源：http://zen.redwolf501.top

Ruby: 42.to_s
来源：http://fbs.yuanzhike.top

C#:   42.ToString()
来源：http://atw.yonumen.top

[A08] 取整与四舍五入
来源：http://wsf.jinyuanbaomall.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cxg.svipenyu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pxh.jinqigfzy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nhq.jianghu66.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cir.sufxvd.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://msc.cucudq.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zch.c1oappe.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://qlk.zdqjudy.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://fdh.316326.xyz

[A09] 绝对值与最大最小值
来源：http://sxj.feifeiyinyue.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ffr.zhijiandao.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://zce.havefunace.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gqk.epnwcf.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tao.xuetiantiany.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kix.nwbrower.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hwl.cucudq.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://agp.jianghu66.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xib.meibo888.top

[A10] 生成随机数
来源：http://rnv.shanyushiyangkeji.top

Py:   import random; random.randint(1, 100)
来源：http://gur.chenlongwang.top

PHP:  random_int(1, 100);
来源：http://bid.zhongyouzk.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://oju.gogol.net.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vyk.hnqzz.top

Java: new Random().nextInt(100) + 1
来源：http://hhj.ywan-chungtsiang.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yuq.aizwys.cn

Ruby: rand(1..100)
来源：http://lcv.pycfn.com

C#:   new Random().Next(1, 101)
来源：http://gil.316326.xyz

[A11] 条件表达式（三元）
来源：http://oac.mhx1999.top

Py:   "yes" if x > 0 else "no"
来源：http://wfo.tian-w.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ley.yuxming.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xgo.hammf.cn

TS:   x > 0 ? "yes" : "no"
来源：http://bdi.chenjidiqi.icu

Java: x > 0 ? "yes" : "no"
来源：http://uju.yongpay.top

Go:   // 无三元运算符，需用 if 语句
来源：http://iyc.andypj.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://srg.9152youxi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://meb.52xcode.cn

[A12] 字符串插值 / 格式化
来源：http://jck.ydzc1.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mik.cucudq.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cva.hammf.cn

JS:   `Hello, ${name}!`
来源：http://wod.mhx1999.top

TS:   `Hello, ${name}!`
来源：http://snl.fanxiaobao.xyz

Java: "Hello, %s!".formatted(name)
来源：http://mvs.dianchejie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fxb.epnwcf.com

Ruby: "Hello, #{name}!"
来源：http://sbr.quarkkingdee.top

C#:   $"Hello, {name}!"
来源：http://ftd.ybcxt.top

[A13] 多行字符串（练习 \n 转义）
来源：http://toj.xziqi.cn

Py:   "第一行\n第二行"
来源：http://hbi.tianlin.xyz

PHP:  "第一行\n第二行"
来源：http://itu.ehwqpu.com

JS:   "第一行\n第二行"
来源：http://cbe.hfpthk.cn

TS:   "第一行\n第二行"
来源：http://adh.haohaochexian.top

Java: "第一行\n第二行"
来源：http://ppo.chenjidiqi.icu

Go:   "第一行\n第二行"
来源：http://zah.birdmap.top

Ruby: "第一行\n第二行"
来源：http://uam.smart0.xyz

C#:   "第一行\n第二行"
来源：http://jka.yuanzhike.top

[A14] 注释写法
来源：http://uxm.cdnleiting.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ary.daria6918.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://bnb.yuanzhike.top

JS:   // 单行；/* 多行 */
来源：http://mai.ivvv.top

TS:   // 单行；/* 多行 */
来源：http://bpv.epnwcf.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ynu.snrcjt.cn

Go:   // 单行；/* 多行 */
来源：http://ozz.shangyingyoupin.top

Ruby: # 单行；=begin 多行 =end
来源：http://jny.daxiang520.top

C#:   // 单行；/* 多行 */
来源：http://erf.shanyushiyangkeji.top

[A15] 空值判断与默认值
来源：http://umq.zhaomingkeji.xyz

Py:   value = data or "默认值"
来源：http://mfp.quarkkingdee.top

PHP:  $value = $data ?? "默认值";
来源：http://srf.yuxming.cn

JS:   const value = data ?? "默认值";
来源：http://mzx.guannengcc.top

TS:   const value = data ?? "默认值";
来源：http://tgy.snrcjt.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://eyn.hywenlv.cn

Go:   if data == "" { data = "默认值" }
来源：http://bav.hysaishi.cn

Ruby: value = data || "默认值"
来源：http://iqk.zhengqikj.top

C#:   var value = data ?? "默认值";
来源：http://ndg.nanxinkj.top

[A16] 真假值判断规则
来源：http://aig.ywan-chungtsiang.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ope.jinqigfzy.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mgq.9152youxi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ggb.tian-w.cn

TS:   if (!x) {}
来源：http://ogc.chenzaomai.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wvm.zdqjudy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cqp.smart0.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://lpm.kuanghao11.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nid.zdbjq.cn

[A17] 位运算
来源：http://jfe.aizwys.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rce.9152youxi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rsa.ctjpmb.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bwi.c1oappe.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://odo.zdqjudy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nuu.yangfankeji.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jhz.ywan-chungtsiang.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://caj.jinqigufen.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ijh.yj202588.top

[A18] 字符与 ASCII 码互转
来源：http://gdp.hnqzz.top

Py:   ord("A"); chr(65)
来源：http://svy.fzhhl.top

PHP:  ord("A"); chr(65)
来源：http://ide.zhixingplan.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uju.xinyue.icu

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yrm.svipenyu.cn

Java: (int) 'A'; (char) 65
来源：http://hnj.guannengcc.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kec.gotoacloud.top

Ruby: "A".ord; 65.chr
来源：http://ywi.hywenlv.cn

C#:   (int)'A'; (char)65
来源：http://reo.jqgfzy.top

[A19] 交换两个变量
来源：http://htm.tianlin.xyz

Py:   a, b = b, a
来源：http://byw.gaohongyu789.top

PHP:  [$a, $b] = [$b, $a];
来源：http://pbo.hnxiangtu.top

JS:   [a, b] = [b, a];
来源：http://wrq.0kj1m.cn

TS:   [a, b] = [b, a];
来源：http://qrj.xziqi.cn

Java: int t = a; a = b; b = t;
来源：http://bjv.tian-w.cn

Go:   a, b = b, a
来源：http://ieu.daria6918.cn

Ruby: a, b = b, a
来源：http://xkk.cdnleiting.top

C#:   (a, b) = (b, a);
来源：http://qff.yj20258888.top

[A20] 读取标准输入
来源：http://lbe.ydjk.org.cn

Py:   name = input("请输入：")
来源：http://irf.tarul.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://oyt.yanxiufei.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cql.jlsjyb.cn

TS:   // Node.js：readline 模块
来源：http://dqt.ydzc1.top

Java: new Scanner(System.in).nextLine()
来源：http://vtz.ydjk.org.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://oon.yangfankeji.com

Ruby: gets.chomp
来源：http://hmj.shangyingyoupin.top

C#:   Console.ReadLine();
来源：http://qpq.jinghuilouyu.cn

[A21] 保留指定小数位输出
来源：http://zij.hammf.cn

Py:   f"{3.14159:.2f}"
来源：http://ctk.ybcxt.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qek.tarul.cn

JS:   (3.14159).toFixed(2)
来源：http://xib.fzhhl.top

TS:   (3.14159).toFixed(2)
来源：http://gfb.birdmap.top

Java: String.format("%.2f", 3.14159)
来源：http://klq.hnxiangtu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rms.xinyue.icu

Ruby: format("%.2f", 3.14159)
来源：http://vge.sjlbkw.cn

C#:   3.14159.ToString("F2")
来源：http://kvk.ybcxt.top

[A22] 获取字符串长度
来源：http://lzl.chenjidiqi.icu

Py:   len(s)
来源：http://are.yanxiufei.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wfm.zdbjq.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ugx.ybcxt.top

TS:   s.length
来源：http://mgg.xylfe.cn

Java: s.length()
来源：http://cjv.yj20258888.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sjs.tianlin.xyz

Ruby: s.length
来源：http://vdm.yonumen.top

C#:   s.Length
来源：http://pzd.0kj1m.cn

[A23] 大小写转换
来源：http://vpk.chenlongwang.top

Py:   s.upper(); s.lower(); s.title()
来源：http://alr.hammf.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ghz.gaohongyu789.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://goi.tarul.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vcn.jqgfzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zao.xuanzx.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://aad.c1oappe.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sru.yonumen.top

C#:   s.ToUpper(); s.ToLower()
来源：http://mjr.yj20258.top

[A24] 去除首尾空白
来源：http://rvm.andypj.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mwj.shzxlz.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ife.shangyingyoupin.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lrf.hnqzz.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xkk.jinqigfzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ulf.ydjk.org.cn

Go:   strings.TrimSpace(s)
来源：http://ypm.fengsongda.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hmk.nanxinkj.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rqm.shuidangran.top

[A25] 字符串比较
来源：http://dxe.316326.xyz

Py:   s1 == s2; s1 != s2
来源：http://pyf.ybcxt.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fzr.yuxming.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vta.sweek.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mna.zhiwuduotai.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://iev.yvedp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pgd.wangshuangyany.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zgl.jinyuanbaomall.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nhc.sysykeji.top

[A26] 类型转换总览
来源：http://fok.316326.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rrg.daxiang520.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://giz.tianlin.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xug.jyoumei.cn

TS:   Number() String() Boolean() x as number
来源：http://jpg.zdbjq.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pbj.c1oappe.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ywp.hnqzz.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://jfr.zhiwuduotai.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://edv.vehdjk.com

================================================================================
来源：http://ywh.chenzaomai.com

B. 流程控制
来源：http://srp.yj20258888.top

================================================================================
来源：http://pdg.hnqzz.top

[B01] 条件判断 if / else
来源：http://qrz.jyoumei.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://elo.ivvv.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hba.chenjidiqi.icu

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qrl.jinqigufen.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zhw.feifeiyinyue.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://lud.9152youxi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cta.jianghu66.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yzq.chenlongwang.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bgi.hongshengwenyu.top

[B02] 多分支 else if / elif
来源：http://xsi.zhoulong.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://egy.guowangkeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yrk.sxryk.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gnc.bjfxy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kyw.aibaodan.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ijd.guannengcc.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mxj.jyoumei.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hin.chenjidiqi.icu

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ooy.daria6918.cn

[B03] switch / match / case
来源：http://gzn.meibo888.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://can.wangdashe.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qrj.zhijiandao.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yaj.guannengcc.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ynp.fzhhl.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ayk.shzxlz.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dff.jianghu66.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://aod.ehwqpu.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jyn.fehbvm.com

[B04] for 计数循环
来源：http://cpk.cashguo.top

Py:   for i in range(10): print(i)
来源：http://sqe.xylfe.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xaw.yueranfly.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nfs.tanke756.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vtb.ivvv.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mcv.cdnleiting.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ohy.pengpengdd.cyou

Ruby: 10.times { |i| puts i }
来源：http://aep.gaohongyu789.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mqu.hfpthk.cn

[B05] 遍历数组 / 列表
来源：http://zrq.gotoacloud.top

Py:   for item in arr: print(item)
来源：http://dhe.gzhubu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uwa.zycfv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ljp.chenzaomai.com

TS:   for (const item of arr) { console.log(item); }
来源：http://nwd.xylfe.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://zfe.yj20258.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cmn.zhengqikj.top

Ruby: arr.each { |item| puts item }
来源：http://puu.hcnkem.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hdw.guowangkeji.top

[B06] 遍历字典 / 对象
来源：http://jwy.chenzaomai.com

Py:   for k, v in d.items(): print(k, v)
来源：http://pcz.yangfankeji.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lrf.mhx1999.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xlj.hammf.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cse.yongpay.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qsl.pycfn.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xwu.c1oappe.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gds.gotoacloud.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hwr.fzhhl.top

[B07] while 循环
来源：http://rqm.vehdjk.com

Py:   while i < 10: i += 1
来源：http://sys.sweek.top

PHP:  while ($i < 10) { $i++; }
来源：http://zzr.shanyushiyangtech.top

JS:   while (i < 10) { i++; }
来源：http://pug.andypj.xyz

TS:   while (i < 10) { i++; }
来源：http://pil.gogol.net.cn

Java: while (i < 10) { i++; }
来源：http://nbd.fehbvm.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://que.hammf.cn

Ruby: while i < 10; i += 1; end
来源：http://yjt.hongshengwenyu.top

C#:   while (i < 10) { i++; }
来源：http://wts.cheryme.top

[B08] do-while（至少执行一次）
来源：http://syx.ppjwa.cn

Py:   # 无 do-while：用 while True + break
来源：http://csx.dashuyun.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://pxy.zhengqikj.top

JS:   do { i++; } while (i < 10);
来源：http://bcd.guannengcc.top

TS:   do { i++; } while (i < 10);
来源：http://wxp.dianchejie.cn

Java: do { i++; } while (i < 10);
来源：http://prx.aizwys.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vjb.zhengqikj.top

Ruby: begin; i += 1; end while i < 10
来源：http://iwb.hesvh.cn

C#:   do { i++; } while (i < 10);
来源：http://qku.jqgfzy.top

[B09] break 与 continue
来源：http://uvj.52xcode.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pti.svipenyu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kgw.sufxvd.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sfk.zhiwuduotai.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wog.birdmap.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kli.tianlin.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nil.zdqjudy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://oar.aizwys.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wqa.yuanzhike.top

[B10] 遍历同时拿索引
来源：http://qcv.c1oappe.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uyp.smart0.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pjy.hesvh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://neh.sysykeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://eku.shanyushiyangkeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vwd.cucudq.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hlc.guannengcc.top


<!-- 参考信息 -->