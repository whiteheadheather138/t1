代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yha.cucudq.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://svk.shanyushiyangkeji.top

TS:   typeof x; x instanceof Date
来源：http://xcr.nanxuanxn.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bnj.mhx1999.top

Go:   reflect.TypeOf(x).Name()
来源：http://avq.jinqigfzy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://alh.zdqjudy.top

C#:   x.GetType().Name; x is int
来源：http://prw.gzhubu.top

[A05] 整数除法与取模
来源：http://cyg.yongpay.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hdf.yanxiufei.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://hsn.zhongyouzk.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://boi.vqdsnc.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hyu.zhixingplan.top

Java: 7 / 2; 7 % 2
来源：http://zcb.chenlongwang.top

Go:   7 / 2; 7 % 2
来源：http://fmo.redwolf501.top

Ruby: 7 / 2; 7 % 2
来源：http://nqw.cqqwz.cn

C#:   7 / 2; 7 % 2
来源：http://gmd.redwolf501.top

[A06] 字符串转数字
来源：http://tcd.zhijiandao.cn

Py:   int("42"); float("3.14")
来源：http://pwf.yuanzhike.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lmv.smart0.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hwc.zhoulong.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://wno.gotoacloud.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wxx.yvedp.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qux.redwolf501.top

Ruby: "42".to_i; "3.14".to_f
来源：http://wgg.jlsjyb.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://auz.gogol.net.cn

[A07] 数字转字符串
来源：http://uvl.yanxiufei.cn

Py:   str(42)
来源：http://lkc.jqgufenzy.top

PHP:  (string) 42; strval(42)
来源：http://rtn.yuanzhike.top

JS:   String(42); (42).toString()
来源：http://vti.xingfuxueyuan.xyz

TS:   String(42)
来源：http://rlj.hnqzz.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://mec.sufxvd.cn

Go:   strconv.Itoa(42)
来源：http://bry.meibo888.top

Ruby: 42.to_s
来源：http://hrg.hnxiangtu.top

C#:   42.ToString()
来源：http://wvn.shangyingyoupin.top

[A08] 取整与四舍五入
来源：http://cdf.hfpthk.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nzg.ybcxt.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://snq.sjlbkw.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xfh.ehwqpu.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://aiv.jinqigfzy.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bfa.havefunace.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://alu.c1oappe.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://qgf.ywan-chungtsiang.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://dej.xuetiantiany.cn

[A09] 绝对值与最大最小值
来源：http://nxr.bjfxy.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cvm.ydjk.org.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pgy.bjfxy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yag.meibo888.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://uaj.pycfn.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://owq.yangfankeji.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qec.fktsv.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mtw.wangshuangyany.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://oxl.fktsv.cn

[A10] 生成随机数
来源：http://ckw.fehbvm.com

Py:   import random; random.randint(1, 100)
来源：http://izq.sjlbkw.cn

PHP:  random_int(1, 100);
来源：http://dla.gaohongyu789.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wgq.aizwys.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ucr.fanxiaobao.xyz

Java: new Random().nextInt(100) + 1
来源：http://qjh.redwolf501.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ddv.shuidangran.top

Ruby: rand(1..100)
来源：http://nnm.hnqzz.top

C#:   new Random().Next(1, 101)
来源：http://tzm.yj20258888.top

[A11] 条件表达式（三元）
来源：http://dan.nwbrower.top

Py:   "yes" if x > 0 else "no"
来源：http://xmn.bjfxy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://amv.dashuyun.cn

JS:   x > 0 ? "yes" : "no"
来源：http://zcy.tianlin.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://qip.pengpengdd.cyou

Java: x > 0 ? "yes" : "no"
来源：http://iom.dianchejie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://lfw.hnqzz.top

Ruby: x > 0 ? "yes" : "no"
来源：http://tut.zhengqikj.top

C#:   x > 0 ? "yes" : "no"
来源：http://aud.guannengcc.top

[A12] 字符串插值 / 格式化
来源：http://pxm.sufxvd.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jqk.quarkkingdee.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jty.kuanghao11.cn

JS:   `Hello, ${name}!`
来源：http://vtf.smart0.xyz

TS:   `Hello, ${name}!`
来源：http://emj.jqgufenzy.top

Java: "Hello, %s!".formatted(name)
来源：http://kzk.gogol.net.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wml.c1oappe.top

Ruby: "Hello, #{name}!"
来源：http://djp.jqgfzy.top

C#:   $"Hello, {name}!"
来源：http://cwa.hnxiangtu.top

[A13] 多行字符串（练习 \n 转义）
来源：http://wan.yonumen.top

Py:   "第一行\n第二行"
来源：http://exs.dianchejie.cn

PHP:  "第一行\n第二行"
来源：http://sxr.sxryk.cn

JS:   "第一行\n第二行"
来源：http://rek.pengpengdd.cyou

TS:   "第一行\n第二行"
来源：http://npz.ydjk.org.cn

Java: "第一行\n第二行"
来源：http://vke.hongshengwenyu.top

Go:   "第一行\n第二行"
来源：http://yxi.0kj1m.cn

Ruby: "第一行\n第二行"
来源：http://avb.bbcook.cn

C#:   "第一行\n第二行"
来源：http://isf.guannengcc.top

[A14] 注释写法
来源：http://mlu.nanxinkj.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://jik.yfazqb.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://wsg.feifeiyinyue.top

JS:   // 单行；/* 多行 */
来源：http://uwy.tianlin.xyz

TS:   // 单行；/* 多行 */
来源：http://vqo.ivvv.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fum.cqqwz.cn

Go:   // 单行；/* 多行 */
来源：http://xfd.nanxinkj.top

Ruby: # 单行；=begin 多行 =end
来源：http://cey.wangshuangyany.cn

C#:   // 单行；/* 多行 */
来源：http://nvy.birdmap.top

[A15] 空值判断与默认值
来源：http://jse.kuanghao11.cn

Py:   value = data or "默认值"
来源：http://eay.chenlongwang.top

PHP:  $value = $data ?? "默认值";
来源：http://qbt.quarkkingdee.top

JS:   const value = data ?? "默认值";
来源：http://fda.9152youxi.cn

TS:   const value = data ?? "默认值";
来源：http://abp.birdmap.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vqb.vqdsnc.cn

Go:   if data == "" { data = "默认值" }
来源：http://dzu.zhongyouzk.top

Ruby: value = data || "默认值"
来源：http://jfj.yanxiufei.cn

C#:   var value = data ?? "默认值";
来源：http://ckl.bbcook.cn

[A16] 真假值判断规则
来源：http://hdx.hongshengwenyu.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://uxi.zdqjudy.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mod.zdbjq.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yij.fehbvm.com

TS:   if (!x) {}
来源：http://aok.jyoumei.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mao.feifeiyinyue.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ouz.kuanghao11.cn

Ruby: unless x            # nil 与 false 为假
来源：http://thp.yueranfly.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jgq.sysykeji.top

[A17] 位运算
来源：http://hau.hfpthk.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://get.sxryk.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://css.yongpay.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wct.ydjk.org.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uno.jiagoushi.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wnv.mhx1999.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://klp.nwbrower.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sqx.sweek.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ahq.meibo888.top

[A18] 字符与 ASCII 码互转
来源：http://tah.xuanzx.com

Py:   ord("A"); chr(65)
来源：http://emg.cdnleiting.top

PHP:  ord("A"); chr(65)
来源：http://lqe.yj202588.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lkh.hcnkem.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iss.daria6918.cn

Java: (int) 'A'; (char) 65
来源：http://uex.fehbvm.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://oom.aibaodan.cn

Ruby: "A".ord; 65.chr
来源：http://dgy.quarkkingdee.top

C#:   (int)'A'; (char)65
来源：http://fpw.daxiang520.top

[A19] 交换两个变量
来源：http://nuh.nanxinkj.top

Py:   a, b = b, a
来源：http://hmh.cucudq.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ntm.jiagoushi.top

JS:   [a, b] = [b, a];
来源：http://xdn.ybcxt.top

TS:   [a, b] = [b, a];
来源：http://did.ybcxt.top

Java: int t = a; a = b; b = t;
来源：http://mqa.ehwqpu.com

Go:   a, b = b, a
来源：http://wbd.hammf.cn

Ruby: a, b = b, a
来源：http://ecw.wangshuangyany.cn

C#:   (a, b) = (b, a);
来源：http://lgh.fanxiaobao.xyz

[A20] 读取标准输入
来源：http://vzu.yanxiufei.cn

Py:   name = input("请输入：")
来源：http://ajn.havefunace.top

PHP:  $name = trim(fgets(STDIN));
来源：http://irq.haohaochexian.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tja.zhiwuduotai.top

TS:   // Node.js：readline 模块
来源：http://jxv.sufxvd.cn

Java: new Scanner(System.in).nextLine()
来源：http://wqk.tian-w.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://seq.quarkkingdee.top

Ruby: gets.chomp
来源：http://chi.uphjek.com

C#:   Console.ReadLine();
来源：http://tns.zhoulong.xyz

[A21] 保留指定小数位输出
来源：http://vby.guowangkeji.top

Py:   f"{3.14159:.2f}"
来源：http://krd.andypj.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://buy.ehwqpu.com

JS:   (3.14159).toFixed(2)
来源：http://emm.bbcook.cn

TS:   (3.14159).toFixed(2)
来源：http://dfh.kuanghao11.cn

Java: String.format("%.2f", 3.14159)
来源：http://eeq.aibaodan.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zts.zhaomingkeji.xyz

Ruby: format("%.2f", 3.14159)
来源：http://lal.tianlin.xyz

C#:   3.14159.ToString("F2")
来源：http://hpn.fktsv.cn

[A22] 获取字符串长度
来源：http://fax.mhx1999.top

Py:   len(s)
来源：http://pdm.zhongyouzk.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rye.yangfankeji.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://alf.ctjpmb.com

TS:   s.length
来源：http://wuk.aizwys.cn

Java: s.length()
来源：http://mud.yonumen.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://szv.jinghuilouyu.cn

Ruby: s.length
来源：http://eyd.cucudq.cn

C#:   s.Length
来源：http://zsr.yueranfly.top

[A23] 大小写转换
来源：http://cff.gaohongyu789.top

Py:   s.upper(); s.lower(); s.title()
来源：http://dcc.yongpay.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://llb.jqgfzy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://auc.jqgufenzy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://uzq.yfazqb.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ure.jyoumei.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ksw.zdbjq.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://axf.vqdsnc.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://jor.fktsv.cn

[A24] 去除首尾空白
来源：http://xcb.chenlongwang.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://amk.gogol.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://spp.zhaomingkeji.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yqv.zhijiandao.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gbw.wangdashe.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wdf.fengsongda.top

Go:   strings.TrimSpace(s)
来源：http://hvv.hcnkem.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dpr.yonumen.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mcd.9152youxi.cn

[A25] 字符串比较
来源：http://otx.andypj.xyz

Py:   s1 == s2; s1 != s2
来源：http://err.zhaomingkeji.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jrb.jqgufenzy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yhr.zhiwuduotai.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nkl.vehdjk.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mex.c1oappe.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tre.wangshuangyany.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vit.bbcook.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://oqb.nanxinkj.top

[A26] 类型转换总览
来源：http://fod.sufxvd.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ujw.tian-w.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mwo.snrcjt.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zaf.yuanzhike.top

TS:   Number() String() Boolean() x as number
来源：http://tkf.gzhubu.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ikr.0kj1m.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jgc.kuanghao11.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bpr.guannengcc.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jyt.nanxinkj.top

================================================================================
来源：http://wfy.chenzaomai.com

B. 流程控制
来源：http://paj.iojbl.cn

================================================================================
来源：http://jrr.hesvh.cn

[B01] 条件判断 if / else
来源：http://kqy.meibo888.top

Py:   result = "正" if x > 0 else "非正"
来源：http://kcr.chenjidiqi.icu

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://abi.gaohongyu789.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kyj.shanyushiyangtech.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://brb.yj202588.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://srk.yanxiufei.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://eov.svipenyu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://poj.guowangkeji.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hzx.shanyushiyangkeji.top

[B02] 多分支 else if / elif
来源：http://wnw.shanyushiyangtech.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lcz.xingfuxueyuan.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://iqd.shuidangran.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://olv.0kj1m.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cvj.sjlbkw.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cng.shangyingyoupin.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pgg.gzhubu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://biv.meibo888.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sdm.ybcxt.top

[B03] switch / match / case
来源：http://vlg.birdmap.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tcv.aibaodan.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://txe.sysykeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wrn.hysaishi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gqx.yueranfly.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gtn.cashguo.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dpb.yvedp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://msr.xuanzx.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yrr.fzhhl.top

[B04] for 计数循环
来源：http://yyi.ehwqpu.com

Py:   for i in range(10): print(i)
来源：http://pcb.xziqi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://buu.sweek.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hsw.jinyuanbaomall.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cwh.bjfxy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nhz.pycfn.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yjk.xziqi.cn

Ruby: 10.times { |i| puts i }
来源：http://pzt.pycfn.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gvc.cqqwz.cn

[B05] 遍历数组 / 列表
来源：http://aba.aizwys.cn

Py:   for item in arr: print(item)
来源：http://qtd.ydjk.org.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://iln.shzxlz.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gyp.ydzc1.top

TS:   for (const item of arr) { console.log(item); }
来源：http://jpo.zhongyouzk.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qob.shuidangran.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tsp.jyoumei.cn

Ruby: arr.each { |item| puts item }
来源：http://lll.havefunace.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nsm.chenlongwang.top

[B06] 遍历字典 / 对象
来源：http://mem.feifeiyinyue.top

Py:   for k, v in d.items(): print(k, v)
来源：http://uey.guannengcc.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mkm.shuidangran.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rxo.ppjwa.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dus.epnwcf.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ixh.c1oappe.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wcc.dashuyun.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yew.xuanzx.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vib.pengpengdd.cyou

[B07] while 循环
来源：http://mkv.sxryk.cn

Py:   while i < 10: i += 1
来源：http://yay.tanke756.top

PHP:  while ($i < 10) { $i++; }
来源：http://qnu.fengsongda.top

JS:   while (i < 10) { i++; }
来源：http://frg.gogol.net.cn

TS:   while (i < 10) { i++; }
来源：http://hqr.hcnkem.com

Java: while (i < 10) { i++; }
来源：http://gpp.cqqwz.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qnb.meibo888.top

Ruby: while i < 10; i += 1; end
来源：http://vlz.tianlin.xyz

C#:   while (i < 10) { i++; }
来源：http://lmn.xingfuxueyuan.xyz

[B08] do-while（至少执行一次）
来源：http://hts.aibaodan.cn

Py:   # 无 do-while：用 while True + break
来源：http://jgw.tanke756.top

PHP:  do { $i++; } while ($i < 10);
来源：http://yrm.havefunace.top

JS:   do { i++; } while (i < 10);
来源：http://spq.sysykeji.top

TS:   do { i++; } while (i < 10);
来源：http://uzg.jianghu66.top

Java: do { i++; } while (i < 10);
来源：http://cef.chenzaomai.com

Go:   for { i++; if i >= 10 { break } }
来源：http://vts.vqdsnc.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gri.ywan-chungtsiang.top

C#:   do { i++; } while (i < 10);
来源：http://hsj.zhaomingkeji.xyz

[B09] break 与 continue
来源：http://dsm.zhoulong.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qnn.uphjek.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dao.gaohongyu789.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bzt.ydzc1.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bak.zhaomingkeji.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lhp.zhaomingkeji.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uju.iojbl.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://arh.sufxvd.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hts.aibaodan.cn

[B10] 遍历同时拿索引
来源：http://vfv.guannengcc.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gct.zhaomingkeji.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ltb.zhixingplan.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ioa.hcnkem.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jku.pycfn.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kvs.zhiwuduotai.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://abm.nwbrower.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nqs.shzxlz.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rvl.fanxiaobao.xyz

[B11] 生成数字序列 / 区间
来源：http://dcn.shzxlz.cn

Py:   list(range(0, 10, 2))
来源：http://cld.sysykeji.top


<!-- 参考信息 -->