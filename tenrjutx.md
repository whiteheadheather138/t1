代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://smj.zhiwuduotai.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hkc.gzhubu.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qjz.yvedp.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gic.guannengcc.top

================================================================================
来源：http://mhx.wangdashe.top

A. 基础语法与类型
来源：http://nps.fehbvm.com

================================================================================
来源：http://vpo.daria6918.cn

[A01] Hello World
来源：http://jxk.ivvv.top

Py:   print("Hello, World!")
来源：http://nje.gaohongyu789.top

PHP:  echo "Hello, World!";
来源：http://hgi.sysykeji.top

JS:   console.log("Hello, World!");
来源：http://hfd.sjlbkw.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ysz.yonumen.top

Java: System.out.println("Hello, World!");
来源：http://phf.sysykeji.top

Go:   fmt.Println("Hello, World!")
来源：http://vbv.zhongyouzk.top

Ruby: puts "Hello, World!"
来源：http://lee.iojbl.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://snp.bjfxy.top

[A02] 变量声明与赋值
来源：http://uyh.jiagoushi.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zmw.gzhubu.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ips.yueranfly.top

JS:   let name = "Alex"; const age = 20;
来源：http://gfy.chenzaomai.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wsf.gogol.net.cn

Java: String name = "Alex"; int age = 20;
来源：http://xqg.zhongyouzk.top

Go:   name := "Alex"; age := 20
来源：http://ntj.xuetiantiany.cn

Ruby: name = "Alex"; age = 20
来源：http://vhv.fanxiaobao.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://ipz.cqqwz.cn

[A03] 常量定义
来源：http://iqt.jyoumei.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://eig.ctjpmb.com

PHP:  const PI = 3.14159;
来源：http://fxj.bbcook.cn

JS:   const PI = 3.14159;
来源：http://eis.hongshengwenyu.top

TS:   const PI: number = 3.14159;
来源：http://wnt.yuanzhike.top

Java: static final double PI = 3.14159;
来源：http://kot.xinyue.icu

Go:   const PI = 3.14159
来源：http://eia.xingfuxueyuan.xyz

Ruby: PI = 3.14159
来源：http://qnl.nanxuanxn.top

C#:   const double PI = 3.14159;
来源：http://pty.yuanzhike.top

[A04] 判断变量类型
来源：http://rsy.zhongyouzk.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://hfs.xuetiantiany.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bvy.mhx1999.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://uor.ydzc1.top

TS:   typeof x; x instanceof Date
来源：http://nze.epnwcf.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://erp.yangfankeji.com

Go:   reflect.TypeOf(x).Name()
来源：http://tuf.cashguo.top

Ruby: x.class; x.is_a?(Integer)
来源：http://stv.guannengcc.top

C#:   x.GetType().Name; x is int
来源：http://qwq.wangshuangyany.cn

[A05] 整数除法与取模
来源：http://aaq.dianchejie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://eko.hammf.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://tsv.fktsv.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yjq.birdmap.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vnc.c1oappe.top

Java: 7 / 2; 7 % 2
来源：http://zka.jlsjyb.cn

Go:   7 / 2; 7 % 2
来源：http://lgl.xylfe.cn

Ruby: 7 / 2; 7 % 2
来源：http://jca.jinghuilouyu.cn

C#:   7 / 2; 7 % 2
来源：http://upt.jqgufenzy.top

[A06] 字符串转数字
来源：http://sgq.zdbjq.cn

Py:   int("42"); float("3.14")
来源：http://gbw.hfpthk.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jfu.svipenyu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yjy.aizwys.cn

TS:   parseInt("42", 10); Number("42")
来源：http://kkx.vqdsnc.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jyp.yfazqb.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rig.vqdsnc.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://waz.jyoumei.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wny.snrcjt.cn

[A07] 数字转字符串
来源：http://qak.xylfe.cn

Py:   str(42)
来源：http://bsa.yvedp.cn

PHP:  (string) 42; strval(42)
来源：http://wrk.hongshengwenyu.top

JS:   String(42); (42).toString()
来源：http://pnu.feifeiyinyue.top

TS:   String(42)
来源：http://lpo.dianchejie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zuc.xinyue.icu

Go:   strconv.Itoa(42)
来源：http://nas.316326.xyz

Ruby: 42.to_s
来源：http://qud.sjlbkw.cn

C#:   42.ToString()
来源：http://ozr.shzxlz.cn

[A08] 取整与四舍五入
来源：http://rki.dianchejie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://esv.guowangkeji.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://poz.xinyue.icu

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ccr.vqdsnc.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hin.hcnkem.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fhl.ehwqpu.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fuv.cheryme.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://yij.sweek.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://smc.ivvv.top

[A09] 绝对值与最大最小值
来源：http://fck.yuxming.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ntd.wangshuangyany.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rte.jqgfzy.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jpw.xuanzx.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mgl.jinqigufen.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lwa.zhiwuduotai.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cgr.chenlongwang.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://adr.shangyingyoupin.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zju.yfazqb.com

[A10] 生成随机数
来源：http://rqj.aibaodan.cn

Py:   import random; random.randint(1, 100)
来源：http://mpn.haohaochexian.top

PHP:  random_int(1, 100);
来源：http://nkc.haohaochexian.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vgd.meibo888.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nwk.gotoacloud.top

Java: new Random().nextInt(100) + 1
来源：http://ysi.zhaomingkeji.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://emy.jianghu66.top

Ruby: rand(1..100)
来源：http://mqz.yonumen.top

C#:   new Random().Next(1, 101)
来源：http://uiz.jinqigfzy.top

[A11] 条件表达式（三元）
来源：http://cte.yfazqb.com

Py:   "yes" if x > 0 else "no"
来源：http://hmp.ppjwa.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ojm.pengpengdd.cyou

JS:   x > 0 ? "yes" : "no"
来源：http://gvw.hywenlv.cn

TS:   x > 0 ? "yes" : "no"
来源：http://zim.c1oappe.top

Java: x > 0 ? "yes" : "no"
来源：http://uzn.vqdsnc.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://cxw.pengpengdd.cyou

Ruby: x > 0 ? "yes" : "no"
来源：http://waf.yj20258888.top

C#:   x > 0 ? "yes" : "no"
来源：http://tfz.wangshuangyany.cn

[A12] 字符串插值 / 格式化
来源：http://fkv.nwbrower.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ftc.zdbjq.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://qtg.ybcxt.top

JS:   `Hello, ${name}!`
来源：http://ycz.meibo888.top

TS:   `Hello, ${name}!`
来源：http://gay.zhongyouzk.top

Java: "Hello, %s!".formatted(name)
来源：http://kqb.jqgufenzy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://axw.sweek.top

Ruby: "Hello, #{name}!"
来源：http://hqw.gzhubu.top

C#:   $"Hello, {name}!"
来源：http://qqs.mhx1999.top

[A13] 多行字符串（练习 \n 转义）
来源：http://iel.kuanghao11.cn

Py:   "第一行\n第二行"
来源：http://erk.ctjpmb.com

PHP:  "第一行\n第二行"
来源：http://adg.daria6918.cn

JS:   "第一行\n第二行"
来源：http://xig.tanke756.top

TS:   "第一行\n第二行"
来源：http://hdi.jinyuanbaomall.cn

Java: "第一行\n第二行"
来源：http://spf.fengsongda.top

Go:   "第一行\n第二行"
来源：http://nff.shangyingyoupin.top

Ruby: "第一行\n第二行"
来源：http://sdf.yuxming.cn

C#:   "第一行\n第二行"
来源：http://qde.hammf.cn

[A14] 注释写法
来源：http://vsf.shzxlz.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://emv.chenlongwang.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://nhc.bbcook.cn

JS:   // 单行；/* 多行 */
来源：http://bnr.wangshuangyany.cn

TS:   // 单行；/* 多行 */
来源：http://mxz.nwbrower.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qgj.gaohongyu789.top

Go:   // 单行；/* 多行 */
来源：http://ypw.xuanzx.com

Ruby: # 单行；=begin 多行 =end
来源：http://kfc.yvedp.cn

C#:   // 单行；/* 多行 */
来源：http://fjq.zhiwuduotai.top

[A15] 空值判断与默认值
来源：http://ugl.xuanzx.com

Py:   value = data or "默认值"
来源：http://jmy.snrcjt.cn

PHP:  $value = $data ?? "默认值";
来源：http://opk.guannengcc.top

JS:   const value = data ?? "默认值";
来源：http://gbr.mhx1999.top

TS:   const value = data ?? "默认值";
来源：http://pqn.vqdsnc.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://skf.sxryk.cn

Go:   if data == "" { data = "默认值" }
来源：http://ibd.tanke756.top

Ruby: value = data || "默认值"
来源：http://mfp.fktsv.cn

C#:   var value = data ?? "默认值";
来源：http://kje.sjlbkw.cn

[A16] 真假值判断规则
来源：http://obh.cheryme.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ytx.nanxuanxn.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bac.jlsjyb.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tai.yangfankeji.com

TS:   if (!x) {}
来源：http://vuj.52xcode.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bgt.wangdashe.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://aam.hysaishi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://wod.tian-w.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wmu.jqgufenzy.top

[A17] 位运算
来源：http://doa.sweek.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://evt.gzhubu.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gkg.andypj.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dit.quarkkingdee.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://omq.shanyushiyangtech.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hqn.ehwqpu.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vei.jinqigufen.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pjh.shanyushiyangtech.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rbv.tanke756.top

[A18] 字符与 ASCII 码互转
来源：http://mua.zdbjq.cn

Py:   ord("A"); chr(65)
来源：http://fww.jqgfzy.top

PHP:  ord("A"); chr(65)
来源：http://xuh.hywenlv.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://juo.zhijiandao.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uqz.hywenlv.cn

Java: (int) 'A'; (char) 65
来源：http://zls.shangyingyoupin.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lkv.xuetiantiany.cn

Ruby: "A".ord; 65.chr
来源：http://ypa.0kj1m.cn

C#:   (int)'A'; (char)65
来源：http://gsj.shanyushiyangkeji.top

[A19] 交换两个变量
来源：http://yus.shuidangran.top

Py:   a, b = b, a
来源：http://qyt.jinghuilouyu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://isl.sweek.top

JS:   [a, b] = [b, a];
来源：http://xfs.ydzc1.top

TS:   [a, b] = [b, a];
来源：http://eto.zhijiandao.cn

Java: int t = a; a = b; b = t;
来源：http://vbd.chenjidiqi.icu

Go:   a, b = b, a
来源：http://kzi.daxiang520.top

Ruby: a, b = b, a
来源：http://tmz.bjfxy.top

C#:   (a, b) = (b, a);
来源：http://wcx.zycfv.cn

[A20] 读取标准输入
来源：http://nbn.hnxiangtu.top

Py:   name = input("请输入：")
来源：http://xgb.haohaochexian.top

PHP:  $name = trim(fgets(STDIN));
来源：http://bdf.sxryk.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hln.yj20258888.top

TS:   // Node.js：readline 模块
来源：http://sts.ehwqpu.com

Java: new Scanner(System.in).nextLine()
来源：http://xfw.jyoumei.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qvq.dashuyun.cn

Ruby: gets.chomp
来源：http://xri.0kj1m.cn

C#:   Console.ReadLine();
来源：http://klp.gzhubu.top

[A21] 保留指定小数位输出
来源：http://fvm.nwbrower.top

Py:   f"{3.14159:.2f}"
来源：http://mkm.jqgufenzy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://scn.yfazqb.com

JS:   (3.14159).toFixed(2)
来源：http://mzy.feifeiyinyue.top

TS:   (3.14159).toFixed(2)
来源：http://dru.epnwcf.com

Java: String.format("%.2f", 3.14159)
来源：http://yep.tanke756.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ira.ydjk.org.cn

Ruby: format("%.2f", 3.14159)
来源：http://hlz.zhoulong.xyz

C#:   3.14159.ToString("F2")
来源：http://glq.chenjidiqi.icu

[A22] 获取字符串长度
来源：http://rho.9152youxi.cn

Py:   len(s)
来源：http://nhh.316326.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vaf.nanxinkj.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pgp.ctjpmb.com

TS:   s.length
来源：http://knc.chenlongwang.top

Java: s.length()
来源：http://icf.sysykeji.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://asu.jinyuanbaomall.cn

Ruby: s.length
来源：http://jxc.hcnkem.com

C#:   s.Length
来源：http://yvt.xinyue.icu

[A23] 大小写转换
来源：http://spk.jianghu66.top

Py:   s.upper(); s.lower(); s.title()
来源：http://owr.dashuyun.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xsf.hcnkem.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mgx.vehdjk.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lrb.dianchejie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zeu.nanxinkj.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://etj.sxryk.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qvf.tanke756.top

C#:   s.ToUpper(); s.ToLower()
来源：http://vfs.tianlin.xyz

[A24] 去除首尾空白
来源：http://ena.meibo888.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nin.bjfxy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yze.xingfuxueyuan.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bmq.yueranfly.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wqg.yvedp.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tdr.jinqigfzy.top

Go:   strings.TrimSpace(s)
来源：http://xqx.ywan-chungtsiang.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rst.zhixingplan.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ukm.uphjek.com

[A25] 字符串比较
来源：http://yih.9152youxi.cn

Py:   s1 == s2; s1 != s2
来源：http://kuf.yj20258.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qqm.yfazqb.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qxm.chenzaomai.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://oww.snrcjt.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kob.yuanzhike.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fty.kuanghao11.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://und.daxiang520.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jxo.vqdsnc.cn

[A26] 类型转换总览
来源：http://gyg.feifeiyinyue.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cuv.nanxuanxn.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pap.yanxiufei.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nmc.yuanzhike.top

TS:   Number() String() Boolean() x as number
来源：http://lbc.birdmap.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://etg.hywenlv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wpd.cucudq.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ouz.dianchejie.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xis.shuidangran.top

================================================================================
来源：http://ppv.zdbjq.cn

B. 流程控制
来源：http://yft.sxryk.cn

================================================================================
来源：http://vhp.tianlin.xyz

[B01] 条件判断 if / else
来源：http://owv.nanxinkj.top

Py:   result = "正" if x > 0 else "非正"
来源：http://hcs.hnxiangtu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://piw.yanxiufei.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pcy.yj202588.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uig.shuidangran.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://oni.zhoulong.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jvy.yvedp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kcs.redwolf501.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uga.sysykeji.top

[B02] 多分支 else if / elif
来源：http://ufm.meibo888.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wyc.tarul.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pst.dianchejie.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xth.ehwqpu.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ilp.hcnkem.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wug.shuidangran.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zbo.yfazqb.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zwh.zhaomingkeji.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uuj.uphjek.com

[B03] switch / match / case
来源：http://ztu.hesvh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://aoj.gzhubu.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://phn.nanxuanxn.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://szv.zhoulong.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bvp.vqdsnc.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tgk.sysykeji.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kew.dashuyun.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qsq.zhongyouzk.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ufu.ywan-chungtsiang.top

[B04] for 计数循环
来源：http://stn.ydzc1.top

Py:   for i in range(10): print(i)
来源：http://zly.316326.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lrx.zhoulong.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qsl.hnxiangtu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nxc.tianlin.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zaf.hammf.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kpk.jinqigfzy.top

Ruby: 10.times { |i| puts i }
来源：http://lks.bbcook.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nmz.ppjwa.cn

[B05] 遍历数组 / 列表
来源：http://yzu.ydjk.org.cn

Py:   for item in arr: print(item)
来源：http://btv.fktsv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://glt.jinghuilouyu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ztl.zhixingplan.top

TS:   for (const item of arr) { console.log(item); }
来源：http://nnz.xuanzx.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://svk.hammf.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ddh.nanxinkj.top

Ruby: arr.each { |item| puts item }
来源：http://aos.aibaodan.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://euc.cucudq.cn

[B06] 遍历字典 / 对象
来源：http://fxc.zhijiandao.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://thg.fehbvm.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lqj.yj20258.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iyy.zdbjq.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kct.shanyushiyangtech.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dgd.cheryme.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jez.andypj.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ndi.yj202588.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sxb.kuanghao11.cn

[B07] while 循环
来源：http://hdf.xylfe.cn

Py:   while i < 10: i += 1
来源：http://mui.316326.xyz


<!-- 参考信息 -->