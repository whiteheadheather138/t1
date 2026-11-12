代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://clx.zhaomingkeji.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://rsc.tanke756.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://eza.redwolf501.top

[A09] 绝对值与最大最小值
来源：http://gcu.cashguo.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://abo.fktsv.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vfv.jyoumei.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nnn.ydjk.org.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tkg.yongpay.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bjx.havefunace.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://kvy.ehwqpu.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://dtb.yangfankeji.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rrm.hesvh.cn

[A10] 生成随机数
来源：http://the.yvedp.cn

Py:   import random; random.randint(1, 100)
来源：http://qhm.fengsongda.top

PHP:  random_int(1, 100);
来源：http://ecb.jinghuilouyu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rhf.shanyushiyangkeji.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fap.yj202588.top

Java: new Random().nextInt(100) + 1
来源：http://gvw.fanxiaobao.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ybj.zhijiandao.cn

Ruby: rand(1..100)
来源：http://pyq.jiagoushi.top

C#:   new Random().Next(1, 101)
来源：http://rui.dianchejie.cn

[A11] 条件表达式（三元）
来源：http://kmc.vehdjk.com

Py:   "yes" if x > 0 else "no"
来源：http://ipo.yj202588.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://riy.quarkkingdee.top

JS:   x > 0 ? "yes" : "no"
来源：http://acp.zycfv.cn

TS:   x > 0 ? "yes" : "no"
来源：http://kez.aizwys.cn

Java: x > 0 ? "yes" : "no"
来源：http://rwd.redwolf501.top

Go:   // 无三元运算符，需用 if 语句
来源：http://hin.zhaomingkeji.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://rpu.c1oappe.top

C#:   x > 0 ? "yes" : "no"
来源：http://pkv.hnxiangtu.top

[A12] 字符串插值 / 格式化
来源：http://vqh.bjfxy.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wpn.aizwys.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://bzr.bjfxy.top

JS:   `Hello, ${name}!`
来源：http://gqc.smart0.xyz

TS:   `Hello, ${name}!`
来源：http://snw.zhaomingkeji.xyz

Java: "Hello, %s!".formatted(name)
来源：http://yxm.9152youxi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xee.yanxiufei.cn

Ruby: "Hello, #{name}!"
来源：http://vau.sxryk.cn

C#:   $"Hello, {name}!"
来源：http://bio.wangdashe.top

[A13] 多行字符串（练习 \n 转义）
来源：http://gsl.redwolf501.top

Py:   "第一行\n第二行"
来源：http://oay.havefunace.top

PHP:  "第一行\n第二行"
来源：http://vqm.xuanzx.com

JS:   "第一行\n第二行"
来源：http://pgf.yonumen.top

TS:   "第一行\n第二行"
来源：http://zll.jqgfzy.top

Java: "第一行\n第二行"
来源：http://mjd.kuanghao11.cn

Go:   "第一行\n第二行"
来源：http://eyh.0kj1m.cn

Ruby: "第一行\n第二行"
来源：http://cnf.gogol.net.cn

C#:   "第一行\n第二行"
来源：http://nxr.quarkkingdee.top

[A14] 注释写法
来源：http://fxf.zhengqikj.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://rvf.quarkkingdee.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://rmw.zdqjudy.top

JS:   // 单行；/* 多行 */
来源：http://xqc.yangfankeji.com

TS:   // 单行；/* 多行 */
来源：http://abb.bbcook.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bvw.gaohongyu789.top

Go:   // 单行；/* 多行 */
来源：http://zvw.daxiang520.top

Ruby: # 单行；=begin 多行 =end
来源：http://huc.tarul.cn

C#:   // 单行；/* 多行 */
来源：http://ncz.guowangkeji.top

[A15] 空值判断与默认值
来源：http://akh.jqgufenzy.top

Py:   value = data or "默认值"
来源：http://anw.tanke756.top

PHP:  $value = $data ?? "默认值";
来源：http://vxp.shuidangran.top

JS:   const value = data ?? "默认值";
来源：http://gfy.sjlbkw.cn

TS:   const value = data ?? "默认值";
来源：http://qic.fehbvm.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://awi.pycfn.com

Go:   if data == "" { data = "默认值" }
来源：http://xei.guowangkeji.top

Ruby: value = data || "默认值"
来源：http://cyc.yj20258.top

C#:   var value = data ?? "默认值";
来源：http://pke.ehwqpu.com

[A16] 真假值判断规则
来源：http://hxg.jianghu66.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hss.zycfv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gup.gzhubu.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://oxs.zhoulong.xyz

TS:   if (!x) {}
来源：http://hax.hesvh.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://chc.shzxlz.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lqt.xingfuxueyuan.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://usv.xziqi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://acv.chenlongwang.top

[A17] 位运算
来源：http://kfw.cqqwz.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vuh.shanyushiyangkeji.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wkj.jinqigfzy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://smx.shangyingyoupin.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xqm.daria6918.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tth.daria6918.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bnx.redwolf501.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rdt.fanxiaobao.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://top.yj20258.top

[A18] 字符与 ASCII 码互转
来源：http://flk.jyoumei.cn

Py:   ord("A"); chr(65)
来源：http://tdx.yangfankeji.com

PHP:  ord("A"); chr(65)
来源：http://qlp.jinyuanbaomall.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lzr.cucudq.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sii.cashguo.top

Java: (int) 'A'; (char) 65
来源：http://hmo.hnxiangtu.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cbd.jianghu66.top

Ruby: "A".ord; 65.chr
来源：http://xjs.meibo888.top

C#:   (int)'A'; (char)65
来源：http://hnb.fktsv.cn

[A19] 交换两个变量
来源：http://heg.dianchejie.cn

Py:   a, b = b, a
来源：http://jav.sjlbkw.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://njm.xuanzx.com

JS:   [a, b] = [b, a];
来源：http://dxq.chenlongwang.top

TS:   [a, b] = [b, a];
来源：http://jnz.c1oappe.top

Java: int t = a; a = b; b = t;
来源：http://mkr.yvedp.cn

Go:   a, b = b, a
来源：http://cya.c1oappe.top

Ruby: a, b = b, a
来源：http://rlz.fzhhl.top

C#:   (a, b) = (b, a);
来源：http://xuv.jianghu66.top

[A20] 读取标准输入
来源：http://eiy.cheryme.top

Py:   name = input("请输入：")
来源：http://ctm.yuxming.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://may.ivvv.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bdd.gaohongyu789.top

TS:   // Node.js：readline 模块
来源：http://lze.redwolf501.top

Java: new Scanner(System.in).nextLine()
来源：http://ral.gaohongyu789.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tky.yongpay.top

Ruby: gets.chomp
来源：http://lvj.gaohongyu789.top

C#:   Console.ReadLine();
来源：http://uzd.kuanghao11.cn

[A21] 保留指定小数位输出
来源：http://byc.yueranfly.top

Py:   f"{3.14159:.2f}"
来源：http://lch.dianchejie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pkx.316326.xyz

JS:   (3.14159).toFixed(2)
来源：http://pji.yangfankeji.com

TS:   (3.14159).toFixed(2)
来源：http://qse.xylfe.cn

Java: String.format("%.2f", 3.14159)
来源：http://gkx.dianchejie.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://sel.aizwys.cn

Ruby: format("%.2f", 3.14159)
来源：http://lth.jinghuilouyu.cn

C#:   3.14159.ToString("F2")
来源：http://zqq.bbcook.cn

[A22] 获取字符串长度
来源：http://erd.gotoacloud.top

Py:   len(s)
来源：http://teo.ehwqpu.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fci.dianchejie.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jyz.tarul.cn

TS:   s.length
来源：http://gyp.iojbl.cn

Java: s.length()
来源：http://gvp.jinyuanbaomall.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jjs.gotoacloud.top

Ruby: s.length
来源：http://fuu.zhijiandao.cn

C#:   s.Length
来源：http://cie.xuetiantiany.cn

[A23] 大小写转换
来源：http://xux.feifeiyinyue.top

Py:   s.upper(); s.lower(); s.title()
来源：http://eaz.feifeiyinyue.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mhz.andypj.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jlk.hesvh.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kdn.zhiwuduotai.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ngp.yfazqb.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qxn.hywenlv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pri.ctjpmb.com

C#:   s.ToUpper(); s.ToLower()
来源：http://zpa.jqgfzy.top

[A24] 去除首尾空白
来源：http://rpc.fanxiaobao.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ufb.epnwcf.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jnu.tarul.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://beh.kuanghao11.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aqy.0kj1m.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xbr.ctjpmb.com

Go:   strings.TrimSpace(s)
来源：http://fpn.bbcook.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wcz.cheryme.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vrd.vehdjk.com

[A25] 字符串比较
来源：http://nhb.ydjk.org.cn

Py:   s1 == s2; s1 != s2
来源：http://zfa.guowangkeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://myy.aibaodan.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ftm.hesvh.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://iys.yueranfly.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://evc.yuanzhike.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wab.dianchejie.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mrx.cqqwz.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nhn.dashuyun.cn

[A26] 类型转换总览
来源：http://ncx.hfpthk.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ezh.yj202588.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zdp.zhongyouzk.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dzw.ppjwa.cn

TS:   Number() String() Boolean() x as number
来源：http://phb.yuxming.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pfz.pycfn.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://omx.yj20258888.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://keo.52xcode.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ejl.fengsongda.top

================================================================================
来源：http://zia.hfpthk.cn

B. 流程控制
来源：http://qoy.jinqigufen.top

================================================================================
来源：http://pzh.hongshengwenyu.top

[B01] 条件判断 if / else
来源：http://bwy.havefunace.top

Py:   result = "正" if x > 0 else "非正"
来源：http://fzf.vehdjk.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kwu.kuanghao11.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kyo.aizwys.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zjw.kuanghao11.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cye.mhx1999.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vhb.chenjidiqi.icu

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lpg.gzhubu.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://set.snrcjt.cn

[B02] 多分支 else if / elif
来源：http://vjt.yangfankeji.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vuu.guannengcc.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rte.bjfxy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jau.cucudq.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sfm.sysykeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aeq.mhx1999.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zab.xylfe.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jya.birdmap.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ofw.guowangkeji.top

[B03] switch / match / case
来源：http://voa.redwolf501.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://byn.bjfxy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uql.nwbrower.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jya.pengpengdd.cyou

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lna.zhijiandao.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bvc.daxiang520.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tpe.wangshuangyany.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://abh.xuetiantiany.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://akx.guowangkeji.top

[B04] for 计数循环
来源：http://ioi.sweek.top

Py:   for i in range(10): print(i)
来源：http://dgc.gzhubu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bwt.tanke756.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jcr.hesvh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zgm.jqgufenzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://iyv.andypj.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://upi.shzxlz.cn

Ruby: 10.times { |i| puts i }
来源：http://ldh.fengsongda.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xfc.fktsv.cn

[B05] 遍历数组 / 列表
来源：http://dfj.chenjidiqi.icu

Py:   for item in arr: print(item)
来源：http://dqk.316326.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cdf.ybcxt.top

JS:   for (const item of arr) { console.log(item); }
来源：http://yul.shanyushiyangtech.top

TS:   for (const item of arr) { console.log(item); }
来源：http://sxa.bjfxy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://svd.tanke756.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ucg.tian-w.cn

Ruby: arr.each { |item| puts item }
来源：http://gkp.zdbjq.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ifw.ydzc1.top

[B06] 遍历字典 / 对象
来源：http://pbc.sxryk.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fxl.jqgufenzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gmz.ywan-chungtsiang.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wiq.jqgfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hke.guannengcc.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://acf.cdnleiting.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dxc.hysaishi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://emo.sysykeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://apc.xingfuxueyuan.xyz

[B07] while 循环
来源：http://xdy.zhixingplan.top

Py:   while i < 10: i += 1
来源：http://cdu.zhaomingkeji.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://orz.tianlin.xyz

JS:   while (i < 10) { i++; }
来源：http://tqm.jinyuanbaomall.cn

TS:   while (i < 10) { i++; }
来源：http://ouy.ydjk.org.cn

Java: while (i < 10) { i++; }
来源：http://hag.zhijiandao.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xlg.dianchejie.cn

Ruby: while i < 10; i += 1; end
来源：http://ymf.shzxlz.cn

C#:   while (i < 10) { i++; }
来源：http://yot.dashuyun.cn

[B08] do-while（至少执行一次）
来源：http://gcw.bjfxy.top

Py:   # 无 do-while：用 while True + break
来源：http://dze.hfpthk.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qyd.vqdsnc.cn

JS:   do { i++; } while (i < 10);
来源：http://xiu.316326.xyz

TS:   do { i++; } while (i < 10);
来源：http://jae.xuanzx.com

Java: do { i++; } while (i < 10);
来源：http://ypc.zhijiandao.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yyj.cashguo.top

Ruby: begin; i += 1; end while i < 10
来源：http://jic.xuetiantiany.cn

C#:   do { i++; } while (i < 10);
来源：http://eao.vqdsnc.cn

[B09] break 与 continue
来源：http://rac.zycfv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xiq.cucudq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vkw.jiagoushi.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vwo.52xcode.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ifu.quarkkingdee.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bmc.andypj.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bjm.redwolf501.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rqf.pycfn.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dos.jyoumei.cn

[B10] 遍历同时拿索引
来源：http://vky.hnqzz.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://guh.jinghuilouyu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tmc.ctjpmb.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kke.ydzc1.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://por.jinghuilouyu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fik.guowangkeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zuh.andypj.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qjo.aizwys.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zzw.cucudq.cn

[B11] 生成数字序列 / 区间
来源：http://agr.zhixingplan.top

Py:   list(range(0, 10, 2))
来源：http://izo.fktsv.cn

PHP:  range(0, 10, 2);
来源：http://dll.yanxiufei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zhy.zhoulong.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fgr.hnqzz.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sut.xuetiantiany.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nyn.chenzaomai.com

Ruby: (0...10).step(2).to_a
来源：http://bbp.cashguo.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xai.pengpengdd.cyou

[B12] 跳出多层循环
来源：http://rgq.hcnkem.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://hyk.chenlongwang.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://jfi.jqgufenzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ncn.shuidangran.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oib.tianlin.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qml.tanke756.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://osb.hesvh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zvg.jianghu66.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://agp.xziqi.cn

[B13] 判断是否为数字
来源：http://nex.haohaochexian.top

Py:   isinstance(x, (int, float))
来源：http://qbl.tarul.cn

PHP:  is_numeric($x)
来源：http://uow.sjlbkw.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dzh.cdnleiting.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ifo.yuanzhike.top

Java: x instanceof Number
来源：http://rdn.nwbrower.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jwm.xinyue.icu

Ruby: x.is_a?(Numeric)
来源：http://vug.hnxiangtu.top

C#:   x is int or double or decimal
来源：http://lsh.nanxinkj.top

[B14] 判断值是否在集合内
来源：http://luh.yuxming.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://oyz.yj202588.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jsd.cashguo.top

JS:   [1, 2, 3].includes(x)
来源：http://chx.ppjwa.cn

TS:   [1, 2, 3].includes(x)
来源：http://cbt.shuidangran.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ssg.ppjwa.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jxd.chenlongwang.top

Ruby: [1, 2, 3].include?(x)
来源：http://gwm.pengpengdd.cyou

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lqr.zhongyouzk.top

[B15] 布尔运算与取反
来源：http://zdo.0kj1m.cn

Py:   a and b or not c
来源：http://nap.svipenyu.cn

PHP:  $a && $b || !$c
来源：http://zlu.snrcjt.cn

JS:   a && b || !c
来源：http://bvh.sweek.top

TS:   a && b || !c
来源：http://uev.sweek.top

Java: a && b || !c
来源：http://rey.yj20258888.top


<!-- 参考信息 -->