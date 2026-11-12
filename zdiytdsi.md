代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://qpk.sxryk.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hku.iojbl.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fve.yj20258888.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ltd.9152youxi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ldq.yanxiufei.cn

[A07] 数字转字符串
来源：http://emm.zhaomingkeji.xyz

Py:   str(42)
来源：http://bxf.vqdsnc.cn

PHP:  (string) 42; strval(42)
来源：http://urx.yangfankeji.com

JS:   String(42); (42).toString()
来源：http://pab.fzhhl.top

TS:   String(42)
来源：http://lrq.ydjk.org.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://tcr.fanxiaobao.xyz

Go:   strconv.Itoa(42)
来源：http://xcm.shanyushiyangtech.top

Ruby: 42.to_s
来源：http://ulh.dianchejie.cn

C#:   42.ToString()
来源：http://kof.zhaomingkeji.xyz

[A08] 取整与四舍五入
来源：http://cta.ybcxt.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://loa.snrcjt.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://woq.jinqigfzy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://trq.birdmap.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qae.nwbrower.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hyr.svipenyu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qug.mhx1999.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://imv.shanyushiyangtech.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wml.0kj1m.cn

[A09] 绝对值与最大最小值
来源：http://sff.feifeiyinyue.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kbs.zhiwuduotai.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ier.316326.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pfq.aibaodan.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gzh.ybcxt.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://egr.gaohongyu789.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://way.fengsongda.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pts.ivvv.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://aes.jlsjyb.cn

[A10] 生成随机数
来源：http://rcj.yanxiufei.cn

Py:   import random; random.randint(1, 100)
来源：http://dnl.iojbl.cn

PHP:  random_int(1, 100);
来源：http://mkd.zhaomingkeji.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://thj.wangdashe.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jwn.c1oappe.top

Java: new Random().nextInt(100) + 1
来源：http://yvu.zhijiandao.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tyo.cheryme.top

Ruby: rand(1..100)
来源：http://hca.birdmap.top

C#:   new Random().Next(1, 101)
来源：http://gxt.feifeiyinyue.top

[A11] 条件表达式（三元）
来源：http://tkr.iojbl.cn

Py:   "yes" if x > 0 else "no"
来源：http://beu.kuanghao11.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rwh.hnxiangtu.top

JS:   x > 0 ? "yes" : "no"
来源：http://yrk.yongpay.top

TS:   x > 0 ? "yes" : "no"
来源：http://kza.cashguo.top

Java: x > 0 ? "yes" : "no"
来源：http://kaf.birdmap.top

Go:   // 无三元运算符，需用 if 语句
来源：http://qtg.ywan-chungtsiang.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ksb.hfpthk.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ami.cdnleiting.top

[A12] 字符串插值 / 格式化
来源：http://dxg.aibaodan.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hmc.yanxiufei.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xhb.zhengqikj.top

JS:   `Hello, ${name}!`
来源：http://iob.shanyushiyangtech.top

TS:   `Hello, ${name}!`
来源：http://byd.nanxuanxn.top

Java: "Hello, %s!".formatted(name)
来源：http://nmy.shzxlz.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://uxr.yueranfly.top

Ruby: "Hello, #{name}!"
来源：http://wzu.sxryk.cn

C#:   $"Hello, {name}!"
来源：http://xhy.zhoulong.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://fcd.zdqjudy.top

Py:   "第一行\n第二行"
来源：http://nzi.xziqi.cn

PHP:  "第一行\n第二行"
来源：http://idd.yj202588.top

JS:   "第一行\n第二行"
来源：http://hej.chenjidiqi.icu

TS:   "第一行\n第二行"
来源：http://ooo.fzhhl.top

Java: "第一行\n第二行"
来源：http://och.yanxiufei.cn

Go:   "第一行\n第二行"
来源：http://psi.meibo888.top

Ruby: "第一行\n第二行"
来源：http://vyy.yongpay.top

C#:   "第一行\n第二行"
来源：http://xjh.xuanzx.com

[A14] 注释写法
来源：http://zcs.hesvh.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://hxx.52xcode.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://zfr.ywan-chungtsiang.top

JS:   // 单行；/* 多行 */
来源：http://tdo.nanxuanxn.top

TS:   // 单行；/* 多行 */
来源：http://nrr.cheryme.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fgo.sysykeji.top

Go:   // 单行；/* 多行 */
来源：http://bnr.pengpengdd.cyou

Ruby: # 单行；=begin 多行 =end
来源：http://our.xingfuxueyuan.xyz

C#:   // 单行；/* 多行 */
来源：http://fqt.yangfankeji.com

[A15] 空值判断与默认值
来源：http://njc.fktsv.cn

Py:   value = data or "默认值"
来源：http://yri.pycfn.com

PHP:  $value = $data ?? "默认值";
来源：http://aeb.jqgufenzy.top

JS:   const value = data ?? "默认值";
来源：http://uyj.wangshuangyany.cn

TS:   const value = data ?? "默认值";
来源：http://nnn.fengsongda.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kpx.xingfuxueyuan.xyz

Go:   if data == "" { data = "默认值" }
来源：http://kah.tarul.cn

Ruby: value = data || "默认值"
来源：http://qqy.jqgfzy.top

C#:   var value = data ?? "默认值";
来源：http://kja.316326.xyz

[A16] 真假值判断规则
来源：http://bwo.vehdjk.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://txh.uphjek.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ybx.jyoumei.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ihj.uphjek.com

TS:   if (!x) {}
来源：http://zrw.aibaodan.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jal.shanyushiyangtech.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rjh.jlsjyb.cn

Ruby: unless x            # nil 与 false 为假
来源：http://tpr.haohaochexian.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://owu.tarul.cn

[A17] 位运算
来源：http://lva.jinghuilouyu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zfr.vehdjk.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xsg.kuanghao11.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vav.c1oappe.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cre.c1oappe.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ikg.zhongyouzk.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kcn.tarul.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lsy.chenzaomai.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nia.smart0.xyz

[A18] 字符与 ASCII 码互转
来源：http://qfz.yj202588.top

Py:   ord("A"); chr(65)
来源：http://qcd.jinyuanbaomall.cn

PHP:  ord("A"); chr(65)
来源：http://wxd.dashuyun.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ohv.bjfxy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://isg.hnqzz.top

Java: (int) 'A'; (char) 65
来源：http://fjg.chenzaomai.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jyk.hnqzz.top

Ruby: "A".ord; 65.chr
来源：http://lnc.xuetiantiany.cn

C#:   (int)'A'; (char)65
来源：http://pvl.gaohongyu789.top

[A19] 交换两个变量
来源：http://vfh.sjlbkw.cn

Py:   a, b = b, a
来源：http://rtq.aibaodan.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jry.zhengqikj.top

JS:   [a, b] = [b, a];
来源：http://xol.uphjek.com

TS:   [a, b] = [b, a];
来源：http://deu.fktsv.cn

Java: int t = a; a = b; b = t;
来源：http://bzv.uphjek.com

Go:   a, b = b, a
来源：http://jup.nwbrower.top

Ruby: a, b = b, a
来源：http://pao.tarul.cn

C#:   (a, b) = (b, a);
来源：http://diu.zycfv.cn

[A20] 读取标准输入
来源：http://zje.yj20258888.top

Py:   name = input("请输入：")
来源：http://vbc.xinyue.icu

PHP:  $name = trim(fgets(STDIN));
来源：http://brr.smart0.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ghk.yueranfly.top

TS:   // Node.js：readline 模块
来源：http://vwo.pengpengdd.cyou

Java: new Scanner(System.in).nextLine()
来源：http://kks.xinyue.icu

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://crl.hywenlv.cn

Ruby: gets.chomp
来源：http://rlh.sysykeji.top

C#:   Console.ReadLine();
来源：http://oti.ivvv.top

[A21] 保留指定小数位输出
来源：http://cxu.sweek.top

Py:   f"{3.14159:.2f}"
来源：http://uax.jiagoushi.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://suq.smart0.xyz

JS:   (3.14159).toFixed(2)
来源：http://izf.cheryme.top

TS:   (3.14159).toFixed(2)
来源：http://elh.andypj.xyz

Java: String.format("%.2f", 3.14159)
来源：http://wkk.ivvv.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fml.ctjpmb.com

Ruby: format("%.2f", 3.14159)
来源：http://tzy.hfpthk.cn

C#:   3.14159.ToString("F2")
来源：http://ior.jlsjyb.cn

[A22] 获取字符串长度
来源：http://hhl.dashuyun.cn

Py:   len(s)
来源：http://jbq.gotoacloud.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bfq.fktsv.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xfq.gotoacloud.top

TS:   s.length
来源：http://ksb.iojbl.cn

Java: s.length()
来源：http://vob.xziqi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bgs.fktsv.cn

Ruby: s.length
来源：http://jxc.ywan-chungtsiang.top

C#:   s.Length
来源：http://lld.xuetiantiany.cn

[A23] 大小写转换
来源：http://akw.yvedp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fqj.svipenyu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ofw.gaohongyu789.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xye.yuxming.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://oig.nwbrower.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kls.ppjwa.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ngs.daria6918.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vqq.bjfxy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://vrq.shzxlz.cn

[A24] 去除首尾空白
来源：http://gob.cucudq.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vjv.nanxinkj.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://msc.9152youxi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://shi.chenlongwang.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fld.ydjk.org.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qoe.hcnkem.com

Go:   strings.TrimSpace(s)
来源：http://afm.sweek.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uya.hammf.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://brx.xuanzx.com

[A25] 字符串比较
来源：http://ush.chenjidiqi.icu

Py:   s1 == s2; s1 != s2
来源：http://guo.snrcjt.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xdf.jyoumei.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://icd.gzhubu.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ebx.jlsjyb.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tol.0kj1m.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xeg.hfpthk.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pug.xingfuxueyuan.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rkw.chenlongwang.top

[A26] 类型转换总览
来源：http://mok.zhixingplan.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ppk.fzhhl.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lht.shanyushiyangtech.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ptv.52xcode.cn

TS:   Number() String() Boolean() x as number
来源：http://rnu.yfazqb.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pzu.jiagoushi.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cqy.yangfankeji.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://pnt.ybcxt.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sti.jqgufenzy.top

================================================================================
来源：http://xaw.tianlin.xyz

B. 流程控制
来源：http://hdk.0kj1m.cn

================================================================================
来源：http://tzs.jqgfzy.top

[B01] 条件判断 if / else
来源：http://oxd.ivvv.top

Py:   result = "正" if x > 0 else "非正"
来源：http://mrq.jianghu66.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yei.jyoumei.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qyw.tianlin.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cwd.tanke756.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://shv.jinqigufen.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://otn.hongshengwenyu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ucg.xingfuxueyuan.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pmr.yvedp.cn

[B02] 多分支 else if / elif
来源：http://gfp.guannengcc.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dtj.gaohongyu789.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nhk.316326.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xig.hongshengwenyu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://som.cdnleiting.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oty.jyoumei.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lfu.jyoumei.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nsv.hysaishi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jgj.hongshengwenyu.top

[B03] switch / match / case
来源：http://kld.nwbrower.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tdy.wangshuangyany.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jwp.wangdashe.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eax.shangyingyoupin.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rtm.shanyushiyangtech.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://otw.gzhubu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jiq.sysykeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://eca.quarkkingdee.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://oyk.bbcook.cn

[B04] for 计数循环
来源：http://oxn.aizwys.cn

Py:   for i in range(10): print(i)
来源：http://uit.vqdsnc.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hni.jinyuanbaomall.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fvx.yj20258.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rhw.jqgfzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cyv.pycfn.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jdh.hnxiangtu.top

Ruby: 10.times { |i| puts i }
来源：http://jok.jqgufenzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gua.0kj1m.cn

[B05] 遍历数组 / 列表
来源：http://qpg.havefunace.top

Py:   for item in arr: print(item)
来源：http://rlb.chenzaomai.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://feg.zhijiandao.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://gdr.chenzaomai.com

TS:   for (const item of arr) { console.log(item); }
来源：http://wrw.aizwys.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ejl.jiagoushi.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rgz.meibo888.top

Ruby: arr.each { |item| puts item }
来源：http://yet.uphjek.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zdi.quarkkingdee.top

[B06] 遍历字典 / 对象
来源：http://ihf.shanyushiyangkeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://oha.sysykeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dti.zhongyouzk.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ypj.daria6918.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xaq.dianchejie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://url.zhixingplan.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uep.zhiwuduotai.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tyh.sysykeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bky.sysykeji.top

[B07] while 循环
来源：http://iof.xuetiantiany.cn

Py:   while i < 10: i += 1
来源：http://srb.iojbl.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ity.dianchejie.cn

JS:   while (i < 10) { i++; }
来源：http://gmh.jqgufenzy.top

TS:   while (i < 10) { i++; }
来源：http://cfm.shanyushiyangtech.top

Java: while (i < 10) { i++; }
来源：http://mjw.fanxiaobao.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sak.chenlongwang.top

Ruby: while i < 10; i += 1; end
来源：http://dvh.52xcode.cn

C#:   while (i < 10) { i++; }
来源：http://urn.xuetiantiany.cn

[B08] do-while（至少执行一次）
来源：http://qap.iojbl.cn

Py:   # 无 do-while：用 while True + break
来源：http://zrf.cucudq.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dja.ppjwa.cn

JS:   do { i++; } while (i < 10);
来源：http://bdw.ehwqpu.com

TS:   do { i++; } while (i < 10);
来源：http://mps.aizwys.cn

Java: do { i++; } while (i < 10);
来源：http://cmz.guowangkeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://yii.hnqzz.top

Ruby: begin; i += 1; end while i < 10
来源：http://ran.jqgufenzy.top

C#:   do { i++; } while (i < 10);
来源：http://gnm.zhongyouzk.top

[B09] break 与 continue
来源：http://nix.andypj.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yjg.svipenyu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://aql.ivvv.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aoy.xylfe.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://afs.haohaochexian.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://exj.yuxming.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sjb.cucudq.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://npm.jinyuanbaomall.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zwy.guannengcc.top

[B10] 遍历同时拿索引
来源：http://mun.yanxiufei.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://aqr.sysykeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bpv.yuanzhike.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ijr.zdqjudy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gmk.yongpay.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://anc.fktsv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nut.sxryk.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yjd.feifeiyinyue.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bjj.tanke756.top

[B11] 生成数字序列 / 区间
来源：http://wmp.smart0.xyz

Py:   list(range(0, 10, 2))
来源：http://qth.sxryk.cn

PHP:  range(0, 10, 2);
来源：http://zlj.hfpthk.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bjd.hesvh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ial.zycfv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ksx.yongpay.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ebh.cdnleiting.top

Ruby: (0...10).step(2).to_a
来源：http://vki.c1oappe.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tsp.hfpthk.cn

[B12] 跳出多层循环
来源：http://hdh.gogol.net.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pyk.pengpengdd.cyou

PHP:  # 无标签：用 goto 或函数返回
来源：http://taf.tarul.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qcm.yuxming.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mqf.nanxinkj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zdc.bjfxy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://aee.daxiang520.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mew.andypj.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://umn.vqdsnc.cn

[B13] 判断是否为数字
来源：http://efc.chenzaomai.com

Py:   isinstance(x, (int, float))
来源：http://quu.iojbl.cn

PHP:  is_numeric($x)
来源：http://wir.ybcxt.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qlf.shanyushiyangkeji.top


<!-- 参考信息 -->