代发 wailian999

Py:   print("Hello, World!")
来源：http://grq.ehwqpu.com

PHP:  echo "Hello, World!";
来源：http://dyj.vehdjk.com

JS:   console.log("Hello, World!");
来源：http://xzv.cdnleiting.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fqp.snrcjt.cn

Java: System.out.println("Hello, World!");
来源：http://uzj.pengpengdd.cyou

Go:   fmt.Println("Hello, World!")
来源：http://rys.hysaishi.cn

Ruby: puts "Hello, World!"
来源：http://zbv.zdbjq.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zke.gzhubu.top

[A02] 变量声明与赋值
来源：http://bos.svipenyu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ycj.yueranfly.top

PHP:  $name = "Alex"; $age = 20;
来源：http://lfx.shanyushiyangtech.top

JS:   let name = "Alex"; const age = 20;
来源：http://oto.smart0.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://eqm.daria6918.cn

Java: String name = "Alex"; int age = 20;
来源：http://frs.svipenyu.cn

Go:   name := "Alex"; age := 20
来源：http://kjv.feifeiyinyue.top

Ruby: name = "Alex"; age = 20
来源：http://yps.gzhubu.top

C#:   string name = "Alex"; int age = 20;
来源：http://tma.shanyushiyangkeji.top

[A03] 常量定义
来源：http://uxc.svipenyu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pvo.xziqi.cn

PHP:  const PI = 3.14159;
来源：http://yif.sweek.top

JS:   const PI = 3.14159;
来源：http://jgv.pycfn.com

TS:   const PI: number = 3.14159;
来源：http://odn.zdqjudy.top

Java: static final double PI = 3.14159;
来源：http://sva.tian-w.cn

Go:   const PI = 3.14159
来源：http://cec.yonumen.top

Ruby: PI = 3.14159
来源：http://uyx.hcnkem.com

C#:   const double PI = 3.14159;
来源：http://see.haohaochexian.top

[A04] 判断变量类型
来源：http://jkl.nanxinkj.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://uxi.yuanzhike.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fto.cqqwz.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gzd.haohaochexian.top

TS:   typeof x; x instanceof Date
来源：http://dng.zdqjudy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jnr.zhongyouzk.top

Go:   reflect.TypeOf(x).Name()
来源：http://vle.yuanzhike.top

Ruby: x.class; x.is_a?(Integer)
来源：http://kef.tarul.cn

C#:   x.GetType().Name; x is int
来源：http://rgx.guowangkeji.top

[A05] 整数除法与取模
来源：http://rle.sysykeji.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://nzn.nwbrower.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://mnm.ppjwa.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://prb.jinqigufen.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rdq.fengsongda.top

Java: 7 / 2; 7 % 2
来源：http://exl.shuidangran.top

Go:   7 / 2; 7 % 2
来源：http://tob.yj20258888.top

Ruby: 7 / 2; 7 % 2
来源：http://enc.cqqwz.cn

C#:   7 / 2; 7 % 2
来源：http://nbq.sxryk.cn

[A06] 字符串转数字
来源：http://nrm.yj202588.top

Py:   int("42"); float("3.14")
来源：http://haf.yanxiufei.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yjx.zhengqikj.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kva.pycfn.com

TS:   parseInt("42", 10); Number("42")
来源：http://lbw.jinqigufen.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qlc.svipenyu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ype.uphjek.com

Ruby: "42".to_i; "3.14".to_f
来源：http://fvf.yanxiufei.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://sep.yj20258888.top

[A07] 数字转字符串
来源：http://ykc.yonumen.top

Py:   str(42)
来源：http://aon.pycfn.com

PHP:  (string) 42; strval(42)
来源：http://jkm.zdqjudy.top

JS:   String(42); (42).toString()
来源：http://wli.havefunace.top

TS:   String(42)
来源：http://jag.yuanzhike.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://yqg.bjfxy.top

Go:   strconv.Itoa(42)
来源：http://wzq.xingfuxueyuan.xyz

Ruby: 42.to_s
来源：http://dnx.xuetiantiany.cn

C#:   42.ToString()
来源：http://qhr.cdnleiting.top

[A08] 取整与四舍五入
来源：http://skc.ehwqpu.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xqe.52xcode.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://lwa.feifeiyinyue.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lmf.0kj1m.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dev.hammf.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ntv.vqdsnc.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fky.snrcjt.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://kvt.gzhubu.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xio.zhengqikj.top

[A09] 绝对值与最大最小值
来源：http://fhp.bjfxy.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ybw.jinqigfzy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ykz.yuxming.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hka.hfpthk.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xtc.wangshuangyany.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bme.andypj.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jqv.nanxuanxn.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ndd.yj20258.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tbo.iojbl.cn

[A10] 生成随机数
来源：http://gax.daxiang520.top

Py:   import random; random.randint(1, 100)
来源：http://tby.bjfxy.top

PHP:  random_int(1, 100);
来源：http://ewh.hfpthk.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://flx.quarkkingdee.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tfm.tarul.cn

Java: new Random().nextInt(100) + 1
来源：http://snr.gaohongyu789.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://aet.xziqi.cn

Ruby: rand(1..100)
来源：http://zlq.sysykeji.top

C#:   new Random().Next(1, 101)
来源：http://hwf.c1oappe.top

[A11] 条件表达式（三元）
来源：http://ruy.yj20258888.top

Py:   "yes" if x > 0 else "no"
来源：http://qwc.yj202588.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://cir.zdqjudy.top

JS:   x > 0 ? "yes" : "no"
来源：http://dtt.uphjek.com

TS:   x > 0 ? "yes" : "no"
来源：http://jds.cheryme.top

Java: x > 0 ? "yes" : "no"
来源：http://sch.yuxming.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://dhl.yj20258.top

Ruby: x > 0 ? "yes" : "no"
来源：http://blj.zhengqikj.top

C#:   x > 0 ? "yes" : "no"
来源：http://zdt.ydjk.org.cn

[A12] 字符串插值 / 格式化
来源：http://adj.kuanghao11.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pmx.jlsjyb.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rhh.xingfuxueyuan.xyz

JS:   `Hello, ${name}!`
来源：http://ffb.fktsv.cn

TS:   `Hello, ${name}!`
来源：http://bad.c1oappe.top

Java: "Hello, %s!".formatted(name)
来源：http://grp.yj202588.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ubb.daria6918.cn

Ruby: "Hello, #{name}!"
来源：http://mhh.cashguo.top

C#:   $"Hello, {name}!"
来源：http://gap.hongshengwenyu.top

[A13] 多行字符串（练习 \n 转义）
来源：http://zcf.hcnkem.com

Py:   "第一行\n第二行"
来源：http://yao.fktsv.cn

PHP:  "第一行\n第二行"
来源：http://krm.zycfv.cn

JS:   "第一行\n第二行"
来源：http://fbs.bbcook.cn

TS:   "第一行\n第二行"
来源：http://zsp.zhiwuduotai.top

Java: "第一行\n第二行"
来源：http://uca.nanxinkj.top

Go:   "第一行\n第二行"
来源：http://tdc.zhijiandao.cn

Ruby: "第一行\n第二行"
来源：http://ysw.fengsongda.top

C#:   "第一行\n第二行"
来源：http://wax.nanxinkj.top

[A14] 注释写法
来源：http://joj.jiagoushi.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://inz.havefunace.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://fvn.ybcxt.top

JS:   // 单行；/* 多行 */
来源：http://vaf.jinqigufen.top

TS:   // 单行；/* 多行 */
来源：http://ksm.zhaomingkeji.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xum.9152youxi.cn

Go:   // 单行；/* 多行 */
来源：http://hju.gogol.net.cn

Ruby: # 单行；=begin 多行 =end
来源：http://chv.hnxiangtu.top

C#:   // 单行；/* 多行 */
来源：http://rzr.quarkkingdee.top

[A15] 空值判断与默认值
来源：http://nsb.zhaomingkeji.xyz

Py:   value = data or "默认值"
来源：http://dfk.andypj.xyz

PHP:  $value = $data ?? "默认值";
来源：http://cuh.daria6918.cn

JS:   const value = data ?? "默认值";
来源：http://ezu.aizwys.cn

TS:   const value = data ?? "默认值";
来源：http://mxp.cheryme.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nlx.andypj.xyz

Go:   if data == "" { data = "默认值" }
来源：http://vtw.bbcook.cn

Ruby: value = data || "默认值"
来源：http://eka.0kj1m.cn

C#:   var value = data ?? "默认值";
来源：http://sgh.pycfn.com

[A16] 真假值判断规则
来源：http://icf.tianlin.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nup.ydzc1.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://swt.sweek.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://onw.hysaishi.cn

TS:   if (!x) {}
来源：http://kev.fehbvm.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mlj.zhoulong.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ymv.hywenlv.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vdu.shuidangran.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zsc.guannengcc.top

[A17] 位运算
来源：http://mmy.dashuyun.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vsw.yangfankeji.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://frt.sxryk.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yje.fengsongda.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gbf.cqqwz.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tdu.feifeiyinyue.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xot.gogol.net.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ytf.fktsv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hds.uphjek.com

[A18] 字符与 ASCII 码互转
来源：http://yaw.vqdsnc.cn

Py:   ord("A"); chr(65)
来源：http://rbd.fzhhl.top

PHP:  ord("A"); chr(65)
来源：http://gxm.yangfankeji.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dhf.yuanzhike.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cjz.sjlbkw.cn

Java: (int) 'A'; (char) 65
来源：http://uka.ywan-chungtsiang.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pwc.guannengcc.top

Ruby: "A".ord; 65.chr
来源：http://iqt.sxryk.cn

C#:   (int)'A'; (char)65
来源：http://iyq.hnqzz.top

[A19] 交换两个变量
来源：http://gcz.sjlbkw.cn

Py:   a, b = b, a
来源：http://zbb.jianghu66.top

PHP:  [$a, $b] = [$b, $a];
来源：http://osz.birdmap.top

JS:   [a, b] = [b, a];
来源：http://qxg.sweek.top

TS:   [a, b] = [b, a];
来源：http://mmp.tian-w.cn

Java: int t = a; a = b; b = t;
来源：http://ylm.birdmap.top

Go:   a, b = b, a
来源：http://blq.wangdashe.top

Ruby: a, b = b, a
来源：http://xpm.daxiang520.top

C#:   (a, b) = (b, a);
来源：http://gfh.hesvh.cn

[A20] 读取标准输入
来源：http://yzs.hnxiangtu.top

Py:   name = input("请输入：")
来源：http://iou.zdbjq.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rhc.wangdashe.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nhf.hammf.cn

TS:   // Node.js：readline 模块
来源：http://fsy.c1oappe.top

Java: new Scanner(System.in).nextLine()
来源：http://psn.cdnleiting.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qja.vqdsnc.cn

Ruby: gets.chomp
来源：http://pfh.haohaochexian.top

C#:   Console.ReadLine();
来源：http://mah.hfpthk.cn

[A21] 保留指定小数位输出
来源：http://jgr.yj202588.top

Py:   f"{3.14159:.2f}"
来源：http://klo.nanxuanxn.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bfy.sxryk.cn

JS:   (3.14159).toFixed(2)
来源：http://wjw.fzhhl.top

TS:   (3.14159).toFixed(2)
来源：http://vvl.gotoacloud.top

Java: String.format("%.2f", 3.14159)
来源：http://qqi.hesvh.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lge.aibaodan.cn

Ruby: format("%.2f", 3.14159)
来源：http://mmd.xuanzx.com

C#:   3.14159.ToString("F2")
来源：http://mnu.yj20258.top

[A22] 获取字符串长度
来源：http://shj.0kj1m.cn

Py:   len(s)
来源：http://fha.ydjk.org.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mxb.ydzc1.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vie.feifeiyinyue.top

TS:   s.length
来源：http://sya.chenlongwang.top

Java: s.length()
来源：http://hzg.hammf.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zaj.yongpay.top

Ruby: s.length
来源：http://rwy.chenzaomai.com

C#:   s.Length
来源：http://jia.hysaishi.cn

[A23] 大小写转换
来源：http://bki.zycfv.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ykf.bbcook.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wol.iojbl.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jub.nanxinkj.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cas.svipenyu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mcw.zdbjq.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tlp.zycfv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cdm.shanyushiyangtech.top

C#:   s.ToUpper(); s.ToLower()
来源：http://dky.yfazqb.com

[A24] 去除首尾空白
来源：http://ivi.ybcxt.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jti.xylfe.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rwz.hnqzz.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ihw.xingfuxueyuan.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vcz.zycfv.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qst.fengsongda.top

Go:   strings.TrimSpace(s)
来源：http://fis.vehdjk.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xnc.zycfv.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wjp.xuanzx.com

[A25] 字符串比较
来源：http://gxb.yj20258.top

Py:   s1 == s2; s1 != s2
来源：http://cvn.c1oappe.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xrc.dianchejie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tsr.zycfv.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://abt.fanxiaobao.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://oxr.yongpay.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ivp.9152youxi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vqk.guowangkeji.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gqt.cqqwz.cn

[A26] 类型转换总览
来源：http://pgr.mhx1999.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vuf.chenjidiqi.icu

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pfz.havefunace.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pdk.haohaochexian.top

TS:   Number() String() Boolean() x as number
来源：http://jlt.wangshuangyany.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qhs.hongshengwenyu.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://uvm.nanxuanxn.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://mlo.zhixingplan.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blv.iojbl.cn

================================================================================
来源：http://fzd.sysykeji.top

B. 流程控制
来源：http://zwc.pengpengdd.cyou

================================================================================
来源：http://yzo.epnwcf.com

[B01] 条件判断 if / else
来源：http://fwb.ehwqpu.com

Py:   result = "正" if x > 0 else "非正"
来源：http://dmo.chenlongwang.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gpy.yuxming.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pch.hammf.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qkp.bjfxy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://otp.chenlongwang.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://itf.aizwys.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xns.daria6918.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lgz.fzhhl.top

[B02] 多分支 else if / elif
来源：http://xhn.hammf.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ifx.shanyushiyangkeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zqk.sxryk.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://niz.hysaishi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lct.yuxming.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://taw.pengpengdd.cyou

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gkp.daria6918.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ejl.yj20258.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kom.ydzc1.top

[B03] switch / match / case
来源：http://xqj.mhx1999.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fot.jqgufenzy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://orp.vqdsnc.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ghm.cashguo.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wve.yonumen.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://try.bjfxy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kpb.yvedp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wcy.fehbvm.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pfb.yuanzhike.top

[B04] for 计数循环
来源：http://ywm.pengpengdd.cyou

Py:   for i in range(10): print(i)
来源：http://qpk.meibo888.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://awh.9152youxi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://frn.cucudq.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mch.wangshuangyany.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eqs.chenjidiqi.icu

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sjm.shanyushiyangtech.top

Ruby: 10.times { |i| puts i }
来源：http://igk.sysykeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ngj.svipenyu.cn

[B05] 遍历数组 / 列表
来源：http://epe.wangshuangyany.cn

Py:   for item in arr: print(item)
来源：http://fuv.fktsv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gig.xziqi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qgy.sxryk.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mgo.redwolf501.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://hun.fanxiaobao.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ypb.zhijiandao.cn

Ruby: arr.each { |item| puts item }
来源：http://mlx.fanxiaobao.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wsf.hesvh.cn

[B06] 遍历字典 / 对象
来源：http://cjf.birdmap.top

Py:   for k, v in d.items(): print(k, v)
来源：http://wbb.vehdjk.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uia.yvedp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aib.wangdashe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iyq.quarkkingdee.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tkr.hesvh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vcg.316326.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lwm.kuanghao11.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://acj.bjfxy.top

[B07] while 循环
来源：http://onq.c1oappe.top

Py:   while i < 10: i += 1
来源：http://tqo.havefunace.top

PHP:  while ($i < 10) { $i++; }
来源：http://hhz.aizwys.cn

JS:   while (i < 10) { i++; }
来源：http://fyf.snrcjt.cn

TS:   while (i < 10) { i++; }
来源：http://zoa.ehwqpu.com

Java: while (i < 10) { i++; }
来源：http://ojx.yj20258.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yob.iojbl.cn

Ruby: while i < 10; i += 1; end
来源：http://gkz.iojbl.cn

C#:   while (i < 10) { i++; }
来源：http://txl.zhiwuduotai.top

[B08] do-while（至少执行一次）
来源：http://xne.zhengqikj.top


<!-- 参考信息 -->