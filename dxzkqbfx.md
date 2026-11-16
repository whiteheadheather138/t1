代发 wailian999

[A06] 字符串转数字
来源：http://dcb.9152youxi.cn

Py:   int("42"); float("3.14")
来源：http://akw.vehdjk.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gcp.sysykeji.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ine.dianchejie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://mtz.ybcxt.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qjj.xingfuxueyuan.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wex.sxryk.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bhb.yangfankeji.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cyv.haohaochexian.top

[A07] 数字转字符串
来源：http://lmt.zycfv.cn

Py:   str(42)
来源：http://tce.cashguo.top

PHP:  (string) 42; strval(42)
来源：http://gnv.jinyuanbaomall.cn

JS:   String(42); (42).toString()
来源：http://jzg.cheryme.top

TS:   String(42)
来源：http://dpx.dianchejie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://hig.feifeiyinyue.top

Go:   strconv.Itoa(42)
来源：http://abb.guowangkeji.top

Ruby: 42.to_s
来源：http://oaz.zhoulong.xyz

C#:   42.ToString()
来源：http://ffu.nanxuanxn.top

[A08] 取整与四舍五入
来源：http://zom.zdbjq.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qfu.0kj1m.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://htj.fktsv.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jfl.sjlbkw.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://udk.guannengcc.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gnt.ehwqpu.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ifw.yangfankeji.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://ljk.jlsjyb.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gth.jqgufenzy.top

[A09] 绝对值与最大最小值
来源：http://bwa.guannengcc.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kzs.jinghuilouyu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://iyw.yuanzhike.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nac.vqdsnc.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qcj.yvedp.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jng.wangshuangyany.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://svq.hfpthk.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ryc.gzhubu.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rbq.ppjwa.cn

[A10] 生成随机数
来源：http://kob.bjfxy.top

Py:   import random; random.randint(1, 100)
来源：http://ssv.jlsjyb.cn

PHP:  random_int(1, 100);
来源：http://vut.redwolf501.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://waq.nanxinkj.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hyx.shzxlz.cn

Java: new Random().nextInt(100) + 1
来源：http://sjv.xuanzx.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qxv.chenjidiqi.icu

Ruby: rand(1..100)
来源：http://eqk.zhixingplan.top

C#:   new Random().Next(1, 101)
来源：http://onu.jinqigufen.top

[A11] 条件表达式（三元）
来源：http://sgj.hnqzz.top

Py:   "yes" if x > 0 else "no"
来源：http://htd.ppjwa.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://hwy.mhx1999.top

JS:   x > 0 ? "yes" : "no"
来源：http://ykk.yj20258888.top

TS:   x > 0 ? "yes" : "no"
来源：http://bsc.hysaishi.cn

Java: x > 0 ? "yes" : "no"
来源：http://tvi.cucudq.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://sba.dashuyun.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vdz.shzxlz.cn

C#:   x > 0 ? "yes" : "no"
来源：http://olo.smart0.xyz

[A12] 字符串插值 / 格式化
来源：http://bmr.sweek.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hpf.zdbjq.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jmh.zhixingplan.top

JS:   `Hello, ${name}!`
来源：http://hqy.gzhubu.top

TS:   `Hello, ${name}!`
来源：http://iox.gotoacloud.top

Java: "Hello, %s!".formatted(name)
来源：http://dnn.jinyuanbaomall.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vad.uphjek.com

Ruby: "Hello, #{name}!"
来源：http://kqm.epnwcf.com

C#:   $"Hello, {name}!"
来源：http://sov.guannengcc.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ewi.sjlbkw.cn

Py:   "第一行\n第二行"
来源：http://gzi.tanke756.top

PHP:  "第一行\n第二行"
来源：http://vct.gotoacloud.top

JS:   "第一行\n第二行"
来源：http://kol.ydzc1.top

TS:   "第一行\n第二行"
来源：http://ron.zdqjudy.top

Java: "第一行\n第二行"
来源：http://uuq.gotoacloud.top

Go:   "第一行\n第二行"
来源：http://ial.wangdashe.top

Ruby: "第一行\n第二行"
来源：http://ibo.ivvv.top

C#:   "第一行\n第二行"
来源：http://vqa.aizwys.cn

[A14] 注释写法
来源：http://blh.iojbl.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ycn.snrcjt.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ccs.havefunace.top

JS:   // 单行；/* 多行 */
来源：http://urj.hfpthk.cn

TS:   // 单行；/* 多行 */
来源：http://did.sjlbkw.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://buf.zhaomingkeji.xyz

Go:   // 单行；/* 多行 */
来源：http://hsp.hnqzz.top

Ruby: # 单行；=begin 多行 =end
来源：http://krb.smart0.xyz

C#:   // 单行；/* 多行 */
来源：http://oju.zhijiandao.cn

[A15] 空值判断与默认值
来源：http://akd.gaohongyu789.top

Py:   value = data or "默认值"
来源：http://glt.zhijiandao.cn

PHP:  $value = $data ?? "默认值";
来源：http://eei.ydzc1.top

JS:   const value = data ?? "默认值";
来源：http://qex.iojbl.cn

TS:   const value = data ?? "默认值";
来源：http://ywb.bbcook.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://twh.hysaishi.cn

Go:   if data == "" { data = "默认值" }
来源：http://zdp.yvedp.cn

Ruby: value = data || "默认值"
来源：http://ldy.guowangkeji.top

C#:   var value = data ?? "默认值";
来源：http://jgj.fehbvm.com

[A16] 真假值判断规则
来源：http://tay.jiagoushi.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qnx.c1oappe.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ihe.zhongyouzk.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://itw.xuetiantiany.cn

TS:   if (!x) {}
来源：http://viu.mhx1999.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cqq.hfpthk.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tqh.fanxiaobao.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://nji.yj20258.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://uyy.yj20258.top

[A17] 位运算
来源：http://jdz.andypj.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yet.zycfv.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gtm.dianchejie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://peo.hnxiangtu.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nsh.birdmap.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zzt.zhixingplan.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://saz.guannengcc.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qak.sjlbkw.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yrq.mhx1999.top

[A18] 字符与 ASCII 码互转
来源：http://mio.zhoulong.xyz

Py:   ord("A"); chr(65)
来源：http://lwl.yonumen.top

PHP:  ord("A"); chr(65)
来源：http://qim.c1oappe.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vsi.smart0.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mlo.nwbrower.top

Java: (int) 'A'; (char) 65
来源：http://mno.daxiang520.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rjd.bjfxy.top

Ruby: "A".ord; 65.chr
来源：http://cqz.jinghuilouyu.cn

C#:   (int)'A'; (char)65
来源：http://dru.yj20258888.top

[A19] 交换两个变量
来源：http://jqh.gaohongyu789.top

Py:   a, b = b, a
来源：http://gwe.shanyushiyangtech.top

PHP:  [$a, $b] = [$b, $a];
来源：http://qsx.yangfankeji.com

JS:   [a, b] = [b, a];
来源：http://cdh.yj202588.top

TS:   [a, b] = [b, a];
来源：http://soi.meibo888.top

Java: int t = a; a = b; b = t;
来源：http://kib.316326.xyz

Go:   a, b = b, a
来源：http://odg.cdnleiting.top

Ruby: a, b = b, a
来源：http://hee.bjfxy.top

C#:   (a, b) = (b, a);
来源：http://mez.feifeiyinyue.top

[A20] 读取标准输入
来源：http://wfu.hnxiangtu.top

Py:   name = input("请输入：")
来源：http://ktc.ctjpmb.com

PHP:  $name = trim(fgets(STDIN));
来源：http://til.havefunace.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bzi.hywenlv.cn

TS:   // Node.js：readline 模块
来源：http://rmt.316326.xyz

Java: new Scanner(System.in).nextLine()
来源：http://gos.daria6918.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pdb.c1oappe.top

Ruby: gets.chomp
来源：http://qvy.jinyuanbaomall.cn

C#:   Console.ReadLine();
来源：http://ucx.jqgfzy.top

[A21] 保留指定小数位输出
来源：http://icp.dianchejie.cn

Py:   f"{3.14159:.2f}"
来源：http://aro.mhx1999.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zrh.zycfv.cn

JS:   (3.14159).toFixed(2)
来源：http://qmg.fengsongda.top

TS:   (3.14159).toFixed(2)
来源：http://zpq.hywenlv.cn

Java: String.format("%.2f", 3.14159)
来源：http://qrr.yuanzhike.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://val.epnwcf.com

Ruby: format("%.2f", 3.14159)
来源：http://kdk.zhaomingkeji.xyz

C#:   3.14159.ToString("F2")
来源：http://kjz.daxiang520.top

[A22] 获取字符串长度
来源：http://wxz.shzxlz.cn

Py:   len(s)
来源：http://zax.guannengcc.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rgl.hywenlv.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ymz.jyoumei.cn

TS:   s.length
来源：http://rec.shzxlz.cn

Java: s.length()
来源：http://giv.fktsv.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ncv.zhoulong.xyz

Ruby: s.length
来源：http://mnm.tianlin.xyz

C#:   s.Length
来源：http://yjh.xingfuxueyuan.xyz

[A23] 大小写转换
来源：http://jhe.iojbl.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ssi.xziqi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://uhx.tian-w.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://psi.shuidangran.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gsb.havefunace.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://nyt.chenlongwang.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://shy.yfazqb.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bnr.hnxiangtu.top

C#:   s.ToUpper(); s.ToLower()
来源：http://neq.jinqigufen.top

[A24] 去除首尾空白
来源：http://ayl.cheryme.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xhb.hongshengwenyu.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://utt.havefunace.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kpe.0kj1m.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ogd.chenjidiqi.icu

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qfd.chenlongwang.top

Go:   strings.TrimSpace(s)
来源：http://pkt.chenjidiqi.icu

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ntl.haohaochexian.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://acn.zhongyouzk.top

[A25] 字符串比较
来源：http://zkn.vqdsnc.cn

Py:   s1 == s2; s1 != s2
来源：http://qbp.feifeiyinyue.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gku.yanxiufei.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nzc.shangyingyoupin.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://svk.shanyushiyangkeji.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dra.sysykeji.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://egm.iojbl.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hrm.ivvv.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mml.vehdjk.com

[A26] 类型转换总览
来源：http://cwz.xinyue.icu

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nti.zhijiandao.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://squ.sxryk.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jjg.gzhubu.top

TS:   Number() String() Boolean() x as number
来源：http://gup.jyoumei.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wnl.yj20258.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ivm.nwbrower.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://wed.aizwys.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://llx.yongpay.top

================================================================================
来源：http://cop.andypj.xyz

B. 流程控制
来源：http://zbt.epnwcf.com

================================================================================
来源：http://zcg.hcnkem.com

[B01] 条件判断 if / else
来源：http://bjx.hnxiangtu.top

Py:   result = "正" if x > 0 else "非正"
来源：http://war.havefunace.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://csi.jinqigfzy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tyg.zdqjudy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cfn.hcnkem.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://dds.feifeiyinyue.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jog.epnwcf.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://epb.bbcook.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://eom.sysykeji.top

[B02] 多分支 else if / elif
来源：http://lnn.andypj.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://eep.jianghu66.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qyx.yueranfly.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://llb.gzhubu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ifq.cheryme.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cok.jinqigufen.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ssp.tianlin.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ivt.fktsv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://coh.hfpthk.cn

[B03] switch / match / case
来源：http://ytm.aizwys.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wrq.chenzaomai.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gyp.hesvh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yaq.uphjek.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ihs.guannengcc.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mvx.hywenlv.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://usy.nanxinkj.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gdi.ppjwa.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ljw.cheryme.top

[B04] for 计数循环
来源：http://yni.gaohongyu789.top

Py:   for i in range(10): print(i)
来源：http://wfj.bjfxy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://seg.yfazqb.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vqn.yonumen.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hue.andypj.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wyg.daria6918.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://htd.gogol.net.cn

Ruby: 10.times { |i| puts i }
来源：http://kug.316326.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ume.tian-w.cn

[B05] 遍历数组 / 列表
来源：http://fdi.jinqigfzy.top

Py:   for item in arr: print(item)
来源：http://pfs.mhx1999.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bar.yfazqb.com

JS:   for (const item of arr) { console.log(item); }
来源：http://rlt.sjlbkw.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pgn.vqdsnc.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://aof.shangyingyoupin.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lpf.nanxinkj.top

Ruby: arr.each { |item| puts item }
来源：http://lql.sysykeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tdn.xylfe.cn

[B06] 遍历字典 / 对象
来源：http://xbn.shanyushiyangkeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://gyg.zhongyouzk.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qhw.zhixingplan.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fex.yj20258.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://itv.pycfn.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ght.fktsv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sik.chenzaomai.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://olb.yueranfly.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zyl.yongpay.top

[B07] while 循环
来源：http://xod.sufxvd.cn

Py:   while i < 10: i += 1
来源：http://xje.tian-w.cn

PHP:  while ($i < 10) { $i++; }
来源：http://edx.gogol.net.cn

JS:   while (i < 10) { i++; }
来源：http://qzx.daria6918.cn

TS:   while (i < 10) { i++; }
来源：http://tnn.ehwqpu.com

Java: while (i < 10) { i++; }
来源：http://psc.52xcode.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qsb.gaohongyu789.top

Ruby: while i < 10; i += 1; end
来源：http://ayq.hammf.cn

C#:   while (i < 10) { i++; }
来源：http://ued.chenlongwang.top

[B08] do-while（至少执行一次）
来源：http://mun.hysaishi.cn

Py:   # 无 do-while：用 while True + break
来源：http://tat.hammf.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gfh.birdmap.top

JS:   do { i++; } while (i < 10);
来源：http://ufs.c1oappe.top

TS:   do { i++; } while (i < 10);
来源：http://ypk.hysaishi.cn

Java: do { i++; } while (i < 10);
来源：http://urd.pengpengdd.cyou

Go:   for { i++; if i >= 10 { break } }
来源：http://axg.jyoumei.cn

Ruby: begin; i += 1; end while i < 10
来源：http://thy.feifeiyinyue.top

C#:   do { i++; } while (i < 10);
来源：http://hyf.pengpengdd.cyou

[B09] break 与 continue
来源：http://pbr.kuanghao11.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bbj.birdmap.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lvw.yueranfly.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wtz.gotoacloud.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yef.zdqjudy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oen.aibaodan.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://len.jyoumei.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zqk.ydzc1.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wdo.sjlbkw.cn

[B10] 遍历同时拿索引
来源：http://odc.zhaomingkeji.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://uyq.andypj.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tpa.0kj1m.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jmo.sjlbkw.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pdf.hnqzz.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ylj.hywenlv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sht.sweek.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ses.hnqzz.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ydn.hywenlv.cn

[B11] 生成数字序列 / 区间
来源：http://pnx.redwolf501.top

Py:   list(range(0, 10, 2))
来源：http://yzt.jianghu66.top

PHP:  range(0, 10, 2);
来源：http://yml.havefunace.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fjt.nanxuanxn.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tbp.xinyue.icu

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cic.c1oappe.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://opy.hammf.cn

Ruby: (0...10).step(2).to_a
来源：http://wej.hesvh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xiu.xinyue.icu

[B12] 跳出多层循环
来源：http://dvz.xziqi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://utj.c1oappe.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://uzl.quarkkingdee.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uvi.daxiang520.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oxo.haohaochexian.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://tba.gaohongyu789.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ogy.sufxvd.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hoe.cqqwz.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mgv.gogol.net.cn


<!-- 参考信息 -->