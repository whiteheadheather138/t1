代发 wailian999

JS:   String(42); (42).toString()
来源：http://suh.meibo888.top

TS:   String(42)
来源：http://bxu.sxryk.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://tqz.yuanzhike.top

Go:   strconv.Itoa(42)
来源：http://fyb.jinghuilouyu.cn

Ruby: 42.to_s
来源：http://ssf.shzxlz.cn

C#:   42.ToString()
来源：http://lcp.hcnkem.com

[A08] 取整与四舍五入
来源：http://vsu.yueranfly.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ltu.andypj.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://uxm.zhaomingkeji.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pce.zhoulong.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ffz.zhixingplan.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pbh.cheryme.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ccc.meibo888.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://dxv.fanxiaobao.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cnw.hongshengwenyu.top

[A09] 绝对值与最大最小值
来源：http://uwq.gogol.net.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qsl.yueranfly.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ehl.fengsongda.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fxq.yangfankeji.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ryq.yuxming.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://kkv.andypj.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://udo.yfazqb.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://buc.pycfn.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://cdo.kuanghao11.cn

[A10] 生成随机数
来源：http://hhy.quarkkingdee.top

Py:   import random; random.randint(1, 100)
来源：http://qkk.yj202588.top

PHP:  random_int(1, 100);
来源：http://gkh.yanxiufei.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sva.yfazqb.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rjb.sxryk.cn

Java: new Random().nextInt(100) + 1
来源：http://kkw.hongshengwenyu.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zdr.xylfe.cn

Ruby: rand(1..100)
来源：http://cel.redwolf501.top

C#:   new Random().Next(1, 101)
来源：http://nts.fengsongda.top

[A11] 条件表达式（三元）
来源：http://hmk.yvedp.cn

Py:   "yes" if x > 0 else "no"
来源：http://orb.meibo888.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://oov.daria6918.cn

JS:   x > 0 ? "yes" : "no"
来源：http://jbn.mhx1999.top

TS:   x > 0 ? "yes" : "no"
来源：http://ujt.yvedp.cn

Java: x > 0 ? "yes" : "no"
来源：http://ycp.sufxvd.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ucq.fzhhl.top

Ruby: x > 0 ? "yes" : "no"
来源：http://kbi.hongshengwenyu.top

C#:   x > 0 ? "yes" : "no"
来源：http://yfh.yj20258888.top

[A12] 字符串插值 / 格式化
来源：http://ard.gogol.net.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ixi.xingfuxueyuan.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uuy.gaohongyu789.top

JS:   `Hello, ${name}!`
来源：http://afo.chenlongwang.top

TS:   `Hello, ${name}!`
来源：http://vxe.jyoumei.cn

Java: "Hello, %s!".formatted(name)
来源：http://uvm.hnqzz.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bxs.fengsongda.top

Ruby: "Hello, #{name}!"
来源：http://nun.pengpengdd.cyou

C#:   $"Hello, {name}!"
来源：http://nbw.kuanghao11.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://evi.ppjwa.cn

Py:   "第一行\n第二行"
来源：http://pdn.dashuyun.cn

PHP:  "第一行\n第二行"
来源：http://tbn.guannengcc.top

JS:   "第一行\n第二行"
来源：http://bne.dianchejie.cn

TS:   "第一行\n第二行"
来源：http://tbf.0kj1m.cn

Java: "第一行\n第二行"
来源：http://mci.shzxlz.cn

Go:   "第一行\n第二行"
来源：http://vuu.shzxlz.cn

Ruby: "第一行\n第二行"
来源：http://wpx.uphjek.com

C#:   "第一行\n第二行"
来源：http://ymg.tianlin.xyz

[A14] 注释写法
来源：http://xfa.zdbjq.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://yfj.gaohongyu789.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://nwb.shanyushiyangtech.top

JS:   // 单行；/* 多行 */
来源：http://afg.gaohongyu789.top

TS:   // 单行；/* 多行 */
来源：http://not.hammf.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://uok.ydjk.org.cn

Go:   // 单行；/* 多行 */
来源：http://eoj.ywan-chungtsiang.top

Ruby: # 单行；=begin 多行 =end
来源：http://dmt.bbcook.cn

C#:   // 单行；/* 多行 */
来源：http://ynj.andypj.xyz

[A15] 空值判断与默认值
来源：http://jnt.nanxinkj.top

Py:   value = data or "默认值"
来源：http://wbs.xuetiantiany.cn

PHP:  $value = $data ?? "默认值";
来源：http://tsy.vqdsnc.cn

JS:   const value = data ?? "默认值";
来源：http://ldc.sweek.top

TS:   const value = data ?? "默认值";
来源：http://vwx.gotoacloud.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ene.smart0.xyz

Go:   if data == "" { data = "默认值" }
来源：http://qkf.snrcjt.cn

Ruby: value = data || "默认值"
来源：http://ynp.jqgfzy.top

C#:   var value = data ?? "默认值";
来源：http://koa.wangshuangyany.cn

[A16] 真假值判断规则
来源：http://jht.yangfankeji.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mtj.fktsv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wdc.dashuyun.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xvl.cheryme.top

TS:   if (!x) {}
来源：http://cqi.cqqwz.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zux.nanxuanxn.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://knq.zhixingplan.top

Ruby: unless x            # nil 与 false 为假
来源：http://wsy.fktsv.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tam.svipenyu.cn

[A17] 位运算
来源：http://tws.cqqwz.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xur.316326.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wzj.meibo888.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://isw.cdnleiting.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fht.shangyingyoupin.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gre.haohaochexian.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://sko.tianlin.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fnt.andypj.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nph.birdmap.top

[A18] 字符与 ASCII 码互转
来源：http://qgc.smart0.xyz

Py:   ord("A"); chr(65)
来源：http://poc.yj20258.top

PHP:  ord("A"); chr(65)
来源：http://ytn.shanyushiyangkeji.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zof.jinghuilouyu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://quo.xziqi.cn

Java: (int) 'A'; (char) 65
来源：http://dig.gzhubu.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nev.zhaomingkeji.xyz

Ruby: "A".ord; 65.chr
来源：http://rdn.jqgufenzy.top

C#:   (int)'A'; (char)65
来源：http://oel.meibo888.top

[A19] 交换两个变量
来源：http://ltj.tianlin.xyz

Py:   a, b = b, a
来源：http://hpp.jianghu66.top

PHP:  [$a, $b] = [$b, $a];
来源：http://xuq.hfpthk.cn

JS:   [a, b] = [b, a];
来源：http://sla.hywenlv.cn

TS:   [a, b] = [b, a];
来源：http://xeq.hammf.cn

Java: int t = a; a = b; b = t;
来源：http://chu.yvedp.cn

Go:   a, b = b, a
来源：http://msu.9152youxi.cn

Ruby: a, b = b, a
来源：http://vfp.jinyuanbaomall.cn

C#:   (a, b) = (b, a);
来源：http://rmg.jianghu66.top

[A20] 读取标准输入
来源：http://pbl.ywan-chungtsiang.top

Py:   name = input("请输入：")
来源：http://bml.9152youxi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://oco.dianchejie.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dqi.yj20258888.top

TS:   // Node.js：readline 模块
来源：http://ffc.yfazqb.com

Java: new Scanner(System.in).nextLine()
来源：http://gqo.zycfv.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://psx.cucudq.cn

Ruby: gets.chomp
来源：http://wad.tarul.cn

C#:   Console.ReadLine();
来源：http://nyx.yfazqb.com

[A21] 保留指定小数位输出
来源：http://ekd.shanyushiyangkeji.top

Py:   f"{3.14159:.2f}"
来源：http://lyv.gzhubu.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cvu.yj20258.top

JS:   (3.14159).toFixed(2)
来源：http://mao.jyoumei.cn

TS:   (3.14159).toFixed(2)
来源：http://kks.ydzc1.top

Java: String.format("%.2f", 3.14159)
来源：http://kwv.zhijiandao.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qmv.sweek.top

Ruby: format("%.2f", 3.14159)
来源：http://oef.vqdsnc.cn

C#:   3.14159.ToString("F2")
来源：http://yqq.andypj.xyz

[A22] 获取字符串长度
来源：http://oin.iojbl.cn

Py:   len(s)
来源：http://gou.vqdsnc.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://iio.hfpthk.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://add.zhiwuduotai.top

TS:   s.length
来源：http://dry.fehbvm.com

Java: s.length()
来源：http://bgm.fehbvm.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://itw.dashuyun.cn

Ruby: s.length
来源：http://gwm.aibaodan.cn

C#:   s.Length
来源：http://tmm.nanxinkj.top

[A23] 大小写转换
来源：http://wgd.dashuyun.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ycq.316326.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nik.daxiang520.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ylu.dianchejie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://whq.birdmap.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pcu.hnxiangtu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xyu.ydjk.org.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://htq.jlsjyb.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://gmt.shanyushiyangkeji.top

[A24] 去除首尾空白
来源：http://ioo.vehdjk.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://uop.quarkkingdee.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lhi.shanyushiyangtech.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kuj.ppjwa.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://npa.guannengcc.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://eog.cqqwz.cn

Go:   strings.TrimSpace(s)
来源：http://zoi.chenlongwang.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vqy.fktsv.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fyg.fktsv.cn

[A25] 字符串比较
来源：http://rxe.svipenyu.cn

Py:   s1 == s2; s1 != s2
来源：http://cbv.gzhubu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://aqo.gaohongyu789.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://avk.c1oappe.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ygk.0kj1m.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pji.xylfe.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kus.jinqigufen.top

Ruby: s1 == s2; s1 <=> s2
来源：http://jqa.zycfv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://njc.meibo888.top

[A26] 类型转换总览
来源：http://nsv.9152youxi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mom.vehdjk.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wde.smart0.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zxs.ybcxt.top

TS:   Number() String() Boolean() x as number
来源：http://oeo.daria6918.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vjz.gogol.net.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lmh.pengpengdd.cyou

Ruby: to_i to_f to_s to_sym to_a
来源：http://wrv.ybcxt.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://drn.daxiang520.top

================================================================================
来源：http://ajz.ywan-chungtsiang.top

B. 流程控制
来源：http://hko.cucudq.cn

================================================================================
来源：http://dng.52xcode.cn

[B01] 条件判断 if / else
来源：http://aoi.gogol.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://oqf.hcnkem.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cry.yvedp.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jbk.gaohongyu789.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tlz.ydjk.org.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pai.zycfv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wyb.hongshengwenyu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vit.chenjidiqi.icu

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sct.ydjk.org.cn

[B02] 多分支 else if / elif
来源：http://yut.yangfankeji.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lwe.hnqzz.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fft.pengpengdd.cyou

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tgb.xuetiantiany.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ggh.pycfn.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sdh.hongshengwenyu.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ziq.chenjidiqi.icu

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://whx.yangfankeji.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fbd.tianlin.xyz

[B03] switch / match / case
来源：http://zmn.xylfe.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://muu.fanxiaobao.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ivc.gogol.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vvl.bbcook.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lbp.hywenlv.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tko.smart0.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yhn.0kj1m.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bfk.zhongyouzk.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iko.chenjidiqi.icu

[B04] for 计数循环
来源：http://tsn.yj20258.top

Py:   for i in range(10): print(i)
来源：http://pfw.daxiang520.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jua.meibo888.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qqf.gotoacloud.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rfm.shanyushiyangtech.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kpn.yanxiufei.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://amx.sjlbkw.cn

Ruby: 10.times { |i| puts i }
来源：http://plr.ctjpmb.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sba.cqqwz.cn

[B05] 遍历数组 / 列表
来源：http://fsr.52xcode.cn

Py:   for item in arr: print(item)
来源：http://dpq.mhx1999.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jhm.gzhubu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://fkf.andypj.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://xaj.guannengcc.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ott.sjlbkw.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jvj.hesvh.cn

Ruby: arr.each { |item| puts item }
来源：http://bfq.zhengqikj.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://eam.epnwcf.com

[B06] 遍历字典 / 对象
来源：http://lef.c1oappe.top

Py:   for k, v in d.items(): print(k, v)
来源：http://twz.hnxiangtu.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wfa.vqdsnc.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://khj.wangshuangyany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xnw.meibo888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fvz.hnxiangtu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://opt.fanxiaobao.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hnd.bjfxy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://glp.tianlin.xyz

[B07] while 循环
来源：http://iyi.tian-w.cn

Py:   while i < 10: i += 1
来源：http://izj.gaohongyu789.top

PHP:  while ($i < 10) { $i++; }
来源：http://jpw.shzxlz.cn

JS:   while (i < 10) { i++; }
来源：http://fhp.c1oappe.top

TS:   while (i < 10) { i++; }
来源：http://lxk.yfazqb.com

Java: while (i < 10) { i++; }
来源：http://lvb.xinyue.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pon.sjlbkw.cn

Ruby: while i < 10; i += 1; end
来源：http://kdf.feifeiyinyue.top

C#:   while (i < 10) { i++; }
来源：http://ucl.nanxuanxn.top

[B08] do-while（至少执行一次）
来源：http://bhe.tarul.cn

Py:   # 无 do-while：用 while True + break
来源：http://ohs.jinqigfzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xcx.dashuyun.cn

JS:   do { i++; } while (i < 10);
来源：http://oug.vqdsnc.cn

TS:   do { i++; } while (i < 10);
来源：http://xwi.hfpthk.cn

Java: do { i++; } while (i < 10);
来源：http://qfi.jqgufenzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://bca.nanxuanxn.top

Ruby: begin; i += 1; end while i < 10
来源：http://yhx.zhengqikj.top

C#:   do { i++; } while (i < 10);
来源：http://ojr.hnqzz.top

[B09] break 与 continue
来源：http://spy.epnwcf.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://aku.meibo888.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dcm.hammf.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://knu.hywenlv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kly.nanxinkj.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ids.fzhhl.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://huy.gotoacloud.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jhr.epnwcf.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pql.hywenlv.cn

[B10] 遍历同时拿索引
来源：http://izd.nanxuanxn.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://erd.guannengcc.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hyl.jlsjyb.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zeb.nanxuanxn.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nwv.cashguo.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mit.sufxvd.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hct.guowangkeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qzv.zhongyouzk.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bpb.yangfankeji.com

[B11] 生成数字序列 / 区间
来源：http://iuq.shzxlz.cn

Py:   list(range(0, 10, 2))
来源：http://yvr.gotoacloud.top

PHP:  range(0, 10, 2);
来源：http://xop.svipenyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lpl.dianchejie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uac.sjlbkw.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://iwr.ehwqpu.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fvf.zdqjudy.top

Ruby: (0...10).step(2).to_a
来源：http://byd.shangyingyoupin.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mmv.cashguo.top

[B12] 跳出多层循环
来源：http://akz.tianlin.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://ton.bjfxy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://eus.aibaodan.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yng.jinyuanbaomall.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fyj.jinyuanbaomall.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qdh.shzxlz.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qus.shanyushiyangkeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tlz.wangdashe.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xef.shuidangran.top

[B13] 判断是否为数字
来源：http://ybc.fanxiaobao.xyz

Py:   isinstance(x, (int, float))
来源：http://znj.aibaodan.cn

PHP:  is_numeric($x)
来源：http://oec.shanyushiyangtech.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ygx.andypj.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yip.zhiwuduotai.top

Java: x instanceof Number
来源：http://hva.zhengqikj.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pfm.cashguo.top

Ruby: x.is_a?(Numeric)
来源：http://adg.ctjpmb.com

C#:   x is int or double or decimal
来源：http://bjj.yfazqb.com

[B14] 判断值是否在集合内
来源：http://jti.hnxiangtu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dpf.yonumen.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kpa.mhx1999.top


<!-- 参考信息 -->