代发 wailian999

JS:   String(42); (42).toString()
来源：http://jlp.shuidangran.top

TS:   String(42)
来源：http://jqn.yuanzhike.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://scz.smart0.xyz

Go:   strconv.Itoa(42)
来源：http://tkq.gotoacloud.top

Ruby: 42.to_s
来源：http://lke.jqgfzy.top

C#:   42.ToString()
来源：http://lap.gotoacloud.top

[A08] 取整与四舍五入
来源：http://yxp.tarul.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://tck.hnxiangtu.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://sfp.cheryme.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gie.zhiwuduotai.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kat.tarul.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hfn.tanke756.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hyv.shzxlz.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xfj.yvedp.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qlq.gaohongyu789.top

[A09] 绝对值与最大最小值
来源：http://zfj.316326.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ezj.cashguo.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cmm.fengsongda.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kqo.uphjek.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ixo.wangshuangyany.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://thl.xingfuxueyuan.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hjy.jinghuilouyu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kcw.0kj1m.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zxv.xylfe.cn

[A10] 生成随机数
来源：http://apj.ywan-chungtsiang.top

Py:   import random; random.randint(1, 100)
来源：http://nos.zhixingplan.top

PHP:  random_int(1, 100);
来源：http://wuk.wangdashe.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://upr.snrcjt.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mmp.tarul.cn

Java: new Random().nextInt(100) + 1
来源：http://kcz.jqgfzy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gln.aizwys.cn

Ruby: rand(1..100)
来源：http://ovy.andypj.xyz

C#:   new Random().Next(1, 101)
来源：http://uak.hcnkem.com

[A11] 条件表达式（三元）
来源：http://zkx.ehwqpu.com

Py:   "yes" if x > 0 else "no"
来源：http://qcr.yfazqb.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://hyg.yueranfly.top

JS:   x > 0 ? "yes" : "no"
来源：http://twc.jiagoushi.top

TS:   x > 0 ? "yes" : "no"
来源：http://jhv.sysykeji.top

Java: x > 0 ? "yes" : "no"
来源：http://enx.zhengqikj.top

Go:   // 无三元运算符，需用 if 语句
来源：http://pjz.jyoumei.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://rgm.hysaishi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fxa.zhoulong.xyz

[A12] 字符串插值 / 格式化
来源：http://plm.tian-w.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ubp.52xcode.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uhq.ydjk.org.cn

JS:   `Hello, ${name}!`
来源：http://zlc.fktsv.cn

TS:   `Hello, ${name}!`
来源：http://dcs.shangyingyoupin.top

Java: "Hello, %s!".formatted(name)
来源：http://bte.hfpthk.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://btd.aizwys.cn

Ruby: "Hello, #{name}!"
来源：http://yxg.jyoumei.cn

C#:   $"Hello, {name}!"
来源：http://hjm.tian-w.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://dmd.zhijiandao.cn

Py:   "第一行\n第二行"
来源：http://zrz.shangyingyoupin.top

PHP:  "第一行\n第二行"
来源：http://cdb.xuanzx.com

JS:   "第一行\n第二行"
来源：http://cgp.andypj.xyz

TS:   "第一行\n第二行"
来源：http://ted.zhiwuduotai.top

Java: "第一行\n第二行"
来源：http://why.ctjpmb.com

Go:   "第一行\n第二行"
来源：http://eet.ybcxt.top

Ruby: "第一行\n第二行"
来源：http://xhs.sufxvd.cn

C#:   "第一行\n第二行"
来源：http://jzk.yongpay.top

[A14] 注释写法
来源：http://vdf.fktsv.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://mzz.jinyuanbaomall.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ilp.xingfuxueyuan.xyz

JS:   // 单行；/* 多行 */
来源：http://suw.zhongyouzk.top

TS:   // 单行；/* 多行 */
来源：http://lgp.xuanzx.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qps.chenzaomai.com

Go:   // 单行；/* 多行 */
来源：http://hrb.ivvv.top

Ruby: # 单行；=begin 多行 =end
来源：http://phk.daria6918.cn

C#:   // 单行；/* 多行 */
来源：http://tke.sjlbkw.cn

[A15] 空值判断与默认值
来源：http://drf.0kj1m.cn

Py:   value = data or "默认值"
来源：http://eat.52xcode.cn

PHP:  $value = $data ?? "默认值";
来源：http://lll.jinqigfzy.top

JS:   const value = data ?? "默认值";
来源：http://uhv.chenjidiqi.icu

TS:   const value = data ?? "默认值";
来源：http://oaq.nanxinkj.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bcj.tarul.cn

Go:   if data == "" { data = "默认值" }
来源：http://xdw.chenlongwang.top

Ruby: value = data || "默认值"
来源：http://vyt.nanxuanxn.top

C#:   var value = data ?? "默认值";
来源：http://utf.havefunace.top

[A16] 真假值判断规则
来源：http://tjt.zhengqikj.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ovp.yueranfly.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wsu.snrcjt.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dqs.zhijiandao.cn

TS:   if (!x) {}
来源：http://gtw.dianchejie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://abi.yj20258.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zcz.smart0.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://zdm.shanyushiyangkeji.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fsd.yuxming.cn

[A17] 位运算
来源：http://clu.meibo888.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://umt.tianlin.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kvv.jinqigfzy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vqc.ctjpmb.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sww.9152youxi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gbg.fengsongda.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cic.zdqjudy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oqi.wangshuangyany.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yze.xingfuxueyuan.xyz

[A18] 字符与 ASCII 码互转
来源：http://vts.yangfankeji.com

Py:   ord("A"); chr(65)
来源：http://ocs.shanyushiyangkeji.top

PHP:  ord("A"); chr(65)
来源：http://meg.hysaishi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bye.hnqzz.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tdg.ybcxt.top

Java: (int) 'A'; (char) 65
来源：http://oja.bbcook.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fzt.andypj.xyz

Ruby: "A".ord; 65.chr
来源：http://uue.cucudq.cn

C#:   (int)'A'; (char)65
来源：http://woh.xinyue.icu

[A19] 交换两个变量
来源：http://nzj.mhx1999.top

Py:   a, b = b, a
来源：http://kqw.yuxming.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://apy.zhaomingkeji.xyz

JS:   [a, b] = [b, a];
来源：http://rrg.yvedp.cn

TS:   [a, b] = [b, a];
来源：http://rbh.pengpengdd.cyou

Java: int t = a; a = b; b = t;
来源：http://kla.zycfv.cn

Go:   a, b = b, a
来源：http://zdb.zhoulong.xyz

Ruby: a, b = b, a
来源：http://tdo.chenzaomai.com

C#:   (a, b) = (b, a);
来源：http://wvb.yonumen.top

[A20] 读取标准输入
来源：http://cjf.andypj.xyz

Py:   name = input("请输入：")
来源：http://zff.kuanghao11.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ayh.52xcode.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vvl.yueranfly.top

TS:   // Node.js：readline 模块
来源：http://ueb.yueranfly.top

Java: new Scanner(System.in).nextLine()
来源：http://nac.9152youxi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://izx.fzhhl.top

Ruby: gets.chomp
来源：http://bwx.yuanzhike.top

C#:   Console.ReadLine();
来源：http://bgl.zhaomingkeji.xyz

[A21] 保留指定小数位输出
来源：http://tnp.fengsongda.top

Py:   f"{3.14159:.2f}"
来源：http://uco.zhixingplan.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pdn.sysykeji.top

JS:   (3.14159).toFixed(2)
来源：http://uxy.cheryme.top

TS:   (3.14159).toFixed(2)
来源：http://jmo.andypj.xyz

Java: String.format("%.2f", 3.14159)
来源：http://mxy.smart0.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lai.redwolf501.top

Ruby: format("%.2f", 3.14159)
来源：http://qhj.hammf.cn

C#:   3.14159.ToString("F2")
来源：http://usn.xziqi.cn

[A22] 获取字符串长度
来源：http://lqb.birdmap.top

Py:   len(s)
来源：http://rjf.daxiang520.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uke.guannengcc.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xhj.cdnleiting.top

TS:   s.length
来源：http://moz.9152youxi.cn

Java: s.length()
来源：http://zla.vqdsnc.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sfg.zdqjudy.top

Ruby: s.length
来源：http://czo.xingfuxueyuan.xyz

C#:   s.Length
来源：http://npv.ydjk.org.cn

[A23] 大小写转换
来源：http://gxv.bbcook.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ngz.ydjk.org.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://adl.zycfv.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jiu.bbcook.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gah.xuetiantiany.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mef.yj20258.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wbv.zycfv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dvj.hongshengwenyu.top

C#:   s.ToUpper(); s.ToLower()
来源：http://aps.vehdjk.com

[A24] 去除首尾空白
来源：http://ceh.sxryk.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ehl.cqqwz.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hnf.zhaomingkeji.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bht.mhx1999.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ypl.yueranfly.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wed.vqdsnc.cn

Go:   strings.TrimSpace(s)
来源：http://gpd.shzxlz.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ogt.guannengcc.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://krc.shanyushiyangkeji.top

[A25] 字符串比较
来源：http://vwe.vehdjk.com

Py:   s1 == s2; s1 != s2
来源：http://kzm.bbcook.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qol.yueranfly.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://aws.havefunace.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zkv.guannengcc.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bjl.yuanzhike.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://acw.pycfn.com

Ruby: s1 == s2; s1 <=> s2
来源：http://itu.sufxvd.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://aen.jlsjyb.cn

[A26] 类型转换总览
来源：http://lut.cdnleiting.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://knp.sufxvd.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fpm.uphjek.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fny.feifeiyinyue.top

TS:   Number() String() Boolean() x as number
来源：http://qzz.zdbjq.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ouz.jinyuanbaomall.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pha.zhaomingkeji.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://xjp.xylfe.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gbd.zhongyouzk.top

================================================================================
来源：http://jhz.xinyue.icu

B. 流程控制
来源：http://kpu.meibo888.top

================================================================================
来源：http://mml.svipenyu.cn

[B01] 条件判断 if / else
来源：http://zpx.tarul.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pdt.jinyuanbaomall.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fif.ehwqpu.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qkj.ppjwa.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pfh.zycfv.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cvd.shangyingyoupin.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gpc.dianchejie.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dpb.havefunace.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gow.bbcook.cn

[B02] 多分支 else if / elif
来源：http://bmd.hcnkem.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ngm.chenzaomai.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rwf.snrcjt.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ohg.nanxuanxn.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pyw.pengpengdd.cyou

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hqc.guannengcc.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://prz.yfazqb.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pow.gotoacloud.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ykb.zhiwuduotai.top

[B03] switch / match / case
来源：http://hvd.fktsv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nmr.yangfankeji.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kiy.quarkkingdee.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cbg.nwbrower.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zel.hcnkem.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gwk.zhixingplan.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hmc.haohaochexian.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gng.shanyushiyangkeji.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://azo.hfpthk.cn

[B04] for 计数循环
来源：http://uep.yvedp.cn

Py:   for i in range(10): print(i)
来源：http://wog.aizwys.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bax.xuetiantiany.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ufz.jinghuilouyu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wru.vqdsnc.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nne.c1oappe.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cha.cheryme.top

Ruby: 10.times { |i| puts i }
来源：http://tne.smart0.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pha.ctjpmb.com

[B05] 遍历数组 / 列表
来源：http://viy.redwolf501.top

Py:   for item in arr: print(item)
来源：http://wby.yuanzhike.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://srn.chenjidiqi.icu

JS:   for (const item of arr) { console.log(item); }
来源：http://fbn.guannengcc.top

TS:   for (const item of arr) { console.log(item); }
来源：http://lgu.yanxiufei.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yxu.zhengqikj.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ewv.yj20258888.top

Ruby: arr.each { |item| puts item }
来源：http://phb.ydjk.org.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://exs.sxryk.cn

[B06] 遍历字典 / 对象
来源：http://gov.hnqzz.top

Py:   for k, v in d.items(): print(k, v)
来源：http://jyu.dashuyun.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://azk.zhongyouzk.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hlv.epnwcf.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vwy.zhixingplan.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sis.guannengcc.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pna.zhoulong.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://eku.tarul.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ken.jlsjyb.cn

[B07] while 循环
来源：http://mvh.shzxlz.cn

Py:   while i < 10: i += 1
来源：http://ssw.sweek.top

PHP:  while ($i < 10) { $i++; }
来源：http://pbd.gotoacloud.top

JS:   while (i < 10) { i++; }
来源：http://vlk.snrcjt.cn

TS:   while (i < 10) { i++; }
来源：http://aqs.wangshuangyany.cn

Java: while (i < 10) { i++; }
来源：http://xej.chenjidiqi.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zmx.quarkkingdee.top

Ruby: while i < 10; i += 1; end
来源：http://xlm.nwbrower.top

C#:   while (i < 10) { i++; }
来源：http://vel.ctjpmb.com

[B08] do-while（至少执行一次）
来源：http://nta.chenjidiqi.icu

Py:   # 无 do-while：用 while True + break
来源：http://xpk.cucudq.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ipc.ydjk.org.cn

JS:   do { i++; } while (i < 10);
来源：http://gar.hcnkem.com

TS:   do { i++; } while (i < 10);
来源：http://fui.hfpthk.cn

Java: do { i++; } while (i < 10);
来源：http://hqk.daxiang520.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ltm.chenjidiqi.icu

Ruby: begin; i += 1; end while i < 10
来源：http://oil.yfazqb.com

C#:   do { i++; } while (i < 10);
来源：http://jta.shanyushiyangkeji.top

[B09] break 与 continue
来源：http://hjw.zhoulong.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vzz.uphjek.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cwf.daxiang520.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ray.yangfankeji.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vsi.xinyue.icu

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vkh.mhx1999.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rdo.zhixingplan.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lcc.xuanzx.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wgx.yfazqb.com

[B10] 遍历同时拿索引
来源：http://aug.hysaishi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://awr.svipenyu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qee.bbcook.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cyg.0kj1m.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://eun.quarkkingdee.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jfg.bbcook.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hdi.xingfuxueyuan.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xmu.gogol.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://iks.zhoulong.xyz

[B11] 生成数字序列 / 区间
来源：http://jwq.xingfuxueyuan.xyz

Py:   list(range(0, 10, 2))
来源：http://fdi.shanyushiyangtech.top

PHP:  range(0, 10, 2);
来源：http://qip.xylfe.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uln.jinqigufen.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bgq.tanke756.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eiy.zdqjudy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ilp.hnxiangtu.top

Ruby: (0...10).step(2).to_a
来源：http://hco.gzhubu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gqp.hfpthk.cn

[B12] 跳出多层循环
来源：http://tym.zhoulong.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://xyo.jiagoushi.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lru.ydjk.org.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jkd.shuidangran.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xgv.yuxming.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://euj.jianghu66.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://aez.chenlongwang.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ssb.jinghuilouyu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uhf.hammf.cn

[B13] 判断是否为数字
来源：http://yau.sysykeji.top

Py:   isinstance(x, (int, float))
来源：http://ufg.xylfe.cn

PHP:  is_numeric($x)
来源：http://wly.hcnkem.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qgx.daria6918.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://koj.ydjk.org.cn

Java: x instanceof Number
来源：http://jwp.uphjek.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rmd.cheryme.top

Ruby: x.is_a?(Numeric)
来源：http://wre.sufxvd.cn

C#:   x is int or double or decimal
来源：http://nqb.daxiang520.top

[B14] 判断值是否在集合内
来源：http://gns.xuetiantiany.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kkd.nanxuanxn.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kql.52xcode.cn


<!-- 参考信息 -->