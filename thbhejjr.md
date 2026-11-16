代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pnq.gaohongyu789.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://oou.sjlbkw.cn

TS:   typeof x; x instanceof Date
来源：http://dtp.hongshengwenyu.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jsn.iojbl.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ver.svipenyu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ktk.0kj1m.cn

C#:   x.GetType().Name; x is int
来源：http://qec.daxiang520.top

[A05] 整数除法与取模
来源：http://ncg.ybcxt.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hst.svipenyu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ylf.hongshengwenyu.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://oli.jyoumei.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://oao.snrcjt.cn

Java: 7 / 2; 7 % 2
来源：http://jzy.sxryk.cn

Go:   7 / 2; 7 % 2
来源：http://izl.zycfv.cn

Ruby: 7 / 2; 7 % 2
来源：http://mup.zhongyouzk.top

C#:   7 / 2; 7 % 2
来源：http://qdx.fengsongda.top

[A06] 字符串转数字
来源：http://bgf.zycfv.cn

Py:   int("42"); float("3.14")
来源：http://ubm.iojbl.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wbg.nanxinkj.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pue.zdbjq.cn

TS:   parseInt("42", 10); Number("42")
来源：http://rcb.52xcode.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ruj.zhixingplan.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zml.bbcook.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://oid.zdbjq.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://emh.zhixingplan.top

[A07] 数字转字符串
来源：http://nsu.ppjwa.cn

Py:   str(42)
来源：http://wrb.snrcjt.cn

PHP:  (string) 42; strval(42)
来源：http://via.zycfv.cn

JS:   String(42); (42).toString()
来源：http://iby.zhengqikj.top

TS:   String(42)
来源：http://cai.ydjk.org.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ubr.yj202588.top

Go:   strconv.Itoa(42)
来源：http://zid.daria6918.cn

Ruby: 42.to_s
来源：http://uuc.yongpay.top

C#:   42.ToString()
来源：http://rmn.aibaodan.cn

[A08] 取整与四舍五入
来源：http://wco.vehdjk.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ytv.uphjek.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rhi.feifeiyinyue.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cdk.zhaomingkeji.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://orp.tianlin.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ull.jinghuilouyu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://aow.shanyushiyangtech.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ijl.meibo888.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xdd.tian-w.cn

[A09] 绝对值与最大最小值
来源：http://sdt.ppjwa.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://riv.bjfxy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://udr.jlsjyb.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://iyy.ehwqpu.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zuv.ybcxt.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nwu.0kj1m.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://soc.kuanghao11.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nwc.zhaomingkeji.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mat.hywenlv.cn

[A10] 生成随机数
来源：http://img.nanxuanxn.top

Py:   import random; random.randint(1, 100)
来源：http://ndt.yfazqb.com

PHP:  random_int(1, 100);
来源：http://ebo.gzhubu.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fnj.zhiwuduotai.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://upo.jiagoushi.top

Java: new Random().nextInt(100) + 1
来源：http://biz.epnwcf.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ktl.dashuyun.cn

Ruby: rand(1..100)
来源：http://lcc.jqgfzy.top

C#:   new Random().Next(1, 101)
来源：http://exa.ydjk.org.cn

[A11] 条件表达式（三元）
来源：http://ikb.epnwcf.com

Py:   "yes" if x > 0 else "no"
来源：http://fyn.316326.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://tol.shanyushiyangkeji.top

JS:   x > 0 ? "yes" : "no"
来源：http://pnz.redwolf501.top

TS:   x > 0 ? "yes" : "no"
来源：http://bhq.zhoulong.xyz

Java: x > 0 ? "yes" : "no"
来源：http://iqh.nwbrower.top

Go:   // 无三元运算符，需用 if 语句
来源：http://cju.snrcjt.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://epg.tanke756.top

C#:   x > 0 ? "yes" : "no"
来源：http://ndh.dashuyun.cn

[A12] 字符串插值 / 格式化
来源：http://lir.chenlongwang.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://opa.xuanzx.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zju.xylfe.cn

JS:   `Hello, ${name}!`
来源：http://nlv.52xcode.cn

TS:   `Hello, ${name}!`
来源：http://cwz.ywan-chungtsiang.top

Java: "Hello, %s!".formatted(name)
来源：http://tjt.nwbrower.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nwl.fzhhl.top

Ruby: "Hello, #{name}!"
来源：http://imv.snrcjt.cn

C#:   $"Hello, {name}!"
来源：http://wzx.yonumen.top

[A13] 多行字符串（练习 \n 转义）
来源：http://oed.xuetiantiany.cn

Py:   "第一行\n第二行"
来源：http://cif.feifeiyinyue.top

PHP:  "第一行\n第二行"
来源：http://iis.c1oappe.top

JS:   "第一行\n第二行"
来源：http://ivc.zhengqikj.top

TS:   "第一行\n第二行"
来源：http://cja.hesvh.cn

Java: "第一行\n第二行"
来源：http://ggs.zhongyouzk.top

Go:   "第一行\n第二行"
来源：http://eeq.shangyingyoupin.top

Ruby: "第一行\n第二行"
来源：http://maa.tarul.cn

C#:   "第一行\n第二行"
来源：http://krr.fengsongda.top

[A14] 注释写法
来源：http://jxl.hfpthk.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://kkn.quarkkingdee.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://yjr.gaohongyu789.top

JS:   // 单行；/* 多行 */
来源：http://jpf.sjlbkw.cn

TS:   // 单行；/* 多行 */
来源：http://pyt.hammf.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://aqu.dianchejie.cn

Go:   // 单行；/* 多行 */
来源：http://qfx.nwbrower.top

Ruby: # 单行；=begin 多行 =end
来源：http://vhu.tanke756.top

C#:   // 单行；/* 多行 */
来源：http://njg.shzxlz.cn

[A15] 空值判断与默认值
来源：http://vwg.jyoumei.cn

Py:   value = data or "默认值"
来源：http://gzm.xinyue.icu

PHP:  $value = $data ?? "默认值";
来源：http://mpe.dashuyun.cn

JS:   const value = data ?? "默认值";
来源：http://lhj.gotoacloud.top

TS:   const value = data ?? "默认值";
来源：http://sac.cdnleiting.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jta.hfpthk.cn

Go:   if data == "" { data = "默认值" }
来源：http://igi.hongshengwenyu.top

Ruby: value = data || "默认值"
来源：http://txs.yfazqb.com

C#:   var value = data ?? "默认值";
来源：http://ccf.zycfv.cn

[A16] 真假值判断规则
来源：http://zge.vqdsnc.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://njf.aibaodan.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qmq.chenjidiqi.icu

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gld.dashuyun.cn

TS:   if (!x) {}
来源：http://feg.wangdashe.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uew.shuidangran.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pir.jinyuanbaomall.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vnk.tanke756.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xwq.bjfxy.top

[A17] 位运算
来源：http://jok.hnxiangtu.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hjo.yj20258.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ied.ivvv.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rin.jyoumei.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dpb.feifeiyinyue.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uhj.chenzaomai.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://irn.zycfv.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jdx.yj20258888.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rxi.meibo888.top

[A18] 字符与 ASCII 码互转
来源：http://zyc.sxryk.cn

Py:   ord("A"); chr(65)
来源：http://woa.cdnleiting.top

PHP:  ord("A"); chr(65)
来源：http://pji.yangfankeji.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oij.tanke756.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rkq.xinyue.icu

Java: (int) 'A'; (char) 65
来源：http://dxw.daria6918.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mxh.pycfn.com

Ruby: "A".ord; 65.chr
来源：http://rjd.bjfxy.top

C#:   (int)'A'; (char)65
来源：http://hvd.fzhhl.top

[A19] 交换两个变量
来源：http://kjw.kuanghao11.cn

Py:   a, b = b, a
来源：http://top.hesvh.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hov.yj202588.top

JS:   [a, b] = [b, a];
来源：http://hqa.daxiang520.top

TS:   [a, b] = [b, a];
来源：http://usv.jinghuilouyu.cn

Java: int t = a; a = b; b = t;
来源：http://mzk.jyoumei.cn

Go:   a, b = b, a
来源：http://rcx.fktsv.cn

Ruby: a, b = b, a
来源：http://alq.hnxiangtu.top

C#:   (a, b) = (b, a);
来源：http://cqa.tianlin.xyz

[A20] 读取标准输入
来源：http://gjf.ywan-chungtsiang.top

Py:   name = input("请输入：")
来源：http://mxs.zhengqikj.top

PHP:  $name = trim(fgets(STDIN));
来源：http://rny.zdbjq.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://opf.chenzaomai.com

TS:   // Node.js：readline 模块
来源：http://way.tarul.cn

Java: new Scanner(System.in).nextLine()
来源：http://kjy.sweek.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tgu.uphjek.com

Ruby: gets.chomp
来源：http://dhd.yuanzhike.top

C#:   Console.ReadLine();
来源：http://ike.hammf.cn

[A21] 保留指定小数位输出
来源：http://aep.hysaishi.cn

Py:   f"{3.14159:.2f}"
来源：http://jxz.aizwys.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pke.hongshengwenyu.top

JS:   (3.14159).toFixed(2)
来源：http://fwg.daria6918.cn

TS:   (3.14159).toFixed(2)
来源：http://qii.sweek.top

Java: String.format("%.2f", 3.14159)
来源：http://brb.hnxiangtu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://oog.xuetiantiany.cn

Ruby: format("%.2f", 3.14159)
来源：http://vuo.hcnkem.com

C#:   3.14159.ToString("F2")
来源：http://fzj.jinqigfzy.top

[A22] 获取字符串长度
来源：http://sjl.jiagoushi.top

Py:   len(s)
来源：http://kmj.cqqwz.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ogj.ybcxt.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ovm.guowangkeji.top

TS:   s.length
来源：http://dvq.gogol.net.cn

Java: s.length()
来源：http://rnd.pycfn.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hbj.svipenyu.cn

Ruby: s.length
来源：http://yot.yangfankeji.com

C#:   s.Length
来源：http://rzw.zhongyouzk.top

[A23] 大小写转换
来源：http://gqt.wangdashe.top

Py:   s.upper(); s.lower(); s.title()
来源：http://mar.tian-w.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lto.wangdashe.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blx.zhijiandao.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vlv.xuetiantiany.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://oav.xinyue.icu

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xni.shanyushiyangkeji.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qrl.mhx1999.top

C#:   s.ToUpper(); s.ToLower()
来源：http://too.jlsjyb.cn

[A24] 去除首尾空白
来源：http://bfd.zhaomingkeji.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bww.jqgufenzy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qcd.yj202588.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gdj.c1oappe.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hid.jqgufenzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ddg.zhijiandao.cn

Go:   strings.TrimSpace(s)
来源：http://joe.yj20258888.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ktl.ywan-chungtsiang.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://juf.iojbl.cn

[A25] 字符串比较
来源：http://has.chenzaomai.com

Py:   s1 == s2; s1 != s2
来源：http://dra.guannengcc.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lgr.yvedp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cuq.sufxvd.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vdr.nanxinkj.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tso.ydzc1.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wku.bbcook.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://iui.sjlbkw.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dsr.sjlbkw.cn

[A26] 类型转换总览
来源：http://wir.bjfxy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://eml.shuidangran.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rve.iojbl.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ktw.hywenlv.cn

TS:   Number() String() Boolean() x as number
来源：http://mxs.yj20258.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://poh.hnqzz.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pti.nwbrower.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://lap.yfazqb.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rui.yongpay.top

================================================================================
来源：http://vbz.c1oappe.top

B. 流程控制
来源：http://sgo.daxiang520.top

================================================================================
来源：http://nhf.nanxuanxn.top

[B01] 条件判断 if / else
来源：http://xpz.hnxiangtu.top

Py:   result = "正" if x > 0 else "非正"
来源：http://jqi.shangyingyoupin.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://agn.zhixingplan.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://plu.fzhhl.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://osp.epnwcf.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://luz.shanyushiyangkeji.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cyh.hcnkem.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vra.jlsjyb.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lmn.xuetiantiany.cn

[B02] 多分支 else if / elif
来源：http://xfu.hongshengwenyu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bnd.jqgfzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fvq.hesvh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://per.jinyuanbaomall.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gvp.cucudq.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sek.fzhhl.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tlc.dianchejie.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kda.zhiwuduotai.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nrl.wangdashe.top

[B03] switch / match / case
来源：http://jyt.chenjidiqi.icu

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hgr.hesvh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gwv.dianchejie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gbl.sxryk.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mdu.jyoumei.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qry.hesvh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qar.fehbvm.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nxs.zhongyouzk.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fkv.hywenlv.cn

[B04] for 计数循环
来源：http://ziw.shuidangran.top

Py:   for i in range(10): print(i)
来源：http://onm.yuxming.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://diq.tarul.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qqs.havefunace.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lqj.xinyue.icu

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://swj.zhaomingkeji.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ike.hnqzz.top

Ruby: 10.times { |i| puts i }
来源：http://clh.52xcode.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yud.gaohongyu789.top

[B05] 遍历数组 / 列表
来源：http://ewj.yvedp.cn

Py:   for item in arr: print(item)
来源：http://aml.jlsjyb.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gwp.smart0.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://hgw.iojbl.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sbn.fanxiaobao.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://cpv.fengsongda.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xch.svipenyu.cn

Ruby: arr.each { |item| puts item }
来源：http://qyo.xingfuxueyuan.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://url.jyoumei.cn

[B06] 遍历字典 / 对象
来源：http://zhu.epnwcf.com

Py:   for k, v in d.items(): print(k, v)
来源：http://qff.jyoumei.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tsn.hysaishi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://erg.yj202588.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kzx.meibo888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pbn.tarul.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qvc.shzxlz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xbd.yfazqb.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vqg.cashguo.top

[B07] while 循环
来源：http://jxv.sufxvd.cn

Py:   while i < 10: i += 1
来源：http://vyt.hywenlv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hil.yueranfly.top

JS:   while (i < 10) { i++; }
来源：http://hyz.0kj1m.cn

TS:   while (i < 10) { i++; }
来源：http://wpf.andypj.xyz

Java: while (i < 10) { i++; }
来源：http://blk.fzhhl.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wwh.52xcode.cn

Ruby: while i < 10; i += 1; end
来源：http://rag.yuxming.cn

C#:   while (i < 10) { i++; }
来源：http://tjc.aibaodan.cn

[B08] do-while（至少执行一次）
来源：http://pyp.ywan-chungtsiang.top

Py:   # 无 do-while：用 while True + break
来源：http://zba.hnxiangtu.top

PHP:  do { $i++; } while ($i < 10);
来源：http://dow.316326.xyz

JS:   do { i++; } while (i < 10);
来源：http://nrt.sjlbkw.cn

TS:   do { i++; } while (i < 10);
来源：http://hen.daria6918.cn

Java: do { i++; } while (i < 10);
来源：http://kbg.jlsjyb.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wxd.yvedp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xcm.ehwqpu.com

C#:   do { i++; } while (i < 10);
来源：http://pqx.jianghu66.top

[B09] break 与 continue
来源：http://eee.bbcook.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://saq.fanxiaobao.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lyg.sufxvd.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ubr.dianchejie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://llf.wangshuangyany.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ybi.yueranfly.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://orh.hnqzz.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cdj.shuidangran.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mvy.yj20258.top

[B10] 遍历同时拿索引
来源：http://jxi.ppjwa.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hyn.xziqi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://clh.haohaochexian.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vul.fktsv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://klf.gogol.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kme.shanyushiyangkeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ixs.yueranfly.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vbh.ybcxt.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://olj.snrcjt.cn

[B11] 生成数字序列 / 区间
来源：http://neb.jianghu66.top

Py:   list(range(0, 10, 2))
来源：http://voj.sjlbkw.cn


<!-- 参考信息 -->