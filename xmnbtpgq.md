代发 wailian999

Ruby: 42.to_s
来源：http://ali.iojbl.cn

C#:   42.ToString()
来源：http://utd.jinghuilouyu.cn

[A08] 取整与四舍五入
来源：http://sbh.tianlin.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nmu.dianchejie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qgl.kuanghao11.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://uup.yanxiufei.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jce.hnqzz.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rmz.yueranfly.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xoa.zdqjudy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://csn.chenzaomai.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mfm.pycfn.com

[A09] 绝对值与最大最小值
来源：http://xtj.bbcook.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ork.shuidangran.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nwk.xuanzx.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://owh.316326.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qzv.jiagoushi.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://npn.andypj.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vfp.tian-w.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tbp.zhoulong.xyz

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jsb.daxiang520.top

[A10] 生成随机数
来源：http://nnf.svipenyu.cn

Py:   import random; random.randint(1, 100)
来源：http://iml.fehbvm.com

PHP:  random_int(1, 100);
来源：http://oja.316326.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://aqn.yuxming.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dzk.jinyuanbaomall.cn

Java: new Random().nextInt(100) + 1
来源：http://ndj.hongshengwenyu.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fmn.yvedp.cn

Ruby: rand(1..100)
来源：http://kjr.yonumen.top

C#:   new Random().Next(1, 101)
来源：http://hnw.haohaochexian.top

[A11] 条件表达式（三元）
来源：http://wvg.shangyingyoupin.top

Py:   "yes" if x > 0 else "no"
来源：http://igf.tanke756.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://oze.nanxinkj.top

JS:   x > 0 ? "yes" : "no"
来源：http://irb.jqgufenzy.top

TS:   x > 0 ? "yes" : "no"
来源：http://ntz.zdqjudy.top

Java: x > 0 ? "yes" : "no"
来源：http://iak.jinqigfzy.top

Go:   // 无三元运算符，需用 if 语句
来源：http://wiq.xuetiantiany.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://iac.shangyingyoupin.top

C#:   x > 0 ? "yes" : "no"
来源：http://dmb.xingfuxueyuan.xyz

[A12] 字符串插值 / 格式化
来源：http://yms.aibaodan.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bbu.ctjpmb.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hmi.dianchejie.cn

JS:   `Hello, ${name}!`
来源：http://sko.cucudq.cn

TS:   `Hello, ${name}!`
来源：http://uco.tarul.cn

Java: "Hello, %s!".formatted(name)
来源：http://oeq.iojbl.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tpo.shanyushiyangkeji.top

Ruby: "Hello, #{name}!"
来源：http://agb.tarul.cn

C#:   $"Hello, {name}!"
来源：http://qml.fehbvm.com

[A13] 多行字符串（练习 \n 转义）
来源：http://lqy.sysykeji.top

Py:   "第一行\n第二行"
来源：http://qfu.9152youxi.cn

PHP:  "第一行\n第二行"
来源：http://zjt.shuidangran.top

JS:   "第一行\n第二行"
来源：http://llj.pengpengdd.cyou

TS:   "第一行\n第二行"
来源：http://tfv.ydzc1.top

Java: "第一行\n第二行"
来源：http://kaw.hysaishi.cn

Go:   "第一行\n第二行"
来源：http://mqh.shuidangran.top

Ruby: "第一行\n第二行"
来源：http://tzm.jianghu66.top

C#:   "第一行\n第二行"
来源：http://bus.nwbrower.top

[A14] 注释写法
来源：http://mod.pycfn.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://ujr.hnqzz.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://sbu.fzhhl.top

JS:   // 单行；/* 多行 */
来源：http://axg.ctjpmb.com

TS:   // 单行；/* 多行 */
来源：http://erw.kuanghao11.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://riq.nanxuanxn.top

Go:   // 单行；/* 多行 */
来源：http://kbd.yangfankeji.com

Ruby: # 单行；=begin 多行 =end
来源：http://xny.dianchejie.cn

C#:   // 单行；/* 多行 */
来源：http://yfa.hongshengwenyu.top

[A15] 空值判断与默认值
来源：http://ipw.dianchejie.cn

Py:   value = data or "默认值"
来源：http://rqq.jqgufenzy.top

PHP:  $value = $data ?? "默认值";
来源：http://xvi.zhaomingkeji.xyz

JS:   const value = data ?? "默认值";
来源：http://obw.zhengqikj.top

TS:   const value = data ?? "默认值";
来源：http://kda.xziqi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gni.shzxlz.cn

Go:   if data == "" { data = "默认值" }
来源：http://hdl.jinqigufen.top

Ruby: value = data || "默认值"
来源：http://cii.epnwcf.com

C#:   var value = data ?? "默认值";
来源：http://ofa.havefunace.top

[A16] 真假值判断规则
来源：http://gdd.sxryk.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nvh.fehbvm.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rbq.snrcjt.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://srs.yueranfly.top

TS:   if (!x) {}
来源：http://udy.svipenyu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://luq.kuanghao11.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bgx.cdnleiting.top

Ruby: unless x            # nil 与 false 为假
来源：http://ogx.sysykeji.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mxk.jinyuanbaomall.cn

[A17] 位运算
来源：http://abe.xingfuxueyuan.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cju.chenlongwang.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bny.9152youxi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ccq.hnxiangtu.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://oye.haohaochexian.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xen.zycfv.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://uav.shzxlz.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ikj.svipenyu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zfb.daxiang520.top

[A18] 字符与 ASCII 码互转
来源：http://ctg.9152youxi.cn

Py:   ord("A"); chr(65)
来源：http://biy.ivvv.top

PHP:  ord("A"); chr(65)
来源：http://khq.jqgfzy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ynk.jianghu66.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qoj.yonumen.top

Java: (int) 'A'; (char) 65
来源：http://bfc.dianchejie.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jxw.jianghu66.top

Ruby: "A".ord; 65.chr
来源：http://amc.yvedp.cn

C#:   (int)'A'; (char)65
来源：http://aep.sufxvd.cn

[A19] 交换两个变量
来源：http://ngt.ydjk.org.cn

Py:   a, b = b, a
来源：http://ahb.cqqwz.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://kku.daria6918.cn

JS:   [a, b] = [b, a];
来源：http://fmv.nanxuanxn.top

TS:   [a, b] = [b, a];
来源：http://okw.epnwcf.com

Java: int t = a; a = b; b = t;
来源：http://hio.cqqwz.cn

Go:   a, b = b, a
来源：http://ofe.sweek.top

Ruby: a, b = b, a
来源：http://ghu.tian-w.cn

C#:   (a, b) = (b, a);
来源：http://ojb.ywan-chungtsiang.top

[A20] 读取标准输入
来源：http://rbu.iojbl.cn

Py:   name = input("请输入：")
来源：http://cvj.hongshengwenyu.top

PHP:  $name = trim(fgets(STDIN));
来源：http://wkm.uphjek.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vde.haohaochexian.top

TS:   // Node.js：readline 模块
来源：http://xna.uphjek.com

Java: new Scanner(System.in).nextLine()
来源：http://kjt.hammf.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hcn.jlsjyb.cn

Ruby: gets.chomp
来源：http://dlo.feifeiyinyue.top

C#:   Console.ReadLine();
来源：http://amc.shangyingyoupin.top

[A21] 保留指定小数位输出
来源：http://npd.gotoacloud.top

Py:   f"{3.14159:.2f}"
来源：http://vqs.vqdsnc.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://upe.pycfn.com

JS:   (3.14159).toFixed(2)
来源：http://emr.pengpengdd.cyou

TS:   (3.14159).toFixed(2)
来源：http://kld.jyoumei.cn

Java: String.format("%.2f", 3.14159)
来源：http://ilj.wangdashe.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pee.zhixingplan.top

Ruby: format("%.2f", 3.14159)
来源：http://kni.hongshengwenyu.top

C#:   3.14159.ToString("F2")
来源：http://dif.sweek.top

[A22] 获取字符串长度
来源：http://qsc.xingfuxueyuan.xyz

Py:   len(s)
来源：http://ffo.zhaomingkeji.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jsf.zdqjudy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fcd.chenlongwang.top

TS:   s.length
来源：http://chz.birdmap.top

Java: s.length()
来源：http://ucw.zhiwuduotai.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ljr.gaohongyu789.top

Ruby: s.length
来源：http://jvg.hesvh.cn

C#:   s.Length
来源：http://xzr.9152youxi.cn

[A23] 大小写转换
来源：http://hpx.nwbrower.top

Py:   s.upper(); s.lower(); s.title()
来源：http://xgu.svipenyu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ore.dashuyun.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fvw.zhaomingkeji.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://arb.9152youxi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rti.wangshuangyany.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xka.vehdjk.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://flz.aibaodan.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://uou.jinqigufen.top

[A24] 去除首尾空白
来源：http://xne.hongshengwenyu.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://elr.feifeiyinyue.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gwd.shzxlz.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cjy.fanxiaobao.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zwa.havefunace.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qvz.yanxiufei.cn

Go:   strings.TrimSpace(s)
来源：http://nsw.mhx1999.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ace.zhongyouzk.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rdu.zdqjudy.top

[A25] 字符串比较
来源：http://rcc.nanxuanxn.top

Py:   s1 == s2; s1 != s2
来源：http://wet.52xcode.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qdq.guowangkeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rpf.fzhhl.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://adb.zhoulong.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rms.cucudq.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zut.bbcook.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mmy.dashuyun.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://asf.jianghu66.top

[A26] 类型转换总览
来源：http://taa.tarul.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://voo.jlsjyb.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://utf.nwbrower.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vau.yj20258888.top

TS:   Number() String() Boolean() x as number
来源：http://sgq.chenlongwang.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bqj.xingfuxueyuan.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fnq.ydzc1.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://aqx.quarkkingdee.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dyi.svipenyu.cn

================================================================================
来源：http://rap.jyoumei.cn

B. 流程控制
来源：http://ami.nanxuanxn.top

================================================================================
来源：http://jlr.nanxuanxn.top

[B01] 条件判断 if / else
来源：http://yfz.shanyushiyangkeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://dpd.xingfuxueyuan.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qcf.pengpengdd.cyou

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lqb.yfazqb.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://twu.cashguo.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://jeg.smart0.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://htf.yuanzhike.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fgt.tarul.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uva.xinyue.icu

[B02] 多分支 else if / elif
来源：http://xgb.bbcook.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ylx.guowangkeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sly.xziqi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ekq.pengpengdd.cyou

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rql.sysykeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://phs.yangfankeji.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://okt.chenlongwang.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rou.fehbvm.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ezb.wangshuangyany.cn

[B03] switch / match / case
来源：http://yty.bjfxy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://keu.wangshuangyany.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ucq.dashuyun.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dvl.yj20258.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://amt.fktsv.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oue.hesvh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://eug.cheryme.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zfz.daria6918.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tpe.yonumen.top

[B04] for 计数循环
来源：http://wog.ybcxt.top

Py:   for i in range(10): print(i)
来源：http://cpx.yuxming.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mnh.vqdsnc.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kpi.xuanzx.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ayx.hcnkem.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ztb.haohaochexian.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://eqv.jinqigfzy.top

Ruby: 10.times { |i| puts i }
来源：http://jzb.guowangkeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yje.c1oappe.top

[B05] 遍历数组 / 列表
来源：http://mjx.kuanghao11.cn

Py:   for item in arr: print(item)
来源：http://xgp.bjfxy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sqd.fengsongda.top

JS:   for (const item of arr) { console.log(item); }
来源：http://xlo.epnwcf.com

TS:   for (const item of arr) { console.log(item); }
来源：http://juv.fzhhl.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fqb.zhoulong.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fbf.fzhhl.top

Ruby: arr.each { |item| puts item }
来源：http://kcn.hfpthk.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dme.jlsjyb.cn

[B06] 遍历字典 / 对象
来源：http://wim.smart0.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://liy.redwolf501.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uej.52xcode.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bpu.316326.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mmg.zhixingplan.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gmh.cqqwz.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jtq.nwbrower.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tjo.52xcode.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bcw.ydjk.org.cn

[B07] while 循环
来源：http://vth.52xcode.cn

Py:   while i < 10: i += 1
来源：http://bsh.dianchejie.cn

PHP:  while ($i < 10) { $i++; }
来源：http://skt.wangdashe.top

JS:   while (i < 10) { i++; }
来源：http://jyv.ydzc1.top

TS:   while (i < 10) { i++; }
来源：http://pef.hesvh.cn

Java: while (i < 10) { i++; }
来源：http://rst.havefunace.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mqn.ppjwa.cn

Ruby: while i < 10; i += 1; end
来源：http://mct.gotoacloud.top

C#:   while (i < 10) { i++; }
来源：http://hum.uphjek.com

[B08] do-while（至少执行一次）
来源：http://stk.shangyingyoupin.top

Py:   # 无 do-while：用 while True + break
来源：http://ugq.tanke756.top

PHP:  do { $i++; } while ($i < 10);
来源：http://qtg.chenjidiqi.icu

JS:   do { i++; } while (i < 10);
来源：http://ebg.zhengqikj.top

TS:   do { i++; } while (i < 10);
来源：http://awe.sysykeji.top

Java: do { i++; } while (i < 10);
来源：http://jaq.xziqi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gee.aizwys.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dmd.shanyushiyangtech.top

C#:   do { i++; } while (i < 10);
来源：http://lhx.zhaomingkeji.xyz

[B09] break 与 continue
来源：http://epk.jlsjyb.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vab.fehbvm.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eeo.svipenyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fwi.ydzc1.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ctg.andypj.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tem.tarul.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ycc.ywan-chungtsiang.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wzw.feifeiyinyue.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cvz.shanyushiyangtech.top

[B10] 遍历同时拿索引
来源：http://hey.nanxuanxn.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bns.yangfankeji.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://axw.sjlbkw.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dhw.gzhubu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gtl.yuanzhike.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kfc.sweek.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yis.tianlin.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://btm.ywan-chungtsiang.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://eok.cdnleiting.top

[B11] 生成数字序列 / 区间
来源：http://vwv.wangshuangyany.cn

Py:   list(range(0, 10, 2))
来源：http://lwh.yvedp.cn

PHP:  range(0, 10, 2);
来源：http://isq.guannengcc.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ssa.sjlbkw.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pxf.cashguo.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://kok.ydjk.org.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ask.shanyushiyangkeji.top

Ruby: (0...10).step(2).to_a
来源：http://lac.andypj.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://txj.chenzaomai.com

[B12] 跳出多层循环
来源：http://xtw.yj20258888.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://yuu.hesvh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://lpt.hnxiangtu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rvp.hammf.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://clw.yj20258.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vjs.snrcjt.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cbz.cdnleiting.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xnk.yangfankeji.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tjt.ehwqpu.com

[B13] 判断是否为数字
来源：http://zoe.havefunace.top

Py:   isinstance(x, (int, float))
来源：http://ijo.daxiang520.top

PHP:  is_numeric($x)
来源：http://wkd.smart0.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qfs.redwolf501.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ome.xuanzx.com

Java: x instanceof Number
来源：http://mzj.yj202588.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dzs.guowangkeji.top

Ruby: x.is_a?(Numeric)
来源：http://hyy.cqqwz.cn

C#:   x is int or double or decimal
来源：http://txe.uphjek.com

[B14] 判断值是否在集合内
来源：http://ykv.ppjwa.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://imu.yonumen.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xnw.haohaochexian.top

JS:   [1, 2, 3].includes(x)
来源：http://ivb.hfpthk.cn

TS:   [1, 2, 3].includes(x)
来源：http://wli.xuanzx.com

Java: List.of(1, 2, 3).contains(x)
来源：http://ogh.hfpthk.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ync.tianlin.xyz


<!-- 参考信息 -->