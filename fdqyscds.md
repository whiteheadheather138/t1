代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://vqu.shanyushiyangkeji.top

Go:   fmt.Println("Hello, World!")
来源：http://ccd.hammf.cn

Ruby: puts "Hello, World!"
来源：http://vwb.hnqzz.top

C#:   Console.WriteLine("Hello, World!");
来源：http://esx.sxryk.cn

[A02] 变量声明与赋值
来源：http://otz.dashuyun.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rpd.ehwqpu.com

PHP:  $name = "Alex"; $age = 20;
来源：http://thd.jinqigufen.top

JS:   let name = "Alex"; const age = 20;
来源：http://qiu.shanyushiyangtech.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bxt.aizwys.cn

Java: String name = "Alex"; int age = 20;
来源：http://lbf.yuxming.cn

Go:   name := "Alex"; age := 20
来源：http://zoa.jiagoushi.top

Ruby: name = "Alex"; age = 20
来源：http://yeo.nwbrower.top

C#:   string name = "Alex"; int age = 20;
来源：http://erj.sweek.top

[A03] 常量定义
来源：http://bxq.fehbvm.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bri.jinghuilouyu.cn

PHP:  const PI = 3.14159;
来源：http://etg.guowangkeji.top

JS:   const PI = 3.14159;
来源：http://oag.ehwqpu.com

TS:   const PI: number = 3.14159;
来源：http://qmx.dianchejie.cn

Java: static final double PI = 3.14159;
来源：http://jel.zhiwuduotai.top

Go:   const PI = 3.14159
来源：http://fgq.yanxiufei.cn

Ruby: PI = 3.14159
来源：http://grz.tianlin.xyz

C#:   const double PI = 3.14159;
来源：http://dqe.cdnleiting.top

[A04] 判断变量类型
来源：http://dll.jinghuilouyu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://cfn.mhx1999.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tcn.zhixingplan.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kye.yanxiufei.cn

TS:   typeof x; x instanceof Date
来源：http://yxz.shanyushiyangkeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bmv.aibaodan.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ops.ydjk.org.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ngt.yj202588.top

C#:   x.GetType().Name; x is int
来源：http://vjy.meibo888.top

[A05] 整数除法与取模
来源：http://rqc.yuxming.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ztj.c1oappe.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://pgw.tian-w.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lta.xinyue.icu

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kii.fengsongda.top

Java: 7 / 2; 7 % 2
来源：http://snt.fktsv.cn

Go:   7 / 2; 7 % 2
来源：http://pfm.havefunace.top

Ruby: 7 / 2; 7 % 2
来源：http://ria.sxryk.cn

C#:   7 / 2; 7 % 2
来源：http://rvu.zhengqikj.top

[A06] 字符串转数字
来源：http://zlc.xuetiantiany.cn

Py:   int("42"); float("3.14")
来源：http://ddu.andypj.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://uzz.gzhubu.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gyg.hammf.cn

TS:   parseInt("42", 10); Number("42")
来源：http://hrr.tianlin.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yfd.zhaomingkeji.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pyx.bjfxy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://lmc.fengsongda.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://lkk.svipenyu.cn

[A07] 数字转字符串
来源：http://rex.hcnkem.com

Py:   str(42)
来源：http://gyh.pycfn.com

PHP:  (string) 42; strval(42)
来源：http://nwg.bjfxy.top

JS:   String(42); (42).toString()
来源：http://tgq.gotoacloud.top

TS:   String(42)
来源：http://vew.zhengqikj.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://gkk.jqgfzy.top

Go:   strconv.Itoa(42)
来源：http://ohr.gaohongyu789.top

Ruby: 42.to_s
来源：http://uxp.shangyingyoupin.top

C#:   42.ToString()
来源：http://wsf.zhiwuduotai.top

[A08] 取整与四舍五入
来源：http://rhg.vqdsnc.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://epj.jiagoushi.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mmv.xylfe.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://sgy.c1oappe.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://emi.bbcook.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://krt.wangdashe.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tsd.yueranfly.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://sgt.xylfe.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wgf.wangdashe.top

[A09] 绝对值与最大最小值
来源：http://srz.shanyushiyangtech.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rlj.aibaodan.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://lgn.cheryme.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ucz.shzxlz.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://org.pycfn.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hlh.pycfn.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://svd.jinqigfzy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://agi.hfpthk.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://nyg.chenjidiqi.icu

[A10] 生成随机数
来源：http://mie.ydjk.org.cn

Py:   import random; random.randint(1, 100)
来源：http://tpw.bbcook.cn

PHP:  random_int(1, 100);
来源：http://rea.shangyingyoupin.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xnr.gzhubu.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fky.fehbvm.com

Java: new Random().nextInt(100) + 1
来源：http://fzu.zhijiandao.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hqc.hfpthk.cn

Ruby: rand(1..100)
来源：http://tco.guowangkeji.top

C#:   new Random().Next(1, 101)
来源：http://nij.guowangkeji.top

[A11] 条件表达式（三元）
来源：http://yma.jiagoushi.top

Py:   "yes" if x > 0 else "no"
来源：http://yjc.yueranfly.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://afx.sxryk.cn

JS:   x > 0 ? "yes" : "no"
来源：http://tzo.xziqi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rzf.dashuyun.cn

Java: x > 0 ? "yes" : "no"
来源：http://fnd.sjlbkw.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hzm.hysaishi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pkq.jinghuilouyu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://qwu.daxiang520.top

[A12] 字符串插值 / 格式化
来源：http://swl.tian-w.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ncj.tianlin.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lfc.jinqigufen.top

JS:   `Hello, ${name}!`
来源：http://wgo.ydjk.org.cn

TS:   `Hello, ${name}!`
来源：http://kkm.pengpengdd.cyou

Java: "Hello, %s!".formatted(name)
来源：http://rif.316326.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xlv.cqqwz.cn

Ruby: "Hello, #{name}!"
来源：http://xcq.pengpengdd.cyou

C#:   $"Hello, {name}!"
来源：http://knn.fktsv.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://qdg.zhongyouzk.top

Py:   "第一行\n第二行"
来源：http://qsm.dashuyun.cn

PHP:  "第一行\n第二行"
来源：http://wlz.sysykeji.top

JS:   "第一行\n第二行"
来源：http://nuo.pycfn.com

TS:   "第一行\n第二行"
来源：http://sqd.dashuyun.cn

Java: "第一行\n第二行"
来源：http://via.vqdsnc.cn

Go:   "第一行\n第二行"
来源：http://mwg.bjfxy.top

Ruby: "第一行\n第二行"
来源：http://xtf.iojbl.cn

C#:   "第一行\n第二行"
来源：http://eej.hywenlv.cn

[A14] 注释写法
来源：http://pil.hfpthk.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://znn.feifeiyinyue.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://wvw.cucudq.cn

JS:   // 单行；/* 多行 */
来源：http://hkc.yuanzhike.top

TS:   // 单行；/* 多行 */
来源：http://xdk.tanke756.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://sdy.ehwqpu.com

Go:   // 单行；/* 多行 */
来源：http://fee.snrcjt.cn

Ruby: # 单行；=begin 多行 =end
来源：http://kwp.316326.xyz

C#:   // 单行；/* 多行 */
来源：http://gef.jianghu66.top

[A15] 空值判断与默认值
来源：http://edn.gzhubu.top

Py:   value = data or "默认值"
来源：http://pgc.zhaomingkeji.xyz

PHP:  $value = $data ?? "默认值";
来源：http://iyh.cqqwz.cn

JS:   const value = data ?? "默认值";
来源：http://uov.gzhubu.top

TS:   const value = data ?? "默认值";
来源：http://gid.havefunace.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jhi.ywan-chungtsiang.top

Go:   if data == "" { data = "默认值" }
来源：http://gda.hysaishi.cn

Ruby: value = data || "默认值"
来源：http://kaz.cdnleiting.top

C#:   var value = data ?? "默认值";
来源：http://epv.xylfe.cn

[A16] 真假值判断规则
来源：http://blc.yj20258.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://iuz.shzxlz.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xop.meibo888.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kly.dashuyun.cn

TS:   if (!x) {}
来源：http://pfj.xinyue.icu

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mjx.quarkkingdee.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gku.zycfv.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hig.shangyingyoupin.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://plw.jqgfzy.top

[A17] 位运算
来源：http://mcj.chenlongwang.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ysw.meibo888.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fev.hesvh.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dre.hcnkem.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rgz.guowangkeji.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iur.fehbvm.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://uxq.yuxming.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nhh.dashuyun.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zzy.andypj.xyz

[A18] 字符与 ASCII 码互转
来源：http://bxb.fanxiaobao.xyz

Py:   ord("A"); chr(65)
来源：http://ntx.daria6918.cn

PHP:  ord("A"); chr(65)
来源：http://goc.yvedp.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xct.shzxlz.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sxv.zhijiandao.cn

Java: (int) 'A'; (char) 65
来源：http://vhx.shanyushiyangkeji.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://utk.guowangkeji.top

Ruby: "A".ord; 65.chr
来源：http://lue.jlsjyb.cn

C#:   (int)'A'; (char)65
来源：http://deo.shangyingyoupin.top

[A19] 交换两个变量
来源：http://zyr.gogol.net.cn

Py:   a, b = b, a
来源：http://ega.zhongyouzk.top

PHP:  [$a, $b] = [$b, $a];
来源：http://tir.hesvh.cn

JS:   [a, b] = [b, a];
来源：http://rxw.cdnleiting.top

TS:   [a, b] = [b, a];
来源：http://zpk.xziqi.cn

Java: int t = a; a = b; b = t;
来源：http://fsw.fktsv.cn

Go:   a, b = b, a
来源：http://tho.xziqi.cn

Ruby: a, b = b, a
来源：http://rvu.tianlin.xyz

C#:   (a, b) = (b, a);
来源：http://jha.shanyushiyangtech.top

[A20] 读取标准输入
来源：http://drp.cheryme.top

Py:   name = input("请输入：")
来源：http://tsq.guannengcc.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ojd.andypj.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gxd.316326.xyz

TS:   // Node.js：readline 模块
来源：http://vsi.ydzc1.top

Java: new Scanner(System.in).nextLine()
来源：http://phv.fehbvm.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rjc.ehwqpu.com

Ruby: gets.chomp
来源：http://fkv.quarkkingdee.top

C#:   Console.ReadLine();
来源：http://yba.aibaodan.cn

[A21] 保留指定小数位输出
来源：http://cgm.gogol.net.cn

Py:   f"{3.14159:.2f}"
来源：http://jja.vqdsnc.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://uuc.jyoumei.cn

JS:   (3.14159).toFixed(2)
来源：http://tjd.xingfuxueyuan.xyz

TS:   (3.14159).toFixed(2)
来源：http://ntr.xuanzx.com

Java: String.format("%.2f", 3.14159)
来源：http://pay.hysaishi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dkv.shanyushiyangtech.top

Ruby: format("%.2f", 3.14159)
来源：http://doq.bbcook.cn

C#:   3.14159.ToString("F2")
来源：http://jqa.iojbl.cn

[A22] 获取字符串长度
来源：http://gbz.zhixingplan.top

Py:   len(s)
来源：http://tcl.yonumen.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://unw.jinqigfzy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://arq.meibo888.top

TS:   s.length
来源：http://cxk.wangdashe.top

Java: s.length()
来源：http://enr.hongshengwenyu.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wmb.chenjidiqi.icu

Ruby: s.length
来源：http://kcu.daxiang520.top

C#:   s.Length
来源：http://ndx.wangdashe.top

[A23] 大小写转换
来源：http://ftz.zdbjq.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ccj.pycfn.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jle.mhx1999.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pmr.zycfv.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dmt.bbcook.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qdo.pengpengdd.cyou

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tdl.nanxuanxn.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pgw.epnwcf.com

C#:   s.ToUpper(); s.ToLower()
来源：http://wsh.jinqigufen.top

[A24] 去除首尾空白
来源：http://zdq.svipenyu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://whn.cheryme.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://inu.xuetiantiany.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jxt.nwbrower.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ppy.mhx1999.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hxy.shangyingyoupin.top

Go:   strings.TrimSpace(s)
来源：http://veb.yj202588.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://luj.yvedp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vcd.tian-w.cn

[A25] 字符串比较
来源：http://hbb.ybcxt.top

Py:   s1 == s2; s1 != s2
来源：http://cdx.yueranfly.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kka.havefunace.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wtn.316326.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cxa.ybcxt.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dfo.xingfuxueyuan.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rak.cucudq.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ebo.shuidangran.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://snp.zdqjudy.top

[A26] 类型转换总览
来源：http://uje.sxryk.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fdg.sjlbkw.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://atk.hysaishi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fxd.gzhubu.top

TS:   Number() String() Boolean() x as number
来源：http://hta.gogol.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vtt.feifeiyinyue.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jup.yangfankeji.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://tat.jqgfzy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pfp.fengsongda.top

================================================================================
来源：http://dfn.ybcxt.top

B. 流程控制
来源：http://phe.kuanghao11.cn

================================================================================
来源：http://amb.cashguo.top

[B01] 条件判断 if / else
来源：http://qzm.yonumen.top

Py:   result = "正" if x > 0 else "非正"
来源：http://yzr.tanke756.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gjr.hammf.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xqr.fanxiaobao.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://els.9152youxi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://gja.shzxlz.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://srd.wangdashe.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lxd.ppjwa.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dci.xuanzx.com

[B02] 多分支 else if / elif
来源：http://byd.jinyuanbaomall.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ylh.zdqjudy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tte.gzhubu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://giv.wangshuangyany.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://isd.yangfankeji.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://flt.tianlin.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qqq.fanxiaobao.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nou.feifeiyinyue.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://csd.ydjk.org.cn

[B03] switch / match / case
来源：http://aqa.hongshengwenyu.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hdf.fengsongda.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iei.fktsv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://btc.9152youxi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gar.tanke756.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kbh.nanxinkj.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nja.hywenlv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rbg.zhaomingkeji.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://umv.bbcook.cn

[B04] for 计数循环
来源：http://joz.ywan-chungtsiang.top

Py:   for i in range(10): print(i)
来源：http://jfr.mhx1999.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rpd.guannengcc.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wpu.aizwys.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vnh.iojbl.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://siv.birdmap.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vqc.zhijiandao.cn

Ruby: 10.times { |i| puts i }
来源：http://wfb.ivvv.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mjg.chenjidiqi.icu

[B05] 遍历数组 / 列表
来源：http://vik.gaohongyu789.top

Py:   for item in arr: print(item)
来源：http://zvl.gzhubu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pcx.zhoulong.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://mer.meibo888.top

TS:   for (const item of arr) { console.log(item); }
来源：http://cwx.aibaodan.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lkh.tianlin.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yan.birdmap.top

Ruby: arr.each { |item| puts item }
来源：http://hpr.fengsongda.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pgi.feifeiyinyue.top

[B06] 遍历字典 / 对象
来源：http://lsz.redwolf501.top

Py:   for k, v in d.items(): print(k, v)
来源：http://zca.52xcode.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qhq.jinghuilouyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eds.kuanghao11.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wti.sxryk.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xoe.shuidangran.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cex.zhengqikj.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yjl.ivvv.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dqr.hysaishi.cn

[B07] while 循环
来源：http://pgn.tian-w.cn

Py:   while i < 10: i += 1
来源：http://anb.zhengqikj.top

PHP:  while ($i < 10) { $i++; }
来源：http://frx.tianlin.xyz

JS:   while (i < 10) { i++; }
来源：http://rfp.cashguo.top

TS:   while (i < 10) { i++; }
来源：http://zrj.xziqi.cn

Java: while (i < 10) { i++; }
来源：http://nmp.sufxvd.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bmb.zhengqikj.top

Ruby: while i < 10; i += 1; end
来源：http://bvs.svipenyu.cn

C#:   while (i < 10) { i++; }
来源：http://mwy.daxiang520.top

[B08] do-while（至少执行一次）
来源：http://lfv.yvedp.cn

Py:   # 无 do-while：用 while True + break
来源：http://qvh.zhoulong.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://auq.epnwcf.com

JS:   do { i++; } while (i < 10);
来源：http://bfo.ehwqpu.com

TS:   do { i++; } while (i < 10);
来源：http://ufc.ydjk.org.cn


<!-- 参考信息 -->