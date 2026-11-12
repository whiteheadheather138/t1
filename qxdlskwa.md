代发 wailian999

[A06] 字符串转数字
来源：http://kmb.svipenyu.cn

Py:   int("42"); float("3.14")
来源：http://qxo.hesvh.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://heg.xuetiantiany.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ach.yj20258888.top

TS:   parseInt("42", 10); Number("42")
来源：http://gpk.vehdjk.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kzl.aizwys.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dxu.jinqigfzy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://gek.dashuyun.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gxp.ppjwa.cn

[A07] 数字转字符串
来源：http://ini.wangshuangyany.cn

Py:   str(42)
来源：http://khh.zycfv.cn

PHP:  (string) 42; strval(42)
来源：http://syp.havefunace.top

JS:   String(42); (42).toString()
来源：http://mmj.chenlongwang.top

TS:   String(42)
来源：http://wgg.zhengqikj.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://xvt.ywan-chungtsiang.top

Go:   strconv.Itoa(42)
来源：http://scf.haohaochexian.top

Ruby: 42.to_s
来源：http://eso.redwolf501.top

C#:   42.ToString()
来源：http://yvw.quarkkingdee.top

[A08] 取整与四舍五入
来源：http://xoq.yj202588.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lov.jinghuilouyu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dia.yj202588.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kdg.jlsjyb.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cfd.zycfv.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kte.tarul.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://pmq.zhaomingkeji.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://ajm.redwolf501.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://eqy.sysykeji.top

[A09] 绝对值与最大最小值
来源：http://anr.sysykeji.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vbf.52xcode.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xzo.nanxinkj.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fej.chenjidiqi.icu

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ref.bjfxy.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pcj.cheryme.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rkt.xuetiantiany.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kuh.hnqzz.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hus.yanxiufei.cn

[A10] 生成随机数
来源：http://lbs.sxryk.cn

Py:   import random; random.randint(1, 100)
来源：http://efq.yj202588.top

PHP:  random_int(1, 100);
来源：http://oxj.yueranfly.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://azn.fehbvm.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lwz.ybcxt.top

Java: new Random().nextInt(100) + 1
来源：http://kzc.aizwys.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tan.ydzc1.top

Ruby: rand(1..100)
来源：http://arl.jlsjyb.cn

C#:   new Random().Next(1, 101)
来源：http://ckh.guowangkeji.top

[A11] 条件表达式（三元）
来源：http://auw.ywan-chungtsiang.top

Py:   "yes" if x > 0 else "no"
来源：http://ecs.zhijiandao.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://tiz.316326.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://kvj.xingfuxueyuan.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://kuh.gogol.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://vbv.cqqwz.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://kcy.zhongyouzk.top

Ruby: x > 0 ? "yes" : "no"
来源：http://rio.jianghu66.top

C#:   x > 0 ? "yes" : "no"
来源：http://kfp.jyoumei.cn

[A12] 字符串插值 / 格式化
来源：http://mku.hysaishi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://cxy.xuetiantiany.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tzd.gaohongyu789.top

JS:   `Hello, ${name}!`
来源：http://gtt.yongpay.top

TS:   `Hello, ${name}!`
来源：http://pph.guowangkeji.top

Java: "Hello, %s!".formatted(name)
来源：http://rbt.0kj1m.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dfn.wangdashe.top

Ruby: "Hello, #{name}!"
来源：http://sfn.pycfn.com

C#:   $"Hello, {name}!"
来源：http://ajt.dashuyun.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://bfu.fengsongda.top

Py:   "第一行\n第二行"
来源：http://xsq.uphjek.com

PHP:  "第一行\n第二行"
来源：http://krl.9152youxi.cn

JS:   "第一行\n第二行"
来源：http://swb.jianghu66.top

TS:   "第一行\n第二行"
来源：http://cea.pycfn.com

Java: "第一行\n第二行"
来源：http://pyr.zhongyouzk.top

Go:   "第一行\n第二行"
来源：http://cgj.vqdsnc.cn

Ruby: "第一行\n第二行"
来源：http://cxt.ivvv.top

C#:   "第一行\n第二行"
来源：http://vau.daria6918.cn

[A14] 注释写法
来源：http://syl.ppjwa.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://mrr.ydzc1.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://zev.sxryk.cn

JS:   // 单行；/* 多行 */
来源：http://itq.quarkkingdee.top

TS:   // 单行；/* 多行 */
来源：http://ojm.quarkkingdee.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cfr.hongshengwenyu.top

Go:   // 单行；/* 多行 */
来源：http://ghc.jqgufenzy.top

Ruby: # 单行；=begin 多行 =end
来源：http://fmi.sysykeji.top

C#:   // 单行；/* 多行 */
来源：http://rcl.bjfxy.top

[A15] 空值判断与默认值
来源：http://ggj.sxryk.cn

Py:   value = data or "默认值"
来源：http://ioe.9152youxi.cn

PHP:  $value = $data ?? "默认值";
来源：http://aph.zhengqikj.top

JS:   const value = data ?? "默认值";
来源：http://wcx.yangfankeji.com

TS:   const value = data ?? "默认值";
来源：http://xol.cqqwz.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rtd.ydzc1.top

Go:   if data == "" { data = "默认值" }
来源：http://wbn.jinyuanbaomall.cn

Ruby: value = data || "默认值"
来源：http://xym.yfazqb.com

C#:   var value = data ?? "默认值";
来源：http://gec.hywenlv.cn

[A16] 真假值判断规则
来源：http://chi.ivvv.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cwj.birdmap.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://uoi.chenjidiqi.icu

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ygg.wangshuangyany.cn

TS:   if (!x) {}
来源：http://btv.wangshuangyany.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://icj.hcnkem.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cnv.wangshuangyany.cn

Ruby: unless x            # nil 与 false 为假
来源：http://noz.hysaishi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xzf.hcnkem.com

[A17] 位运算
来源：http://qwg.yuxming.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://arn.hesvh.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gaj.cdnleiting.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vgd.gaohongyu789.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ils.zhengqikj.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cym.daxiang520.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gma.yanxiufei.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nof.jinqigufen.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ptg.chenlongwang.top

[A18] 字符与 ASCII 码互转
来源：http://qzi.jinghuilouyu.cn

Py:   ord("A"); chr(65)
来源：http://dvq.feifeiyinyue.top

PHP:  ord("A"); chr(65)
来源：http://xhp.xylfe.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bsz.bbcook.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kab.jinqigfzy.top

Java: (int) 'A'; (char) 65
来源：http://vtq.daxiang520.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mzb.redwolf501.top

Ruby: "A".ord; 65.chr
来源：http://fyn.gogol.net.cn

C#:   (int)'A'; (char)65
来源：http://jko.birdmap.top

[A19] 交换两个变量
来源：http://pyc.gotoacloud.top

Py:   a, b = b, a
来源：http://gqb.shuidangran.top

PHP:  [$a, $b] = [$b, $a];
来源：http://xhs.hongshengwenyu.top

JS:   [a, b] = [b, a];
来源：http://nby.pengpengdd.cyou

TS:   [a, b] = [b, a];
来源：http://xnn.yj202588.top

Java: int t = a; a = b; b = t;
来源：http://nkq.zhiwuduotai.top

Go:   a, b = b, a
来源：http://kjj.jiagoushi.top

Ruby: a, b = b, a
来源：http://xxu.sweek.top

C#:   (a, b) = (b, a);
来源：http://iei.sufxvd.cn

[A20] 读取标准输入
来源：http://gby.jinghuilouyu.cn

Py:   name = input("请输入：")
来源：http://xal.yonumen.top

PHP:  $name = trim(fgets(STDIN));
来源：http://hcs.xziqi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ubk.jiagoushi.top

TS:   // Node.js：readline 模块
来源：http://xce.hongshengwenyu.top

Java: new Scanner(System.in).nextLine()
来源：http://ygc.xingfuxueyuan.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://omu.ehwqpu.com

Ruby: gets.chomp
来源：http://ciq.sweek.top

C#:   Console.ReadLine();
来源：http://ibu.yangfankeji.com

[A21] 保留指定小数位输出
来源：http://jqf.ivvv.top

Py:   f"{3.14159:.2f}"
来源：http://uso.hnqzz.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://buw.jinyuanbaomall.cn

JS:   (3.14159).toFixed(2)
来源：http://rps.jinghuilouyu.cn

TS:   (3.14159).toFixed(2)
来源：http://ywu.nwbrower.top

Java: String.format("%.2f", 3.14159)
来源：http://wlt.xziqi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tht.guannengcc.top

Ruby: format("%.2f", 3.14159)
来源：http://hna.ctjpmb.com

C#:   3.14159.ToString("F2")
来源：http://ngr.yangfankeji.com

[A22] 获取字符串长度
来源：http://gth.tianlin.xyz

Py:   len(s)
来源：http://wys.zhengqikj.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dkl.hcnkem.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bjo.xylfe.cn

TS:   s.length
来源：http://hjp.haohaochexian.top

Java: s.length()
来源：http://siq.cashguo.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wrf.zhixingplan.top

Ruby: s.length
来源：http://ngt.bbcook.cn

C#:   s.Length
来源：http://qtf.tian-w.cn

[A23] 大小写转换
来源：http://kgb.redwolf501.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ufu.fzhhl.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kbp.chenzaomai.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fzx.jqgufenzy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lrx.zdbjq.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://txr.ydzc1.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nui.pycfn.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ldn.hywenlv.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ixr.uphjek.com

[A24] 去除首尾空白
来源：http://lim.bjfxy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tzl.xylfe.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://abl.hammf.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fbu.zhengqikj.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ukq.jinyuanbaomall.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ugs.andypj.xyz

Go:   strings.TrimSpace(s)
来源：http://ceg.yvedp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nau.hnxiangtu.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://knw.yuxming.cn

[A25] 字符串比较
来源：http://ahj.dianchejie.cn

Py:   s1 == s2; s1 != s2
来源：http://wwc.yuxming.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://piz.bbcook.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://adt.fanxiaobao.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ath.sufxvd.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gdj.quarkkingdee.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tnh.xuetiantiany.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wym.andypj.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vfh.svipenyu.cn

[A26] 类型转换总览
来源：http://yyk.zycfv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bxs.epnwcf.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rig.9152youxi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yus.xziqi.cn

TS:   Number() String() Boolean() x as number
来源：http://atl.tianlin.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fzt.nanxuanxn.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://edt.yonumen.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://gfc.hfpthk.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cfj.hnqzz.top

================================================================================
来源：http://tpc.gaohongyu789.top

B. 流程控制
来源：http://upk.zdqjudy.top

================================================================================
来源：http://yeu.zycfv.cn

[B01] 条件判断 if / else
来源：http://yym.sysykeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://zyl.gzhubu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qti.316326.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://byl.xuanzx.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fxh.fengsongda.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://mgq.redwolf501.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mtd.hongshengwenyu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wdo.gaohongyu789.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://otw.tian-w.cn

[B02] 多分支 else if / elif
来源：http://crj.shanyushiyangkeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sxx.aizwys.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://psx.haohaochexian.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ysu.vehdjk.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rdt.guowangkeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ufr.hysaishi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iib.hnqzz.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jos.xuetiantiany.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://alx.ehwqpu.com

[B03] switch / match / case
来源：http://lkg.chenzaomai.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://drk.uphjek.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vum.ehwqpu.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uyb.hesvh.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yig.52xcode.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zhi.hammf.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://atv.jinqigfzy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pnh.fehbvm.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jjk.jlsjyb.cn

[B04] for 计数循环
来源：http://smt.pengpengdd.cyou

Py:   for i in range(10): print(i)
来源：http://nfv.zhiwuduotai.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://eba.fzhhl.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mlj.cqqwz.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gqm.tianlin.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bry.sufxvd.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gyh.zhixingplan.top

Ruby: 10.times { |i| puts i }
来源：http://gyb.sweek.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lie.cheryme.top

[B05] 遍历数组 / 列表
来源：http://kii.tanke756.top

Py:   for item in arr: print(item)
来源：http://xmc.xinyue.icu

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jhq.zhongyouzk.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vsu.jianghu66.top

TS:   for (const item of arr) { console.log(item); }
来源：http://tgl.xinyue.icu

Java: for (var item : arr) { System.out.println(item); }
来源：http://kku.ehwqpu.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zij.hnxiangtu.top

Ruby: arr.each { |item| puts item }
来源：http://uzm.shanyushiyangkeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://imv.hammf.cn

[B06] 遍历字典 / 对象
来源：http://cjl.sjlbkw.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vil.xuetiantiany.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vog.sxryk.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jot.jiagoushi.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ayg.birdmap.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ubk.hongshengwenyu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xnw.jianghu66.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ieo.tianlin.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wad.yj20258.top

[B07] while 循环
来源：http://kpp.jyoumei.cn

Py:   while i < 10: i += 1
来源：http://xok.fanxiaobao.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://tnj.dianchejie.cn

JS:   while (i < 10) { i++; }
来源：http://hos.yongpay.top

TS:   while (i < 10) { i++; }
来源：http://xkp.yuanzhike.top

Java: while (i < 10) { i++; }
来源：http://fwz.svipenyu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cks.jyoumei.cn

Ruby: while i < 10; i += 1; end
来源：http://rgq.tanke756.top

C#:   while (i < 10) { i++; }
来源：http://iwf.ivvv.top

[B08] do-while（至少执行一次）
来源：http://uhd.birdmap.top

Py:   # 无 do-while：用 while True + break
来源：http://pyy.havefunace.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jha.fanxiaobao.xyz

JS:   do { i++; } while (i < 10);
来源：http://wfe.yj202588.top

TS:   do { i++; } while (i < 10);
来源：http://hpm.pycfn.com

Java: do { i++; } while (i < 10);
来源：http://njy.zhongyouzk.top

Go:   for { i++; if i >= 10 { break } }
来源：http://agi.jqgfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://bbh.xuetiantiany.cn

C#:   do { i++; } while (i < 10);
来源：http://esu.316326.xyz

[B09] break 与 continue
来源：http://ish.fzhhl.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://meh.smart0.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nhj.ehwqpu.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qog.xuetiantiany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zsq.bbcook.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://atb.52xcode.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nxs.sysykeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dkk.ivvv.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cjv.haohaochexian.top

[B10] 遍历同时拿索引
来源：http://gck.zhongyouzk.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hql.jqgfzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uwq.mhx1999.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jzo.jianghu66.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://syz.yonumen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bfs.c1oappe.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tzl.sysykeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zet.tarul.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qvz.redwolf501.top

[B11] 生成数字序列 / 区间
来源：http://gdr.zhengqikj.top

Py:   list(range(0, 10, 2))
来源：http://yks.vqdsnc.cn

PHP:  range(0, 10, 2);
来源：http://lbq.xingfuxueyuan.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lpy.snrcjt.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pxp.xingfuxueyuan.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://laq.yongpay.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ved.snrcjt.cn

Ruby: (0...10).step(2).to_a
来源：http://snt.ywan-chungtsiang.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://psy.ctjpmb.com

[B12] 跳出多层循环
来源：http://mdz.tanke756.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://roc.fengsongda.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://bor.guowangkeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gdq.fzhhl.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ucf.zhengqikj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kxh.yuanzhike.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oue.jinyuanbaomall.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pwt.redwolf501.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://alw.ehwqpu.com


<!-- 参考信息 -->