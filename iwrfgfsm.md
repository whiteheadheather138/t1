代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bme.zhoulong.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://abj.hnxiangtu.top

TS:   typeof x; x instanceof Date
来源：http://ich.yuxming.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wmf.fehbvm.com

Go:   reflect.TypeOf(x).Name()
来源：http://ihj.sweek.top

Ruby: x.class; x.is_a?(Integer)
来源：http://jox.chenlongwang.top

C#:   x.GetType().Name; x is int
来源：http://bqn.zhaomingkeji.xyz

[A05] 整数除法与取模
来源：http://pep.uphjek.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hei.feifeiyinyue.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ppl.shzxlz.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mom.mhx1999.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hsf.zhixingplan.top

Java: 7 / 2; 7 % 2
来源：http://erk.hysaishi.cn

Go:   7 / 2; 7 % 2
来源：http://kdl.cqqwz.cn

Ruby: 7 / 2; 7 % 2
来源：http://zdo.nanxuanxn.top

C#:   7 / 2; 7 % 2
来源：http://gtq.hywenlv.cn

[A06] 字符串转数字
来源：http://ocr.jinghuilouyu.cn

Py:   int("42"); float("3.14")
来源：http://xcg.yvedp.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rqg.cdnleiting.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fbm.iojbl.cn

TS:   parseInt("42", 10); Number("42")
来源：http://tck.smart0.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://szt.yj20258888.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qqg.fehbvm.com

Ruby: "42".to_i; "3.14".to_f
来源：http://yon.birdmap.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://knf.shanyushiyangkeji.top

[A07] 数字转字符串
来源：http://bck.ydzc1.top

Py:   str(42)
来源：http://lyf.zhengqikj.top

PHP:  (string) 42; strval(42)
来源：http://tal.wangdashe.top

JS:   String(42); (42).toString()
来源：http://zgj.zhoulong.xyz

TS:   String(42)
来源：http://seq.fktsv.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vya.tanke756.top

Go:   strconv.Itoa(42)
来源：http://xak.dianchejie.cn

Ruby: 42.to_s
来源：http://dbq.gzhubu.top

C#:   42.ToString()
来源：http://esi.nanxuanxn.top

[A08] 取整与四舍五入
来源：http://vnb.jinyuanbaomall.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mzg.xuetiantiany.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://god.meibo888.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hjp.chenzaomai.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://uce.ydzc1.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nnw.chenzaomai.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://epi.ywan-chungtsiang.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://hsb.quarkkingdee.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ncc.chenlongwang.top

[A09] 绝对值与最大最小值
来源：http://crt.hywenlv.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fxt.sufxvd.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rdh.fengsongda.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hqj.sxryk.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://uyc.jinqigfzy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ygc.epnwcf.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://eyr.pengpengdd.cyou

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xaq.cucudq.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ryt.shuidangran.top

[A10] 生成随机数
来源：http://pbh.sweek.top

Py:   import random; random.randint(1, 100)
来源：http://efu.hesvh.cn

PHP:  random_int(1, 100);
来源：http://qlc.sxryk.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gey.fengsongda.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bxv.ywan-chungtsiang.top

Java: new Random().nextInt(100) + 1
来源：http://pmz.zycfv.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kkz.zhaomingkeji.xyz

Ruby: rand(1..100)
来源：http://zwd.fehbvm.com

C#:   new Random().Next(1, 101)
来源：http://lyo.aibaodan.cn

[A11] 条件表达式（三元）
来源：http://aeh.pengpengdd.cyou

Py:   "yes" if x > 0 else "no"
来源：http://sqm.tanke756.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://uug.chenlongwang.top

JS:   x > 0 ? "yes" : "no"
来源：http://wzj.uphjek.com

TS:   x > 0 ? "yes" : "no"
来源：http://mrf.jyoumei.cn

Java: x > 0 ? "yes" : "no"
来源：http://vpr.jinyuanbaomall.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://awz.ppjwa.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://aoi.nanxuanxn.top

C#:   x > 0 ? "yes" : "no"
来源：http://skl.jinqigufen.top

[A12] 字符串插值 / 格式化
来源：http://gct.feifeiyinyue.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://air.xingfuxueyuan.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://vai.hywenlv.cn

JS:   `Hello, ${name}!`
来源：http://xhh.yuanzhike.top

TS:   `Hello, ${name}!`
来源：http://edl.nwbrower.top

Java: "Hello, %s!".formatted(name)
来源：http://kny.sweek.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://yxu.shanyushiyangtech.top

Ruby: "Hello, #{name}!"
来源：http://ggd.yj20258.top

C#:   $"Hello, {name}!"
来源：http://rji.xziqi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zhw.uphjek.com

Py:   "第一行\n第二行"
来源：http://lei.xingfuxueyuan.xyz

PHP:  "第一行\n第二行"
来源：http://qdd.jinghuilouyu.cn

JS:   "第一行\n第二行"
来源：http://hpv.jiagoushi.top

TS:   "第一行\n第二行"
来源：http://plz.daxiang520.top

Java: "第一行\n第二行"
来源：http://hpq.jinqigfzy.top

Go:   "第一行\n第二行"
来源：http://xuc.tarul.cn

Ruby: "第一行\n第二行"
来源：http://slx.cqqwz.cn

C#:   "第一行\n第二行"
来源：http://zbr.ybcxt.top

[A14] 注释写法
来源：http://bzi.yangfankeji.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://eex.shangyingyoupin.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://uhg.vqdsnc.cn

JS:   // 单行；/* 多行 */
来源：http://ysv.gogol.net.cn

TS:   // 单行；/* 多行 */
来源：http://jsj.birdmap.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kod.vehdjk.com

Go:   // 单行；/* 多行 */
来源：http://nym.ywan-chungtsiang.top

Ruby: # 单行；=begin 多行 =end
来源：http://sqb.ppjwa.cn

C#:   // 单行；/* 多行 */
来源：http://ltk.ydjk.org.cn

[A15] 空值判断与默认值
来源：http://klb.dashuyun.cn

Py:   value = data or "默认值"
来源：http://icr.yfazqb.com

PHP:  $value = $data ?? "默认值";
来源：http://qgf.sxryk.cn

JS:   const value = data ?? "默认值";
来源：http://eez.xuetiantiany.cn

TS:   const value = data ?? "默认值";
来源：http://kig.hongshengwenyu.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://uwj.zhiwuduotai.top

Go:   if data == "" { data = "默认值" }
来源：http://vdx.cdnleiting.top

Ruby: value = data || "默认值"
来源：http://jbl.epnwcf.com

C#:   var value = data ?? "默认值";
来源：http://qnl.hesvh.cn

[A16] 真假值判断规则
来源：http://tru.xuanzx.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dpx.chenjidiqi.icu

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wyh.xuanzx.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ept.jinyuanbaomall.cn

TS:   if (!x) {}
来源：http://hra.guowangkeji.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hly.wangshuangyany.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tpc.xinyue.icu

Ruby: unless x            # nil 与 false 为假
来源：http://jzw.zycfv.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://weq.jinghuilouyu.cn

[A17] 位运算
来源：http://krs.316326.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wmh.tianlin.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://knk.xziqi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ofl.dashuyun.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ifh.xinyue.icu

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wpe.zhixingplan.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wgo.jyoumei.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iya.c1oappe.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ejj.bjfxy.top

[A18] 字符与 ASCII 码互转
来源：http://ryq.feifeiyinyue.top

Py:   ord("A"); chr(65)
来源：http://bbh.hesvh.cn

PHP:  ord("A"); chr(65)
来源：http://aie.0kj1m.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fpy.hcnkem.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gyx.ehwqpu.com

Java: (int) 'A'; (char) 65
来源：http://vuc.cqqwz.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dxt.sxryk.cn

Ruby: "A".ord; 65.chr
来源：http://vla.aizwys.cn

C#:   (int)'A'; (char)65
来源：http://fwg.daria6918.cn

[A19] 交换两个变量
来源：http://cni.fehbvm.com

Py:   a, b = b, a
来源：http://wcj.ybcxt.top

PHP:  [$a, $b] = [$b, $a];
来源：http://fwr.ivvv.top

JS:   [a, b] = [b, a];
来源：http://mmu.zhixingplan.top

TS:   [a, b] = [b, a];
来源：http://kdt.ivvv.top

Java: int t = a; a = b; b = t;
来源：http://dan.vqdsnc.cn

Go:   a, b = b, a
来源：http://lci.zhixingplan.top

Ruby: a, b = b, a
来源：http://prd.xuanzx.com

C#:   (a, b) = (b, a);
来源：http://kfd.sufxvd.cn

[A20] 读取标准输入
来源：http://zox.yj20258.top

Py:   name = input("请输入：")
来源：http://mai.52xcode.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://lhs.jlsjyb.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://opa.yueranfly.top

TS:   // Node.js：readline 模块
来源：http://auq.svipenyu.cn

Java: new Scanner(System.in).nextLine()
来源：http://lto.jianghu66.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mar.bjfxy.top

Ruby: gets.chomp
来源：http://ubd.yonumen.top

C#:   Console.ReadLine();
来源：http://ova.zdqjudy.top

[A21] 保留指定小数位输出
来源：http://vdv.gogol.net.cn

Py:   f"{3.14159:.2f}"
来源：http://xhx.feifeiyinyue.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hiw.hammf.cn

JS:   (3.14159).toFixed(2)
来源：http://emi.hnxiangtu.top

TS:   (3.14159).toFixed(2)
来源：http://lhh.bjfxy.top

Java: String.format("%.2f", 3.14159)
来源：http://puf.sjlbkw.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nrh.cdnleiting.top

Ruby: format("%.2f", 3.14159)
来源：http://zbl.gotoacloud.top

C#:   3.14159.ToString("F2")
来源：http://vzq.aizwys.cn

[A22] 获取字符串长度
来源：http://six.hesvh.cn

Py:   len(s)
来源：http://qzo.hnxiangtu.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://myz.bbcook.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rvb.daxiang520.top

TS:   s.length
来源：http://fhd.epnwcf.com

Java: s.length()
来源：http://ofo.yj20258.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zuy.jyoumei.cn

Ruby: s.length
来源：http://kfq.hfpthk.cn

C#:   s.Length
来源：http://ywt.cashguo.top

[A23] 大小写转换
来源：http://pce.fzhhl.top

Py:   s.upper(); s.lower(); s.title()
来源：http://rft.gzhubu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tye.hysaishi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mnb.jinyuanbaomall.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://teb.zhengqikj.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mbb.cdnleiting.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nay.yfazqb.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qik.zycfv.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rir.cashguo.top

[A24] 去除首尾空白
来源：http://pep.ppjwa.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fto.cdnleiting.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cmx.xingfuxueyuan.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ykl.ivvv.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rzt.cqqwz.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://boq.smart0.xyz

Go:   strings.TrimSpace(s)
来源：http://khd.yj20258888.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mzu.zhongyouzk.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://een.yfazqb.com

[A25] 字符串比较
来源：http://gtg.xuetiantiany.cn

Py:   s1 == s2; s1 != s2
来源：http://fle.zhengqikj.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://usg.daxiang520.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xsb.chenzaomai.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mll.xuetiantiany.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qiu.zhijiandao.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://aso.xingfuxueyuan.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://uxd.gotoacloud.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ran.jinghuilouyu.cn

[A26] 类型转换总览
来源：http://bju.9152youxi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://aiy.hnxiangtu.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kpi.jinqigfzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://amu.nwbrower.top

TS:   Number() String() Boolean() x as number
来源：http://vac.aizwys.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fgt.yuxming.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ybo.52xcode.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://imx.gotoacloud.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://slb.hnqzz.top

================================================================================
来源：http://imz.jinyuanbaomall.cn

B. 流程控制
来源：http://ktu.hammf.cn

================================================================================
来源：http://adq.chenzaomai.com

[B01] 条件判断 if / else
来源：http://lex.nwbrower.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ren.sweek.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kxh.fanxiaobao.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pio.sweek.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vdk.haohaochexian.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ufw.jinyuanbaomall.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dde.havefunace.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lon.hammf.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ntm.meibo888.top

[B02] 多分支 else if / elif
来源：http://owm.zhijiandao.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ywm.hnxiangtu.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vaw.shangyingyoupin.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cpg.jiagoushi.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ktr.zhiwuduotai.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uim.zhijiandao.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qfb.yvedp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://izv.0kj1m.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pbi.cheryme.top

[B03] switch / match / case
来源：http://pfn.yonumen.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fxi.zdbjq.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lnk.jyoumei.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vgy.vehdjk.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zzx.kuanghao11.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wuz.fehbvm.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ijp.xinyue.icu

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://grw.xingfuxueyuan.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dax.redwolf501.top

[B04] for 计数循环
来源：http://osb.birdmap.top

Py:   for i in range(10): print(i)
来源：http://cuk.ehwqpu.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://phz.yueranfly.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eks.chenzaomai.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bpm.cashguo.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rlv.xuetiantiany.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wlk.xziqi.cn

Ruby: 10.times { |i| puts i }
来源：http://oxr.jinqigufen.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qoz.tanke756.top

[B05] 遍历数组 / 列表
来源：http://udc.vehdjk.com

Py:   for item in arr: print(item)
来源：http://erh.ywan-chungtsiang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://izz.cucudq.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sun.nanxinkj.top

TS:   for (const item of arr) { console.log(item); }
来源：http://bgj.yuanzhike.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://xdk.yj202588.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bmc.jyoumei.cn

Ruby: arr.each { |item| puts item }
来源：http://dhu.vehdjk.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tmr.shangyingyoupin.top

[B06] 遍历字典 / 对象
来源：http://kde.gotoacloud.top

Py:   for k, v in d.items(): print(k, v)
来源：http://deq.jinqigfzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pls.vehdjk.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yru.chenlongwang.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xne.xuetiantiany.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dem.cucudq.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pbc.haohaochexian.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://liy.haohaochexian.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qda.iojbl.cn

[B07] while 循环
来源：http://pxe.xziqi.cn

Py:   while i < 10: i += 1
来源：http://cap.tarul.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hki.dianchejie.cn

JS:   while (i < 10) { i++; }
来源：http://cdb.tarul.cn

TS:   while (i < 10) { i++; }
来源：http://ggh.jinghuilouyu.cn

Java: while (i < 10) { i++; }
来源：http://zil.gogol.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vrm.jinyuanbaomall.cn

Ruby: while i < 10; i += 1; end
来源：http://awy.vehdjk.com

C#:   while (i < 10) { i++; }
来源：http://cso.daria6918.cn

[B08] do-while（至少执行一次）
来源：http://hqb.ppjwa.cn

Py:   # 无 do-while：用 while True + break
来源：http://rcq.daxiang520.top

PHP:  do { $i++; } while ($i < 10);
来源：http://uad.hfpthk.cn

JS:   do { i++; } while (i < 10);
来源：http://ues.gzhubu.top

TS:   do { i++; } while (i < 10);
来源：http://wqf.sweek.top

Java: do { i++; } while (i < 10);
来源：http://ktx.shangyingyoupin.top

Go:   for { i++; if i >= 10 { break } }
来源：http://jbe.gogol.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://usr.redwolf501.top

C#:   do { i++; } while (i < 10);
来源：http://khs.jqgfzy.top

[B09] break 与 continue
来源：http://lzz.smart0.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://esi.shuidangran.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pot.svipenyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cam.hesvh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aoa.gogol.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zfw.yangfankeji.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sgb.shangyingyoupin.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uyu.yanxiufei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zsh.yj20258888.top

[B10] 遍历同时拿索引
来源：http://teq.gaohongyu789.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bae.aizwys.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fhd.zhoulong.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ofo.wangshuangyany.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wcn.sjlbkw.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fcz.hesvh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cot.haohaochexian.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ofe.hnxiangtu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vhq.jinqigfzy.top

[B11] 生成数字序列 / 区间
来源：http://eeh.ctjpmb.com

Py:   list(range(0, 10, 2))
来源：http://dxk.fanxiaobao.xyz


<!-- 参考信息 -->