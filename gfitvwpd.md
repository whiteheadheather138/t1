代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://lip.aibaodan.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zkm.ybcxt.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wzc.zhongyouzk.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mhj.yvedp.cn

================================================================================
来源：http://hzd.guannengcc.top

A. 基础语法与类型
来源：http://pis.fanxiaobao.xyz

================================================================================
来源：http://xfn.yvedp.cn

[A01] Hello World
来源：http://mhv.sxryk.cn

Py:   print("Hello, World!")
来源：http://qzi.daria6918.cn

PHP:  echo "Hello, World!";
来源：http://hpu.redwolf501.top

JS:   console.log("Hello, World!");
来源：http://fwu.52xcode.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vek.hesvh.cn

Java: System.out.println("Hello, World!");
来源：http://mqc.jianghu66.top

Go:   fmt.Println("Hello, World!")
来源：http://xtr.nwbrower.top

Ruby: puts "Hello, World!"
来源：http://jlx.fzhhl.top

C#:   Console.WriteLine("Hello, World!");
来源：http://nmq.zhiwuduotai.top

[A02] 变量声明与赋值
来源：http://sms.xylfe.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://byg.fktsv.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://idd.jiagoushi.top

JS:   let name = "Alex"; const age = 20;
来源：http://bhw.hnqzz.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zqu.pycfn.com

Java: String name = "Alex"; int age = 20;
来源：http://wtk.jianghu66.top

Go:   name := "Alex"; age := 20
来源：http://xct.yj202588.top

Ruby: name = "Alex"; age = 20
来源：http://pym.haohaochexian.top

C#:   string name = "Alex"; int age = 20;
来源：http://zpb.wangshuangyany.cn

[A03] 常量定义
来源：http://vac.chenlongwang.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vou.hesvh.cn

PHP:  const PI = 3.14159;
来源：http://kug.52xcode.cn

JS:   const PI = 3.14159;
来源：http://oqz.hysaishi.cn

TS:   const PI: number = 3.14159;
来源：http://yov.pengpengdd.cyou

Java: static final double PI = 3.14159;
来源：http://sdg.wangdashe.top

Go:   const PI = 3.14159
来源：http://hjo.c1oappe.top

Ruby: PI = 3.14159
来源：http://cyz.chenjidiqi.icu

C#:   const double PI = 3.14159;
来源：http://qyd.zhiwuduotai.top

[A04] 判断变量类型
来源：http://xny.yanxiufei.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://rml.cashguo.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rgv.yj20258888.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://esx.bjfxy.top

TS:   typeof x; x instanceof Date
来源：http://ovj.jlsjyb.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://prb.ppjwa.cn

Go:   reflect.TypeOf(x).Name()
来源：http://oky.daxiang520.top

Ruby: x.class; x.is_a?(Integer)
来源：http://ggz.hnqzz.top

C#:   x.GetType().Name; x is int
来源：http://rno.chenlongwang.top

[A05] 整数除法与取模
来源：http://ohm.uphjek.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dha.yuanzhike.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://idq.cashguo.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ikb.wangdashe.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xxr.chenlongwang.top

Java: 7 / 2; 7 % 2
来源：http://cgw.aizwys.cn

Go:   7 / 2; 7 % 2
来源：http://yvz.cheryme.top

Ruby: 7 / 2; 7 % 2
来源：http://hnk.xuanzx.com

C#:   7 / 2; 7 % 2
来源：http://ozr.aibaodan.cn

[A06] 字符串转数字
来源：http://mgr.zycfv.cn

Py:   int("42"); float("3.14")
来源：http://zhl.xingfuxueyuan.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lfd.xuetiantiany.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ysd.shuidangran.top

TS:   parseInt("42", 10); Number("42")
来源：http://tsx.nanxuanxn.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dvq.nanxinkj.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jhy.sjlbkw.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://qij.yj20258.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://owt.zdbjq.cn

[A07] 数字转字符串
来源：http://mif.jqgfzy.top

Py:   str(42)
来源：http://vof.zhengqikj.top

PHP:  (string) 42; strval(42)
来源：http://vqo.jqgfzy.top

JS:   String(42); (42).toString()
来源：http://thk.uphjek.com

TS:   String(42)
来源：http://eep.shangyingyoupin.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://jrf.yangfankeji.com

Go:   strconv.Itoa(42)
来源：http://gco.daria6918.cn

Ruby: 42.to_s
来源：http://zyf.zdbjq.cn

C#:   42.ToString()
来源：http://iyb.yanxiufei.cn

[A08] 取整与四舍五入
来源：http://gxb.yuanzhike.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jcn.hfpthk.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lin.9152youxi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://cxx.birdmap.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vay.shangyingyoupin.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://msa.jqgfzy.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wvc.yuanzhike.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://bek.jqgufenzy.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kdi.chenzaomai.com

[A09] 绝对值与最大最小值
来源：http://pce.zhongyouzk.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gcy.jyoumei.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pqd.epnwcf.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://bee.redwolf501.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://str.ybcxt.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pvw.zhixingplan.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ifl.jinqigufen.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://uur.zhiwuduotai.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://sdw.tian-w.cn

[A10] 生成随机数
来源：http://hle.aizwys.cn

Py:   import random; random.randint(1, 100)
来源：http://cit.gotoacloud.top

PHP:  random_int(1, 100);
来源：http://thd.dianchejie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zbf.shanyushiyangtech.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bxb.pycfn.com

Java: new Random().nextInt(100) + 1
来源：http://znk.zdqjudy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wvv.fktsv.cn

Ruby: rand(1..100)
来源：http://xlt.daxiang520.top

C#:   new Random().Next(1, 101)
来源：http://qig.zhongyouzk.top

[A11] 条件表达式（三元）
来源：http://qvr.aizwys.cn

Py:   "yes" if x > 0 else "no"
来源：http://nwf.vqdsnc.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rkl.sweek.top

JS:   x > 0 ? "yes" : "no"
来源：http://prl.yangfankeji.com

TS:   x > 0 ? "yes" : "no"
来源：http://jts.xuanzx.com

Java: x > 0 ? "yes" : "no"
来源：http://wrt.cdnleiting.top

Go:   // 无三元运算符，需用 if 语句
来源：http://rgu.fehbvm.com

Ruby: x > 0 ? "yes" : "no"
来源：http://frd.nwbrower.top

C#:   x > 0 ? "yes" : "no"
来源：http://aiz.wangshuangyany.cn

[A12] 字符串插值 / 格式化
来源：http://ggd.yuanzhike.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ojh.zdqjudy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bnc.hysaishi.cn

JS:   `Hello, ${name}!`
来源：http://vnq.9152youxi.cn

TS:   `Hello, ${name}!`
来源：http://jyi.xingfuxueyuan.xyz

Java: "Hello, %s!".formatted(name)
来源：http://wfv.wangshuangyany.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tty.xingfuxueyuan.xyz

Ruby: "Hello, #{name}!"
来源：http://cku.52xcode.cn

C#:   $"Hello, {name}!"
来源：http://bws.cqqwz.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://djz.c1oappe.top

Py:   "第一行\n第二行"
来源：http://elw.jinyuanbaomall.cn

PHP:  "第一行\n第二行"
来源：http://its.hcnkem.com

JS:   "第一行\n第二行"
来源：http://wsw.cheryme.top

TS:   "第一行\n第二行"
来源：http://zns.xingfuxueyuan.xyz

Java: "第一行\n第二行"
来源：http://rhk.hnxiangtu.top

Go:   "第一行\n第二行"
来源：http://qqy.ppjwa.cn

Ruby: "第一行\n第二行"
来源：http://saz.yangfankeji.com

C#:   "第一行\n第二行"
来源：http://jpx.chenlongwang.top

[A14] 注释写法
来源：http://hun.zhiwuduotai.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://aao.gogol.net.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ivc.daria6918.cn

JS:   // 单行；/* 多行 */
来源：http://lkf.zhixingplan.top

TS:   // 单行；/* 多行 */
来源：http://olm.chenzaomai.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zsn.sufxvd.cn

Go:   // 单行；/* 多行 */
来源：http://tfp.zhongyouzk.top

Ruby: # 单行；=begin 多行 =end
来源：http://daz.daria6918.cn

C#:   // 单行；/* 多行 */
来源：http://qlu.jqgfzy.top

[A15] 空值判断与默认值
来源：http://lng.hammf.cn

Py:   value = data or "默认值"
来源：http://vbj.mhx1999.top

PHP:  $value = $data ?? "默认值";
来源：http://omk.kuanghao11.cn

JS:   const value = data ?? "默认值";
来源：http://bqv.ybcxt.top

TS:   const value = data ?? "默认值";
来源：http://ztt.tarul.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zrv.fanxiaobao.xyz

Go:   if data == "" { data = "默认值" }
来源：http://hsp.jiagoushi.top

Ruby: value = data || "默认值"
来源：http://jjr.316326.xyz

C#:   var value = data ?? "默认值";
来源：http://gah.aizwys.cn

[A16] 真假值判断规则
来源：http://yxk.ehwqpu.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ytb.redwolf501.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nus.haohaochexian.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tqt.jqgufenzy.top

TS:   if (!x) {}
来源：http://wta.yfazqb.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ila.yuanzhike.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nkd.aizwys.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xkf.dashuyun.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hdh.vqdsnc.cn

[A17] 位运算
来源：http://akj.jinghuilouyu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cdu.xylfe.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ykd.tarul.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iky.jinghuilouyu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://oew.sxryk.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sod.fanxiaobao.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nqg.zhengqikj.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lfi.yj202588.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://slx.xingfuxueyuan.xyz

[A18] 字符与 ASCII 码互转
来源：http://mnu.yueranfly.top

Py:   ord("A"); chr(65)
来源：http://pcz.nanxuanxn.top

PHP:  ord("A"); chr(65)
来源：http://eis.wangshuangyany.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nly.yonumen.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tex.zhaomingkeji.xyz

Java: (int) 'A'; (char) 65
来源：http://txb.ehwqpu.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://iep.jlsjyb.cn

Ruby: "A".ord; 65.chr
来源：http://siw.yj202588.top

C#:   (int)'A'; (char)65
来源：http://kya.sufxvd.cn

[A19] 交换两个变量
来源：http://dad.ydzc1.top

Py:   a, b = b, a
来源：http://ard.zhaomingkeji.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://zmi.andypj.xyz

JS:   [a, b] = [b, a];
来源：http://ckz.bjfxy.top

TS:   [a, b] = [b, a];
来源：http://mga.ybcxt.top

Java: int t = a; a = b; b = t;
来源：http://umb.jyoumei.cn

Go:   a, b = b, a
来源：http://esx.sysykeji.top

Ruby: a, b = b, a
来源：http://qqf.fzhhl.top

C#:   (a, b) = (b, a);
来源：http://idy.bbcook.cn

[A20] 读取标准输入
来源：http://nov.zhaomingkeji.xyz

Py:   name = input("请输入：")
来源：http://fnn.havefunace.top

PHP:  $name = trim(fgets(STDIN));
来源：http://svs.shanyushiyangkeji.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bvx.andypj.xyz

TS:   // Node.js：readline 模块
来源：http://oly.316326.xyz

Java: new Scanner(System.in).nextLine()
来源：http://zbz.bbcook.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://umn.aizwys.cn

Ruby: gets.chomp
来源：http://jyw.yfazqb.com

C#:   Console.ReadLine();
来源：http://mfb.yj202588.top

[A21] 保留指定小数位输出
来源：http://gpl.cashguo.top

Py:   f"{3.14159:.2f}"
来源：http://bgx.tianlin.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wgm.hnqzz.top

JS:   (3.14159).toFixed(2)
来源：http://lje.chenjidiqi.icu

TS:   (3.14159).toFixed(2)
来源：http://uxi.jianghu66.top

Java: String.format("%.2f", 3.14159)
来源：http://twv.ctjpmb.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rwh.c1oappe.top

Ruby: format("%.2f", 3.14159)
来源：http://mot.sxryk.cn

C#:   3.14159.ToString("F2")
来源：http://tqk.yj20258888.top

[A22] 获取字符串长度
来源：http://awe.ydzc1.top

Py:   len(s)
来源：http://rxu.cucudq.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wfm.yangfankeji.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mrf.ehwqpu.com

TS:   s.length
来源：http://fya.bjfxy.top

Java: s.length()
来源：http://zcq.xuetiantiany.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mjd.uphjek.com

Ruby: s.length
来源：http://anw.wangshuangyany.cn

C#:   s.Length
来源：http://zge.dianchejie.cn

[A23] 大小写转换
来源：http://uqn.jinyuanbaomall.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://gxs.tanke756.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ydr.zhengqikj.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ojk.sxryk.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pbu.aibaodan.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dpp.vehdjk.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://akr.zhixingplan.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://acu.cheryme.top

C#:   s.ToUpper(); s.ToLower()
来源：http://dwv.c1oappe.top

[A24] 去除首尾空白
来源：http://wzu.cdnleiting.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bje.chenzaomai.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://klo.shuidangran.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sdj.52xcode.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hyx.tarul.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nay.gotoacloud.top

Go:   strings.TrimSpace(s)
来源：http://lue.pycfn.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qib.xuetiantiany.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://epn.tarul.cn

[A25] 字符串比较
来源：http://mha.cqqwz.cn

Py:   s1 == s2; s1 != s2
来源：http://dkf.shanyushiyangkeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://umw.yj202588.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fgs.dashuyun.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vth.ehwqpu.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nvk.zhijiandao.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://epg.ppjwa.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nbm.sxryk.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kgz.dianchejie.cn

[A26] 类型转换总览
来源：http://dkl.chenjidiqi.icu

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tfd.bjfxy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://psi.birdmap.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pef.kuanghao11.cn

TS:   Number() String() Boolean() x as number
来源：http://azu.tianlin.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uav.ppjwa.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kuw.jinghuilouyu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fkq.hongshengwenyu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://njd.fehbvm.com

================================================================================
来源：http://fru.feifeiyinyue.top

B. 流程控制
来源：http://eil.nwbrower.top

================================================================================
来源：http://vud.zhijiandao.cn

[B01] 条件判断 if / else
来源：http://ibc.ppjwa.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://eov.yfazqb.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ixx.yonumen.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pek.gaohongyu789.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://von.pengpengdd.cyou

Java: String r = x > 0 ? "正" : "非正";
来源：http://xkw.zhixingplan.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xsk.nwbrower.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mvi.andypj.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qst.vqdsnc.cn

[B02] 多分支 else if / elif
来源：http://api.zhiwuduotai.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jns.cqqwz.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pzg.nanxinkj.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vxs.guowangkeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://syp.guowangkeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dcq.quarkkingdee.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nco.zdqjudy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://srd.guowangkeji.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ehl.vehdjk.com

[B03] switch / match / case
来源：http://wbk.chenjidiqi.icu

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nvv.gogol.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xom.fengsongda.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cqj.sweek.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zyd.fzhhl.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://eli.gaohongyu789.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://emu.zhijiandao.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hjl.guannengcc.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hor.fehbvm.com

[B04] for 计数循环
来源：http://tuv.fanxiaobao.xyz

Py:   for i in range(10): print(i)
来源：http://wir.ywan-chungtsiang.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tfl.epnwcf.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ipg.cucudq.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mup.yangfankeji.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://faf.zhoulong.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wnp.epnwcf.com

Ruby: 10.times { |i| puts i }
来源：http://usx.9152youxi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yoy.snrcjt.cn

[B05] 遍历数组 / 列表
来源：http://vmg.yj202588.top

Py:   for item in arr: print(item)
来源：http://qdn.nanxuanxn.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qqa.0kj1m.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mhs.52xcode.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ymb.c1oappe.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://pua.jinqigufen.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vuh.bjfxy.top

Ruby: arr.each { |item| puts item }
来源：http://ita.ehwqpu.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://asl.gzhubu.top

[B06] 遍历字典 / 对象
来源：http://hng.shuidangran.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ufl.hongshengwenyu.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yjf.snrcjt.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gfb.vehdjk.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://orc.ivvv.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bev.tian-w.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://soo.xylfe.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rmd.gotoacloud.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tdn.ppjwa.cn

[B07] while 循环
来源：http://ifq.wangshuangyany.cn

Py:   while i < 10: i += 1
来源：http://ltu.aizwys.cn


<!-- 参考信息 -->