代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lay.vqdsnc.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ggi.birdmap.top

TS:   typeof x; x instanceof Date
来源：http://mdr.shzxlz.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lzj.shuidangran.top

Go:   reflect.TypeOf(x).Name()
来源：http://rkk.kuanghao11.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://boc.dashuyun.cn

C#:   x.GetType().Name; x is int
来源：http://pir.dianchejie.cn

[A05] 整数除法与取模
来源：http://fdm.sjlbkw.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://znm.shzxlz.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://rlh.ybcxt.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://azx.hysaishi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tfj.52xcode.cn

Java: 7 / 2; 7 % 2
来源：http://tnd.hcnkem.com

Go:   7 / 2; 7 % 2
来源：http://zxj.chenlongwang.top

Ruby: 7 / 2; 7 % 2
来源：http://wiw.tian-w.cn

C#:   7 / 2; 7 % 2
来源：http://flv.birdmap.top

[A06] 字符串转数字
来源：http://wmq.haohaochexian.top

Py:   int("42"); float("3.14")
来源：http://mlo.xingfuxueyuan.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://uyz.yj20258888.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mid.chenjidiqi.icu

TS:   parseInt("42", 10); Number("42")
来源：http://rqo.xuanzx.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jih.epnwcf.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tbv.guowangkeji.top

Ruby: "42".to_i; "3.14".to_f
来源：http://zrv.ehwqpu.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qjk.zhengqikj.top

[A07] 数字转字符串
来源：http://ztz.iojbl.cn

Py:   str(42)
来源：http://iwt.mhx1999.top

PHP:  (string) 42; strval(42)
来源：http://aqp.feifeiyinyue.top

JS:   String(42); (42).toString()
来源：http://qfb.feifeiyinyue.top

TS:   String(42)
来源：http://gcl.yonumen.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://mpl.hnqzz.top

Go:   strconv.Itoa(42)
来源：http://fla.hnqzz.top

Ruby: 42.to_s
来源：http://tnm.bbcook.cn

C#:   42.ToString()
来源：http://szi.yueranfly.top

[A08] 取整与四舍五入
来源：http://lqd.cashguo.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dyd.zhongyouzk.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zfq.ctjpmb.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://yiw.sxryk.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://phc.daria6918.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://uku.quarkkingdee.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jcd.shangyingyoupin.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://lld.sweek.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tmb.fehbvm.com

[A09] 绝对值与最大最小值
来源：http://dhv.aizwys.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rxt.shanyushiyangkeji.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ybs.aizwys.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://skj.ydjk.org.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ral.xziqi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zel.gzhubu.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hns.zhengqikj.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://iwx.dashuyun.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wsc.yonumen.top

[A10] 生成随机数
来源：http://pak.cashguo.top

Py:   import random; random.randint(1, 100)
来源：http://yns.hysaishi.cn

PHP:  random_int(1, 100);
来源：http://hro.ybcxt.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://khk.hywenlv.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://osd.dashuyun.cn

Java: new Random().nextInt(100) + 1
来源：http://xba.tanke756.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lsi.jinyuanbaomall.cn

Ruby: rand(1..100)
来源：http://jcz.shanyushiyangtech.top

C#:   new Random().Next(1, 101)
来源：http://lyg.cashguo.top

[A11] 条件表达式（三元）
来源：http://eaq.fengsongda.top

Py:   "yes" if x > 0 else "no"
来源：http://itr.nanxinkj.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://mnp.cheryme.top

JS:   x > 0 ? "yes" : "no"
来源：http://jdo.quarkkingdee.top

TS:   x > 0 ? "yes" : "no"
来源：http://vzq.hywenlv.cn

Java: x > 0 ? "yes" : "no"
来源：http://zsx.zhongyouzk.top

Go:   // 无三元运算符，需用 if 语句
来源：http://yoi.kuanghao11.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://agw.fanxiaobao.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://kce.zhixingplan.top

[A12] 字符串插值 / 格式化
来源：http://wko.sufxvd.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tmi.jinqigfzy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yjm.guannengcc.top

JS:   `Hello, ${name}!`
来源：http://ovl.tianlin.xyz

TS:   `Hello, ${name}!`
来源：http://sls.yongpay.top

Java: "Hello, %s!".formatted(name)
来源：http://vss.fktsv.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kzb.shanyushiyangtech.top

Ruby: "Hello, #{name}!"
来源：http://srb.yuanzhike.top

C#:   $"Hello, {name}!"
来源：http://som.yj20258888.top

[A13] 多行字符串（练习 \n 转义）
来源：http://pft.sjlbkw.cn

Py:   "第一行\n第二行"
来源：http://vfx.tarul.cn

PHP:  "第一行\n第二行"
来源：http://ibk.cqqwz.cn

JS:   "第一行\n第二行"
来源：http://qem.shangyingyoupin.top

TS:   "第一行\n第二行"
来源：http://dxd.yueranfly.top

Java: "第一行\n第二行"
来源：http://min.sweek.top

Go:   "第一行\n第二行"
来源：http://auq.yonumen.top

Ruby: "第一行\n第二行"
来源：http://hjl.wangshuangyany.cn

C#:   "第一行\n第二行"
来源：http://txa.jianghu66.top

[A14] 注释写法
来源：http://bhi.vqdsnc.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://lsf.snrcjt.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xck.feifeiyinyue.top

JS:   // 单行；/* 多行 */
来源：http://psc.sufxvd.cn

TS:   // 单行；/* 多行 */
来源：http://bax.guannengcc.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tsx.ywan-chungtsiang.top

Go:   // 单行；/* 多行 */
来源：http://gna.vehdjk.com

Ruby: # 单行；=begin 多行 =end
来源：http://uyj.hywenlv.cn

C#:   // 单行；/* 多行 */
来源：http://rec.daria6918.cn

[A15] 空值判断与默认值
来源：http://kji.yj202588.top

Py:   value = data or "默认值"
来源：http://qco.xinyue.icu

PHP:  $value = $data ?? "默认值";
来源：http://cih.daria6918.cn

JS:   const value = data ?? "默认值";
来源：http://cas.chenlongwang.top

TS:   const value = data ?? "默认值";
来源：http://gfb.gogol.net.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://psb.shangyingyoupin.top

Go:   if data == "" { data = "默认值" }
来源：http://ztl.ydjk.org.cn

Ruby: value = data || "默认值"
来源：http://bjq.gzhubu.top

C#:   var value = data ?? "默认值";
来源：http://vgg.xuanzx.com

[A16] 真假值判断规则
来源：http://wsq.jyoumei.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dqu.jinqigufen.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jxb.hysaishi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kgx.smart0.xyz

TS:   if (!x) {}
来源：http://uif.jyoumei.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://svq.daxiang520.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kmw.kuanghao11.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jwc.shanyushiyangtech.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://syg.ydzc1.top

[A17] 位运算
来源：http://rcx.tarul.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bxy.daria6918.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ffq.hysaishi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wui.fehbvm.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hhw.zhijiandao.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://myw.zhengqikj.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fuy.tianlin.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zpw.hywenlv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bcu.aizwys.cn

[A18] 字符与 ASCII 码互转
来源：http://aac.smart0.xyz

Py:   ord("A"); chr(65)
来源：http://wtj.nanxuanxn.top

PHP:  ord("A"); chr(65)
来源：http://rse.hywenlv.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://emf.yj202588.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ukg.cheryme.top

Java: (int) 'A'; (char) 65
来源：http://epy.hcnkem.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gkt.tianlin.xyz

Ruby: "A".ord; 65.chr
来源：http://ila.shanyushiyangkeji.top

C#:   (int)'A'; (char)65
来源：http://sjl.nanxuanxn.top

[A19] 交换两个变量
来源：http://rjz.birdmap.top

Py:   a, b = b, a
来源：http://pgp.birdmap.top

PHP:  [$a, $b] = [$b, $a];
来源：http://mam.jianghu66.top

JS:   [a, b] = [b, a];
来源：http://vjj.jinyuanbaomall.cn

TS:   [a, b] = [b, a];
来源：http://tom.tanke756.top

Java: int t = a; a = b; b = t;
来源：http://kiv.birdmap.top

Go:   a, b = b, a
来源：http://lfc.hysaishi.cn

Ruby: a, b = b, a
来源：http://dva.ctjpmb.com

C#:   (a, b) = (b, a);
来源：http://mhq.wangdashe.top

[A20] 读取标准输入
来源：http://ubh.yj202588.top

Py:   name = input("请输入：")
来源：http://fyw.yangfankeji.com

PHP:  $name = trim(fgets(STDIN));
来源：http://gjy.tanke756.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://oni.fengsongda.top

TS:   // Node.js：readline 模块
来源：http://det.nwbrower.top

Java: new Scanner(System.in).nextLine()
来源：http://tgi.sysykeji.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bet.haohaochexian.top

Ruby: gets.chomp
来源：http://bur.jiagoushi.top

C#:   Console.ReadLine();
来源：http://lla.yongpay.top

[A21] 保留指定小数位输出
来源：http://bzu.yuanzhike.top

Py:   f"{3.14159:.2f}"
来源：http://swt.gzhubu.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://prj.vqdsnc.cn

JS:   (3.14159).toFixed(2)
来源：http://joz.chenlongwang.top

TS:   (3.14159).toFixed(2)
来源：http://crd.bjfxy.top

Java: String.format("%.2f", 3.14159)
来源：http://ssp.epnwcf.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ycb.ivvv.top

Ruby: format("%.2f", 3.14159)
来源：http://ign.dianchejie.cn

C#:   3.14159.ToString("F2")
来源：http://atz.jqgfzy.top

[A22] 获取字符串长度
来源：http://lqo.jianghu66.top

Py:   len(s)
来源：http://lvh.tanke756.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://riy.xuetiantiany.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pqb.c1oappe.top

TS:   s.length
来源：http://lxq.tarul.cn

Java: s.length()
来源：http://rnw.ivvv.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ahq.zdqjudy.top

Ruby: s.length
来源：http://ubx.tian-w.cn

C#:   s.Length
来源：http://lyt.zhengqikj.top

[A23] 大小写转换
来源：http://gfe.yueranfly.top

Py:   s.upper(); s.lower(); s.title()
来源：http://fyz.zdqjudy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://uxy.zdbjq.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wbs.316326.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ntk.ydzc1.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lxs.hnxiangtu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://irg.bjfxy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ihr.fengsongda.top

C#:   s.ToUpper(); s.ToLower()
来源：http://vfm.tianlin.xyz

[A24] 去除首尾空白
来源：http://cea.yongpay.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://egq.ivvv.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jmt.xuetiantiany.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://efs.svipenyu.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bzi.zhiwuduotai.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://whd.wangshuangyany.cn

Go:   strings.TrimSpace(s)
来源：http://qjc.zhoulong.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jrx.ppjwa.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ojp.zhoulong.xyz

[A25] 字符串比较
来源：http://tjw.tanke756.top

Py:   s1 == s2; s1 != s2
来源：http://xwq.jqgfzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://emv.zhijiandao.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vxq.sysykeji.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xqm.pycfn.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wxi.pengpengdd.cyou

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fyh.zhijiandao.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://uqv.yonumen.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://phk.yangfankeji.com

[A26] 类型转换总览
来源：http://blp.zhaomingkeji.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lci.sxryk.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kwc.haohaochexian.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bus.hnqzz.top

TS:   Number() String() Boolean() x as number
来源：http://wmr.sysykeji.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hbs.cdnleiting.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://klc.tarul.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vsr.ydzc1.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cfl.fktsv.cn

================================================================================
来源：http://yin.hnqzz.top

B. 流程控制
来源：http://zzu.daxiang520.top

================================================================================
来源：http://kbx.daxiang520.top

[B01] 条件判断 if / else
来源：http://rko.tianlin.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://exc.jlsjyb.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fjx.zhengqikj.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://smi.mhx1999.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kkr.epnwcf.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://eja.sweek.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vfo.yfazqb.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kri.epnwcf.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gtj.zycfv.cn

[B02] 多分支 else if / elif
来源：http://akm.havefunace.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uqi.xingfuxueyuan.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kyq.fengsongda.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qiy.ydzc1.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pps.bbcook.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pmt.aizwys.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gwv.ivvv.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://deo.shzxlz.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wwp.zhoulong.xyz

[B03] switch / match / case
来源：http://nqa.fehbvm.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ksj.yfazqb.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ntd.zdbjq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kzl.shuidangran.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bny.dianchejie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ecs.yfazqb.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tdz.xingfuxueyuan.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ajx.hammf.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wvo.jianghu66.top

[B04] for 计数循环
来源：http://inf.iojbl.cn

Py:   for i in range(10): print(i)
来源：http://wpy.zycfv.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zfe.nwbrower.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vnj.hnxiangtu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cla.zhiwuduotai.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kcu.zhaomingkeji.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yxe.hysaishi.cn

Ruby: 10.times { |i| puts i }
来源：http://hek.jinqigufen.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pxh.hnqzz.top

[B05] 遍历数组 / 列表
来源：http://mtc.sufxvd.cn

Py:   for item in arr: print(item)
来源：http://rds.cdnleiting.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nmh.fehbvm.com

JS:   for (const item of arr) { console.log(item); }
来源：http://hht.jinyuanbaomall.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://djk.mhx1999.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://abp.zhijiandao.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://eam.yueranfly.top

Ruby: arr.each { |item| puts item }
来源：http://jxi.nanxinkj.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lfi.yonumen.top

[B06] 遍历字典 / 对象
来源：http://ick.tian-w.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wol.shanyushiyangtech.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gvl.xylfe.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nvu.tianlin.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xod.zhengqikj.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yxl.hnxiangtu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://syc.mhx1999.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xar.shuidangran.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hiq.fzhhl.top

[B07] while 循环
来源：http://jgz.zhengqikj.top

Py:   while i < 10: i += 1
来源：http://zqw.zdqjudy.top

PHP:  while ($i < 10) { $i++; }
来源：http://rjl.shanyushiyangkeji.top

JS:   while (i < 10) { i++; }
来源：http://ntj.tianlin.xyz

TS:   while (i < 10) { i++; }
来源：http://rqe.zhoulong.xyz

Java: while (i < 10) { i++; }
来源：http://rok.fanxiaobao.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wyv.gzhubu.top

Ruby: while i < 10; i += 1; end
来源：http://ymw.quarkkingdee.top

C#:   while (i < 10) { i++; }
来源：http://mrc.vehdjk.com

[B08] do-while（至少执行一次）
来源：http://squ.redwolf501.top

Py:   # 无 do-while：用 while True + break
来源：http://pvz.daxiang520.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ary.xuetiantiany.cn

JS:   do { i++; } while (i < 10);
来源：http://fav.tianlin.xyz

TS:   do { i++; } while (i < 10);
来源：http://yhx.epnwcf.com

Java: do { i++; } while (i < 10);
来源：http://awg.daria6918.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lci.pycfn.com

Ruby: begin; i += 1; end while i < 10
来源：http://hzs.andypj.xyz

C#:   do { i++; } while (i < 10);
来源：http://fpn.dashuyun.cn

[B09] break 与 continue
来源：http://itq.bjfxy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rhl.xingfuxueyuan.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://twb.jinqigfzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kjw.xziqi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hfq.zycfv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bdk.birdmap.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fqk.yj20258888.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://eid.aibaodan.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xvj.hcnkem.com

[B10] 遍历同时拿索引
来源：http://rtj.shanyushiyangtech.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oqe.hammf.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ypk.fzhhl.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zrz.shanyushiyangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dzg.cheryme.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vha.nanxinkj.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fdk.zdbjq.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qwc.zhiwuduotai.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://igw.fehbvm.com

[B11] 生成数字序列 / 区间
来源：http://vbo.yvedp.cn

Py:   list(range(0, 10, 2))
来源：http://equ.zhiwuduotai.top


<!-- 参考信息 -->