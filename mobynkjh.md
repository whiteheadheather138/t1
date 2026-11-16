代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://acs.meibo888.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pge.snrcjt.cn

TS:   typeof x; x instanceof Date
来源：http://hxb.quarkkingdee.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vvy.aizwys.cn

Go:   reflect.TypeOf(x).Name()
来源：http://lxx.gotoacloud.top

Ruby: x.class; x.is_a?(Integer)
来源：http://xhv.yj202588.top

C#:   x.GetType().Name; x is int
来源：http://ybj.pycfn.com

[A05] 整数除法与取模
来源：http://ekb.jinyuanbaomall.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lsl.shanyushiyangkeji.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://rki.ydzc1.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dcx.nanxuanxn.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hzl.xziqi.cn

Java: 7 / 2; 7 % 2
来源：http://qvp.yj20258888.top

Go:   7 / 2; 7 % 2
来源：http://dce.gotoacloud.top

Ruby: 7 / 2; 7 % 2
来源：http://bvb.9152youxi.cn

C#:   7 / 2; 7 % 2
来源：http://iwr.hnqzz.top

[A06] 字符串转数字
来源：http://dhg.jyoumei.cn

Py:   int("42"); float("3.14")
来源：http://tsm.shzxlz.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ikm.yj20258888.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lxb.zycfv.cn

TS:   parseInt("42", 10); Number("42")
来源：http://tny.jinghuilouyu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nug.ppjwa.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://amh.jianghu66.top

Ruby: "42".to_i; "3.14".to_f
来源：http://tun.ppjwa.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jew.gotoacloud.top

[A07] 数字转字符串
来源：http://awb.yj20258888.top

Py:   str(42)
来源：http://gon.ppjwa.cn

PHP:  (string) 42; strval(42)
来源：http://pvw.mhx1999.top

JS:   String(42); (42).toString()
来源：http://qzb.iojbl.cn

TS:   String(42)
来源：http://gsk.jiagoushi.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://aww.uphjek.com

Go:   strconv.Itoa(42)
来源：http://efd.zhijiandao.cn

Ruby: 42.to_s
来源：http://mpk.fehbvm.com

C#:   42.ToString()
来源：http://kwg.gogol.net.cn

[A08] 取整与四舍五入
来源：http://olu.fengsongda.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lkj.epnwcf.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qsw.xuetiantiany.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xho.kuanghao11.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://csx.zhongyouzk.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dhh.cqqwz.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://paa.jqgufenzy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://xwl.guannengcc.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wye.pengpengdd.cyou

[A09] 绝对值与最大最小值
来源：http://ckx.yonumen.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://veg.hnqzz.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ogk.fktsv.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cui.yj202588.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://uqy.zycfv.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rqs.birdmap.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pyp.sxryk.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wfs.yj202588.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zem.meibo888.top

[A10] 生成随机数
来源：http://sqx.meibo888.top

Py:   import random; random.randint(1, 100)
来源：http://rhe.gzhubu.top

PHP:  random_int(1, 100);
来源：http://wxc.cdnleiting.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xia.bbcook.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tlc.hnqzz.top

Java: new Random().nextInt(100) + 1
来源：http://pfd.ydjk.org.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dxh.jinqigufen.top

Ruby: rand(1..100)
来源：http://cbc.aizwys.cn

C#:   new Random().Next(1, 101)
来源：http://qsn.hfpthk.cn

[A11] 条件表达式（三元）
来源：http://aiw.havefunace.top

Py:   "yes" if x > 0 else "no"
来源：http://rpt.cdnleiting.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://rzw.tanke756.top

JS:   x > 0 ? "yes" : "no"
来源：http://glj.cheryme.top

TS:   x > 0 ? "yes" : "no"
来源：http://sbq.yongpay.top

Java: x > 0 ? "yes" : "no"
来源：http://xli.ppjwa.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://loy.chenlongwang.top

Ruby: x > 0 ? "yes" : "no"
来源：http://aoq.feifeiyinyue.top

C#:   x > 0 ? "yes" : "no"
来源：http://fhs.hnqzz.top

[A12] 字符串插值 / 格式化
来源：http://tnn.yonumen.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://brx.quarkkingdee.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://oes.wangdashe.top

JS:   `Hello, ${name}!`
来源：http://muk.hongshengwenyu.top

TS:   `Hello, ${name}!`
来源：http://tgb.jinyuanbaomall.cn

Java: "Hello, %s!".formatted(name)
来源：http://kis.tianlin.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wij.shuidangran.top

Ruby: "Hello, #{name}!"
来源：http://jsp.fengsongda.top

C#:   $"Hello, {name}!"
来源：http://knq.tian-w.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://xxg.quarkkingdee.top

Py:   "第一行\n第二行"
来源：http://pgz.cashguo.top

PHP:  "第一行\n第二行"
来源：http://mdq.hesvh.cn

JS:   "第一行\n第二行"
来源：http://lek.zhijiandao.cn

TS:   "第一行\n第二行"
来源：http://egj.sxryk.cn

Java: "第一行\n第二行"
来源：http://bhi.c1oappe.top

Go:   "第一行\n第二行"
来源：http://xjk.gotoacloud.top

Ruby: "第一行\n第二行"
来源：http://lot.shangyingyoupin.top

C#:   "第一行\n第二行"
来源：http://chm.yj202588.top

[A14] 注释写法
来源：http://mol.c1oappe.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://unx.gogol.net.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wrp.daria6918.cn

JS:   // 单行；/* 多行 */
来源：http://bcn.ehwqpu.com

TS:   // 单行；/* 多行 */
来源：http://oej.hnqzz.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zai.shuidangran.top

Go:   // 单行；/* 多行 */
来源：http://obi.ybcxt.top

Ruby: # 单行；=begin 多行 =end
来源：http://iro.yfazqb.com

C#:   // 单行；/* 多行 */
来源：http://ksl.tanke756.top

[A15] 空值判断与默认值
来源：http://wkl.jqgufenzy.top

Py:   value = data or "默认值"
来源：http://rhe.nanxuanxn.top

PHP:  $value = $data ?? "默认值";
来源：http://jtp.cucudq.cn

JS:   const value = data ?? "默认值";
来源：http://ine.yongpay.top

TS:   const value = data ?? "默认值";
来源：http://iyb.ywan-chungtsiang.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mle.kuanghao11.cn

Go:   if data == "" { data = "默认值" }
来源：http://cot.yanxiufei.cn

Ruby: value = data || "默认值"
来源：http://jll.birdmap.top

C#:   var value = data ?? "默认值";
来源：http://uyn.ehwqpu.com

[A16] 真假值判断规则
来源：http://pwn.zhaomingkeji.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cur.sjlbkw.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qaa.xinyue.icu

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sdv.xylfe.cn

TS:   if (!x) {}
来源：http://nrq.wangdashe.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hvu.zhoulong.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://iqj.daria6918.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xeg.52xcode.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vtf.gogol.net.cn

[A17] 位运算
来源：http://hmw.zdqjudy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wot.xylfe.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rev.hammf.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mrt.andypj.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://myg.bbcook.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xyj.jqgfzy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hng.vqdsnc.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vbz.ybcxt.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tje.fktsv.cn

[A18] 字符与 ASCII 码互转
来源：http://eki.ywan-chungtsiang.top

Py:   ord("A"); chr(65)
来源：http://nol.jinghuilouyu.cn

PHP:  ord("A"); chr(65)
来源：http://xyr.uphjek.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hab.zhixingplan.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tfz.chenlongwang.top

Java: (int) 'A'; (char) 65
来源：http://nzx.9152youxi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dzi.zhoulong.xyz

Ruby: "A".ord; 65.chr
来源：http://rya.ydjk.org.cn

C#:   (int)'A'; (char)65
来源：http://xks.vehdjk.com

[A19] 交换两个变量
来源：http://etg.yongpay.top

Py:   a, b = b, a
来源：http://lbe.xinyue.icu

PHP:  [$a, $b] = [$b, $a];
来源：http://jaa.bjfxy.top

JS:   [a, b] = [b, a];
来源：http://vwm.jyoumei.cn

TS:   [a, b] = [b, a];
来源：http://pvf.hongshengwenyu.top

Java: int t = a; a = b; b = t;
来源：http://zlb.yuanzhike.top

Go:   a, b = b, a
来源：http://efd.xuetiantiany.cn

Ruby: a, b = b, a
来源：http://dnq.zdbjq.cn

C#:   (a, b) = (b, a);
来源：http://ahd.9152youxi.cn

[A20] 读取标准输入
来源：http://apy.nanxinkj.top

Py:   name = input("请输入：")
来源：http://ebs.tian-w.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://agb.aibaodan.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://glk.ywan-chungtsiang.top

TS:   // Node.js：readline 模块
来源：http://dar.jinqigufen.top

Java: new Scanner(System.in).nextLine()
来源：http://kld.0kj1m.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://uhh.hongshengwenyu.top

Ruby: gets.chomp
来源：http://jkn.quarkkingdee.top

C#:   Console.ReadLine();
来源：http://wsl.guowangkeji.top

[A21] 保留指定小数位输出
来源：http://qwj.zhixingplan.top

Py:   f"{3.14159:.2f}"
来源：http://emb.hfpthk.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ijp.jinyuanbaomall.cn

JS:   (3.14159).toFixed(2)
来源：http://wjt.yongpay.top

TS:   (3.14159).toFixed(2)
来源：http://jug.9152youxi.cn

Java: String.format("%.2f", 3.14159)
来源：http://prq.yfazqb.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qgt.iojbl.cn

Ruby: format("%.2f", 3.14159)
来源：http://ori.yonumen.top

C#:   3.14159.ToString("F2")
来源：http://roa.gaohongyu789.top

[A22] 获取字符串长度
来源：http://xop.aibaodan.cn

Py:   len(s)
来源：http://dtp.zdqjudy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ipy.fktsv.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ylu.pycfn.com

TS:   s.length
来源：http://mib.zhijiandao.cn

Java: s.length()
来源：http://zgz.meibo888.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fty.chenzaomai.com

Ruby: s.length
来源：http://naj.jinghuilouyu.cn

C#:   s.Length
来源：http://gga.guowangkeji.top

[A23] 大小写转换
来源：http://obg.nwbrower.top

Py:   s.upper(); s.lower(); s.title()
来源：http://cva.gogol.net.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://txn.cashguo.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kcf.hnxiangtu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ver.c1oappe.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://exf.vqdsnc.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cps.yj20258.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://thu.cashguo.top

C#:   s.ToUpper(); s.ToLower()
来源：http://kbp.quarkkingdee.top

[A24] 去除首尾空白
来源：http://fda.yonumen.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://srx.jinyuanbaomall.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xtk.zhiwuduotai.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hae.zhongyouzk.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vrl.havefunace.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rho.zhiwuduotai.top

Go:   strings.TrimSpace(s)
来源：http://aen.ydjk.org.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fmm.hfpthk.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dfe.guowangkeji.top

[A25] 字符串比较
来源：http://fhq.hongshengwenyu.top

Py:   s1 == s2; s1 != s2
来源：http://cyr.tian-w.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://twb.fehbvm.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wtu.jianghu66.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ssr.xingfuxueyuan.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fey.shanyushiyangkeji.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wgd.daxiang520.top

Ruby: s1 == s2; s1 <=> s2
来源：http://nsh.sweek.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qgq.ivvv.top

[A26] 类型转换总览
来源：http://grc.jianghu66.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ppo.bbcook.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jwo.snrcjt.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yoq.redwolf501.top

TS:   Number() String() Boolean() x as number
来源：http://cfq.svipenyu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bcy.epnwcf.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://peb.ydjk.org.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yez.fktsv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kis.316326.xyz

================================================================================
来源：http://yxf.zhiwuduotai.top

B. 流程控制
来源：http://auw.meibo888.top

================================================================================
来源：http://jvx.hnqzz.top

[B01] 条件判断 if / else
来源：http://kua.yj202588.top

Py:   result = "正" if x > 0 else "非正"
来源：http://puq.zdqjudy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hau.jyoumei.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zne.gogol.net.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zfe.bbcook.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://osj.jqgufenzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://thb.bjfxy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kfv.jinghuilouyu.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uwf.gogol.net.cn

[B02] 多分支 else if / elif
来源：http://lwr.hnqzz.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yrt.chenjidiqi.icu

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kyv.hammf.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jxi.jqgufenzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://owe.hcnkem.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wjl.jiagoushi.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fpb.feifeiyinyue.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pwj.hongshengwenyu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iqy.nanxinkj.top

[B03] switch / match / case
来源：http://ysj.daxiang520.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sef.yangfankeji.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xqg.xuanzx.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://scg.jyoumei.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wfx.shanyushiyangkeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ghr.tanke756.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tpy.sxryk.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hol.jianghu66.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vwd.ivvv.top

[B04] for 计数循环
来源：http://exz.yvedp.cn

Py:   for i in range(10): print(i)
来源：http://cal.bjfxy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sop.tian-w.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dxr.shanyushiyangtech.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vga.0kj1m.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://grp.ivvv.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gqc.bjfxy.top

Ruby: 10.times { |i| puts i }
来源：http://yif.shanyushiyangkeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vxb.ivvv.top

[B05] 遍历数组 / 列表
来源：http://fou.shanyushiyangtech.top

Py:   for item in arr: print(item)
来源：http://mzm.xuanzx.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kmq.bjfxy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://oca.jyoumei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cvp.daria6918.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://avg.zhengqikj.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://npb.nanxinkj.top

Ruby: arr.each { |item| puts item }
来源：http://fat.hnqzz.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sla.xziqi.cn

[B06] 遍历字典 / 对象
来源：http://vlj.yj202588.top

Py:   for k, v in d.items(): print(k, v)
来源：http://cca.hnxiangtu.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://krs.xuetiantiany.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jiq.zhoulong.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qzo.yj20258.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pos.fehbvm.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://elm.svipenyu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xwi.smart0.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://suk.yangfankeji.com

[B07] while 循环
来源：http://pqf.zdqjudy.top

Py:   while i < 10: i += 1
来源：http://skh.hysaishi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://nqv.snrcjt.cn

JS:   while (i < 10) { i++; }
来源：http://ryn.svipenyu.cn

TS:   while (i < 10) { i++; }
来源：http://paf.chenzaomai.com

Java: while (i < 10) { i++; }
来源：http://lgm.tanke756.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://txw.havefunace.top

Ruby: while i < 10; i += 1; end
来源：http://mxo.epnwcf.com

C#:   while (i < 10) { i++; }
来源：http://wgc.cheryme.top

[B08] do-while（至少执行一次）
来源：http://mud.zhoulong.xyz

Py:   # 无 do-while：用 while True + break
来源：http://ibl.hcnkem.com

PHP:  do { $i++; } while ($i < 10);
来源：http://uvu.hnxiangtu.top

JS:   do { i++; } while (i < 10);
来源：http://tpq.gaohongyu789.top

TS:   do { i++; } while (i < 10);
来源：http://atc.hnxiangtu.top

Java: do { i++; } while (i < 10);
来源：http://djy.chenlongwang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://usz.xingfuxueyuan.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://ves.ydzc1.top

C#:   do { i++; } while (i < 10);
来源：http://wsd.jinqigfzy.top

[B09] break 与 continue
来源：http://erx.yangfankeji.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wjw.gotoacloud.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cez.316326.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gif.jqgfzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mze.jinyuanbaomall.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qid.andypj.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hsf.sufxvd.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wuf.xylfe.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bup.jqgufenzy.top

[B10] 遍历同时拿索引
来源：http://ukh.bjfxy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dvv.yuanzhike.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tkq.xuetiantiany.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fvv.hongshengwenyu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://azu.hammf.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vyk.yuanzhike.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tdg.yongpay.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sio.tian-w.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rhy.zycfv.cn

[B11] 生成数字序列 / 区间
来源：http://dtz.smart0.xyz

Py:   list(range(0, 10, 2))
来源：http://rzy.zhongyouzk.top


<!-- 参考信息 -->