代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://vvq.cheryme.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jsb.cdnleiting.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://clo.gotoacloud.top

Ruby: "42".to_i; "3.14".to_f
来源：http://myc.kuanghao11.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://bbo.gogol.net.cn

[A07] 数字转字符串
来源：http://gcy.yanxiufei.cn

Py:   str(42)
来源：http://nrf.smart0.xyz

PHP:  (string) 42; strval(42)
来源：http://byd.sjlbkw.cn

JS:   String(42); (42).toString()
来源：http://ala.snrcjt.cn

TS:   String(42)
来源：http://eoh.jiagoushi.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://oir.yuanzhike.top

Go:   strconv.Itoa(42)
来源：http://poo.guannengcc.top

Ruby: 42.to_s
来源：http://laa.daria6918.cn

C#:   42.ToString()
来源：http://wqs.zdbjq.cn

[A08] 取整与四舍五入
来源：http://jqd.haohaochexian.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://faw.havefunace.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cfa.tian-w.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lqx.meibo888.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gmc.dashuyun.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://paj.tarul.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://nqi.pycfn.com

Ruby: 3.567.round(2); 3.9.floor
来源：http://hem.iojbl.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kxy.zhoulong.xyz

[A09] 绝对值与最大最小值
来源：http://lds.havefunace.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jfk.zhiwuduotai.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gdi.ydzc1.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lrh.ehwqpu.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lai.quarkkingdee.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tml.guowangkeji.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://iyu.shzxlz.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mcj.fengsongda.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://caf.yj20258.top

[A10] 生成随机数
来源：http://mvu.yfazqb.com

Py:   import random; random.randint(1, 100)
来源：http://ksc.cdnleiting.top

PHP:  random_int(1, 100);
来源：http://tlu.daxiang520.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ypu.jqgfzy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://obi.sweek.top

Java: new Random().nextInt(100) + 1
来源：http://yvc.hysaishi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bvy.yangfankeji.com

Ruby: rand(1..100)
来源：http://omj.ywan-chungtsiang.top

C#:   new Random().Next(1, 101)
来源：http://vio.9152youxi.cn

[A11] 条件表达式（三元）
来源：http://feq.chenlongwang.top

Py:   "yes" if x > 0 else "no"
来源：http://nqw.jqgufenzy.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://iuf.aizwys.cn

JS:   x > 0 ? "yes" : "no"
来源：http://xxw.dianchejie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xpm.tanke756.top

Java: x > 0 ? "yes" : "no"
来源：http://jvh.chenlongwang.top

Go:   // 无三元运算符，需用 if 语句
来源：http://lzf.gzhubu.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ail.bjfxy.top

C#:   x > 0 ? "yes" : "no"
来源：http://sub.daria6918.cn

[A12] 字符串插值 / 格式化
来源：http://yro.pycfn.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lyn.zhijiandao.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xpg.aizwys.cn

JS:   `Hello, ${name}!`
来源：http://afa.hnqzz.top

TS:   `Hello, ${name}!`
来源：http://dic.zdbjq.cn

Java: "Hello, %s!".formatted(name)
来源：http://qcc.meibo888.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qtd.jiagoushi.top

Ruby: "Hello, #{name}!"
来源：http://gmw.zhixingplan.top

C#:   $"Hello, {name}!"
来源：http://iwm.zhengqikj.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ucc.jlsjyb.cn

Py:   "第一行\n第二行"
来源：http://ixh.gogol.net.cn

PHP:  "第一行\n第二行"
来源：http://mne.vqdsnc.cn

JS:   "第一行\n第二行"
来源：http://fti.xuanzx.com

TS:   "第一行\n第二行"
来源：http://xqz.yvedp.cn

Java: "第一行\n第二行"
来源：http://luj.hnxiangtu.top

Go:   "第一行\n第二行"
来源：http://icw.zhijiandao.cn

Ruby: "第一行\n第二行"
来源：http://nol.sjlbkw.cn

C#:   "第一行\n第二行"
来源：http://awy.zhoulong.xyz

[A14] 注释写法
来源：http://uhm.yj20258.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ojs.haohaochexian.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://lpt.zhijiandao.cn

JS:   // 单行；/* 多行 */
来源：http://mof.zycfv.cn

TS:   // 单行；/* 多行 */
来源：http://cda.zhongyouzk.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qwv.zycfv.cn

Go:   // 单行；/* 多行 */
来源：http://eav.hongshengwenyu.top

Ruby: # 单行；=begin 多行 =end
来源：http://bdj.ctjpmb.com

C#:   // 单行；/* 多行 */
来源：http://juc.nanxinkj.top

[A15] 空值判断与默认值
来源：http://ysp.yonumen.top

Py:   value = data or "默认值"
来源：http://kbq.ehwqpu.com

PHP:  $value = $data ?? "默认值";
来源：http://jxi.sysykeji.top

JS:   const value = data ?? "默认值";
来源：http://lin.chenjidiqi.icu

TS:   const value = data ?? "默认值";
来源：http://vpg.nwbrower.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fzg.nanxuanxn.top

Go:   if data == "" { data = "默认值" }
来源：http://jgo.xuetiantiany.cn

Ruby: value = data || "默认值"
来源：http://jwq.fengsongda.top

C#:   var value = data ?? "默认值";
来源：http://iti.gaohongyu789.top

[A16] 真假值判断规则
来源：http://ipz.feifeiyinyue.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cij.havefunace.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://kho.guannengcc.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yuc.yfazqb.com

TS:   if (!x) {}
来源：http://jeu.zhongyouzk.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jyj.dianchejie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nki.hongshengwenyu.top

Ruby: unless x            # nil 与 false 为假
来源：http://cdm.aibaodan.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bob.yvedp.cn

[A17] 位运算
来源：http://pfr.shangyingyoupin.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hhz.jqgufenzy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://idn.feifeiyinyue.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xkp.0kj1m.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ter.zdqjudy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kdz.pengpengdd.cyou

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vva.jinyuanbaomall.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nyc.pycfn.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fdy.gotoacloud.top

[A18] 字符与 ASCII 码互转
来源：http://sfm.fanxiaobao.xyz

Py:   ord("A"); chr(65)
来源：http://hfq.shzxlz.cn

PHP:  ord("A"); chr(65)
来源：http://iec.c1oappe.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kzz.yanxiufei.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xjv.pengpengdd.cyou

Java: (int) 'A'; (char) 65
来源：http://mxi.nanxuanxn.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://idk.bbcook.cn

Ruby: "A".ord; 65.chr
来源：http://jjj.zhoulong.xyz

C#:   (int)'A'; (char)65
来源：http://elz.ywan-chungtsiang.top

[A19] 交换两个变量
来源：http://ftd.guowangkeji.top

Py:   a, b = b, a
来源：http://zxo.redwolf501.top

PHP:  [$a, $b] = [$b, $a];
来源：http://gct.iojbl.cn

JS:   [a, b] = [b, a];
来源：http://mjf.snrcjt.cn

TS:   [a, b] = [b, a];
来源：http://cna.yvedp.cn

Java: int t = a; a = b; b = t;
来源：http://qqx.gaohongyu789.top

Go:   a, b = b, a
来源：http://sxq.fanxiaobao.xyz

Ruby: a, b = b, a
来源：http://zdz.ybcxt.top

C#:   (a, b) = (b, a);
来源：http://yii.hammf.cn

[A20] 读取标准输入
来源：http://kyo.nwbrower.top

Py:   name = input("请输入：")
来源：http://cgj.zhengqikj.top

PHP:  $name = trim(fgets(STDIN));
来源：http://gqn.sweek.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jqy.9152youxi.cn

TS:   // Node.js：readline 模块
来源：http://kvv.guowangkeji.top

Java: new Scanner(System.in).nextLine()
来源：http://rkb.ehwqpu.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qez.ydzc1.top

Ruby: gets.chomp
来源：http://eap.iojbl.cn

C#:   Console.ReadLine();
来源：http://chu.gotoacloud.top

[A21] 保留指定小数位输出
来源：http://bjr.c1oappe.top

Py:   f"{3.14159:.2f}"
来源：http://yww.gzhubu.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ljq.cucudq.cn

JS:   (3.14159).toFixed(2)
来源：http://fua.jqgufenzy.top

TS:   (3.14159).toFixed(2)
来源：http://ikl.yuanzhike.top

Java: String.format("%.2f", 3.14159)
来源：http://tkt.shangyingyoupin.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://stp.cucudq.cn

Ruby: format("%.2f", 3.14159)
来源：http://sky.zdbjq.cn

C#:   3.14159.ToString("F2")
来源：http://qqn.hfpthk.cn

[A22] 获取字符串长度
来源：http://gwa.hnxiangtu.top

Py:   len(s)
来源：http://gyx.yj20258888.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://eyb.wangdashe.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ekf.ehwqpu.com

TS:   s.length
来源：http://nbl.jqgufenzy.top

Java: s.length()
来源：http://zgj.cucudq.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ikv.gzhubu.top

Ruby: s.length
来源：http://uiu.cashguo.top

C#:   s.Length
来源：http://tmy.sjlbkw.cn

[A23] 大小写转换
来源：http://pmg.gotoacloud.top

Py:   s.upper(); s.lower(); s.title()
来源：http://jqj.c1oappe.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://yoq.hesvh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hcy.yj20258.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wij.jinqigfzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jis.yongpay.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://scs.cucudq.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://imu.bjfxy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://gvl.yj20258888.top

[A24] 去除首尾空白
来源：http://xgc.feifeiyinyue.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ani.jqgfzy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bpl.nanxinkj.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gjt.fengsongda.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sbn.xziqi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lpn.andypj.xyz

Go:   strings.TrimSpace(s)
来源：http://hbr.svipenyu.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cxa.jlsjyb.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://prx.zhaomingkeji.xyz

[A25] 字符串比较
来源：http://rtm.fzhhl.top

Py:   s1 == s2; s1 != s2
来源：http://zdm.chenzaomai.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qzg.gaohongyu789.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lek.zdqjudy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://drz.tarul.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yza.yvedp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://osc.cucudq.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vzj.yanxiufei.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xhd.uphjek.com

[A26] 类型转换总览
来源：http://vmt.ppjwa.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://aml.yangfankeji.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://arp.nwbrower.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rue.shanyushiyangtech.top

TS:   Number() String() Boolean() x as number
来源：http://thy.xuetiantiany.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dfu.hesvh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://iqu.hnxiangtu.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://adg.daxiang520.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wjy.0kj1m.cn

================================================================================
来源：http://pag.hesvh.cn

B. 流程控制
来源：http://xjo.ywan-chungtsiang.top

================================================================================
来源：http://end.snrcjt.cn

[B01] 条件判断 if / else
来源：http://awa.hammf.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ftd.pengpengdd.cyou

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qon.yj20258.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xko.jianghu66.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kvc.hfpthk.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ilc.jinyuanbaomall.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://oey.fengsongda.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://plf.cashguo.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qri.nwbrower.top

[B02] 多分支 else if / elif
来源：http://nwa.jqgufenzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fuo.daxiang520.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hyx.jlsjyb.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iuq.sufxvd.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vcp.bjfxy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lcz.shanyushiyangkeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://enj.guannengcc.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://aaw.hcnkem.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sla.hammf.cn

[B03] switch / match / case
来源：http://zrk.jiagoushi.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://edu.aibaodan.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bas.sxryk.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://est.quarkkingdee.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dqd.chenjidiqi.icu

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sfj.feifeiyinyue.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lpg.nanxinkj.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ngl.zycfv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://psx.xylfe.cn

[B04] for 计数循环
来源：http://zgr.yvedp.cn

Py:   for i in range(10): print(i)
来源：http://quc.feifeiyinyue.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xuf.jqgfzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xrl.chenzaomai.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rto.zhiwuduotai.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oxd.quarkkingdee.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vky.sysykeji.top

Ruby: 10.times { |i| puts i }
来源：http://irr.pengpengdd.cyou

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bnb.havefunace.top

[B05] 遍历数组 / 列表
来源：http://wbb.jianghu66.top

Py:   for item in arr: print(item)
来源：http://rdg.chenlongwang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hqb.hongshengwenyu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://fce.cucudq.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bfg.zycfv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ubh.yangfankeji.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wki.dianchejie.cn

Ruby: arr.each { |item| puts item }
来源：http://lwj.vehdjk.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rph.hfpthk.cn

[B06] 遍历字典 / 对象
来源：http://seq.jinyuanbaomall.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://uyl.zhiwuduotai.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pzo.xziqi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qtn.sysykeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ogl.svipenyu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zos.zycfv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ymw.xziqi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ocb.redwolf501.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ogw.yj20258.top

[B07] while 循环
来源：http://hhp.snrcjt.cn

Py:   while i < 10: i += 1
来源：http://ewg.chenzaomai.com

PHP:  while ($i < 10) { $i++; }
来源：http://iou.xingfuxueyuan.xyz

JS:   while (i < 10) { i++; }
来源：http://jsj.gaohongyu789.top

TS:   while (i < 10) { i++; }
来源：http://mzz.0kj1m.cn

Java: while (i < 10) { i++; }
来源：http://hcm.bjfxy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://osp.pycfn.com

Ruby: while i < 10; i += 1; end
来源：http://ehd.svipenyu.cn

C#:   while (i < 10) { i++; }
来源：http://urk.iojbl.cn

[B08] do-while（至少执行一次）
来源：http://lni.guannengcc.top

Py:   # 无 do-while：用 while True + break
来源：http://waf.zhoulong.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://gsj.chenzaomai.com

JS:   do { i++; } while (i < 10);
来源：http://gan.gotoacloud.top

TS:   do { i++; } while (i < 10);
来源：http://myq.xuetiantiany.cn

Java: do { i++; } while (i < 10);
来源：http://gkt.wangshuangyany.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gup.yanxiufei.cn

Ruby: begin; i += 1; end while i < 10
来源：http://spc.shanyushiyangkeji.top

C#:   do { i++; } while (i < 10);
来源：http://kgl.jianghu66.top

[B09] break 与 continue
来源：http://oja.chenlongwang.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lvj.vqdsnc.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mgs.yongpay.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://top.gogol.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://poa.yvedp.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://egd.chenlongwang.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hlp.zhiwuduotai.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jbx.bbcook.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pfn.havefunace.top

[B10] 遍历同时拿索引
来源：http://mol.nwbrower.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://phq.gogol.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xdo.guannengcc.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bvv.daria6918.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://erc.aizwys.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lxz.zhaomingkeji.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tyw.iojbl.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qye.svipenyu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qmf.gzhubu.top

[B11] 生成数字序列 / 区间
来源：http://zrk.epnwcf.com

Py:   list(range(0, 10, 2))
来源：http://jqb.zhaomingkeji.xyz

PHP:  range(0, 10, 2);
来源：http://ios.c1oappe.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lwt.jyoumei.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mtx.yvedp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rvl.yfazqb.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://brs.zhijiandao.cn

Ruby: (0...10).step(2).to_a
来源：http://mwo.kuanghao11.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://elx.ehwqpu.com

[B12] 跳出多层循环
来源：http://fib.jinqigfzy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://gwp.ehwqpu.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://wvo.52xcode.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hao.guowangkeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kem.cheryme.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hju.cucudq.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nbh.hfpthk.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vwr.shuidangran.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kff.zhongyouzk.top

[B13] 判断是否为数字
来源：http://vwc.yangfankeji.com

Py:   isinstance(x, (int, float))
来源：http://njx.shangyingyoupin.top

PHP:  is_numeric($x)
来源：http://pig.uphjek.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xum.fktsv.cn


<!-- 参考信息 -->