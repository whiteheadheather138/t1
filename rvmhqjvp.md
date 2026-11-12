代发 wailian999

JS:   const PI = 3.14159;
来源：http://blq.wangshuangyany.cn

TS:   const PI: number = 3.14159;
来源：http://dmu.pycfn.com

Java: static final double PI = 3.14159;
来源：http://lce.haohaochexian.top

Go:   const PI = 3.14159
来源：http://ozp.jiagoushi.top

Ruby: PI = 3.14159
来源：http://yqm.jlsjyb.cn

C#:   const double PI = 3.14159;
来源：http://taw.aizwys.cn

[A04] 判断变量类型
来源：http://vth.fktsv.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hot.andypj.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://odv.hywenlv.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://grn.ehwqpu.com

TS:   typeof x; x instanceof Date
来源：http://qoc.fktsv.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ueq.hcnkem.com

Go:   reflect.TypeOf(x).Name()
来源：http://ert.yueranfly.top

Ruby: x.class; x.is_a?(Integer)
来源：http://sjq.fehbvm.com

C#:   x.GetType().Name; x is int
来源：http://odc.epnwcf.com

[A05] 整数除法与取模
来源：http://brn.xuanzx.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://etw.tianlin.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://sxx.dianchejie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://num.cqqwz.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ujl.cdnleiting.top

Java: 7 / 2; 7 % 2
来源：http://epr.xuetiantiany.cn

Go:   7 / 2; 7 % 2
来源：http://ink.cqqwz.cn

Ruby: 7 / 2; 7 % 2
来源：http://wzr.fehbvm.com

C#:   7 / 2; 7 % 2
来源：http://nir.cqqwz.cn

[A06] 字符串转数字
来源：http://zkt.xuanzx.com

Py:   int("42"); float("3.14")
来源：http://spt.jyoumei.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cbc.jiagoushi.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ieo.dashuyun.cn

TS:   parseInt("42", 10); Number("42")
来源：http://kmw.pengpengdd.cyou

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ecs.wangdashe.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rcp.jiagoushi.top

Ruby: "42".to_i; "3.14".to_f
来源：http://xnb.yuanzhike.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dnu.sysykeji.top

[A07] 数字转字符串
来源：http://xhv.yonumen.top

Py:   str(42)
来源：http://qst.haohaochexian.top

PHP:  (string) 42; strval(42)
来源：http://syr.snrcjt.cn

JS:   String(42); (42).toString()
来源：http://fle.yueranfly.top

TS:   String(42)
来源：http://mkw.tian-w.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://kxw.fktsv.cn

Go:   strconv.Itoa(42)
来源：http://ynw.andypj.xyz

Ruby: 42.to_s
来源：http://kjq.jqgfzy.top

C#:   42.ToString()
来源：http://tis.gotoacloud.top

[A08] 取整与四舍五入
来源：http://tsd.ivvv.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zst.hesvh.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://avi.feifeiyinyue.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pob.yj202588.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fgl.ppjwa.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pzg.fzhhl.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qyk.jyoumei.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://gwd.9152youxi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mye.jianghu66.top

[A09] 绝对值与最大最小值
来源：http://cjm.shanyushiyangtech.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://uwb.jiagoushi.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cdm.zycfv.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ggq.ehwqpu.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ssx.xuanzx.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mhf.52xcode.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://iwr.sjlbkw.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jnk.tarul.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zsj.haohaochexian.top

[A10] 生成随机数
来源：http://yau.xuanzx.com

Py:   import random; random.randint(1, 100)
来源：http://rzt.yanxiufei.cn

PHP:  random_int(1, 100);
来源：http://cye.hammf.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wnc.ivvv.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qdm.yuanzhike.top

Java: new Random().nextInt(100) + 1
来源：http://dsu.cashguo.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://srw.wangdashe.top

Ruby: rand(1..100)
来源：http://xki.dashuyun.cn

C#:   new Random().Next(1, 101)
来源：http://ush.dashuyun.cn

[A11] 条件表达式（三元）
来源：http://mmm.316326.xyz

Py:   "yes" if x > 0 else "no"
来源：http://qhl.shanyushiyangkeji.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://lvd.ydzc1.top

JS:   x > 0 ? "yes" : "no"
来源：http://pni.cashguo.top

TS:   x > 0 ? "yes" : "no"
来源：http://sbr.guannengcc.top

Java: x > 0 ? "yes" : "no"
来源：http://wbd.fehbvm.com

Go:   // 无三元运算符，需用 if 语句
来源：http://gft.ivvv.top

Ruby: x > 0 ? "yes" : "no"
来源：http://kyp.hfpthk.cn

C#:   x > 0 ? "yes" : "no"
来源：http://tah.gzhubu.top

[A12] 字符串插值 / 格式化
来源：http://sfl.yongpay.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://usf.quarkkingdee.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gnp.xylfe.cn

JS:   `Hello, ${name}!`
来源：http://son.meibo888.top

TS:   `Hello, ${name}!`
来源：http://adx.shanyushiyangtech.top

Java: "Hello, %s!".formatted(name)
来源：http://lxo.sjlbkw.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cjc.daxiang520.top

Ruby: "Hello, #{name}!"
来源：http://kgb.wangshuangyany.cn

C#:   $"Hello, {name}!"
来源：http://lfb.yueranfly.top

[A13] 多行字符串（练习 \n 转义）
来源：http://okb.zhiwuduotai.top

Py:   "第一行\n第二行"
来源：http://bwz.pengpengdd.cyou

PHP:  "第一行\n第二行"
来源：http://dtu.daxiang520.top

JS:   "第一行\n第二行"
来源：http://pue.zhijiandao.cn

TS:   "第一行\n第二行"
来源：http://ouz.shanyushiyangkeji.top

Java: "第一行\n第二行"
来源：http://ccg.jyoumei.cn

Go:   "第一行\n第二行"
来源：http://mbp.fzhhl.top

Ruby: "第一行\n第二行"
来源：http://jsm.haohaochexian.top

C#:   "第一行\n第二行"
来源：http://xht.52xcode.cn

[A14] 注释写法
来源：http://dss.wangshuangyany.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://pwg.xziqi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://lap.yvedp.cn

JS:   // 单行；/* 多行 */
来源：http://kfu.bjfxy.top

TS:   // 单行；/* 多行 */
来源：http://hql.wangdashe.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dbm.9152youxi.cn

Go:   // 单行；/* 多行 */
来源：http://cxh.xingfuxueyuan.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://qbe.gotoacloud.top

C#:   // 单行；/* 多行 */
来源：http://qzm.nanxinkj.top

[A15] 空值判断与默认值
来源：http://emb.9152youxi.cn

Py:   value = data or "默认值"
来源：http://tzh.sxryk.cn

PHP:  $value = $data ?? "默认值";
来源：http://ffo.jinqigufen.top

JS:   const value = data ?? "默认值";
来源：http://chk.shangyingyoupin.top

TS:   const value = data ?? "默认值";
来源：http://vrr.chenjidiqi.icu

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ajb.hammf.cn

Go:   if data == "" { data = "默认值" }
来源：http://woo.ydjk.org.cn

Ruby: value = data || "默认值"
来源：http://koy.chenjidiqi.icu

C#:   var value = data ?? "默认值";
来源：http://cyl.sysykeji.top

[A16] 真假值判断规则
来源：http://yzg.yanxiufei.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jfo.fanxiaobao.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vsx.hnqzz.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lbz.shuidangran.top

TS:   if (!x) {}
来源：http://odn.kuanghao11.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lll.xziqi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://txc.hammf.cn

Ruby: unless x            # nil 与 false 为假
来源：http://yyn.meibo888.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ouu.yanxiufei.cn

[A17] 位运算
来源：http://des.gaohongyu789.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kmm.jqgfzy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://yhb.xylfe.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://chp.fengsongda.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ugc.nwbrower.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gjp.dashuyun.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gwa.jqgufenzy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://und.hnqzz.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ulp.fzhhl.top

[A18] 字符与 ASCII 码互转
来源：http://uzj.cheryme.top

Py:   ord("A"); chr(65)
来源：http://leu.jinqigufen.top

PHP:  ord("A"); chr(65)
来源：http://nmq.ehwqpu.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zbc.bbcook.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://khe.sjlbkw.cn

Java: (int) 'A'; (char) 65
来源：http://ity.zhaomingkeji.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qkk.0kj1m.cn

Ruby: "A".ord; 65.chr
来源：http://wiw.xziqi.cn

C#:   (int)'A'; (char)65
来源：http://qbh.fengsongda.top

[A19] 交换两个变量
来源：http://uin.zhiwuduotai.top

Py:   a, b = b, a
来源：http://jgx.ppjwa.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://lil.hywenlv.cn

JS:   [a, b] = [b, a];
来源：http://avq.hysaishi.cn

TS:   [a, b] = [b, a];
来源：http://jhi.hfpthk.cn

Java: int t = a; a = b; b = t;
来源：http://hnu.xylfe.cn

Go:   a, b = b, a
来源：http://pkw.chenzaomai.com

Ruby: a, b = b, a
来源：http://rmb.yfazqb.com

C#:   (a, b) = (b, a);
来源：http://dec.gogol.net.cn

[A20] 读取标准输入
来源：http://hak.epnwcf.com

Py:   name = input("请输入：")
来源：http://npr.jinghuilouyu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://vin.andypj.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sye.fanxiaobao.xyz

TS:   // Node.js：readline 模块
来源：http://vpc.zhixingplan.top

Java: new Scanner(System.in).nextLine()
来源：http://skf.jinyuanbaomall.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lou.zhijiandao.cn

Ruby: gets.chomp
来源：http://dqu.jinqigfzy.top

C#:   Console.ReadLine();
来源：http://niu.jianghu66.top

[A21] 保留指定小数位输出
来源：http://sar.gzhubu.top

Py:   f"{3.14159:.2f}"
来源：http://voy.jinqigufen.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yda.wangshuangyany.cn

JS:   (3.14159).toFixed(2)
来源：http://ues.pengpengdd.cyou

TS:   (3.14159).toFixed(2)
来源：http://lyv.zhoulong.xyz

Java: String.format("%.2f", 3.14159)
来源：http://qas.daria6918.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ddp.yfazqb.com

Ruby: format("%.2f", 3.14159)
来源：http://gko.quarkkingdee.top

C#:   3.14159.ToString("F2")
来源：http://kvd.birdmap.top

[A22] 获取字符串长度
来源：http://ywx.aibaodan.cn

Py:   len(s)
来源：http://onk.quarkkingdee.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kvj.ywan-chungtsiang.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ruk.yfazqb.com

TS:   s.length
来源：http://cdi.shangyingyoupin.top

Java: s.length()
来源：http://tyu.snrcjt.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://psb.svipenyu.cn

Ruby: s.length
来源：http://kvm.epnwcf.com

C#:   s.Length
来源：http://btz.zhijiandao.cn

[A23] 大小写转换
来源：http://ikp.aibaodan.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://acn.0kj1m.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://frl.bjfxy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://iwf.jinqigufen.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://okl.guowangkeji.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dka.yj202588.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fbb.hnxiangtu.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vmz.ybcxt.top

C#:   s.ToUpper(); s.ToLower()
来源：http://icd.fktsv.cn

[A24] 去除首尾空白
来源：http://kcm.sufxvd.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pku.gzhubu.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zsx.gzhubu.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://unt.316326.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ihj.chenlongwang.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qzp.cdnleiting.top

Go:   strings.TrimSpace(s)
来源：http://qhk.xylfe.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rdb.c1oappe.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pvi.yj20258.top

[A25] 字符串比较
来源：http://orc.hammf.cn

Py:   s1 == s2; s1 != s2
来源：http://lgw.jinghuilouyu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://duu.xinyue.icu

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://acr.nwbrower.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ijz.zhengqikj.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qol.ehwqpu.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tlf.zhijiandao.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://prf.fktsv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nqo.jinghuilouyu.cn

[A26] 类型转换总览
来源：http://yhb.hnqzz.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ghf.meibo888.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ixf.fehbvm.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fkc.yanxiufei.cn

TS:   Number() String() Boolean() x as number
来源：http://olf.yj202588.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pjv.jqgufenzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://uiz.ydzc1.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://tls.wangshuangyany.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qxr.ppjwa.cn

================================================================================
来源：http://pyl.aibaodan.cn

B. 流程控制
来源：http://vrp.tianlin.xyz

================================================================================
来源：http://naz.hfpthk.cn

[B01] 条件判断 if / else
来源：http://pod.ydjk.org.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dhr.hcnkem.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vag.hesvh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zlu.yanxiufei.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dpj.jqgfzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ejh.quarkkingdee.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fvl.zhongyouzk.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wwf.c1oappe.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jaf.cheryme.top

[B02] 多分支 else if / elif
来源：http://vpe.yongpay.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bhm.tarul.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dwf.chenjidiqi.icu

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lof.shangyingyoupin.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xyf.gotoacloud.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fcc.sjlbkw.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nen.yongpay.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://iao.0kj1m.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ues.0kj1m.cn

[B03] switch / match / case
来源：http://qgl.ehwqpu.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hgy.birdmap.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://szi.daria6918.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zed.zycfv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wjg.c1oappe.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ovu.havefunace.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kkt.xinyue.icu

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uxz.snrcjt.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dgg.jianghu66.top

[B04] for 计数循环
来源：http://ruk.nwbrower.top

Py:   for i in range(10): print(i)
来源：http://gty.zdqjudy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kpj.jianghu66.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fgw.tarul.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xov.yuxming.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hkh.epnwcf.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tlv.jlsjyb.cn

Ruby: 10.times { |i| puts i }
来源：http://tex.smart0.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wmg.cdnleiting.top

[B05] 遍历数组 / 列表
来源：http://fvy.jyoumei.cn

Py:   for item in arr: print(item)
来源：http://xmo.yongpay.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ked.sysykeji.top

JS:   for (const item of arr) { console.log(item); }
来源：http://owk.jqgfzy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://jyk.cdnleiting.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ekf.hammf.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bnq.yuanzhike.top

Ruby: arr.each { |item| puts item }
来源：http://him.9152youxi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://evc.zdbjq.cn

[B06] 遍历字典 / 对象
来源：http://jiq.zdbjq.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zlc.c1oappe.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vpg.nanxinkj.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fld.gzhubu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iyh.hongshengwenyu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fkb.snrcjt.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wtp.yueranfly.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hxi.hesvh.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ozs.yvedp.cn

[B07] while 循环
来源：http://vtq.ehwqpu.com

Py:   while i < 10: i += 1
来源：http://pwn.bbcook.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lot.hongshengwenyu.top

JS:   while (i < 10) { i++; }
来源：http://euk.sysykeji.top

TS:   while (i < 10) { i++; }
来源：http://raa.bbcook.cn

Java: while (i < 10) { i++; }
来源：http://hal.smart0.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sqk.yj20258.top

Ruby: while i < 10; i += 1; end
来源：http://mav.vehdjk.com

C#:   while (i < 10) { i++; }
来源：http://ukd.havefunace.top

[B08] do-while（至少执行一次）
来源：http://qkj.cheryme.top

Py:   # 无 do-while：用 while True + break
来源：http://dqt.aibaodan.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ytt.svipenyu.cn

JS:   do { i++; } while (i < 10);
来源：http://kwr.jinghuilouyu.cn

TS:   do { i++; } while (i < 10);
来源：http://ets.vehdjk.com

Java: do { i++; } while (i < 10);
来源：http://zew.ywan-chungtsiang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://bwu.hcnkem.com

Ruby: begin; i += 1; end while i < 10
来源：http://mvi.shanyushiyangtech.top

C#:   do { i++; } while (i < 10);
来源：http://rjj.52xcode.cn

[B09] break 与 continue
来源：http://qws.zhijiandao.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://npc.vehdjk.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ibf.jinyuanbaomall.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nqa.fktsv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uqq.cucudq.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nqx.xylfe.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pby.havefunace.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zwp.haohaochexian.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hrp.sufxvd.cn

[B10] 遍历同时拿索引
来源：http://wgw.hysaishi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dhy.xuetiantiany.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wgk.316326.xyz


<!-- 参考信息 -->