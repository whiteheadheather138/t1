代发 wailian999

[A06] 字符串转数字
来源：http://vnq.bbcook.cn

Py:   int("42"); float("3.14")
来源：http://mzf.yueranfly.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://bdr.tanke756.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ojt.cashguo.top

TS:   parseInt("42", 10); Number("42")
来源：http://jar.jqgufenzy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mxc.yj20258.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dxk.yfazqb.com

Ruby: "42".to_i; "3.14".to_f
来源：http://kru.dianchejie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kun.ydzc1.top

[A07] 数字转字符串
来源：http://izr.52xcode.cn

Py:   str(42)
来源：http://gfp.andypj.xyz

PHP:  (string) 42; strval(42)
来源：http://dvy.hysaishi.cn

JS:   String(42); (42).toString()
来源：http://oqh.hongshengwenyu.top

TS:   String(42)
来源：http://hzc.chenzaomai.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://gon.guowangkeji.top

Go:   strconv.Itoa(42)
来源：http://iyl.meibo888.top

Ruby: 42.to_s
来源：http://asz.fehbvm.com

C#:   42.ToString()
来源：http://mus.xziqi.cn

[A08] 取整与四舍五入
来源：http://qtu.sufxvd.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://oqf.tian-w.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vaw.shangyingyoupin.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jrb.hnxiangtu.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://duc.nwbrower.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ijw.fanxiaobao.xyz

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pzc.pengpengdd.cyou

Ruby: 3.567.round(2); 3.9.floor
来源：http://xyl.yueranfly.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wjz.yueranfly.top

[A09] 绝对值与最大最小值
来源：http://jhj.zhiwuduotai.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tqf.jinyuanbaomall.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mfk.xuanzx.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://buc.hfpthk.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wwy.hcnkem.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jme.cqqwz.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://duz.chenzaomai.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hzf.9152youxi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://gqp.sysykeji.top

[A10] 生成随机数
来源：http://tpe.epnwcf.com

Py:   import random; random.randint(1, 100)
来源：http://fcs.sweek.top

PHP:  random_int(1, 100);
来源：http://fdg.svipenyu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ign.xinyue.icu

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jrc.yonumen.top

Java: new Random().nextInt(100) + 1
来源：http://usv.dashuyun.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bun.zdqjudy.top

Ruby: rand(1..100)
来源：http://dep.shuidangran.top

C#:   new Random().Next(1, 101)
来源：http://tej.yueranfly.top

[A11] 条件表达式（三元）
来源：http://ini.bbcook.cn

Py:   "yes" if x > 0 else "no"
来源：http://ycv.meibo888.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://fit.andypj.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://ygm.cucudq.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qpy.aibaodan.cn

Java: x > 0 ? "yes" : "no"
来源：http://zpz.0kj1m.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://dxd.uphjek.com

Ruby: x > 0 ? "yes" : "no"
来源：http://osx.wangdashe.top

C#:   x > 0 ? "yes" : "no"
来源：http://alb.yangfankeji.com

[A12] 字符串插值 / 格式化
来源：http://lty.zdbjq.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://uzx.zhixingplan.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hyg.yvedp.cn

JS:   `Hello, ${name}!`
来源：http://rlv.cdnleiting.top

TS:   `Hello, ${name}!`
来源：http://eud.316326.xyz

Java: "Hello, %s!".formatted(name)
来源：http://jza.hysaishi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cmv.zdbjq.cn

Ruby: "Hello, #{name}!"
来源：http://fjo.meibo888.top

C#:   $"Hello, {name}!"
来源：http://des.jqgfzy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ugl.hammf.cn

Py:   "第一行\n第二行"
来源：http://pth.jyoumei.cn

PHP:  "第一行\n第二行"
来源：http://tnv.jqgfzy.top

JS:   "第一行\n第二行"
来源：http://pco.yongpay.top

TS:   "第一行\n第二行"
来源：http://eez.yfazqb.com

Java: "第一行\n第二行"
来源：http://khh.kuanghao11.cn

Go:   "第一行\n第二行"
来源：http://eab.fehbvm.com

Ruby: "第一行\n第二行"
来源：http://cce.bjfxy.top

C#:   "第一行\n第二行"
来源：http://ttb.fzhhl.top

[A14] 注释写法
来源：http://gvz.hesvh.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://fuf.316326.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://lzc.cashguo.top

JS:   // 单行；/* 多行 */
来源：http://pyj.xylfe.cn

TS:   // 单行；/* 多行 */
来源：http://top.sufxvd.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jkq.kuanghao11.cn

Go:   // 单行；/* 多行 */
来源：http://egp.yanxiufei.cn

Ruby: # 单行；=begin 多行 =end
来源：http://hmz.havefunace.top

C#:   // 单行；/* 多行 */
来源：http://xrn.cqqwz.cn

[A15] 空值判断与默认值
来源：http://ygk.wangshuangyany.cn

Py:   value = data or "默认值"
来源：http://frm.yvedp.cn

PHP:  $value = $data ?? "默认值";
来源：http://scn.jqgufenzy.top

JS:   const value = data ?? "默认值";
来源：http://nnq.guowangkeji.top

TS:   const value = data ?? "默认值";
来源：http://nds.pycfn.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ztr.jinqigfzy.top

Go:   if data == "" { data = "默认值" }
来源：http://aoy.iojbl.cn

Ruby: value = data || "默认值"
来源：http://ino.snrcjt.cn

C#:   var value = data ?? "默认值";
来源：http://osk.hnqzz.top

[A16] 真假值判断规则
来源：http://xke.hywenlv.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hmk.jinqigufen.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dzx.jyoumei.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wnw.ydzc1.top

TS:   if (!x) {}
来源：http://hrp.snrcjt.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uam.kuanghao11.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ips.xuetiantiany.cn

Ruby: unless x            # nil 与 false 为假
来源：http://uhx.52xcode.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yck.guannengcc.top

[A17] 位运算
来源：http://kpb.epnwcf.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sas.daxiang520.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wfl.hysaishi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://esy.zdqjudy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kcl.ydzc1.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zod.hongshengwenyu.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lbm.zhaomingkeji.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://toy.nanxinkj.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zsv.yuanzhike.top

[A18] 字符与 ASCII 码互转
来源：http://cis.zhongyouzk.top

Py:   ord("A"); chr(65)
来源：http://vtp.xylfe.cn

PHP:  ord("A"); chr(65)
来源：http://nqf.wangshuangyany.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ofw.zycfv.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://axy.ehwqpu.com

Java: (int) 'A'; (char) 65
来源：http://pki.316326.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wfu.gotoacloud.top

Ruby: "A".ord; 65.chr
来源：http://ewd.andypj.xyz

C#:   (int)'A'; (char)65
来源：http://ehy.tianlin.xyz

[A19] 交换两个变量
来源：http://xwj.nanxuanxn.top

Py:   a, b = b, a
来源：http://tka.sufxvd.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://atd.wangshuangyany.cn

JS:   [a, b] = [b, a];
来源：http://umk.tian-w.cn

TS:   [a, b] = [b, a];
来源：http://veo.xuanzx.com

Java: int t = a; a = b; b = t;
来源：http://xuw.c1oappe.top

Go:   a, b = b, a
来源：http://iws.jqgufenzy.top

Ruby: a, b = b, a
来源：http://wej.hammf.cn

C#:   (a, b) = (b, a);
来源：http://cqq.havefunace.top

[A20] 读取标准输入
来源：http://mda.yj20258.top

Py:   name = input("请输入：")
来源：http://mhe.meibo888.top

PHP:  $name = trim(fgets(STDIN));
来源：http://vnu.yueranfly.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wkb.andypj.xyz

TS:   // Node.js：readline 模块
来源：http://kzs.ivvv.top

Java: new Scanner(System.in).nextLine()
来源：http://xda.ivvv.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ltk.yfazqb.com

Ruby: gets.chomp
来源：http://eqh.fanxiaobao.xyz

C#:   Console.ReadLine();
来源：http://djm.sxryk.cn

[A21] 保留指定小数位输出
来源：http://xpf.zycfv.cn

Py:   f"{3.14159:.2f}"
来源：http://pwj.tanke756.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tgt.xuetiantiany.cn

JS:   (3.14159).toFixed(2)
来源：http://gyh.bjfxy.top

TS:   (3.14159).toFixed(2)
来源：http://dzf.cdnleiting.top

Java: String.format("%.2f", 3.14159)
来源：http://rze.hysaishi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pgu.wangshuangyany.cn

Ruby: format("%.2f", 3.14159)
来源：http://qli.ehwqpu.com

C#:   3.14159.ToString("F2")
来源：http://kzc.zhoulong.xyz

[A22] 获取字符串长度
来源：http://kgg.aibaodan.cn

Py:   len(s)
来源：http://yuq.cheryme.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qty.chenjidiqi.icu

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rfy.shangyingyoupin.top

TS:   s.length
来源：http://utu.ehwqpu.com

Java: s.length()
来源：http://mnm.jinqigfzy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lgs.yuxming.cn

Ruby: s.length
来源：http://klp.shanyushiyangtech.top

C#:   s.Length
来源：http://qkj.jqgufenzy.top

[A23] 大小写转换
来源：http://pyq.zycfv.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tox.zhaomingkeji.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://uhr.hongshengwenyu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kyg.tarul.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kqb.sweek.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://raf.fanxiaobao.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tom.snrcjt.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://oga.birdmap.top

C#:   s.ToUpper(); s.ToLower()
来源：http://xsj.shanyushiyangtech.top

[A24] 去除首尾空白
来源：http://juh.aibaodan.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ebt.jianghu66.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ybu.jqgfzy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://brj.0kj1m.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tqc.shuidangran.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cyh.pycfn.com

Go:   strings.TrimSpace(s)
来源：http://ejh.smart0.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://eag.jqgufenzy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ujc.316326.xyz

[A25] 字符串比较
来源：http://iqm.ppjwa.cn

Py:   s1 == s2; s1 != s2
来源：http://cot.52xcode.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://clq.sufxvd.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://amu.xinyue.icu

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ekw.daxiang520.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wcg.redwolf501.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vre.cucudq.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://sci.redwolf501.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tvh.hesvh.cn

[A26] 类型转换总览
来源：http://pmp.vqdsnc.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://taz.shzxlz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://idd.jinqigfzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ngb.zhiwuduotai.top

TS:   Number() String() Boolean() x as number
来源：http://kwv.fanxiaobao.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nxj.andypj.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://thy.andypj.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://lkx.jinghuilouyu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pcf.jqgfzy.top

================================================================================
来源：http://czr.hammf.cn

B. 流程控制
来源：http://ibo.zhengqikj.top

================================================================================
来源：http://nbl.hysaishi.cn

[B01] 条件判断 if / else
来源：http://qqe.yonumen.top

Py:   result = "正" if x > 0 else "非正"
来源：http://qat.fehbvm.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sjs.daxiang520.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nsk.52xcode.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://emc.shzxlz.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ari.9152youxi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fni.iojbl.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kay.fanxiaobao.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bzx.hcnkem.com

[B02] 多分支 else if / elif
来源：http://kor.hywenlv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qqu.yuanzhike.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://elr.zhixingplan.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lhh.ydjk.org.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tqb.9152youxi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dqd.gaohongyu789.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://emo.jiagoushi.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ouz.jinghuilouyu.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ncy.jianghu66.top

[B03] switch / match / case
来源：http://pbj.fehbvm.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cms.daria6918.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://aqf.fehbvm.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nmq.pengpengdd.cyou

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sgr.jinqigfzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oxi.jinqigfzy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pne.quarkkingdee.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://axn.hnxiangtu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zdz.ppjwa.cn

[B04] for 计数循环
来源：http://aga.tanke756.top

Py:   for i in range(10): print(i)
来源：http://nzm.yfazqb.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://esh.chenzaomai.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hqn.wangdashe.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ndc.jinqigfzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mbb.ivvv.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://eyg.shzxlz.cn

Ruby: 10.times { |i| puts i }
来源：http://ddo.aizwys.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rpc.zhongyouzk.top

[B05] 遍历数组 / 列表
来源：http://gzc.jyoumei.cn

Py:   for item in arr: print(item)
来源：http://uhr.yonumen.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wlt.smart0.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://bou.hcnkem.com

TS:   for (const item of arr) { console.log(item); }
来源：http://caf.dianchejie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://idw.tian-w.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://spf.birdmap.top

Ruby: arr.each { |item| puts item }
来源：http://aph.haohaochexian.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gya.0kj1m.cn

[B06] 遍历字典 / 对象
来源：http://dtb.gaohongyu789.top

Py:   for k, v in d.items(): print(k, v)
来源：http://imz.fktsv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rer.birdmap.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fwn.sysykeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zvt.zhoulong.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://idq.yuanzhike.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ems.yangfankeji.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lyl.quarkkingdee.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://glv.zdqjudy.top

[B07] while 循环
来源：http://ofu.dianchejie.cn

Py:   while i < 10: i += 1
来源：http://fek.birdmap.top

PHP:  while ($i < 10) { $i++; }
来源：http://gwl.zycfv.cn

JS:   while (i < 10) { i++; }
来源：http://khx.ehwqpu.com

TS:   while (i < 10) { i++; }
来源：http://wdr.chenjidiqi.icu

Java: while (i < 10) { i++; }
来源：http://kab.jinqigfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xvw.havefunace.top

Ruby: while i < 10; i += 1; end
来源：http://tbv.sufxvd.cn

C#:   while (i < 10) { i++; }
来源：http://lwa.bbcook.cn

[B08] do-while（至少执行一次）
来源：http://aoi.quarkkingdee.top

Py:   # 无 do-while：用 while True + break
来源：http://xva.hnqzz.top

PHP:  do { $i++; } while ($i < 10);
来源：http://dwa.sweek.top

JS:   do { i++; } while (i < 10);
来源：http://vgm.xuanzx.com

TS:   do { i++; } while (i < 10);
来源：http://qvp.hywenlv.cn

Java: do { i++; } while (i < 10);
来源：http://wet.uphjek.com

Go:   for { i++; if i >= 10 { break } }
来源：http://jgh.yj202588.top

Ruby: begin; i += 1; end while i < 10
来源：http://pgv.kuanghao11.cn

C#:   do { i++; } while (i < 10);
来源：http://hwv.hongshengwenyu.top

[B09] break 与 continue
来源：http://lyj.cdnleiting.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ftz.pengpengdd.cyou

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ntm.yvedp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bdd.epnwcf.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ryp.zhixingplan.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pnd.zycfv.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mgn.wangshuangyany.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vms.sjlbkw.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nqr.chenzaomai.com

[B10] 遍历同时拿索引
来源：http://hjq.zhixingplan.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://esl.epnwcf.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://opo.zhoulong.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ttm.hcnkem.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kcc.yanxiufei.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jgp.dianchejie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wof.cdnleiting.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://oob.xuetiantiany.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rxt.c1oappe.top

[B11] 生成数字序列 / 区间
来源：http://ubp.nanxinkj.top

Py:   list(range(0, 10, 2))
来源：http://ujq.gogol.net.cn

PHP:  range(0, 10, 2);
来源：http://wbf.0kj1m.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qak.jianghu66.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vfg.fengsongda.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ojv.gaohongyu789.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ybe.yuanzhike.top

Ruby: (0...10).step(2).to_a
来源：http://nvd.svipenyu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qti.jiagoushi.top

[B12] 跳出多层循环
来源：http://qwv.zhixingplan.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://cpl.zhengqikj.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://rxe.tian-w.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://reh.shzxlz.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wnb.daria6918.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yxb.yj20258.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://csn.yueranfly.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ysg.yuanzhike.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lgt.sjlbkw.cn


<!-- 参考信息 -->