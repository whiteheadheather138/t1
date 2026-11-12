代发 wailian999

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://iwe.shanyushiyangtech.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mgu.zhaomingkeji.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://fto.jinghuilouyu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xcl.zycfv.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pcu.yj20258888.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://wfu.jlsjyb.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bts.fzhhl.top

[A09] 绝对值与最大最小值
来源：http://hgw.ywan-chungtsiang.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rlq.ctjpmb.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yxl.yfazqb.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wdf.hywenlv.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ijt.zhaomingkeji.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://eld.cashguo.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zmy.jqgfzy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zep.kuanghao11.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tog.tianlin.xyz

[A10] 生成随机数
来源：http://qoa.ywan-chungtsiang.top

Py:   import random; random.randint(1, 100)
来源：http://bdo.yangfankeji.com

PHP:  random_int(1, 100);
来源：http://nxw.cheryme.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qgl.fehbvm.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cfv.hysaishi.cn

Java: new Random().nextInt(100) + 1
来源：http://lzx.hywenlv.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hei.hfpthk.cn

Ruby: rand(1..100)
来源：http://bki.fzhhl.top

C#:   new Random().Next(1, 101)
来源：http://axi.shangyingyoupin.top

[A11] 条件表达式（三元）
来源：http://yql.xinyue.icu

Py:   "yes" if x > 0 else "no"
来源：http://atv.yongpay.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://gjl.vehdjk.com

JS:   x > 0 ? "yes" : "no"
来源：http://dpg.chenlongwang.top

TS:   x > 0 ? "yes" : "no"
来源：http://ugq.ctjpmb.com

Java: x > 0 ? "yes" : "no"
来源：http://ria.wangdashe.top

Go:   // 无三元运算符，需用 if 语句
来源：http://sgv.zhijiandao.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://hwj.jinyuanbaomall.cn

C#:   x > 0 ? "yes" : "no"
来源：http://zie.0kj1m.cn

[A12] 字符串插值 / 格式化
来源：http://kik.vehdjk.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bfb.andypj.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://dvy.shuidangran.top

JS:   `Hello, ${name}!`
来源：http://omf.fengsongda.top

TS:   `Hello, ${name}!`
来源：http://qry.aizwys.cn

Java: "Hello, %s!".formatted(name)
来源：http://rsp.ppjwa.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dil.ctjpmb.com

Ruby: "Hello, #{name}!"
来源：http://ljf.xinyue.icu

C#:   $"Hello, {name}!"
来源：http://yty.hcnkem.com

[A13] 多行字符串（练习 \n 转义）
来源：http://cko.quarkkingdee.top

Py:   "第一行\n第二行"
来源：http://dwm.vehdjk.com

PHP:  "第一行\n第二行"
来源：http://two.cheryme.top

JS:   "第一行\n第二行"
来源：http://jax.hysaishi.cn

TS:   "第一行\n第二行"
来源：http://tei.gogol.net.cn

Java: "第一行\n第二行"
来源：http://abo.zhaomingkeji.xyz

Go:   "第一行\n第二行"
来源：http://sdf.zhaomingkeji.xyz

Ruby: "第一行\n第二行"
来源：http://ejx.0kj1m.cn

C#:   "第一行\n第二行"
来源：http://ici.xziqi.cn

[A14] 注释写法
来源：http://rik.meibo888.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ddy.fanxiaobao.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://wgw.xingfuxueyuan.xyz

JS:   // 单行；/* 多行 */
来源：http://hyo.jlsjyb.cn

TS:   // 单行；/* 多行 */
来源：http://jyq.redwolf501.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lam.fehbvm.com

Go:   // 单行；/* 多行 */
来源：http://fxa.shzxlz.cn

Ruby: # 单行；=begin 多行 =end
来源：http://kuv.yanxiufei.cn

C#:   // 单行；/* 多行 */
来源：http://bcm.xinyue.icu

[A15] 空值判断与默认值
来源：http://yta.gotoacloud.top

Py:   value = data or "默认值"
来源：http://hon.cheryme.top

PHP:  $value = $data ?? "默认值";
来源：http://ykw.tarul.cn

JS:   const value = data ?? "默认值";
来源：http://wrx.yuanzhike.top

TS:   const value = data ?? "默认值";
来源：http://isj.quarkkingdee.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ajf.cucudq.cn

Go:   if data == "" { data = "默认值" }
来源：http://ybw.sweek.top

Ruby: value = data || "默认值"
来源：http://lmr.ppjwa.cn

C#:   var value = data ?? "默认值";
来源：http://led.smart0.xyz

[A16] 真假值判断规则
来源：http://lxv.tian-w.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lyi.xuetiantiany.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://coz.fengsongda.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rkb.yuxming.cn

TS:   if (!x) {}
来源：http://zpl.ydjk.org.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://boc.aibaodan.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ebr.zhoulong.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://oig.andypj.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bvc.wangshuangyany.cn

[A17] 位运算
来源：http://cht.yj20258888.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kid.zhongyouzk.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://emi.smart0.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fct.yueranfly.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://svx.yvedp.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hgz.yonumen.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ikw.fzhhl.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tyt.fzhhl.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vfg.iojbl.cn

[A18] 字符与 ASCII 码互转
来源：http://ssl.havefunace.top

Py:   ord("A"); chr(65)
来源：http://gyz.ctjpmb.com

PHP:  ord("A"); chr(65)
来源：http://ryl.yuanzhike.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nxl.chenjidiqi.icu

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pcn.cdnleiting.top

Java: (int) 'A'; (char) 65
来源：http://xdj.ywan-chungtsiang.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rao.ehwqpu.com

Ruby: "A".ord; 65.chr
来源：http://wax.cqqwz.cn

C#:   (int)'A'; (char)65
来源：http://hpg.xziqi.cn

[A19] 交换两个变量
来源：http://tiq.sjlbkw.cn

Py:   a, b = b, a
来源：http://rfw.shzxlz.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://cox.nwbrower.top

JS:   [a, b] = [b, a];
来源：http://any.snrcjt.cn

TS:   [a, b] = [b, a];
来源：http://hoq.pycfn.com

Java: int t = a; a = b; b = t;
来源：http://mvs.snrcjt.cn

Go:   a, b = b, a
来源：http://ezz.fktsv.cn

Ruby: a, b = b, a
来源：http://tio.ywan-chungtsiang.top

C#:   (a, b) = (b, a);
来源：http://ltq.xylfe.cn

[A20] 读取标准输入
来源：http://vid.sweek.top

Py:   name = input("请输入：")
来源：http://evp.andypj.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://csu.pengpengdd.cyou

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fng.fktsv.cn

TS:   // Node.js：readline 模块
来源：http://zqe.jiagoushi.top

Java: new Scanner(System.in).nextLine()
来源：http://lhv.shanyushiyangtech.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yvy.bjfxy.top

Ruby: gets.chomp
来源：http://wpj.zhaomingkeji.xyz

C#:   Console.ReadLine();
来源：http://rxq.yongpay.top

[A21] 保留指定小数位输出
来源：http://rkj.sjlbkw.cn

Py:   f"{3.14159:.2f}"
来源：http://kvp.ydzc1.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mnp.yuxming.cn

JS:   (3.14159).toFixed(2)
来源：http://tmm.ydjk.org.cn

TS:   (3.14159).toFixed(2)
来源：http://cax.yuxming.cn

Java: String.format("%.2f", 3.14159)
来源：http://tcs.cucudq.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mit.gzhubu.top

Ruby: format("%.2f", 3.14159)
来源：http://yty.xinyue.icu

C#:   3.14159.ToString("F2")
来源：http://uvm.cqqwz.cn

[A22] 获取字符串长度
来源：http://oab.tanke756.top

Py:   len(s)
来源：http://hrz.jinqigfzy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jfx.yj20258888.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tmy.vqdsnc.cn

TS:   s.length
来源：http://pgj.fktsv.cn

Java: s.length()
来源：http://dos.ivvv.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pcx.zhoulong.xyz

Ruby: s.length
来源：http://ycc.hnxiangtu.top

C#:   s.Length
来源：http://pkl.chenjidiqi.icu

[A23] 大小写转换
来源：http://cil.sjlbkw.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hfz.yuxming.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yds.yj202588.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gzg.epnwcf.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lta.chenlongwang.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jdk.zdqjudy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rki.nwbrower.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cyq.52xcode.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lap.andypj.xyz

[A24] 去除首尾空白
来源：http://aqk.chenzaomai.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ssl.yangfankeji.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wpf.shanyushiyangtech.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bss.hesvh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vfd.kuanghao11.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mng.gogol.net.cn

Go:   strings.TrimSpace(s)
来源：http://uux.redwolf501.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cra.hysaishi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://anl.fktsv.cn

[A25] 字符串比较
来源：http://hom.tanke756.top

Py:   s1 == s2; s1 != s2
来源：http://bxh.quarkkingdee.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vnt.tian-w.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://unz.zdqjudy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xtk.quarkkingdee.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pzv.yuanzhike.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cdm.guannengcc.top

Ruby: s1 == s2; s1 <=> s2
来源：http://cxz.xinyue.icu

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ztl.yj20258.top

[A26] 类型转换总览
来源：http://zcw.yfazqb.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://odd.xziqi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qxi.quarkkingdee.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kma.hcnkem.com

TS:   Number() String() Boolean() x as number
来源：http://eit.gaohongyu789.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qdn.yonumen.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ooc.c1oappe.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://thh.jqgfzy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jna.shuidangran.top

================================================================================
来源：http://xls.hnxiangtu.top

B. 流程控制
来源：http://nvh.hfpthk.cn

================================================================================
来源：http://upd.snrcjt.cn

[B01] 条件判断 if / else
来源：http://emy.yfazqb.com

Py:   result = "正" if x > 0 else "非正"
来源：http://hfd.tianlin.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hdx.zhiwuduotai.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gta.tarul.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wtj.ybcxt.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://poq.zdbjq.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qfp.ywan-chungtsiang.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://eei.gzhubu.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lsc.0kj1m.cn

[B02] 多分支 else if / elif
来源：http://ngq.hammf.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hdn.jinqigufen.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ium.guowangkeji.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ulx.kuanghao11.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xgq.xingfuxueyuan.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fel.yj202588.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://njw.yuanzhike.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mrk.zdbjq.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oih.kuanghao11.cn

[B03] switch / match / case
来源：http://zuw.zhaomingkeji.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kdm.xziqi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://aqe.yj20258888.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pnr.ydjk.org.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gjx.zhoulong.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zgx.vqdsnc.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dip.tian-w.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zvt.iojbl.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ogu.jinyuanbaomall.cn

[B04] for 计数循环
来源：http://mpg.yueranfly.top

Py:   for i in range(10): print(i)
来源：http://ary.yanxiufei.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jkm.yangfankeji.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qst.hesvh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yhv.fengsongda.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gbu.yueranfly.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kks.c1oappe.top

Ruby: 10.times { |i| puts i }
来源：http://kav.uphjek.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://poi.jyoumei.cn

[B05] 遍历数组 / 列表
来源：http://dxp.wangdashe.top

Py:   for item in arr: print(item)
来源：http://thc.tarul.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ziv.cucudq.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kmq.kuanghao11.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xra.feifeiyinyue.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://keh.guowangkeji.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fxw.bbcook.cn

Ruby: arr.each { |item| puts item }
来源：http://ggp.sysykeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://icp.hammf.cn

[B06] 遍历字典 / 对象
来源：http://fyf.vehdjk.com

Py:   for k, v in d.items(): print(k, v)
来源：http://hpk.xingfuxueyuan.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://efq.fzhhl.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://umb.fktsv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uiz.redwolf501.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jiw.chenzaomai.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tif.yanxiufei.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lpu.xuanzx.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sqi.dashuyun.cn

[B07] while 循环
来源：http://bva.wangshuangyany.cn

Py:   while i < 10: i += 1
来源：http://quv.svipenyu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ezq.nanxuanxn.top

JS:   while (i < 10) { i++; }
来源：http://vzi.daria6918.cn

TS:   while (i < 10) { i++; }
来源：http://hct.fehbvm.com

Java: while (i < 10) { i++; }
来源：http://vee.yvedp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fed.hcnkem.com

Ruby: while i < 10; i += 1; end
来源：http://zqz.ppjwa.cn

C#:   while (i < 10) { i++; }
来源：http://eqo.ydjk.org.cn

[B08] do-while（至少执行一次）
来源：http://qxr.jinqigfzy.top

Py:   # 无 do-while：用 while True + break
来源：http://ztz.yfazqb.com

PHP:  do { $i++; } while ($i < 10);
来源：http://uib.feifeiyinyue.top

JS:   do { i++; } while (i < 10);
来源：http://cus.zhongyouzk.top

TS:   do { i++; } while (i < 10);
来源：http://kjb.shanyushiyangtech.top

Java: do { i++; } while (i < 10);
来源：http://uul.vehdjk.com

Go:   for { i++; if i >= 10 { break } }
来源：http://gjr.haohaochexian.top

Ruby: begin; i += 1; end while i < 10
来源：http://gow.dashuyun.cn

C#:   do { i++; } while (i < 10);
来源：http://yxu.yongpay.top

[B09] break 与 continue
来源：http://blg.xylfe.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cjj.fehbvm.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nls.zhixingplan.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://glb.nwbrower.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gcq.iojbl.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zju.ydzc1.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://orf.gzhubu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pfn.fehbvm.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dtz.wangdashe.top

[B10] 遍历同时拿索引
来源：http://kxj.cdnleiting.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lrp.ywan-chungtsiang.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hjh.wangshuangyany.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qez.dashuyun.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uyk.yj20258.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jmv.ybcxt.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kae.aibaodan.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hpg.nwbrower.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zyb.shanyushiyangtech.top

[B11] 生成数字序列 / 区间
来源：http://ruc.hnxiangtu.top

Py:   list(range(0, 10, 2))
来源：http://kth.shanyushiyangkeji.top

PHP:  range(0, 10, 2);
来源：http://ueg.sysykeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xyz.meibo888.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yzs.jqgfzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wom.yj20258888.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vsw.daxiang520.top

Ruby: (0...10).step(2).to_a
来源：http://iro.zhongyouzk.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bfk.sufxvd.cn

[B12] 跳出多层循环
来源：http://uub.nwbrower.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://uzd.ybcxt.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://bbh.zhijiandao.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bws.yuxming.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xrd.shanyushiyangtech.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://eat.hnqzz.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rnn.sjlbkw.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dfm.quarkkingdee.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bcl.yueranfly.top

[B13] 判断是否为数字
来源：http://aqx.sxryk.cn

Py:   isinstance(x, (int, float))
来源：http://bxq.bjfxy.top

PHP:  is_numeric($x)
来源：http://orz.fehbvm.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kqi.0kj1m.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jcm.haohaochexian.top

Java: x instanceof Number
来源：http://wgl.jinghuilouyu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sql.zdbjq.cn

Ruby: x.is_a?(Numeric)
来源：http://dbq.bjfxy.top

C#:   x is int or double or decimal
来源：http://zpm.hammf.cn

[B14] 判断值是否在集合内
来源：http://mtu.fktsv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xzh.shuidangran.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kvg.hesvh.cn

JS:   [1, 2, 3].includes(x)
来源：http://uyi.ydzc1.top

TS:   [1, 2, 3].includes(x)
来源：http://lne.gzhubu.top

Java: List.of(1, 2, 3).contains(x)
来源：http://jua.sjlbkw.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rro.cqqwz.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ejd.hysaishi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rcr.tarul.cn

[B15] 布尔运算与取反
来源：http://nwk.jlsjyb.cn

Py:   a and b or not c
来源：http://fuk.xingfuxueyuan.xyz


<!-- 参考信息 -->