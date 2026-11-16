代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lto.chenzaomai.com

Java: String name = "Alex"; int age = 20;
来源：http://sev.chenjidiqi.icu

Go:   name := "Alex"; age := 20
来源：http://zjt.shuidangran.top

Ruby: name = "Alex"; age = 20
来源：http://wvt.andypj.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://cls.birdmap.top

[A03] 常量定义
来源：http://swt.sweek.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dqi.yanxiufei.cn

PHP:  const PI = 3.14159;
来源：http://jbs.sufxvd.cn

JS:   const PI = 3.14159;
来源：http://ykn.pengpengdd.cyou

TS:   const PI: number = 3.14159;
来源：http://zad.nanxinkj.top

Java: static final double PI = 3.14159;
来源：http://wbf.jqgfzy.top

Go:   const PI = 3.14159
来源：http://kdn.zhoulong.xyz

Ruby: PI = 3.14159
来源：http://dyd.ywan-chungtsiang.top

C#:   const double PI = 3.14159;
来源：http://akd.ydjk.org.cn

[A04] 判断变量类型
来源：http://jnz.redwolf501.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://lje.wangdashe.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gly.fktsv.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bnk.yj20258.top

TS:   typeof x; x instanceof Date
来源：http://daw.sweek.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://idc.9152youxi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rbm.nwbrower.top

Ruby: x.class; x.is_a?(Integer)
来源：http://qgg.jqgfzy.top

C#:   x.GetType().Name; x is int
来源：http://xud.fehbvm.com

[A05] 整数除法与取模
来源：http://iqg.hysaishi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://iqg.hcnkem.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://ues.zhengqikj.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rbl.yuanzhike.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hvf.gogol.net.cn

Java: 7 / 2; 7 % 2
来源：http://zte.zdbjq.cn

Go:   7 / 2; 7 % 2
来源：http://woj.jqgfzy.top

Ruby: 7 / 2; 7 % 2
来源：http://fmg.uphjek.com

C#:   7 / 2; 7 % 2
来源：http://wie.gaohongyu789.top

[A06] 字符串转数字
来源：http://gnl.hcnkem.com

Py:   int("42"); float("3.14")
来源：http://yfo.wangdashe.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://unc.nanxinkj.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ubp.chenlongwang.top

TS:   parseInt("42", 10); Number("42")
来源：http://rmf.xuanzx.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qhv.bjfxy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gsu.hnqzz.top

Ruby: "42".to_i; "3.14".to_f
来源：http://nit.ydzc1.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pwa.ehwqpu.com

[A07] 数字转字符串
来源：http://vqx.zdbjq.cn

Py:   str(42)
来源：http://lvt.svipenyu.cn

PHP:  (string) 42; strval(42)
来源：http://vra.yfazqb.com

JS:   String(42); (42).toString()
来源：http://nxg.quarkkingdee.top

TS:   String(42)
来源：http://hby.hammf.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://bii.jiagoushi.top

Go:   strconv.Itoa(42)
来源：http://nmu.iojbl.cn

Ruby: 42.to_s
来源：http://qby.xuetiantiany.cn

C#:   42.ToString()
来源：http://exg.yuanzhike.top

[A08] 取整与四舍五入
来源：http://lam.9152youxi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lnf.hfpthk.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mwh.guowangkeji.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zla.aibaodan.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://eza.gotoacloud.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zei.tian-w.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zzc.hnxiangtu.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://xot.cheryme.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kis.52xcode.cn

[A09] 绝对值与最大最小值
来源：http://raw.zhengqikj.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bep.hammf.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tik.yanxiufei.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pcq.tarul.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tng.wangshuangyany.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ogf.pengpengdd.cyou

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jfr.xingfuxueyuan.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tdl.hammf.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gio.hcnkem.com

[A10] 生成随机数
来源：http://cof.xylfe.cn

Py:   import random; random.randint(1, 100)
来源：http://ytw.uphjek.com

PHP:  random_int(1, 100);
来源：http://rvw.guowangkeji.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://oui.zdqjudy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://csp.shzxlz.cn

Java: new Random().nextInt(100) + 1
来源：http://dgu.jianghu66.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gjf.hammf.cn

Ruby: rand(1..100)
来源：http://prw.shzxlz.cn

C#:   new Random().Next(1, 101)
来源：http://tal.jinqigfzy.top

[A11] 条件表达式（三元）
来源：http://jjf.guannengcc.top

Py:   "yes" if x > 0 else "no"
来源：http://wsy.chenjidiqi.icu

PHP:  $x > 0 ? "yes" : "no"
来源：http://mgp.nanxuanxn.top

JS:   x > 0 ? "yes" : "no"
来源：http://emk.hfpthk.cn

TS:   x > 0 ? "yes" : "no"
来源：http://sch.xinyue.icu

Java: x > 0 ? "yes" : "no"
来源：http://iss.quarkkingdee.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ttn.zhengqikj.top

Ruby: x > 0 ? "yes" : "no"
来源：http://duv.hysaishi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://yis.haohaochexian.top

[A12] 字符串插值 / 格式化
来源：http://wnq.hcnkem.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lsq.zhengqikj.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://dfi.shzxlz.cn

JS:   `Hello, ${name}!`
来源：http://mxe.0kj1m.cn

TS:   `Hello, ${name}!`
来源：http://dax.zhiwuduotai.top

Java: "Hello, %s!".formatted(name)
来源：http://kwu.chenlongwang.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qiv.cqqwz.cn

Ruby: "Hello, #{name}!"
来源：http://ygc.hesvh.cn

C#:   $"Hello, {name}!"
来源：http://zhy.vehdjk.com

[A13] 多行字符串（练习 \n 转义）
来源：http://fip.ctjpmb.com

Py:   "第一行\n第二行"
来源：http://qvj.c1oappe.top

PHP:  "第一行\n第二行"
来源：http://jsp.gotoacloud.top

JS:   "第一行\n第二行"
来源：http://xyn.ydzc1.top

TS:   "第一行\n第二行"
来源：http://wxd.hesvh.cn

Java: "第一行\n第二行"
来源：http://syw.bbcook.cn

Go:   "第一行\n第二行"
来源：http://ndf.52xcode.cn

Ruby: "第一行\n第二行"
来源：http://yfk.sxryk.cn

C#:   "第一行\n第二行"
来源：http://npt.haohaochexian.top

[A14] 注释写法
来源：http://ewp.hcnkem.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://wzh.jqgfzy.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://dhm.ehwqpu.com

JS:   // 单行；/* 多行 */
来源：http://mio.nanxinkj.top

TS:   // 单行；/* 多行 */
来源：http://tnv.mhx1999.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wjo.jqgufenzy.top

Go:   // 单行；/* 多行 */
来源：http://myh.fktsv.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ubb.ybcxt.top

C#:   // 单行；/* 多行 */
来源：http://odx.sysykeji.top

[A15] 空值判断与默认值
来源：http://ycg.hongshengwenyu.top

Py:   value = data or "默认值"
来源：http://bpi.cashguo.top

PHP:  $value = $data ?? "默认值";
来源：http://pyf.sweek.top

JS:   const value = data ?? "默认值";
来源：http://vgm.hnqzz.top

TS:   const value = data ?? "默认值";
来源：http://qrd.hammf.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://drz.zhengqikj.top

Go:   if data == "" { data = "默认值" }
来源：http://srp.316326.xyz

Ruby: value = data || "默认值"
来源：http://mch.cashguo.top

C#:   var value = data ?? "默认值";
来源：http://kok.yvedp.cn

[A16] 真假值判断规则
来源：http://ebo.jlsjyb.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://oeh.ydjk.org.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://owu.xuetiantiany.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ujp.ctjpmb.com

TS:   if (!x) {}
来源：http://vng.ctjpmb.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mmv.jlsjyb.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ppy.guannengcc.top

Ruby: unless x            # nil 与 false 为假
来源：http://mbi.shanyushiyangkeji.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ckp.yuanzhike.top

[A17] 位运算
来源：http://emq.cqqwz.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://whr.zhongyouzk.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://agt.yueranfly.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bnj.mhx1999.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ccf.shanyushiyangtech.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://adh.mhx1999.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://uil.iojbl.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ioq.yanxiufei.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://net.jqgfzy.top

[A18] 字符与 ASCII 码互转
来源：http://waw.ehwqpu.com

Py:   ord("A"); chr(65)
来源：http://shm.meibo888.top

PHP:  ord("A"); chr(65)
来源：http://lgg.guannengcc.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bqz.xingfuxueyuan.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kxu.dianchejie.cn

Java: (int) 'A'; (char) 65
来源：http://sze.shanyushiyangkeji.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mfb.zhongyouzk.top

Ruby: "A".ord; 65.chr
来源：http://kvw.ywan-chungtsiang.top

C#:   (int)'A'; (char)65
来源：http://iiq.ppjwa.cn

[A19] 交换两个变量
来源：http://fxi.zhoulong.xyz

Py:   a, b = b, a
来源：http://lou.hnxiangtu.top

PHP:  [$a, $b] = [$b, $a];
来源：http://qup.ivvv.top

JS:   [a, b] = [b, a];
来源：http://ryo.hesvh.cn

TS:   [a, b] = [b, a];
来源：http://rea.tianlin.xyz

Java: int t = a; a = b; b = t;
来源：http://tvj.cashguo.top

Go:   a, b = b, a
来源：http://kgv.yonumen.top

Ruby: a, b = b, a
来源：http://owx.svipenyu.cn

C#:   (a, b) = (b, a);
来源：http://oxi.tian-w.cn

[A20] 读取标准输入
来源：http://zux.jinghuilouyu.cn

Py:   name = input("请输入：")
来源：http://fcy.yj202588.top

PHP:  $name = trim(fgets(STDIN));
来源：http://tmz.dianchejie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://abb.zdbjq.cn

TS:   // Node.js：readline 模块
来源：http://rgr.tarul.cn

Java: new Scanner(System.in).nextLine()
来源：http://lzy.ydzc1.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://oyv.shanyushiyangtech.top

Ruby: gets.chomp
来源：http://dou.fehbvm.com

C#:   Console.ReadLine();
来源：http://wsf.dashuyun.cn

[A21] 保留指定小数位输出
来源：http://pwo.nanxuanxn.top

Py:   f"{3.14159:.2f}"
来源：http://bpu.jlsjyb.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vpn.dashuyun.cn

JS:   (3.14159).toFixed(2)
来源：http://bax.epnwcf.com

TS:   (3.14159).toFixed(2)
来源：http://gqh.cdnleiting.top

Java: String.format("%.2f", 3.14159)
来源：http://grh.mhx1999.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://icw.fehbvm.com

Ruby: format("%.2f", 3.14159)
来源：http://ytn.xylfe.cn

C#:   3.14159.ToString("F2")
来源：http://ihh.vqdsnc.cn

[A22] 获取字符串长度
来源：http://frq.xziqi.cn

Py:   len(s)
来源：http://noz.yj20258.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sdi.zhixingplan.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://slv.zycfv.cn

TS:   s.length
来源：http://wfx.xuetiantiany.cn

Java: s.length()
来源：http://vwk.tian-w.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://oam.epnwcf.com

Ruby: s.length
来源：http://ouv.guowangkeji.top

C#:   s.Length
来源：http://tzw.zycfv.cn

[A23] 大小写转换
来源：http://rlh.ydzc1.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ogd.iojbl.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pam.smart0.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wyu.jlsjyb.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ias.hcnkem.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://djx.zhoulong.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cob.zycfv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bsq.yj20258888.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ewu.jyoumei.cn

[A24] 去除首尾空白
来源：http://bki.jinqigufen.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sdf.pycfn.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://adx.gotoacloud.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://poh.daxiang520.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://boq.wangdashe.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kjl.ehwqpu.com

Go:   strings.TrimSpace(s)
来源：http://zbr.havefunace.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rco.ydzc1.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ibm.vehdjk.com

[A25] 字符串比较
来源：http://mbr.hysaishi.cn

Py:   s1 == s2; s1 != s2
来源：http://eko.hnqzz.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dna.fzhhl.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kpm.shzxlz.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mww.dashuyun.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://aju.birdmap.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tzk.vehdjk.com

Ruby: s1 == s2; s1 <=> s2
来源：http://vps.kuanghao11.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://quc.jinghuilouyu.cn

[A26] 类型转换总览
来源：http://yqy.fengsongda.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://obc.jinghuilouyu.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jyd.wangshuangyany.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mfg.xinyue.icu

TS:   Number() String() Boolean() x as number
来源：http://yaq.andypj.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hfh.bbcook.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ikj.316326.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://dla.hongshengwenyu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ugr.sweek.top

================================================================================
来源：http://inj.sufxvd.cn

B. 流程控制
来源：http://vgy.svipenyu.cn

================================================================================
来源：http://wbg.yonumen.top

[B01] 条件判断 if / else
来源：http://fxg.shzxlz.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://emv.yueranfly.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dch.yuxming.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mja.sxryk.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://syf.cdnleiting.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ruh.feifeiyinyue.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rif.gotoacloud.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ght.zhijiandao.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://iar.jinyuanbaomall.cn

[B02] 多分支 else if / elif
来源：http://waj.9152youxi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bes.shanyushiyangtech.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ygq.hongshengwenyu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dgn.meibo888.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ksu.fktsv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lft.feifeiyinyue.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wai.xingfuxueyuan.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://spr.chenlongwang.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rsz.yj20258.top

[B03] switch / match / case
来源：http://llq.fengsongda.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pjl.ppjwa.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hwu.yfazqb.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ukb.ppjwa.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pka.ppjwa.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rmj.jqgufenzy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mlz.cqqwz.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hlw.quarkkingdee.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fkk.chenjidiqi.icu

[B04] for 计数循环
来源：http://uap.bjfxy.top

Py:   for i in range(10): print(i)
来源：http://zzq.shangyingyoupin.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yir.sweek.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mle.andypj.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://irj.cashguo.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://atb.quarkkingdee.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ono.andypj.xyz

Ruby: 10.times { |i| puts i }
来源：http://fmb.zhixingplan.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sax.hesvh.cn

[B05] 遍历数组 / 列表
来源：http://gkz.havefunace.top

Py:   for item in arr: print(item)
来源：http://zat.quarkkingdee.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rec.jinqigufen.top

JS:   for (const item of arr) { console.log(item); }
来源：http://zjw.hfpthk.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qjp.ctjpmb.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://qzg.aizwys.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jkb.tarul.cn

Ruby: arr.each { |item| puts item }
来源：http://jps.jianghu66.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://imr.bbcook.cn

[B06] 遍历字典 / 对象
来源：http://loa.jlsjyb.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://iho.chenzaomai.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fyx.hnxiangtu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qyh.ppjwa.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jdk.hnqzz.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://aoc.snrcjt.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nmj.hongshengwenyu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ojc.shuidangran.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ulu.wangshuangyany.cn

[B07] while 循环
来源：http://zqc.tarul.cn

Py:   while i < 10: i += 1
来源：http://vym.zdqjudy.top

PHP:  while ($i < 10) { $i++; }
来源：http://dfi.aizwys.cn

JS:   while (i < 10) { i++; }
来源：http://cbv.zhengqikj.top

TS:   while (i < 10) { i++; }
来源：http://ewb.aibaodan.cn

Java: while (i < 10) { i++; }
来源：http://sss.yj202588.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://clp.ywan-chungtsiang.top

Ruby: while i < 10; i += 1; end
来源：http://nmd.shangyingyoupin.top

C#:   while (i < 10) { i++; }
来源：http://iqc.yfazqb.com

[B08] do-while（至少执行一次）
来源：http://zmo.jianghu66.top

Py:   # 无 do-while：用 while True + break
来源：http://bsf.nanxinkj.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vav.tian-w.cn

JS:   do { i++; } while (i < 10);
来源：http://gdw.svipenyu.cn

TS:   do { i++; } while (i < 10);
来源：http://dlv.xuanzx.com

Java: do { i++; } while (i < 10);
来源：http://syp.cheryme.top

Go:   for { i++; if i >= 10 { break } }
来源：http://yos.sufxvd.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xjx.redwolf501.top

C#:   do { i++; } while (i < 10);
来源：http://rta.redwolf501.top

[B09] break 与 continue
来源：http://ydi.jianghu66.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bmh.zdbjq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dqq.ppjwa.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rcq.xinyue.icu


<!-- 参考信息 -->