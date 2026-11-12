代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://irz.shanyushiyangkeji.top

Ruby: x.class; x.is_a?(Integer)
来源：http://fnw.sjlbkw.cn

C#:   x.GetType().Name; x is int
来源：http://jhb.nanxinkj.top

[A05] 整数除法与取模
来源：http://yop.daxiang520.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vst.aizwys.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zxu.nanxuanxn.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rep.xuetiantiany.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pxw.jlsjyb.cn

Java: 7 / 2; 7 % 2
来源：http://uzx.kuanghao11.cn

Go:   7 / 2; 7 % 2
来源：http://oug.shuidangran.top

Ruby: 7 / 2; 7 % 2
来源：http://rnu.wangdashe.top

C#:   7 / 2; 7 % 2
来源：http://jsz.tarul.cn

[A06] 字符串转数字
来源：http://uzh.guowangkeji.top

Py:   int("42"); float("3.14")
来源：http://ejm.yuxming.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://oul.iojbl.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ghf.fengsongda.top

TS:   parseInt("42", 10); Number("42")
来源：http://maf.ivvv.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nvy.0kj1m.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xof.gzhubu.top

Ruby: "42".to_i; "3.14".to_f
来源：http://pgh.uphjek.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://huu.tanke756.top

[A07] 数字转字符串
来源：http://ydx.bbcook.cn

Py:   str(42)
来源：http://dti.sjlbkw.cn

PHP:  (string) 42; strval(42)
来源：http://dtd.zhijiandao.cn

JS:   String(42); (42).toString()
来源：http://dqh.andypj.xyz

TS:   String(42)
来源：http://wkt.zhoulong.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://cjj.shzxlz.cn

Go:   strconv.Itoa(42)
来源：http://jnl.tarul.cn

Ruby: 42.to_s
来源：http://kpb.sjlbkw.cn

C#:   42.ToString()
来源：http://iix.ydzc1.top

[A08] 取整与四舍五入
来源：http://ood.tarul.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dhf.jiagoushi.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lwt.cashguo.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cja.quarkkingdee.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kgf.yanxiufei.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ksb.guannengcc.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ncm.nwbrower.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://vnr.sysykeji.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://nse.ydzc1.top

[A09] 绝对值与最大最小值
来源：http://zjh.sysykeji.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wlh.yj202588.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://smz.fktsv.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kcx.sxryk.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://pyp.shangyingyoupin.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://iby.sjlbkw.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://buv.dianchejie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://htq.ydjk.org.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bvt.vehdjk.com

[A10] 生成随机数
来源：http://oty.fehbvm.com

Py:   import random; random.randint(1, 100)
来源：http://aoj.jqgufenzy.top

PHP:  random_int(1, 100);
来源：http://vzc.birdmap.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bvs.gotoacloud.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://iga.yongpay.top

Java: new Random().nextInt(100) + 1
来源：http://aff.gogol.net.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://psi.fengsongda.top

Ruby: rand(1..100)
来源：http://auk.meibo888.top

C#:   new Random().Next(1, 101)
来源：http://vqm.andypj.xyz

[A11] 条件表达式（三元）
来源：http://kgr.xinyue.icu

Py:   "yes" if x > 0 else "no"
来源：http://xhc.jqgufenzy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://jcg.fzhhl.top

JS:   x > 0 ? "yes" : "no"
来源：http://jap.c1oappe.top

TS:   x > 0 ? "yes" : "no"
来源：http://wze.guowangkeji.top

Java: x > 0 ? "yes" : "no"
来源：http://yad.hfpthk.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://vxp.zdbjq.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://hrf.yvedp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://jcz.sweek.top

[A12] 字符串插值 / 格式化
来源：http://mjh.snrcjt.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mgd.pengpengdd.cyou

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tum.yanxiufei.cn

JS:   `Hello, ${name}!`
来源：http://vas.yj202588.top

TS:   `Hello, ${name}!`
来源：http://rbz.vehdjk.com

Java: "Hello, %s!".formatted(name)
来源：http://yaa.xuetiantiany.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://znw.yonumen.top

Ruby: "Hello, #{name}!"
来源：http://saz.pengpengdd.cyou

C#:   $"Hello, {name}!"
来源：http://uzq.iojbl.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ben.mhx1999.top

Py:   "第一行\n第二行"
来源：http://afw.yuanzhike.top

PHP:  "第一行\n第二行"
来源：http://pzc.zhijiandao.cn

JS:   "第一行\n第二行"
来源：http://twg.zdqjudy.top

TS:   "第一行\n第二行"
来源：http://qkt.nwbrower.top

Java: "第一行\n第二行"
来源：http://veh.xingfuxueyuan.xyz

Go:   "第一行\n第二行"
来源：http://tka.hywenlv.cn

Ruby: "第一行\n第二行"
来源：http://vxe.fehbvm.com

C#:   "第一行\n第二行"
来源：http://uzz.fzhhl.top

[A14] 注释写法
来源：http://xgb.hammf.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://zgt.fanxiaobao.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://cpp.yonumen.top

JS:   // 单行；/* 多行 */
来源：http://xwa.guannengcc.top

TS:   // 单行；/* 多行 */
来源：http://ezt.yj202588.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lya.yangfankeji.com

Go:   // 单行；/* 多行 */
来源：http://lgk.xingfuxueyuan.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://der.tanke756.top

C#:   // 单行；/* 多行 */
来源：http://iou.shangyingyoupin.top

[A15] 空值判断与默认值
来源：http://dfz.shangyingyoupin.top

Py:   value = data or "默认值"
来源：http://rok.hfpthk.cn

PHP:  $value = $data ?? "默认值";
来源：http://zkh.316326.xyz

JS:   const value = data ?? "默认值";
来源：http://lnv.dianchejie.cn

TS:   const value = data ?? "默认值";
来源：http://xhc.hywenlv.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fye.zdqjudy.top

Go:   if data == "" { data = "默认值" }
来源：http://xpj.jianghu66.top

Ruby: value = data || "默认值"
来源：http://hoq.cucudq.cn

C#:   var value = data ?? "默认值";
来源：http://hvj.aizwys.cn

[A16] 真假值判断规则
来源：http://qkg.fanxiaobao.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gsg.zhoulong.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://uhz.gzhubu.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zmk.hcnkem.com

TS:   if (!x) {}
来源：http://zab.shangyingyoupin.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qmh.jqgfzy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://eqk.havefunace.top

Ruby: unless x            # nil 与 false 为假
来源：http://mrq.hnxiangtu.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://qql.zhijiandao.cn

[A17] 位运算
来源：http://wfo.fehbvm.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wpp.guowangkeji.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cce.daxiang520.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tzk.hfpthk.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://slp.chenjidiqi.icu

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nvt.cucudq.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fbt.bjfxy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://opl.shanyushiyangkeji.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kmu.iojbl.cn

[A18] 字符与 ASCII 码互转
来源：http://sej.shanyushiyangkeji.top

Py:   ord("A"); chr(65)
来源：http://wko.hcnkem.com

PHP:  ord("A"); chr(65)
来源：http://wrh.nwbrower.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ibk.fanxiaobao.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qcq.zycfv.cn

Java: (int) 'A'; (char) 65
来源：http://hje.bbcook.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bnr.c1oappe.top

Ruby: "A".ord; 65.chr
来源：http://cep.zhaomingkeji.xyz

C#:   (int)'A'; (char)65
来源：http://eih.yangfankeji.com

[A19] 交换两个变量
来源：http://rrf.fanxiaobao.xyz

Py:   a, b = b, a
来源：http://uhb.wangdashe.top

PHP:  [$a, $b] = [$b, $a];
来源：http://qxi.andypj.xyz

JS:   [a, b] = [b, a];
来源：http://osr.dashuyun.cn

TS:   [a, b] = [b, a];
来源：http://yer.xingfuxueyuan.xyz

Java: int t = a; a = b; b = t;
来源：http://nzq.xylfe.cn

Go:   a, b = b, a
来源：http://ecc.zhaomingkeji.xyz

Ruby: a, b = b, a
来源：http://pcy.hywenlv.cn

C#:   (a, b) = (b, a);
来源：http://vua.svipenyu.cn

[A20] 读取标准输入
来源：http://jlr.jqgfzy.top

Py:   name = input("请输入：")
来源：http://cuj.hysaishi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://zhn.quarkkingdee.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://emo.yfazqb.com

TS:   // Node.js：readline 模块
来源：http://fpa.zhixingplan.top

Java: new Scanner(System.in).nextLine()
来源：http://kfa.hnxiangtu.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ydg.kuanghao11.cn

Ruby: gets.chomp
来源：http://gmt.xuanzx.com

C#:   Console.ReadLine();
来源：http://lvf.epnwcf.com

[A21] 保留指定小数位输出
来源：http://aog.zdbjq.cn

Py:   f"{3.14159:.2f}"
来源：http://xgd.nanxuanxn.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cuc.hysaishi.cn

JS:   (3.14159).toFixed(2)
来源：http://sfg.ppjwa.cn

TS:   (3.14159).toFixed(2)
来源：http://kgi.jinghuilouyu.cn

Java: String.format("%.2f", 3.14159)
来源：http://lpe.zhixingplan.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://eep.snrcjt.cn

Ruby: format("%.2f", 3.14159)
来源：http://hbx.meibo888.top

C#:   3.14159.ToString("F2")
来源：http://qfs.jinghuilouyu.cn

[A22] 获取字符串长度
来源：http://bdd.vqdsnc.cn

Py:   len(s)
来源：http://eyv.jinqigfzy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gcg.xinyue.icu

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hsr.havefunace.top

TS:   s.length
来源：http://cbz.sufxvd.cn

Java: s.length()
来源：http://wjs.svipenyu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://abs.sysykeji.top

Ruby: s.length
来源：http://log.zhoulong.xyz

C#:   s.Length
来源：http://kyr.uphjek.com

[A23] 大小写转换
来源：http://fhw.xinyue.icu

Py:   s.upper(); s.lower(); s.title()
来源：http://xfk.9152youxi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ylo.nanxuanxn.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://eum.zycfv.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mgn.vqdsnc.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dac.iojbl.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cji.bbcook.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dcm.jlsjyb.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://tlq.xinyue.icu

[A24] 去除首尾空白
来源：http://ncu.snrcjt.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://uii.zdbjq.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tnp.zdbjq.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://urv.jinyuanbaomall.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://few.xylfe.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wre.xziqi.cn

Go:   strings.TrimSpace(s)
来源：http://lgp.tian-w.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://spv.wangshuangyany.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jpl.fktsv.cn

[A25] 字符串比较
来源：http://sjq.chenjidiqi.icu

Py:   s1 == s2; s1 != s2
来源：http://jwz.yanxiufei.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dec.9152youxi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://agr.gogol.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://anb.sweek.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mza.jinqigfzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bnh.ybcxt.top

Ruby: s1 == s2; s1 <=> s2
来源：http://qbv.jinqigufen.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ziy.hesvh.cn

[A26] 类型转换总览
来源：http://qkm.cqqwz.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hsb.chenzaomai.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zyd.hongshengwenyu.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sit.jinqigufen.top

TS:   Number() String() Boolean() x as number
来源：http://jyq.cashguo.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vdc.hongshengwenyu.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xqr.fehbvm.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://wik.xuetiantiany.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pud.hammf.cn

================================================================================
来源：http://ess.gogol.net.cn

B. 流程控制
来源：http://aeg.pengpengdd.cyou

================================================================================
来源：http://dit.tanke756.top

[B01] 条件判断 if / else
来源：http://ejk.hesvh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ztp.vqdsnc.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zgx.daria6918.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://myx.zhiwuduotai.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tkw.yuxming.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rve.xinyue.icu

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://czx.chenzaomai.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pir.hammf.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hvx.shangyingyoupin.top

[B02] 多分支 else if / elif
来源：http://kcc.fktsv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wqf.sxryk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wxz.dianchejie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rwg.shzxlz.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bhn.xinyue.icu

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gfx.yangfankeji.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qqv.hcnkem.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jjp.xuetiantiany.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jxf.guannengcc.top

[B03] switch / match / case
来源：http://fad.zhixingplan.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://twp.havefunace.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lhs.fzhhl.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fpg.vqdsnc.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://shg.tianlin.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rvm.ywan-chungtsiang.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qsz.jlsjyb.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vbm.zhiwuduotai.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://myx.yfazqb.com

[B04] for 计数循环
来源：http://iay.ctjpmb.com

Py:   for i in range(10): print(i)
来源：http://xbc.jinqigufen.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lfl.cashguo.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gfc.cqqwz.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://for.gzhubu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xdx.jqgfzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fpx.ydjk.org.cn

Ruby: 10.times { |i| puts i }
来源：http://tbo.sjlbkw.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://drr.dashuyun.cn

[B05] 遍历数组 / 列表
来源：http://tdv.daxiang520.top

Py:   for item in arr: print(item)
来源：http://lco.hongshengwenyu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://aqr.jlsjyb.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ftp.yj20258888.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ixl.9152youxi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jvn.guannengcc.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pfp.bjfxy.top

Ruby: arr.each { |item| puts item }
来源：http://jfq.zhongyouzk.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mna.hfpthk.cn

[B06] 遍历字典 / 对象
来源：http://cbt.svipenyu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qrk.9152youxi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jft.jinqigfzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nfd.c1oappe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lqf.haohaochexian.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://var.zhongyouzk.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ysv.vqdsnc.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xed.yangfankeji.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rtp.9152youxi.cn

[B07] while 循环
来源：http://wnc.mhx1999.top

Py:   while i < 10: i += 1
来源：http://kjc.shanyushiyangtech.top

PHP:  while ($i < 10) { $i++; }
来源：http://eqd.chenzaomai.com

JS:   while (i < 10) { i++; }
来源：http://gyo.bjfxy.top

TS:   while (i < 10) { i++; }
来源：http://iaj.zdbjq.cn

Java: while (i < 10) { i++; }
来源：http://arw.jyoumei.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pqn.hongshengwenyu.top

Ruby: while i < 10; i += 1; end
来源：http://jln.sweek.top

C#:   while (i < 10) { i++; }
来源：http://eka.cucudq.cn

[B08] do-while（至少执行一次）
来源：http://led.sjlbkw.cn

Py:   # 无 do-while：用 while True + break
来源：http://oqj.svipenyu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vav.hnxiangtu.top

JS:   do { i++; } while (i < 10);
来源：http://ynv.bjfxy.top

TS:   do { i++; } while (i < 10);
来源：http://fie.redwolf501.top

Java: do { i++; } while (i < 10);
来源：http://wly.zhoulong.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://rmd.pengpengdd.cyou

Ruby: begin; i += 1; end while i < 10
来源：http://fzj.c1oappe.top

C#:   do { i++; } while (i < 10);
来源：http://lgt.vehdjk.com

[B09] break 与 continue
来源：http://vxz.gaohongyu789.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nav.hywenlv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cua.wangshuangyany.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lue.jinqigufen.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cjv.sxryk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://few.zhixingplan.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yja.yfazqb.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ruj.yanxiufei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ftr.cdnleiting.top

[B10] 遍历同时拿索引
来源：http://bfe.xuetiantiany.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uie.dashuyun.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pma.redwolf501.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qox.chenzaomai.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vmu.fehbvm.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vfn.shuidangran.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ycq.cucudq.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cdc.sufxvd.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rkf.bbcook.cn

[B11] 生成数字序列 / 区间
来源：http://ltm.zhoulong.xyz

Py:   list(range(0, 10, 2))
来源：http://wiu.zhongyouzk.top

PHP:  range(0, 10, 2);
来源：http://njz.iojbl.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eal.wangdashe.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aqq.c1oappe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ivr.ywan-chungtsiang.top


<!-- 参考信息 -->