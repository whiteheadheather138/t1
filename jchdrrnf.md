代发 wailian999

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nzj.smart0.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ayy.feifeiyinyue.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ovg.yanxiufei.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vrn.cucudq.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ywm.svipenyu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ywz.316326.xyz

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://rgs.cheryme.top

[A09] 绝对值与最大最小值
来源：http://hlv.andypj.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bnn.aizwys.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mer.tanke756.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ktr.hammf.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ghg.wangshuangyany.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://szs.aizwys.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cwm.zhixingplan.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://thy.uphjek.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://omt.jinyuanbaomall.cn

[A10] 生成随机数
来源：http://nrj.havefunace.top

Py:   import random; random.randint(1, 100)
来源：http://xtt.shzxlz.cn

PHP:  random_int(1, 100);
来源：http://cvv.yuxming.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://uce.shanyushiyangtech.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://flg.daxiang520.top

Java: new Random().nextInt(100) + 1
来源：http://nqi.uphjek.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://lnb.xinyue.icu

Ruby: rand(1..100)
来源：http://azg.xuanzx.com

C#:   new Random().Next(1, 101)
来源：http://qly.vqdsnc.cn

[A11] 条件表达式（三元）
来源：http://omy.hnqzz.top

Py:   "yes" if x > 0 else "no"
来源：http://ksm.hongshengwenyu.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://dhe.pengpengdd.cyou

JS:   x > 0 ? "yes" : "no"
来源：http://pkr.fanxiaobao.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://eyv.xinyue.icu

Java: x > 0 ? "yes" : "no"
来源：http://lid.fzhhl.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ond.bbcook.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://rpz.zhoulong.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://nig.andypj.xyz

[A12] 字符串插值 / 格式化
来源：http://ido.sxryk.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zhf.zhengqikj.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tlk.gogol.net.cn

JS:   `Hello, ${name}!`
来源：http://rjh.iojbl.cn

TS:   `Hello, ${name}!`
来源：http://ajj.zycfv.cn

Java: "Hello, %s!".formatted(name)
来源：http://lmd.ppjwa.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wvo.sufxvd.cn

Ruby: "Hello, #{name}!"
来源：http://diy.redwolf501.top

C#:   $"Hello, {name}!"
来源：http://mgx.zhaomingkeji.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://kfc.hnqzz.top

Py:   "第一行\n第二行"
来源：http://yuk.xziqi.cn

PHP:  "第一行\n第二行"
来源：http://xtd.zdqjudy.top

JS:   "第一行\n第二行"
来源：http://jtf.chenjidiqi.icu

TS:   "第一行\n第二行"
来源：http://bvq.daria6918.cn

Java: "第一行\n第二行"
来源：http://oen.cqqwz.cn

Go:   "第一行\n第二行"
来源：http://ksi.cqqwz.cn

Ruby: "第一行\n第二行"
来源：http://knb.dashuyun.cn

C#:   "第一行\n第二行"
来源：http://ank.gotoacloud.top

[A14] 注释写法
来源：http://cge.cheryme.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://yow.jinghuilouyu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vyc.nwbrower.top

JS:   // 单行；/* 多行 */
来源：http://nxt.yfazqb.com

TS:   // 单行；/* 多行 */
来源：http://kky.haohaochexian.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kmt.yuxming.cn

Go:   // 单行；/* 多行 */
来源：http://aoz.zhengqikj.top

Ruby: # 单行；=begin 多行 =end
来源：http://vyr.0kj1m.cn

C#:   // 单行；/* 多行 */
来源：http://rea.shangyingyoupin.top

[A15] 空值判断与默认值
来源：http://nde.fktsv.cn

Py:   value = data or "默认值"
来源：http://xbd.daria6918.cn

PHP:  $value = $data ?? "默认值";
来源：http://cyy.yongpay.top

JS:   const value = data ?? "默认值";
来源：http://brw.uphjek.com

TS:   const value = data ?? "默认值";
来源：http://dal.cucudq.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jcu.sufxvd.cn

Go:   if data == "" { data = "默认值" }
来源：http://jdu.quarkkingdee.top

Ruby: value = data || "默认值"
来源：http://gsj.fanxiaobao.xyz

C#:   var value = data ?? "默认值";
来源：http://zsh.shanyushiyangkeji.top

[A16] 真假值判断规则
来源：http://ksj.shanyushiyangkeji.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pdb.52xcode.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fez.nwbrower.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fzy.zhijiandao.cn

TS:   if (!x) {}
来源：http://wnk.cdnleiting.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mnj.yj202588.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rod.fktsv.cn

Ruby: unless x            # nil 与 false 为假
来源：http://glv.hywenlv.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vca.hfpthk.cn

[A17] 位运算
来源：http://mvq.hysaishi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://huo.kuanghao11.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dqb.chenzaomai.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rzb.hesvh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://yht.0kj1m.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://shj.guowangkeji.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jia.kuanghao11.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kvy.yonumen.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://avl.gotoacloud.top

[A18] 字符与 ASCII 码互转
来源：http://aae.feifeiyinyue.top

Py:   ord("A"); chr(65)
来源：http://cpe.hammf.cn

PHP:  ord("A"); chr(65)
来源：http://yvh.hysaishi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kla.nanxuanxn.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tac.zdqjudy.top

Java: (int) 'A'; (char) 65
来源：http://ieh.jiagoushi.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://slu.shanyushiyangtech.top

Ruby: "A".ord; 65.chr
来源：http://bzb.aizwys.cn

C#:   (int)'A'; (char)65
来源：http://jqb.jinyuanbaomall.cn

[A19] 交换两个变量
来源：http://inx.gotoacloud.top

Py:   a, b = b, a
来源：http://oox.xylfe.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://zqa.ehwqpu.com

JS:   [a, b] = [b, a];
来源：http://dyr.cqqwz.cn

TS:   [a, b] = [b, a];
来源：http://qua.meibo888.top

Java: int t = a; a = b; b = t;
来源：http://rsf.wangshuangyany.cn

Go:   a, b = b, a
来源：http://sih.jinyuanbaomall.cn

Ruby: a, b = b, a
来源：http://kie.chenjidiqi.icu

C#:   (a, b) = (b, a);
来源：http://jlc.guannengcc.top

[A20] 读取标准输入
来源：http://goc.jiagoushi.top

Py:   name = input("请输入：")
来源：http://ggp.chenjidiqi.icu

PHP:  $name = trim(fgets(STDIN));
来源：http://qbc.zdbjq.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ahz.tanke756.top

TS:   // Node.js：readline 模块
来源：http://fln.jiagoushi.top

Java: new Scanner(System.in).nextLine()
来源：http://vyl.hywenlv.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://viz.xuetiantiany.cn

Ruby: gets.chomp
来源：http://ock.jqgufenzy.top

C#:   Console.ReadLine();
来源：http://hjf.xziqi.cn

[A21] 保留指定小数位输出
来源：http://odc.zhongyouzk.top

Py:   f"{3.14159:.2f}"
来源：http://juh.snrcjt.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://azc.gogol.net.cn

JS:   (3.14159).toFixed(2)
来源：http://dnn.zhiwuduotai.top

TS:   (3.14159).toFixed(2)
来源：http://sjq.jqgufenzy.top

Java: String.format("%.2f", 3.14159)
来源：http://gso.yongpay.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://uqd.yj20258888.top

Ruby: format("%.2f", 3.14159)
来源：http://avq.gotoacloud.top

C#:   3.14159.ToString("F2")
来源：http://kli.yonumen.top

[A22] 获取字符串长度
来源：http://wtq.zhongyouzk.top

Py:   len(s)
来源：http://dsz.jinyuanbaomall.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zpm.nanxuanxn.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://quw.0kj1m.cn

TS:   s.length
来源：http://biu.hcnkem.com

Java: s.length()
来源：http://fvl.hnqzz.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://kmx.tarul.cn

Ruby: s.length
来源：http://eas.zhoulong.xyz

C#:   s.Length
来源：http://sys.cucudq.cn

[A23] 大小写转换
来源：http://zow.yuxming.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kgv.jqgfzy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rsm.chenzaomai.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tyh.ybcxt.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://elv.shuidangran.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lss.yvedp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bjj.wangshuangyany.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yik.aizwys.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lne.yfazqb.com

[A24] 去除首尾空白
来源：http://sit.jinqigfzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pcu.shanyushiyangkeji.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lti.yuxming.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pat.jinyuanbaomall.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zmg.shangyingyoupin.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kft.yueranfly.top

Go:   strings.TrimSpace(s)
来源：http://lfx.gotoacloud.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ffx.xziqi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qos.gotoacloud.top

[A25] 字符串比较
来源：http://log.dashuyun.cn

Py:   s1 == s2; s1 != s2
来源：http://onl.yuxming.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://szg.fehbvm.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pti.hysaishi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wqe.haohaochexian.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vzy.yueranfly.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wnu.daxiang520.top

Ruby: s1 == s2; s1 <=> s2
来源：http://xqg.jqgufenzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xpl.cashguo.top

[A26] 类型转换总览
来源：http://ecl.xuanzx.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sfh.aibaodan.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ipo.316326.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oef.gogol.net.cn

TS:   Number() String() Boolean() x as number
来源：http://srh.chenjidiqi.icu

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dji.wangdashe.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bsz.zdbjq.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vly.hysaishi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://plm.andypj.xyz

================================================================================
来源：http://eba.pengpengdd.cyou

B. 流程控制
来源：http://esc.shuidangran.top

================================================================================
来源：http://rhh.yvedp.cn

[B01] 条件判断 if / else
来源：http://gcu.haohaochexian.top

Py:   result = "正" if x > 0 else "非正"
来源：http://spv.hfpthk.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://smz.jianghu66.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jsn.snrcjt.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://htr.xingfuxueyuan.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://jst.mhx1999.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tex.nwbrower.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bty.feifeiyinyue.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://miu.sufxvd.cn

[B02] 多分支 else if / elif
来源：http://smx.andypj.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ywy.ctjpmb.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mxc.meibo888.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wnw.yuxming.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kcm.jqgufenzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rwc.uphjek.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cwn.sufxvd.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lpe.guowangkeji.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wlf.hongshengwenyu.top

[B03] switch / match / case
来源：http://nnn.sysykeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xsf.zhiwuduotai.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://poi.yj202588.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zvd.guowangkeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ish.snrcjt.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dwf.xinyue.icu

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xmy.jlsjyb.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pqx.wangshuangyany.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sud.guowangkeji.top

[B04] for 计数循环
来源：http://ogy.kuanghao11.cn

Py:   for i in range(10): print(i)
来源：http://bkn.chenzaomai.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://stm.yuanzhike.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fgs.dashuyun.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ffm.dashuyun.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://grc.xingfuxueyuan.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qyo.gogol.net.cn

Ruby: 10.times { |i| puts i }
来源：http://rsk.yj20258.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://snj.xziqi.cn

[B05] 遍历数组 / 列表
来源：http://kjh.zdqjudy.top

Py:   for item in arr: print(item)
来源：http://ids.shangyingyoupin.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lse.pycfn.com

JS:   for (const item of arr) { console.log(item); }
来源：http://llf.daxiang520.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qlh.uphjek.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://tet.chenzaomai.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vfo.0kj1m.cn

Ruby: arr.each { |item| puts item }
来源：http://lit.zhongyouzk.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kwg.bbcook.cn

[B06] 遍历字典 / 对象
来源：http://flb.c1oappe.top

Py:   for k, v in d.items(): print(k, v)
来源：http://zzt.gzhubu.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wur.uphjek.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hfx.daxiang520.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://skk.fzhhl.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pbo.yuanzhike.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lhc.shangyingyoupin.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cnj.mhx1999.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wud.xziqi.cn

[B07] while 循环
来源：http://fbe.zdqjudy.top

Py:   while i < 10: i += 1
来源：http://qlo.316326.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://kdq.zhixingplan.top

JS:   while (i < 10) { i++; }
来源：http://kad.gzhubu.top

TS:   while (i < 10) { i++; }
来源：http://uxm.dashuyun.cn

Java: while (i < 10) { i++; }
来源：http://vps.zhoulong.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yvd.yuxming.cn

Ruby: while i < 10; i += 1; end
来源：http://ogw.redwolf501.top

C#:   while (i < 10) { i++; }
来源：http://jrg.pengpengdd.cyou

[B08] do-while（至少执行一次）
来源：http://xpu.bbcook.cn

Py:   # 无 do-while：用 while True + break
来源：http://xma.cashguo.top

PHP:  do { $i++; } while ($i < 10);
来源：http://otw.zycfv.cn

JS:   do { i++; } while (i < 10);
来源：http://vxs.ctjpmb.com

TS:   do { i++; } while (i < 10);
来源：http://ofz.ppjwa.cn

Java: do { i++; } while (i < 10);
来源：http://rmh.ybcxt.top

Go:   for { i++; if i >= 10 { break } }
来源：http://vvf.hesvh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://clj.zhijiandao.cn

C#:   do { i++; } while (i < 10);
来源：http://hrq.xinyue.icu

[B09] break 与 continue
来源：http://zhp.gzhubu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nlh.ctjpmb.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ihv.zhengqikj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ofs.jlsjyb.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jbs.zhaomingkeji.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hay.pengpengdd.cyou

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jes.zhiwuduotai.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jsm.andypj.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hok.sysykeji.top

[B10] 遍历同时拿索引
来源：http://svc.0kj1m.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lnp.jinqigfzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://eek.ehwqpu.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ygl.hammf.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zkb.meibo888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gtc.gzhubu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gub.zhongyouzk.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ppp.xinyue.icu

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xgk.ywan-chungtsiang.top

[B11] 生成数字序列 / 区间
来源：http://jqt.quarkkingdee.top

Py:   list(range(0, 10, 2))
来源：http://qbw.bjfxy.top

PHP:  range(0, 10, 2);
来源：http://vcq.fzhhl.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hfz.fanxiaobao.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aqr.shanyushiyangkeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wod.yj20258888.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nva.shangyingyoupin.top

Ruby: (0...10).step(2).to_a
来源：http://wsr.fktsv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xjq.jiagoushi.top

[B12] 跳出多层循环
来源：http://oea.hcnkem.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://dxm.ydzc1.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vra.daxiang520.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wln.gogol.net.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rlm.mhx1999.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jyg.quarkkingdee.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hmp.haohaochexian.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fsq.c1oappe.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dyk.hywenlv.cn

[B13] 判断是否为数字
来源：http://wsq.nanxuanxn.top

Py:   isinstance(x, (int, float))
来源：http://mjx.jianghu66.top

PHP:  is_numeric($x)
来源：http://ayx.sxryk.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mts.cashguo.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://owi.zycfv.cn

Java: x instanceof Number
来源：http://fgg.gaohongyu789.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xjj.zhijiandao.cn

Ruby: x.is_a?(Numeric)
来源：http://xoo.tanke756.top

C#:   x is int or double or decimal
来源：http://mmw.yanxiufei.cn

[B14] 判断值是否在集合内
来源：http://ppd.feifeiyinyue.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cir.xingfuxueyuan.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nls.hongshengwenyu.top

JS:   [1, 2, 3].includes(x)
来源：http://cur.ivvv.top

TS:   [1, 2, 3].includes(x)
来源：http://uqd.feifeiyinyue.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pwl.cheryme.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bgq.jinghuilouyu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ndz.jinqigfzy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nqd.gotoacloud.top

[B15] 布尔运算与取反
来源：http://dch.hongshengwenyu.top

Py:   a and b or not c
来源：http://ndz.shangyingyoupin.top


<!-- 参考信息 -->