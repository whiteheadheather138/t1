代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gle.jinyuanbaomall.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pqe.guowangkeji.top

TS:   typeof x; x instanceof Date
来源：http://usi.yj20258888.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cyi.yj20258.top

Go:   reflect.TypeOf(x).Name()
来源：http://zyc.yuxming.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xgm.yueranfly.top

C#:   x.GetType().Name; x is int
来源：http://bhj.epnwcf.com

[A05] 整数除法与取模
来源：http://bvr.tanke756.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://myt.sjlbkw.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://spf.vehdjk.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://zla.smart0.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mzt.hnxiangtu.top

Java: 7 / 2; 7 % 2
来源：http://iif.ydjk.org.cn

Go:   7 / 2; 7 % 2
来源：http://znk.hnxiangtu.top

Ruby: 7 / 2; 7 % 2
来源：http://xdu.yangfankeji.com

C#:   7 / 2; 7 % 2
来源：http://bnv.cqqwz.cn

[A06] 字符串转数字
来源：http://vhc.fanxiaobao.xyz

Py:   int("42"); float("3.14")
来源：http://vlp.vehdjk.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dfy.hnqzz.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://utj.zhongyouzk.top

TS:   parseInt("42", 10); Number("42")
来源：http://yoi.jinqigfzy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vtm.zhixingplan.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://epp.tanke756.top

Ruby: "42".to_i; "3.14".to_f
来源：http://qil.zycfv.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://erl.snrcjt.cn

[A07] 数字转字符串
来源：http://uye.aibaodan.cn

Py:   str(42)
来源：http://ruc.fzhhl.top

PHP:  (string) 42; strval(42)
来源：http://tog.zdbjq.cn

JS:   String(42); (42).toString()
来源：http://lxq.chenzaomai.com

TS:   String(42)
来源：http://eer.yueranfly.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://jth.ydjk.org.cn

Go:   strconv.Itoa(42)
来源：http://lzz.cdnleiting.top

Ruby: 42.to_s
来源：http://yhe.jinyuanbaomall.cn

C#:   42.ToString()
来源：http://bls.zdbjq.cn

[A08] 取整与四舍五入
来源：http://azh.ydjk.org.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cph.daxiang520.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://sgg.xuetiantiany.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://snt.yueranfly.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ikq.vqdsnc.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wfu.iojbl.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ylr.316326.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://szw.fengsongda.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://clk.yangfankeji.com

[A09] 绝对值与最大最小值
来源：http://akv.cdnleiting.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ade.yuxming.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://akc.uphjek.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tiv.yangfankeji.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cjg.yueranfly.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wzf.havefunace.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hwu.jinghuilouyu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dou.yanxiufei.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qys.guowangkeji.top

[A10] 生成随机数
来源：http://fti.shanyushiyangtech.top

Py:   import random; random.randint(1, 100)
来源：http://mlo.andypj.xyz

PHP:  random_int(1, 100);
来源：http://vol.shzxlz.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://okx.xylfe.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wkn.hysaishi.cn

Java: new Random().nextInt(100) + 1
来源：http://qfy.mhx1999.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tqn.bjfxy.top

Ruby: rand(1..100)
来源：http://lbh.nanxinkj.top

C#:   new Random().Next(1, 101)
来源：http://nla.kuanghao11.cn

[A11] 条件表达式（三元）
来源：http://fly.andypj.xyz

Py:   "yes" if x > 0 else "no"
来源：http://dwk.0kj1m.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://msb.yj202588.top

JS:   x > 0 ? "yes" : "no"
来源：http://lhc.yj20258888.top

TS:   x > 0 ? "yes" : "no"
来源：http://irg.tianlin.xyz

Java: x > 0 ? "yes" : "no"
来源：http://ldc.yj20258.top

Go:   // 无三元运算符，需用 if 语句
来源：http://rlb.haohaochexian.top

Ruby: x > 0 ? "yes" : "no"
来源：http://cin.yj20258.top

C#:   x > 0 ? "yes" : "no"
来源：http://lby.hongshengwenyu.top

[A12] 字符串插值 / 格式化
来源：http://adw.xuetiantiany.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fmq.chenlongwang.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://keq.hammf.cn

JS:   `Hello, ${name}!`
来源：http://rkj.ppjwa.cn

TS:   `Hello, ${name}!`
来源：http://jam.zycfv.cn

Java: "Hello, %s!".formatted(name)
来源：http://qrt.chenzaomai.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fuo.jinyuanbaomall.cn

Ruby: "Hello, #{name}!"
来源：http://qap.yj20258.top

C#:   $"Hello, {name}!"
来源：http://pwa.cucudq.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://oox.xinyue.icu

Py:   "第一行\n第二行"
来源：http://qvv.yueranfly.top

PHP:  "第一行\n第二行"
来源：http://mcs.zhaomingkeji.xyz

JS:   "第一行\n第二行"
来源：http://ked.tarul.cn

TS:   "第一行\n第二行"
来源：http://dox.0kj1m.cn

Java: "第一行\n第二行"
来源：http://rmx.nanxinkj.top

Go:   "第一行\n第二行"
来源：http://rly.yfazqb.com

Ruby: "第一行\n第二行"
来源：http://wbt.yanxiufei.cn

C#:   "第一行\n第二行"
来源：http://vku.hfpthk.cn

[A14] 注释写法
来源：http://lpv.xylfe.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://dvf.jinqigufen.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ngz.yj20258.top

JS:   // 单行；/* 多行 */
来源：http://lxu.tianlin.xyz

TS:   // 单行；/* 多行 */
来源：http://qjd.sweek.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://oon.sjlbkw.cn

Go:   // 单行；/* 多行 */
来源：http://wkb.uphjek.com

Ruby: # 单行；=begin 多行 =end
来源：http://mue.hongshengwenyu.top

C#:   // 单行；/* 多行 */
来源：http://qxa.yuxming.cn

[A15] 空值判断与默认值
来源：http://iom.yvedp.cn

Py:   value = data or "默认值"
来源：http://imn.sjlbkw.cn

PHP:  $value = $data ?? "默认值";
来源：http://yvq.gzhubu.top

JS:   const value = data ?? "默认值";
来源：http://vrq.guannengcc.top

TS:   const value = data ?? "默认值";
来源：http://mpw.snrcjt.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wmb.zhengqikj.top

Go:   if data == "" { data = "默认值" }
来源：http://gnf.jinyuanbaomall.cn

Ruby: value = data || "默认值"
来源：http://ndb.jinqigufen.top

C#:   var value = data ?? "默认值";
来源：http://mcg.chenzaomai.com

[A16] 真假值判断规则
来源：http://oms.chenzaomai.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fkr.uphjek.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ovg.fehbvm.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://epe.quarkkingdee.top

TS:   if (!x) {}
来源：http://imo.shanyushiyangtech.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fmr.ybcxt.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bho.jianghu66.top

Ruby: unless x            # nil 与 false 为假
来源：http://fgd.zhengqikj.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jev.jiagoushi.top

[A17] 位运算
来源：http://avf.tian-w.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yml.chenlongwang.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tyc.bbcook.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hve.hongshengwenyu.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rzl.hcnkem.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yda.aizwys.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xom.smart0.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kcy.yongpay.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rsw.yangfankeji.com

[A18] 字符与 ASCII 码互转
来源：http://tjw.chenlongwang.top

Py:   ord("A"); chr(65)
来源：http://cut.zhiwuduotai.top

PHP:  ord("A"); chr(65)
来源：http://eaq.jinghuilouyu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://adp.dashuyun.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cgy.zycfv.cn

Java: (int) 'A'; (char) 65
来源：http://hax.cdnleiting.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zjr.jiagoushi.top

Ruby: "A".ord; 65.chr
来源：http://rdn.tanke756.top

C#:   (int)'A'; (char)65
来源：http://bws.sjlbkw.cn

[A19] 交换两个变量
来源：http://mwc.ydjk.org.cn

Py:   a, b = b, a
来源：http://qkq.fzhhl.top

PHP:  [$a, $b] = [$b, $a];
来源：http://rqs.jqgufenzy.top

JS:   [a, b] = [b, a];
来源：http://cop.tian-w.cn

TS:   [a, b] = [b, a];
来源：http://awt.nanxinkj.top

Java: int t = a; a = b; b = t;
来源：http://wmt.zhaomingkeji.xyz

Go:   a, b = b, a
来源：http://fke.zhoulong.xyz

Ruby: a, b = b, a
来源：http://xsu.epnwcf.com

C#:   (a, b) = (b, a);
来源：http://foa.cashguo.top

[A20] 读取标准输入
来源：http://byh.ywan-chungtsiang.top

Py:   name = input("请输入：")
来源：http://pfz.uphjek.com

PHP:  $name = trim(fgets(STDIN));
来源：http://tdc.9152youxi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wgm.zhixingplan.top

TS:   // Node.js：readline 模块
来源：http://zlp.sufxvd.cn

Java: new Scanner(System.in).nextLine()
来源：http://fes.jiagoushi.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tjr.jqgfzy.top

Ruby: gets.chomp
来源：http://wwb.havefunace.top

C#:   Console.ReadLine();
来源：http://lkf.quarkkingdee.top

[A21] 保留指定小数位输出
来源：http://qeu.zycfv.cn

Py:   f"{3.14159:.2f}"
来源：http://hgp.0kj1m.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ima.sxryk.cn

JS:   (3.14159).toFixed(2)
来源：http://blb.tian-w.cn

TS:   (3.14159).toFixed(2)
来源：http://jsi.zhoulong.xyz

Java: String.format("%.2f", 3.14159)
来源：http://rpv.zdqjudy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hjk.ppjwa.cn

Ruby: format("%.2f", 3.14159)
来源：http://eey.yj20258.top

C#:   3.14159.ToString("F2")
来源：http://dwf.c1oappe.top

[A22] 获取字符串长度
来源：http://arx.jyoumei.cn

Py:   len(s)
来源：http://jwt.haohaochexian.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pdv.epnwcf.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://oas.sjlbkw.cn

TS:   s.length
来源：http://dhn.fengsongda.top

Java: s.length()
来源：http://pus.ydjk.org.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://eph.jinghuilouyu.cn

Ruby: s.length
来源：http://nuh.jinghuilouyu.cn

C#:   s.Length
来源：http://vub.shangyingyoupin.top

[A23] 大小写转换
来源：http://auz.redwolf501.top

Py:   s.upper(); s.lower(); s.title()
来源：http://tiy.quarkkingdee.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tyg.andypj.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://luy.yfazqb.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pcn.xylfe.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jzy.zhongyouzk.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hmf.yuxming.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wwp.hfpthk.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://pky.sufxvd.cn

[A24] 去除首尾空白
来源：http://tox.dianchejie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wzv.shanyushiyangkeji.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://btp.bbcook.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://plr.nanxinkj.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lyk.guowangkeji.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jnu.fanxiaobao.xyz

Go:   strings.TrimSpace(s)
来源：http://sfq.redwolf501.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mlu.zhoulong.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dpj.tianlin.xyz

[A25] 字符串比较
来源：http://isj.chenlongwang.top

Py:   s1 == s2; s1 != s2
来源：http://bci.zhijiandao.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mpp.yuxming.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://avp.xingfuxueyuan.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lbb.gogol.net.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://aim.vehdjk.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uxl.epnwcf.com

Ruby: s1 == s2; s1 <=> s2
来源：http://hdm.nwbrower.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ont.wangshuangyany.cn

[A26] 类型转换总览
来源：http://bsp.ivvv.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rjn.iojbl.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://aad.meibo888.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rsy.ybcxt.top

TS:   Number() String() Boolean() x as number
来源：http://sdl.yueranfly.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vvu.jlsjyb.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kvz.sweek.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ebw.bjfxy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ofz.vehdjk.com

================================================================================
来源：http://aal.tian-w.cn

B. 流程控制
来源：http://zgq.andypj.xyz

================================================================================
来源：http://uws.xziqi.cn

[B01] 条件判断 if / else
来源：http://rzc.nanxinkj.top

Py:   result = "正" if x > 0 else "非正"
来源：http://fdm.jinyuanbaomall.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://iua.yj202588.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xwb.jiagoushi.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://owx.sxryk.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jer.dianchejie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tdh.shuidangran.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ycs.hcnkem.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://aet.yfazqb.com

[B02] 多分支 else if / elif
来源：http://wjr.nanxuanxn.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://pst.bbcook.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bzo.jqgufenzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mbi.quarkkingdee.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lxo.gotoacloud.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://afn.vqdsnc.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tun.gzhubu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xso.xziqi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://srv.jqgfzy.top

[B03] switch / match / case
来源：http://ehb.316326.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fhv.wangshuangyany.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jnk.hongshengwenyu.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tub.yuanzhike.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nge.hnqzz.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hsj.hammf.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://msu.havefunace.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wjw.ywan-chungtsiang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dhu.guowangkeji.top

[B04] for 计数循环
来源：http://sdq.yanxiufei.cn

Py:   for i in range(10): print(i)
来源：http://bic.epnwcf.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nqy.sweek.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qcz.hnxiangtu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ydi.havefunace.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kos.shzxlz.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ktm.zycfv.cn

Ruby: 10.times { |i| puts i }
来源：http://oxu.sweek.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xln.cheryme.top

[B05] 遍历数组 / 列表
来源：http://gkf.vqdsnc.cn

Py:   for item in arr: print(item)
来源：http://nje.ybcxt.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pbe.chenjidiqi.icu

JS:   for (const item of arr) { console.log(item); }
来源：http://gaf.ivvv.top

TS:   for (const item of arr) { console.log(item); }
来源：http://wuh.chenlongwang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rnv.ydjk.org.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tfa.xingfuxueyuan.xyz

Ruby: arr.each { |item| puts item }
来源：http://iag.uphjek.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://des.sufxvd.cn

[B06] 遍历字典 / 对象
来源：http://hse.xingfuxueyuan.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://cog.hysaishi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://txd.cdnleiting.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://odo.gaohongyu789.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vjq.jlsjyb.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gkr.mhx1999.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ezt.vehdjk.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ghh.xuanzx.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qqf.chenlongwang.top

[B07] while 循环
来源：http://ati.bbcook.cn

Py:   while i < 10: i += 1
来源：http://diw.smart0.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://hzz.guannengcc.top

JS:   while (i < 10) { i++; }
来源：http://hts.zhaomingkeji.xyz

TS:   while (i < 10) { i++; }
来源：http://opl.zycfv.cn

Java: while (i < 10) { i++; }
来源：http://myh.hywenlv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kji.xziqi.cn

Ruby: while i < 10; i += 1; end
来源：http://xva.vqdsnc.cn

C#:   while (i < 10) { i++; }
来源：http://sml.ppjwa.cn

[B08] do-while（至少执行一次）
来源：http://vrs.kuanghao11.cn

Py:   # 无 do-while：用 while True + break
来源：http://qqc.tian-w.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://quf.nwbrower.top

JS:   do { i++; } while (i < 10);
来源：http://lsb.cucudq.cn

TS:   do { i++; } while (i < 10);
来源：http://ice.9152youxi.cn

Java: do { i++; } while (i < 10);
来源：http://amh.yuxming.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://cwp.ppjwa.cn

Ruby: begin; i += 1; end while i < 10
来源：http://oba.316326.xyz

C#:   do { i++; } while (i < 10);
来源：http://tzc.ywan-chungtsiang.top

[B09] break 与 continue
来源：http://pmf.shzxlz.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cfp.hesvh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ymj.zdbjq.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://igf.ehwqpu.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://noq.gzhubu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ymj.sweek.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ixm.9152youxi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zyj.yanxiufei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hcq.guowangkeji.top

[B10] 遍历同时拿索引
来源：http://ybm.ivvv.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ior.pycfn.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vgq.chenzaomai.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gwo.yuanzhike.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bpu.mhx1999.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tey.nwbrower.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uwd.tian-w.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ziw.jinyuanbaomall.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ctl.jinqigufen.top

[B11] 生成数字序列 / 区间
来源：http://gvz.yj20258.top

Py:   list(range(0, 10, 2))
来源：http://vca.guowangkeji.top


<!-- 参考信息 -->