代发 wailian999

JS:   String(42); (42).toString()
来源：http://erw.sxryk.cn

TS:   String(42)
来源：http://qqv.xuanzx.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://xwp.zhoulong.xyz

Go:   strconv.Itoa(42)
来源：http://muf.bjfxy.top

Ruby: 42.to_s
来源：http://gfx.fanxiaobao.xyz

C#:   42.ToString()
来源：http://myz.shanyushiyangkeji.top

[A08] 取整与四舍五入
来源：http://wqf.yuanzhike.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gwj.ybcxt.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rxi.epnwcf.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ifd.shzxlz.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xwq.tarul.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ckw.nwbrower.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ngf.ppjwa.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ein.yanxiufei.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ntt.shanyushiyangtech.top

[A09] 绝对值与最大最小值
来源：http://mdu.yangfankeji.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qmg.zdqjudy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bkc.xuanzx.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://had.guowangkeji.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bbe.cucudq.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://vde.ehwqpu.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://oot.yvedp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fyf.xuetiantiany.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xzp.tianlin.xyz

[A10] 生成随机数
来源：http://dtu.zhiwuduotai.top

Py:   import random; random.randint(1, 100)
来源：http://age.zhijiandao.cn

PHP:  random_int(1, 100);
来源：http://mac.xziqi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://avo.havefunace.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qlw.jqgfzy.top

Java: new Random().nextInt(100) + 1
来源：http://did.yj202588.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://djw.bjfxy.top

Ruby: rand(1..100)
来源：http://uqy.0kj1m.cn

C#:   new Random().Next(1, 101)
来源：http://ile.pycfn.com

[A11] 条件表达式（三元）
来源：http://hps.daria6918.cn

Py:   "yes" if x > 0 else "no"
来源：http://ewh.aizwys.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ycj.zhiwuduotai.top

JS:   x > 0 ? "yes" : "no"
来源：http://piq.sysykeji.top

TS:   x > 0 ? "yes" : "no"
来源：http://vxm.tanke756.top

Java: x > 0 ? "yes" : "no"
来源：http://esb.birdmap.top

Go:   // 无三元运算符，需用 if 语句
来源：http://hwy.cheryme.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ayg.wangshuangyany.cn

C#:   x > 0 ? "yes" : "no"
来源：http://czm.0kj1m.cn

[A12] 字符串插值 / 格式化
来源：http://nor.fanxiaobao.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qsg.hysaishi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fkg.jianghu66.top

JS:   `Hello, ${name}!`
来源：http://tll.yangfankeji.com

TS:   `Hello, ${name}!`
来源：http://tcz.hongshengwenyu.top

Java: "Hello, %s!".formatted(name)
来源：http://cvd.epnwcf.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qgo.yanxiufei.cn

Ruby: "Hello, #{name}!"
来源：http://mqx.cashguo.top

C#:   $"Hello, {name}!"
来源：http://dfl.xuanzx.com

[A13] 多行字符串（练习 \n 转义）
来源：http://nmq.hysaishi.cn

Py:   "第一行\n第二行"
来源：http://efb.hesvh.cn

PHP:  "第一行\n第二行"
来源：http://awx.vqdsnc.cn

JS:   "第一行\n第二行"
来源：http://uzg.kuanghao11.cn

TS:   "第一行\n第二行"
来源：http://zmf.jqgufenzy.top

Java: "第一行\n第二行"
来源：http://keg.chenzaomai.com

Go:   "第一行\n第二行"
来源：http://jvi.daxiang520.top

Ruby: "第一行\n第二行"
来源：http://bhd.zhixingplan.top

C#:   "第一行\n第二行"
来源：http://mui.jiagoushi.top

[A14] 注释写法
来源：http://afa.jinqigufen.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://xvl.c1oappe.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://zac.zdbjq.cn

JS:   // 单行；/* 多行 */
来源：http://tll.fengsongda.top

TS:   // 单行；/* 多行 */
来源：http://aqw.daria6918.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ccf.ivvv.top

Go:   // 单行；/* 多行 */
来源：http://ela.aibaodan.cn

Ruby: # 单行；=begin 多行 =end
来源：http://zla.yfazqb.com

C#:   // 单行；/* 多行 */
来源：http://kcy.zhongyouzk.top

[A15] 空值判断与默认值
来源：http://plq.vehdjk.com

Py:   value = data or "默认值"
来源：http://sut.xuanzx.com

PHP:  $value = $data ?? "默认值";
来源：http://zil.jinyuanbaomall.cn

JS:   const value = data ?? "默认值";
来源：http://rtt.fengsongda.top

TS:   const value = data ?? "默认值";
来源：http://zat.yfazqb.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://via.gzhubu.top

Go:   if data == "" { data = "默认值" }
来源：http://egh.jqgfzy.top

Ruby: value = data || "默认值"
来源：http://jci.gaohongyu789.top

C#:   var value = data ?? "默认值";
来源：http://xdz.shuidangran.top

[A16] 真假值判断规则
来源：http://zpb.chenzaomai.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ivy.yonumen.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tmv.tarul.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://axu.jinqigfzy.top

TS:   if (!x) {}
来源：http://gev.ehwqpu.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mkc.tarul.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://awu.jinqigufen.top

Ruby: unless x            # nil 与 false 为假
来源：http://owj.yj20258888.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lld.daria6918.cn

[A17] 位运算
来源：http://ifi.daria6918.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ivf.tianlin.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mzi.wangshuangyany.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rak.jianghu66.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://brm.xinyue.icu

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lfu.zhixingplan.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ipf.quarkkingdee.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xkd.shzxlz.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gtn.pengpengdd.cyou

[A18] 字符与 ASCII 码互转
来源：http://seg.daria6918.cn

Py:   ord("A"); chr(65)
来源：http://kce.nanxinkj.top

PHP:  ord("A"); chr(65)
来源：http://eix.hesvh.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ixj.xingfuxueyuan.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iei.jiagoushi.top

Java: (int) 'A'; (char) 65
来源：http://ghf.shuidangran.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bax.gotoacloud.top

Ruby: "A".ord; 65.chr
来源：http://nia.snrcjt.cn

C#:   (int)'A'; (char)65
来源：http://aaa.jlsjyb.cn

[A19] 交换两个变量
来源：http://qvn.dianchejie.cn

Py:   a, b = b, a
来源：http://ydw.ydzc1.top

PHP:  [$a, $b] = [$b, $a];
来源：http://jrt.shanyushiyangtech.top

JS:   [a, b] = [b, a];
来源：http://dum.9152youxi.cn

TS:   [a, b] = [b, a];
来源：http://czt.yvedp.cn

Java: int t = a; a = b; b = t;
来源：http://wob.sweek.top

Go:   a, b = b, a
来源：http://ubo.daria6918.cn

Ruby: a, b = b, a
来源：http://sei.sxryk.cn

C#:   (a, b) = (b, a);
来源：http://jdj.birdmap.top

[A20] 读取标准输入
来源：http://ebj.dashuyun.cn

Py:   name = input("请输入：")
来源：http://rfw.xuetiantiany.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://hwn.zdbjq.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vhf.zhengqikj.top

TS:   // Node.js：readline 模块
来源：http://jge.cucudq.cn

Java: new Scanner(System.in).nextLine()
来源：http://hjg.dashuyun.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ida.hnqzz.top

Ruby: gets.chomp
来源：http://ffj.shzxlz.cn

C#:   Console.ReadLine();
来源：http://qdr.cheryme.top

[A21] 保留指定小数位输出
来源：http://hxq.tianlin.xyz

Py:   f"{3.14159:.2f}"
来源：http://ubs.yj202588.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mqh.ivvv.top

JS:   (3.14159).toFixed(2)
来源：http://yty.sufxvd.cn

TS:   (3.14159).toFixed(2)
来源：http://czc.ydjk.org.cn

Java: String.format("%.2f", 3.14159)
来源：http://kkn.zdqjudy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hcb.cucudq.cn

Ruby: format("%.2f", 3.14159)
来源：http://lod.zhijiandao.cn

C#:   3.14159.ToString("F2")
来源：http://gwd.tian-w.cn

[A22] 获取字符串长度
来源：http://rnh.jlsjyb.cn

Py:   len(s)
来源：http://ufz.cucudq.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tox.jinyuanbaomall.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ubn.hfpthk.cn

TS:   s.length
来源：http://fvp.kuanghao11.cn

Java: s.length()
来源：http://lei.svipenyu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cno.ppjwa.cn

Ruby: s.length
来源：http://oiy.zhaomingkeji.xyz

C#:   s.Length
来源：http://utw.pycfn.com

[A23] 大小写转换
来源：http://adl.ivvv.top

Py:   s.upper(); s.lower(); s.title()
来源：http://frv.birdmap.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jok.zhaomingkeji.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rih.hesvh.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wtj.hcnkem.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pyt.nwbrower.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xfo.hnqzz.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://urk.zhiwuduotai.top

C#:   s.ToUpper(); s.ToLower()
来源：http://shq.yangfankeji.com

[A24] 去除首尾空白
来源：http://qae.gotoacloud.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wbi.tianlin.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://njj.hfpthk.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iet.cdnleiting.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://txn.uphjek.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cue.hammf.cn

Go:   strings.TrimSpace(s)
来源：http://roh.sysykeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mkg.sweek.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yvz.iojbl.cn

[A25] 字符串比较
来源：http://msd.epnwcf.com

Py:   s1 == s2; s1 != s2
来源：http://ikh.guannengcc.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uet.vqdsnc.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hlb.guannengcc.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pcw.sjlbkw.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vne.hysaishi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xfo.zhiwuduotai.top

Ruby: s1 == s2; s1 <=> s2
来源：http://nlj.zhengqikj.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://oxe.9152youxi.cn

[A26] 类型转换总览
来源：http://yvt.nanxuanxn.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nhi.quarkkingdee.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://iti.yongpay.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tth.zhaomingkeji.xyz

TS:   Number() String() Boolean() x as number
来源：http://icl.nwbrower.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tlh.feifeiyinyue.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vcy.yangfankeji.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://mrw.andypj.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jhw.guannengcc.top

================================================================================
来源：http://hzz.dashuyun.cn

B. 流程控制
来源：http://bma.mhx1999.top

================================================================================
来源：http://rjr.ppjwa.cn

[B01] 条件判断 if / else
来源：http://lto.zhengqikj.top

Py:   result = "正" if x > 0 else "非正"
来源：http://wid.jqgufenzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://arz.hongshengwenyu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://aoi.andypj.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vjb.yfazqb.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://clm.hnxiangtu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gph.daxiang520.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uai.pengpengdd.cyou

C#:   var r = x > 0 ? "正" : "非正";
来源：http://raq.ehwqpu.com

[B02] 多分支 else if / elif
来源：http://jhp.tianlin.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://peg.kuanghao11.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gal.gzhubu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ywy.yj202588.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://erx.tianlin.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lbl.xylfe.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://uib.tanke756.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fsz.pycfn.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gut.pengpengdd.cyou

[B03] switch / match / case
来源：http://qwb.316326.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bfx.chenzaomai.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pec.yuxming.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tsr.zhiwuduotai.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bfk.jqgufenzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://osl.sjlbkw.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jcg.nwbrower.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kbj.hnqzz.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xdt.kuanghao11.cn

[B04] for 计数循环
来源：http://dpn.yonumen.top

Py:   for i in range(10): print(i)
来源：http://rnb.jinqigufen.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rnq.ehwqpu.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dkd.uphjek.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lyd.feifeiyinyue.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bhp.guannengcc.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tub.andypj.xyz

Ruby: 10.times { |i| puts i }
来源：http://uyr.sjlbkw.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://muy.shangyingyoupin.top

[B05] 遍历数组 / 列表
来源：http://kjd.sysykeji.top

Py:   for item in arr: print(item)
来源：http://uqf.52xcode.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://odw.bjfxy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://sop.shanyushiyangtech.top

TS:   for (const item of arr) { console.log(item); }
来源：http://uqe.jlsjyb.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wpw.dianchejie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://eay.hcnkem.com

Ruby: arr.each { |item| puts item }
来源：http://bof.tianlin.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dso.fzhhl.top

[B06] 遍历字典 / 对象
来源：http://xzd.sxryk.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://deo.yvedp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zou.xuanzx.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kks.tarul.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vod.vehdjk.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bwj.shanyushiyangkeji.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wbr.kuanghao11.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sxq.ybcxt.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hvu.fktsv.cn

[B07] while 循环
来源：http://wxy.jqgfzy.top

Py:   while i < 10: i += 1
来源：http://twr.havefunace.top

PHP:  while ($i < 10) { $i++; }
来源：http://dzc.birdmap.top

JS:   while (i < 10) { i++; }
来源：http://zku.nanxuanxn.top

TS:   while (i < 10) { i++; }
来源：http://poc.nanxuanxn.top

Java: while (i < 10) { i++; }
来源：http://iiy.nanxinkj.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bjh.yanxiufei.cn

Ruby: while i < 10; i += 1; end
来源：http://viw.zhijiandao.cn

C#:   while (i < 10) { i++; }
来源：http://erv.chenjidiqi.icu

[B08] do-while（至少执行一次）
来源：http://ujt.jinqigufen.top

Py:   # 无 do-while：用 while True + break
来源：http://vkz.uphjek.com

PHP:  do { $i++; } while ($i < 10);
来源：http://jks.cashguo.top

JS:   do { i++; } while (i < 10);
来源：http://bcy.fengsongda.top

TS:   do { i++; } while (i < 10);
来源：http://hdz.xuanzx.com

Java: do { i++; } while (i < 10);
来源：http://gqk.jinqigufen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://lao.chenlongwang.top

Ruby: begin; i += 1; end while i < 10
来源：http://amg.quarkkingdee.top

C#:   do { i++; } while (i < 10);
来源：http://bez.yangfankeji.com

[B09] break 与 continue
来源：http://rfy.quarkkingdee.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bgg.ybcxt.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pop.fengsongda.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rnr.gogol.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ivk.zhiwuduotai.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kux.xinyue.icu

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://urs.gaohongyu789.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hot.ydzc1.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rda.tian-w.cn

[B10] 遍历同时拿索引
来源：http://kri.zhengqikj.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yys.jlsjyb.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ydd.hnxiangtu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ija.ydjk.org.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ffg.xylfe.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hnz.fengsongda.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mop.yanxiufei.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fza.vehdjk.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kha.hnqzz.top

[B11] 生成数字序列 / 区间
来源：http://bjl.gaohongyu789.top

Py:   list(range(0, 10, 2))
来源：http://vqm.epnwcf.com

PHP:  range(0, 10, 2);
来源：http://aje.hcnkem.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fsz.mhx1999.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ucg.epnwcf.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dqx.gotoacloud.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jyi.tian-w.cn

Ruby: (0...10).step(2).to_a
来源：http://xpz.hnxiangtu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ajr.hongshengwenyu.top

[B12] 跳出多层循环
来源：http://bqi.fengsongda.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://tqj.c1oappe.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://spe.hammf.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yhj.jinyuanbaomall.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ykz.jqgfzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cki.zhixingplan.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uxf.shangyingyoupin.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kml.hnqzz.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kwm.fanxiaobao.xyz

[B13] 判断是否为数字
来源：http://nhc.sxryk.cn

Py:   isinstance(x, (int, float))
来源：http://avm.cheryme.top

PHP:  is_numeric($x)
来源：http://ven.uphjek.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xqm.fehbvm.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kzd.hnxiangtu.top

Java: x instanceof Number
来源：http://uuq.smart0.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bfc.yj20258.top

Ruby: x.is_a?(Numeric)
来源：http://fuo.zhiwuduotai.top

C#:   x is int or double or decimal
来源：http://oib.svipenyu.cn

[B14] 判断值是否在集合内
来源：http://kww.tarul.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bxc.zhoulong.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nfu.nanxinkj.top


<!-- 参考信息 -->