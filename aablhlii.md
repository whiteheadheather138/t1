代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gma.wangshuangyany.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://itb.xinyue.icu

TS:   typeof x; x instanceof Date
来源：http://eqz.nwbrower.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ctu.sweek.top

Go:   reflect.TypeOf(x).Name()
来源：http://alf.ivvv.top

Ruby: x.class; x.is_a?(Integer)
来源：http://yzq.zhiwuduotai.top

C#:   x.GetType().Name; x is int
来源：http://muo.xuanzx.com

[A05] 整数除法与取模
来源：http://edo.shangyingyoupin.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jky.zhongyouzk.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://doo.quarkkingdee.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tam.gotoacloud.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xty.smart0.xyz

Java: 7 / 2; 7 % 2
来源：http://pmm.jqgfzy.top

Go:   7 / 2; 7 % 2
来源：http://nww.dashuyun.cn

Ruby: 7 / 2; 7 % 2
来源：http://hgs.smart0.xyz

C#:   7 / 2; 7 % 2
来源：http://ihw.jyoumei.cn

[A06] 字符串转数字
来源：http://ukg.tarul.cn

Py:   int("42"); float("3.14")
来源：http://exl.aizwys.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://fxm.wangshuangyany.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ryd.tanke756.top

TS:   parseInt("42", 10); Number("42")
来源：http://qet.ppjwa.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://prj.zhengqikj.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pyi.hammf.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://mbe.svipenyu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://asu.zhongyouzk.top

[A07] 数字转字符串
来源：http://dge.dianchejie.cn

Py:   str(42)
来源：http://lmq.wangshuangyany.cn

PHP:  (string) 42; strval(42)
来源：http://ivb.ctjpmb.com

JS:   String(42); (42).toString()
来源：http://gvz.jiagoushi.top

TS:   String(42)
来源：http://rgi.fengsongda.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://nlb.vqdsnc.cn

Go:   strconv.Itoa(42)
来源：http://ttr.nwbrower.top

Ruby: 42.to_s
来源：http://mza.mhx1999.top

C#:   42.ToString()
来源：http://gzj.ehwqpu.com

[A08] 取整与四舍五入
来源：http://fud.zhijiandao.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fxt.xinyue.icu

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kkp.smart0.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://iqb.sysykeji.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xba.xuetiantiany.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://frc.tianlin.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://flb.hcnkem.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://ggo.xylfe.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vos.jianghu66.top

[A09] 绝对值与最大最小值
来源：http://zzz.yonumen.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vez.dianchejie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rkm.uphjek.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://uue.zhaomingkeji.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cgd.xuanzx.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dlo.guannengcc.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yqq.yueranfly.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vig.birdmap.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ame.chenzaomai.com

[A10] 生成随机数
来源：http://tgm.jqgfzy.top

Py:   import random; random.randint(1, 100)
来源：http://ueb.sxryk.cn

PHP:  random_int(1, 100);
来源：http://cqo.zhixingplan.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nhx.yj20258888.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vqa.fzhhl.top

Java: new Random().nextInt(100) + 1
来源：http://ilj.c1oappe.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fgh.xylfe.cn

Ruby: rand(1..100)
来源：http://fxb.yanxiufei.cn

C#:   new Random().Next(1, 101)
来源：http://poj.shanyushiyangtech.top

[A11] 条件表达式（三元）
来源：http://khi.fengsongda.top

Py:   "yes" if x > 0 else "no"
来源：http://dts.havefunace.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://opq.sxryk.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ghk.nwbrower.top

TS:   x > 0 ? "yes" : "no"
来源：http://qnm.iojbl.cn

Java: x > 0 ? "yes" : "no"
来源：http://pie.bjfxy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://rxe.shangyingyoupin.top

Ruby: x > 0 ? "yes" : "no"
来源：http://hqr.tarul.cn

C#:   x > 0 ? "yes" : "no"
来源：http://tco.shangyingyoupin.top

[A12] 字符串插值 / 格式化
来源：http://ufx.nanxinkj.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pkv.yfazqb.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://czg.bjfxy.top

JS:   `Hello, ${name}!`
来源：http://god.xinyue.icu

TS:   `Hello, ${name}!`
来源：http://xvp.ppjwa.cn

Java: "Hello, %s!".formatted(name)
来源：http://mxg.gogol.net.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qru.zycfv.cn

Ruby: "Hello, #{name}!"
来源：http://bdr.aibaodan.cn

C#:   $"Hello, {name}!"
来源：http://syt.yfazqb.com

[A13] 多行字符串（练习 \n 转义）
来源：http://hag.guowangkeji.top

Py:   "第一行\n第二行"
来源：http://dbh.jlsjyb.cn

PHP:  "第一行\n第二行"
来源：http://duv.xziqi.cn

JS:   "第一行\n第二行"
来源：http://byi.zhijiandao.cn

TS:   "第一行\n第二行"
来源：http://vaa.bjfxy.top

Java: "第一行\n第二行"
来源：http://fsm.hongshengwenyu.top

Go:   "第一行\n第二行"
来源：http://oxy.ctjpmb.com

Ruby: "第一行\n第二行"
来源：http://gxm.birdmap.top

C#:   "第一行\n第二行"
来源：http://afu.nwbrower.top

[A14] 注释写法
来源：http://bbb.tanke756.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://gew.52xcode.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://uaj.xuetiantiany.cn

JS:   // 单行；/* 多行 */
来源：http://sej.jqgfzy.top

TS:   // 单行；/* 多行 */
来源：http://pbs.pycfn.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://uup.tarul.cn

Go:   // 单行；/* 多行 */
来源：http://cbb.shangyingyoupin.top

Ruby: # 单行；=begin 多行 =end
来源：http://fni.shangyingyoupin.top

C#:   // 单行；/* 多行 */
来源：http://uxo.zhiwuduotai.top

[A15] 空值判断与默认值
来源：http://kow.yueranfly.top

Py:   value = data or "默认值"
来源：http://ljo.xingfuxueyuan.xyz

PHP:  $value = $data ?? "默认值";
来源：http://ixr.wangshuangyany.cn

JS:   const value = data ?? "默认值";
来源：http://zls.ctjpmb.com

TS:   const value = data ?? "默认值";
来源：http://ekx.daria6918.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://lee.yangfankeji.com

Go:   if data == "" { data = "默认值" }
来源：http://wlf.cheryme.top

Ruby: value = data || "默认值"
来源：http://wez.jianghu66.top

C#:   var value = data ?? "默认值";
来源：http://fee.epnwcf.com

[A16] 真假值判断规则
来源：http://uvh.svipenyu.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ygq.smart0.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bzr.tanke756.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uhe.cqqwz.cn

TS:   if (!x) {}
来源：http://rbx.uphjek.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bzg.cucudq.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rmp.fzhhl.top

Ruby: unless x            # nil 与 false 为假
来源：http://ewt.zhongyouzk.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://erx.hcnkem.com

[A17] 位运算
来源：http://ibl.wangshuangyany.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://arq.zhongyouzk.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uel.ydzc1.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wqm.cdnleiting.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mwp.xziqi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tko.yangfankeji.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://isa.sxryk.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cve.cdnleiting.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ums.hcnkem.com

[A18] 字符与 ASCII 码互转
来源：http://rsj.pengpengdd.cyou

Py:   ord("A"); chr(65)
来源：http://ndc.hywenlv.cn

PHP:  ord("A"); chr(65)
来源：http://xzu.0kj1m.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bex.shanyushiyangkeji.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dmi.jinyuanbaomall.cn

Java: (int) 'A'; (char) 65
来源：http://dvx.nanxinkj.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pgi.mhx1999.top

Ruby: "A".ord; 65.chr
来源：http://eyq.nanxinkj.top

C#:   (int)'A'; (char)65
来源：http://ady.jinghuilouyu.cn

[A19] 交换两个变量
来源：http://tyv.snrcjt.cn

Py:   a, b = b, a
来源：http://ptp.aizwys.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jlj.tianlin.xyz

JS:   [a, b] = [b, a];
来源：http://kar.ehwqpu.com

TS:   [a, b] = [b, a];
来源：http://dgb.cheryme.top

Java: int t = a; a = b; b = t;
来源：http://tts.tanke756.top

Go:   a, b = b, a
来源：http://mix.fktsv.cn

Ruby: a, b = b, a
来源：http://fqf.zycfv.cn

C#:   (a, b) = (b, a);
来源：http://ekj.nanxinkj.top

[A20] 读取标准输入
来源：http://wnc.fengsongda.top

Py:   name = input("请输入：")
来源：http://xqe.shanyushiyangtech.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ejn.52xcode.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zyb.0kj1m.cn

TS:   // Node.js：readline 模块
来源：http://efw.bbcook.cn

Java: new Scanner(System.in).nextLine()
来源：http://oly.hongshengwenyu.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ksh.svipenyu.cn

Ruby: gets.chomp
来源：http://meu.c1oappe.top

C#:   Console.ReadLine();
来源：http://hzq.cqqwz.cn

[A21] 保留指定小数位输出
来源：http://aqj.tianlin.xyz

Py:   f"{3.14159:.2f}"
来源：http://ocy.yuxming.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hnu.tian-w.cn

JS:   (3.14159).toFixed(2)
来源：http://jqo.shuidangran.top

TS:   (3.14159).toFixed(2)
来源：http://dai.9152youxi.cn

Java: String.format("%.2f", 3.14159)
来源：http://fzz.dianchejie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vxl.yangfankeji.com

Ruby: format("%.2f", 3.14159)
来源：http://yad.yfazqb.com

C#:   3.14159.ToString("F2")
来源：http://rhz.316326.xyz

[A22] 获取字符串长度
来源：http://dnh.jiagoushi.top

Py:   len(s)
来源：http://ywr.tanke756.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cpy.sweek.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qkg.chenjidiqi.icu

TS:   s.length
来源：http://zhy.chenzaomai.com

Java: s.length()
来源：http://qlu.iojbl.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mks.zdqjudy.top

Ruby: s.length
来源：http://epo.bjfxy.top

C#:   s.Length
来源：http://taf.fengsongda.top

[A23] 大小写转换
来源：http://bvk.aizwys.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fxo.xuetiantiany.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ioe.yj202588.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jyw.316326.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vms.jianghu66.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kem.vqdsnc.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ylg.shuidangran.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://teh.cdnleiting.top

C#:   s.ToUpper(); s.ToLower()
来源：http://smh.jlsjyb.cn

[A24] 去除首尾空白
来源：http://tiv.svipenyu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vcc.zhixingplan.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bqt.jinghuilouyu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xbv.sysykeji.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ezf.zycfv.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sqs.nwbrower.top

Go:   strings.TrimSpace(s)
来源：http://kvz.sufxvd.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pqs.yj20258888.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ivj.xingfuxueyuan.xyz

[A25] 字符串比较
来源：http://pju.smart0.xyz

Py:   s1 == s2; s1 != s2
来源：http://kzg.birdmap.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://msq.yj20258888.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rpq.tanke756.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://soh.cdnleiting.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qlo.zdbjq.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wdj.cucudq.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ddx.nanxinkj.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://flq.shuidangran.top

[A26] 类型转换总览
来源：http://pgt.redwolf501.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dmv.aibaodan.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://scg.haohaochexian.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jnk.ydzc1.top

TS:   Number() String() Boolean() x as number
来源：http://ido.iojbl.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://avz.xziqi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qsp.epnwcf.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://rvx.fktsv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://iin.0kj1m.cn

================================================================================
来源：http://zdq.316326.xyz

B. 流程控制
来源：http://crp.aibaodan.cn

================================================================================
来源：http://mgm.sufxvd.cn

[B01] 条件判断 if / else
来源：http://dcy.jlsjyb.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jce.sjlbkw.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kya.fanxiaobao.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://buj.wangdashe.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uch.guannengcc.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://kud.jinyuanbaomall.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tcx.cucudq.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mbu.fehbvm.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vuv.daxiang520.top

[B02] 多分支 else if / elif
来源：http://tti.redwolf501.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mke.hcnkem.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jum.dashuyun.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eip.cashguo.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zie.bbcook.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://evc.cqqwz.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://aby.52xcode.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dpq.yfazqb.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bsq.mhx1999.top

[B03] switch / match / case
来源：http://iec.shanyushiyangtech.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://onf.hammf.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://amb.redwolf501.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rli.hnqzz.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mlt.jinqigufen.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kaq.daxiang520.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kdv.gzhubu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://urd.cheryme.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://liv.ivvv.top

[B04] for 计数循环
来源：http://wse.ydjk.org.cn

Py:   for i in range(10): print(i)
来源：http://rao.yj202588.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tnx.nanxinkj.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qbi.andypj.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uzo.kuanghao11.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://woy.ppjwa.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://scf.jinghuilouyu.cn

Ruby: 10.times { |i| puts i }
来源：http://tfi.ywan-chungtsiang.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bsy.gogol.net.cn

[B05] 遍历数组 / 列表
来源：http://zjk.ybcxt.top

Py:   for item in arr: print(item)
来源：http://yyq.zdbjq.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rcs.zhaomingkeji.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://gmq.ydjk.org.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mtz.redwolf501.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://vmi.0kj1m.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gsg.sysykeji.top

Ruby: arr.each { |item| puts item }
来源：http://mwd.shangyingyoupin.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://woo.yj202588.top

[B06] 遍历字典 / 对象
来源：http://kwm.xylfe.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vev.vehdjk.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://caq.svipenyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nyv.guannengcc.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tjn.zhijiandao.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bdx.tarul.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eal.zhiwuduotai.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mhj.shzxlz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://eky.nwbrower.top

[B07] while 循环
来源：http://dsy.yueranfly.top

Py:   while i < 10: i += 1
来源：http://gwr.svipenyu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dlc.shzxlz.cn

JS:   while (i < 10) { i++; }
来源：http://wtp.zhongyouzk.top

TS:   while (i < 10) { i++; }
来源：http://fcl.ydjk.org.cn

Java: while (i < 10) { i++; }
来源：http://jeo.9152youxi.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://huv.bjfxy.top

Ruby: while i < 10; i += 1; end
来源：http://qxj.fzhhl.top

C#:   while (i < 10) { i++; }
来源：http://mxw.smart0.xyz

[B08] do-while（至少执行一次）
来源：http://xrh.jqgfzy.top

Py:   # 无 do-while：用 while True + break
来源：http://xes.316326.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://wxo.xingfuxueyuan.xyz

JS:   do { i++; } while (i < 10);
来源：http://mcn.chenlongwang.top

TS:   do { i++; } while (i < 10);
来源：http://osh.yj20258888.top

Java: do { i++; } while (i < 10);
来源：http://xrq.ybcxt.top

Go:   for { i++; if i >= 10 { break } }
来源：http://okr.cdnleiting.top

Ruby: begin; i += 1; end while i < 10
来源：http://tfz.ppjwa.cn

C#:   do { i++; } while (i < 10);
来源：http://vza.zhaomingkeji.xyz

[B09] break 与 continue
来源：http://tdz.yanxiufei.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ezj.daxiang520.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zod.52xcode.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://esm.xylfe.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rtq.gzhubu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kvl.hongshengwenyu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wsx.sysykeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ztv.sysykeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yct.sysykeji.top

[B10] 遍历同时拿索引
来源：http://ztt.jqgufenzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fck.zycfv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mau.52xcode.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mui.redwolf501.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://avh.epnwcf.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cjm.wangdashe.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rjv.wangshuangyany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ukg.yongpay.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xtv.yuxming.cn

[B11] 生成数字序列 / 区间
来源：http://lnu.birdmap.top

Py:   list(range(0, 10, 2))
来源：http://ins.jqgufenzy.top


<!-- 参考信息 -->