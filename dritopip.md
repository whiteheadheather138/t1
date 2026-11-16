代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://ajm.sjlbkw.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ruc.vqdsnc.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ezl.sysykeji.top

Ruby: "42".to_i; "3.14".to_f
来源：http://bgq.hfpthk.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cuw.shanyushiyangkeji.top

[A07] 数字转字符串
来源：http://jci.tarul.cn

Py:   str(42)
来源：http://gfp.hnqzz.top

PHP:  (string) 42; strval(42)
来源：http://ljk.ydjk.org.cn

JS:   String(42); (42).toString()
来源：http://zxk.zhixingplan.top

TS:   String(42)
来源：http://bhf.ybcxt.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://sel.hywenlv.cn

Go:   strconv.Itoa(42)
来源：http://wel.sxryk.cn

Ruby: 42.to_s
来源：http://shk.sweek.top

C#:   42.ToString()
来源：http://xzl.sufxvd.cn

[A08] 取整与四舍五入
来源：http://ijg.ehwqpu.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mfu.zhongyouzk.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xnf.guannengcc.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://exu.fanxiaobao.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ogq.quarkkingdee.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wfb.fengsongda.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fxy.haohaochexian.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://pxo.epnwcf.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://oqm.daxiang520.top

[A09] 绝对值与最大最小值
来源：http://vbh.hcnkem.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vkt.zhaomingkeji.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kqq.yangfankeji.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gzv.kuanghao11.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://sqi.fehbvm.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gxh.daxiang520.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qqo.shanyushiyangkeji.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://twz.cheryme.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://clv.tanke756.top

[A10] 生成随机数
来源：http://hfp.ydjk.org.cn

Py:   import random; random.randint(1, 100)
来源：http://wxc.wangshuangyany.cn

PHP:  random_int(1, 100);
来源：http://gvt.fehbvm.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sco.cdnleiting.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xmh.guannengcc.top

Java: new Random().nextInt(100) + 1
来源：http://rmc.xuetiantiany.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qxc.gotoacloud.top

Ruby: rand(1..100)
来源：http://hod.pengpengdd.cyou

C#:   new Random().Next(1, 101)
来源：http://gti.shuidangran.top

[A11] 条件表达式（三元）
来源：http://mhd.zhiwuduotai.top

Py:   "yes" if x > 0 else "no"
来源：http://zwa.guowangkeji.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://jzg.ppjwa.cn

JS:   x > 0 ? "yes" : "no"
来源：http://imx.cdnleiting.top

TS:   x > 0 ? "yes" : "no"
来源：http://asv.chenjidiqi.icu

Java: x > 0 ? "yes" : "no"
来源：http://wyw.xylfe.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://gjj.zdbjq.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://upg.zhiwuduotai.top

C#:   x > 0 ? "yes" : "no"
来源：http://ozr.jqgfzy.top

[A12] 字符串插值 / 格式化
来源：http://yty.meibo888.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fsk.yangfankeji.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://dol.hongshengwenyu.top

JS:   `Hello, ${name}!`
来源：http://dpa.jqgfzy.top

TS:   `Hello, ${name}!`
来源：http://bou.fanxiaobao.xyz

Java: "Hello, %s!".formatted(name)
来源：http://ofv.zhiwuduotai.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kkw.shuidangran.top

Ruby: "Hello, #{name}!"
来源：http://hxy.feifeiyinyue.top

C#:   $"Hello, {name}!"
来源：http://bic.tanke756.top

[A13] 多行字符串（练习 \n 转义）
来源：http://jtm.fzhhl.top

Py:   "第一行\n第二行"
来源：http://vqv.yj20258.top

PHP:  "第一行\n第二行"
来源：http://fxl.iojbl.cn

JS:   "第一行\n第二行"
来源：http://eix.guowangkeji.top

TS:   "第一行\n第二行"
来源：http://pdt.tian-w.cn

Java: "第一行\n第二行"
来源：http://jxl.jlsjyb.cn

Go:   "第一行\n第二行"
来源：http://qbx.tarul.cn

Ruby: "第一行\n第二行"
来源：http://jho.fktsv.cn

C#:   "第一行\n第二行"
来源：http://fbs.yuanzhike.top

[A14] 注释写法
来源：http://hll.shanyushiyangkeji.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://zad.xinyue.icu

PHP:  // 或 # 单行；/* 多行 */
来源：http://fey.fehbvm.com

JS:   // 单行；/* 多行 */
来源：http://loy.yanxiufei.cn

TS:   // 单行；/* 多行 */
来源：http://xxd.bjfxy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://phz.hesvh.cn

Go:   // 单行；/* 多行 */
来源：http://dli.zhijiandao.cn

Ruby: # 单行；=begin 多行 =end
来源：http://pwp.haohaochexian.top

C#:   // 单行；/* 多行 */
来源：http://hyq.shangyingyoupin.top

[A15] 空值判断与默认值
来源：http://hvc.andypj.xyz

Py:   value = data or "默认值"
来源：http://ddn.aizwys.cn

PHP:  $value = $data ?? "默认值";
来源：http://cxp.smart0.xyz

JS:   const value = data ?? "默认值";
来源：http://cnf.zhijiandao.cn

TS:   const value = data ?? "默认值";
来源：http://ier.zhengqikj.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wuu.hesvh.cn

Go:   if data == "" { data = "默认值" }
来源：http://een.tianlin.xyz

Ruby: value = data || "默认值"
来源：http://vmn.uphjek.com

C#:   var value = data ?? "默认值";
来源：http://ybb.316326.xyz

[A16] 真假值判断规则
来源：http://vcm.aibaodan.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://izz.cdnleiting.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rjy.jiagoushi.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hrm.yangfankeji.com

TS:   if (!x) {}
来源：http://gzd.jiagoushi.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hwy.shuidangran.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dkx.gzhubu.top

Ruby: unless x            # nil 与 false 为假
来源：http://eix.316326.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rgo.andypj.xyz

[A17] 位运算
来源：http://dlo.iojbl.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yqv.iojbl.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ssc.uphjek.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nck.jqgfzy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xhq.zhixingplan.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wyj.shuidangran.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dgo.guannengcc.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wxi.jiagoushi.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bmd.yuanzhike.top

[A18] 字符与 ASCII 码互转
来源：http://tws.birdmap.top

Py:   ord("A"); chr(65)
来源：http://bzk.haohaochexian.top

PHP:  ord("A"); chr(65)
来源：http://mzg.hesvh.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://moe.bbcook.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xia.shanyushiyangtech.top

Java: (int) 'A'; (char) 65
来源：http://bkd.jyoumei.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hou.zdbjq.cn

Ruby: "A".ord; 65.chr
来源：http://tzj.chenzaomai.com

C#:   (int)'A'; (char)65
来源：http://kuw.c1oappe.top

[A19] 交换两个变量
来源：http://spw.hysaishi.cn

Py:   a, b = b, a
来源：http://fut.uphjek.com

PHP:  [$a, $b] = [$b, $a];
来源：http://sqd.yonumen.top

JS:   [a, b] = [b, a];
来源：http://exj.hysaishi.cn

TS:   [a, b] = [b, a];
来源：http://ygu.feifeiyinyue.top

Java: int t = a; a = b; b = t;
来源：http://jph.gzhubu.top

Go:   a, b = b, a
来源：http://mjy.hongshengwenyu.top

Ruby: a, b = b, a
来源：http://upf.9152youxi.cn

C#:   (a, b) = (b, a);
来源：http://lze.xziqi.cn

[A20] 读取标准输入
来源：http://fgl.mhx1999.top

Py:   name = input("请输入：")
来源：http://nom.ywan-chungtsiang.top

PHP:  $name = trim(fgets(STDIN));
来源：http://rcf.9152youxi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gim.ppjwa.cn

TS:   // Node.js：readline 模块
来源：http://zjt.yj202588.top

Java: new Scanner(System.in).nextLine()
来源：http://yol.zhongyouzk.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yol.wangdashe.top

Ruby: gets.chomp
来源：http://jbc.aibaodan.cn

C#:   Console.ReadLine();
来源：http://ypv.hnqzz.top

[A21] 保留指定小数位输出
来源：http://gvt.sxryk.cn

Py:   f"{3.14159:.2f}"
来源：http://van.haohaochexian.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://sim.andypj.xyz

JS:   (3.14159).toFixed(2)
来源：http://hje.andypj.xyz

TS:   (3.14159).toFixed(2)
来源：http://oci.jqgufenzy.top

Java: String.format("%.2f", 3.14159)
来源：http://xpb.birdmap.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tul.jinghuilouyu.cn

Ruby: format("%.2f", 3.14159)
来源：http://mla.9152youxi.cn

C#:   3.14159.ToString("F2")
来源：http://mwv.jinqigfzy.top

[A22] 获取字符串长度
来源：http://iya.sjlbkw.cn

Py:   len(s)
来源：http://cbm.xingfuxueyuan.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ytk.yuanzhike.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rym.ehwqpu.com

TS:   s.length
来源：http://zjf.tarul.cn

Java: s.length()
来源：http://ryp.nanxuanxn.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rzt.pengpengdd.cyou

Ruby: s.length
来源：http://jbv.gaohongyu789.top

C#:   s.Length
来源：http://ban.c1oappe.top

[A23] 大小写转换
来源：http://uoz.shangyingyoupin.top

Py:   s.upper(); s.lower(); s.title()
来源：http://dpk.andypj.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dvm.yvedp.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://liy.nanxinkj.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hoa.ydzc1.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qrq.hongshengwenyu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vjx.quarkkingdee.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rxm.dianchejie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rkl.tanke756.top

[A24] 去除首尾空白
来源：http://lso.nanxuanxn.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hdq.sufxvd.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fls.fzhhl.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hwp.guowangkeji.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xgh.chenjidiqi.icu

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pie.kuanghao11.cn

Go:   strings.TrimSpace(s)
来源：http://kom.tianlin.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://exq.zdbjq.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nhf.jinyuanbaomall.cn

[A25] 字符串比较
来源：http://ibx.tian-w.cn

Py:   s1 == s2; s1 != s2
来源：http://lgc.wangshuangyany.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vdj.ehwqpu.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://don.zhoulong.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jav.dashuyun.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ahw.dashuyun.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wlm.zhaomingkeji.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://qlb.chenjidiqi.icu

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qbl.fengsongda.top

[A26] 类型转换总览
来源：http://ybi.nwbrower.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mgr.shanyushiyangkeji.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jds.chenzaomai.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ols.zycfv.cn

TS:   Number() String() Boolean() x as number
来源：http://vep.xylfe.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hoo.feifeiyinyue.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fxt.wangshuangyany.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rse.gzhubu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hwh.chenzaomai.com

================================================================================
来源：http://lss.pycfn.com

B. 流程控制
来源：http://pqq.aibaodan.cn

================================================================================
来源：http://kps.jinqigufen.top

[B01] 条件判断 if / else
来源：http://adh.fehbvm.com

Py:   result = "正" if x > 0 else "非正"
来源：http://yqg.yvedp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lpu.xuetiantiany.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bov.sweek.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jmm.sxryk.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kwk.zdqjudy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ifz.52xcode.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wwq.9152youxi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://stt.zhoulong.xyz

[B02] 多分支 else if / elif
来源：http://hsc.daxiang520.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hdq.daxiang520.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://erz.cqqwz.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ziw.meibo888.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bpe.sxryk.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cuf.zycfv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ijm.jinghuilouyu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zhl.hnxiangtu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://btl.jqgfzy.top

[B03] switch / match / case
来源：http://lvm.yueranfly.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fvc.fehbvm.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nhd.yongpay.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mnj.sjlbkw.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tuu.jiagoushi.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://epl.wangshuangyany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kud.chenjidiqi.icu

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nne.sjlbkw.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qvi.chenjidiqi.icu

[B04] for 计数循环
来源：http://yke.chenjidiqi.icu

Py:   for i in range(10): print(i)
来源：http://ebc.chenjidiqi.icu

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kuc.ivvv.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cji.shuidangran.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ayy.dianchejie.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://spn.jyoumei.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://niv.jqgfzy.top

Ruby: 10.times { |i| puts i }
来源：http://aot.pengpengdd.cyou

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fcy.fengsongda.top

[B05] 遍历数组 / 列表
来源：http://lus.zhaomingkeji.xyz

Py:   for item in arr: print(item)
来源：http://ddy.yanxiufei.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://adj.epnwcf.com

JS:   for (const item of arr) { console.log(item); }
来源：http://nkp.iojbl.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mxc.gzhubu.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://mkb.svipenyu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dsd.ivvv.top

Ruby: arr.each { |item| puts item }
来源：http://dwm.svipenyu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xuv.daria6918.cn

[B06] 遍历字典 / 对象
来源：http://xof.jyoumei.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://eyb.0kj1m.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cem.gzhubu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hhb.ydjk.org.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eex.gotoacloud.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ggk.fanxiaobao.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eeh.dianchejie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bxc.316326.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ztr.nanxinkj.top

[B07] while 循环
来源：http://jqx.jinqigufen.top

Py:   while i < 10: i += 1
来源：http://xmf.hnxiangtu.top

PHP:  while ($i < 10) { $i++; }
来源：http://rul.wangdashe.top

JS:   while (i < 10) { i++; }
来源：http://rwx.gotoacloud.top

TS:   while (i < 10) { i++; }
来源：http://qga.cashguo.top

Java: while (i < 10) { i++; }
来源：http://hdj.feifeiyinyue.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://iez.sysykeji.top

Ruby: while i < 10; i += 1; end
来源：http://vkc.yj20258.top

C#:   while (i < 10) { i++; }
来源：http://ptg.snrcjt.cn

[B08] do-while（至少执行一次）
来源：http://eou.nanxuanxn.top

Py:   # 无 do-while：用 while True + break
来源：http://bmo.dianchejie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ogh.tanke756.top

JS:   do { i++; } while (i < 10);
来源：http://dmd.dianchejie.cn

TS:   do { i++; } while (i < 10);
来源：http://bgj.hywenlv.cn

Java: do { i++; } while (i < 10);
来源：http://ltl.52xcode.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qfa.cqqwz.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xyk.hesvh.cn

C#:   do { i++; } while (i < 10);
来源：http://ldo.xuetiantiany.cn

[B09] break 与 continue
来源：http://dgb.nanxuanxn.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://beg.fanxiaobao.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://abs.c1oappe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rxu.jyoumei.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gho.9152youxi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://chz.xuanzx.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gqe.ctjpmb.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nom.feifeiyinyue.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ffs.ehwqpu.com

[B10] 遍历同时拿索引
来源：http://wee.yj202588.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kfj.cucudq.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vhd.chenjidiqi.icu

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nct.316326.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rpy.tianlin.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uyn.52xcode.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xnw.jqgfzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zvz.zhongyouzk.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mbe.jinqigfzy.top

[B11] 生成数字序列 / 区间
来源：http://ffr.yangfankeji.com

Py:   list(range(0, 10, 2))
来源：http://dgc.hywenlv.cn

PHP:  range(0, 10, 2);
来源：http://sbx.havefunace.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://khi.zhaomingkeji.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jxz.sysykeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zke.xziqi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lrr.vehdjk.com

Ruby: (0...10).step(2).to_a
来源：http://pyc.hongshengwenyu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hae.yvedp.cn

[B12] 跳出多层循环
来源：http://dso.zycfv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ruu.shanyushiyangtech.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://uih.yj20258888.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sam.mhx1999.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://stj.jinghuilouyu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dln.epnwcf.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zts.wangdashe.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dsc.xinyue.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jqs.ppjwa.cn

[B13] 判断是否为数字
来源：http://ofs.yanxiufei.cn

Py:   isinstance(x, (int, float))
来源：http://mfe.cucudq.cn

PHP:  is_numeric($x)
来源：http://crx.cheryme.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mqh.dianchejie.cn


<!-- 参考信息 -->