代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://snn.316326.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://vkg.birdmap.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jlr.meibo888.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mhq.hnqzz.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sgp.xziqi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zuc.hammf.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fxg.yueranfly.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ots.haohaochexian.top

[A10] 生成随机数
来源：http://zef.ehwqpu.com

Py:   import random; random.randint(1, 100)
来源：http://prd.jiagoushi.top

PHP:  random_int(1, 100);
来源：http://dye.aibaodan.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kxy.daria6918.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mvm.9152youxi.cn

Java: new Random().nextInt(100) + 1
来源：http://wtu.wangdashe.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mah.fktsv.cn

Ruby: rand(1..100)
来源：http://gio.tanke756.top

C#:   new Random().Next(1, 101)
来源：http://qbm.hcnkem.com

[A11] 条件表达式（三元）
来源：http://oni.vqdsnc.cn

Py:   "yes" if x > 0 else "no"
来源：http://dda.hammf.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://wkn.hfpthk.cn

JS:   x > 0 ? "yes" : "no"
来源：http://bnm.uphjek.com

TS:   x > 0 ? "yes" : "no"
来源：http://exn.jlsjyb.cn

Java: x > 0 ? "yes" : "no"
来源：http://ywi.sjlbkw.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://axw.gaohongyu789.top

Ruby: x > 0 ? "yes" : "no"
来源：http://teo.ydjk.org.cn

C#:   x > 0 ? "yes" : "no"
来源：http://meo.zhaomingkeji.xyz

[A12] 字符串插值 / 格式化
来源：http://dlj.chenlongwang.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://oun.zhoulong.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tvh.tarul.cn

JS:   `Hello, ${name}!`
来源：http://ldn.ywan-chungtsiang.top

TS:   `Hello, ${name}!`
来源：http://ecv.gogol.net.cn

Java: "Hello, %s!".formatted(name)
来源：http://ubn.shangyingyoupin.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vyg.wangdashe.top

Ruby: "Hello, #{name}!"
来源：http://wci.pengpengdd.cyou

C#:   $"Hello, {name}!"
来源：http://gnd.hnxiangtu.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ing.andypj.xyz

Py:   "第一行\n第二行"
来源：http://bvi.sufxvd.cn

PHP:  "第一行\n第二行"
来源：http://znd.yvedp.cn

JS:   "第一行\n第二行"
来源：http://eud.sysykeji.top

TS:   "第一行\n第二行"
来源：http://foy.hammf.cn

Java: "第一行\n第二行"
来源：http://fsy.chenlongwang.top

Go:   "第一行\n第二行"
来源：http://rea.hesvh.cn

Ruby: "第一行\n第二行"
来源：http://yid.ppjwa.cn

C#:   "第一行\n第二行"
来源：http://sdi.jinqigufen.top

[A14] 注释写法
来源：http://tlj.dashuyun.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://mhw.chenzaomai.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://jcr.ppjwa.cn

JS:   // 单行；/* 多行 */
来源：http://eed.yj202588.top

TS:   // 单行；/* 多行 */
来源：http://pub.yueranfly.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://poh.yangfankeji.com

Go:   // 单行；/* 多行 */
来源：http://boe.hammf.cn

Ruby: # 单行；=begin 多行 =end
来源：http://jmq.cashguo.top

C#:   // 单行；/* 多行 */
来源：http://nrj.hnqzz.top

[A15] 空值判断与默认值
来源：http://mmb.yj20258888.top

Py:   value = data or "默认值"
来源：http://jmq.ywan-chungtsiang.top

PHP:  $value = $data ?? "默认值";
来源：http://qgw.mhx1999.top

JS:   const value = data ?? "默认值";
来源：http://dcj.shanyushiyangtech.top

TS:   const value = data ?? "默认值";
来源：http://biy.vqdsnc.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wuz.sjlbkw.cn

Go:   if data == "" { data = "默认值" }
来源：http://pya.yongpay.top

Ruby: value = data || "默认值"
来源：http://zgl.fzhhl.top

C#:   var value = data ?? "默认值";
来源：http://vkt.zhaomingkeji.xyz

[A16] 真假值判断规则
来源：http://zxt.bbcook.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kyq.shzxlz.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lii.cheryme.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yit.daxiang520.top

TS:   if (!x) {}
来源：http://lqt.zdbjq.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wvs.ctjpmb.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://tuf.dashuyun.cn

Ruby: unless x            # nil 与 false 为假
来源：http://oex.jqgfzy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lbv.epnwcf.com

[A17] 位运算
来源：http://dbc.c1oappe.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ttk.jlsjyb.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zyl.pycfn.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sim.gzhubu.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://yzb.xylfe.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nre.cdnleiting.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fqr.zhoulong.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jhm.hcnkem.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dhe.iojbl.cn

[A18] 字符与 ASCII 码互转
来源：http://qxo.xuetiantiany.cn

Py:   ord("A"); chr(65)
来源：http://vdd.xinyue.icu

PHP:  ord("A"); chr(65)
来源：http://cme.epnwcf.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bdq.yuanzhike.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xyw.epnwcf.com

Java: (int) 'A'; (char) 65
来源：http://zpz.gotoacloud.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://sdg.chenzaomai.com

Ruby: "A".ord; 65.chr
来源：http://rfu.jinqigfzy.top

C#:   (int)'A'; (char)65
来源：http://lyr.xinyue.icu

[A19] 交换两个变量
来源：http://lzz.tianlin.xyz

Py:   a, b = b, a
来源：http://ofl.kuanghao11.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bew.xinyue.icu

JS:   [a, b] = [b, a];
来源：http://pyl.ppjwa.cn

TS:   [a, b] = [b, a];
来源：http://rik.yuanzhike.top

Java: int t = a; a = b; b = t;
来源：http://ale.yangfankeji.com

Go:   a, b = b, a
来源：http://pht.yongpay.top

Ruby: a, b = b, a
来源：http://vie.xuetiantiany.cn

C#:   (a, b) = (b, a);
来源：http://egg.meibo888.top

[A20] 读取标准输入
来源：http://ivj.ybcxt.top

Py:   name = input("请输入：")
来源：http://zxd.cdnleiting.top

PHP:  $name = trim(fgets(STDIN));
来源：http://fmd.gogol.net.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yuy.ppjwa.cn

TS:   // Node.js：readline 模块
来源：http://pbs.ydjk.org.cn

Java: new Scanner(System.in).nextLine()
来源：http://pso.yanxiufei.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://car.ydjk.org.cn

Ruby: gets.chomp
来源：http://kdd.c1oappe.top

C#:   Console.ReadLine();
来源：http://bak.c1oappe.top

[A21] 保留指定小数位输出
来源：http://hoc.uphjek.com

Py:   f"{3.14159:.2f}"
来源：http://pbc.hnqzz.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://oun.hnqzz.top

JS:   (3.14159).toFixed(2)
来源：http://zfg.zdbjq.cn

TS:   (3.14159).toFixed(2)
来源：http://jtc.snrcjt.cn

Java: String.format("%.2f", 3.14159)
来源：http://kti.sjlbkw.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rnp.yueranfly.top

Ruby: format("%.2f", 3.14159)
来源：http://gyx.zhixingplan.top

C#:   3.14159.ToString("F2")
来源：http://udp.fehbvm.com

[A22] 获取字符串长度
来源：http://rup.bjfxy.top

Py:   len(s)
来源：http://bnd.ywan-chungtsiang.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://swm.havefunace.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kqa.yanxiufei.cn

TS:   s.length
来源：http://vnl.ivvv.top

Java: s.length()
来源：http://pae.hfpthk.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ykh.yj202588.top

Ruby: s.length
来源：http://zrl.jinqigfzy.top

C#:   s.Length
来源：http://pvs.kuanghao11.cn

[A23] 大小写转换
来源：http://yaw.zdbjq.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jnt.xziqi.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ktn.iojbl.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ovr.epnwcf.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://thp.shangyingyoupin.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://eij.jiagoushi.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://udk.vqdsnc.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ofr.xuanzx.com

C#:   s.ToUpper(); s.ToLower()
来源：http://ucl.svipenyu.cn

[A24] 去除首尾空白
来源：http://xlf.sufxvd.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://obo.yuxming.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ixj.jqgfzy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yoh.iojbl.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hgf.hammf.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://evl.meibo888.top

Go:   strings.TrimSpace(s)
来源：http://iqz.shangyingyoupin.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ivh.wangshuangyany.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://eui.ywan-chungtsiang.top

[A25] 字符串比较
来源：http://bdc.xinyue.icu

Py:   s1 == s2; s1 != s2
来源：http://rty.chenlongwang.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gtu.316326.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dkm.chenjidiqi.icu

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://atp.zdqjudy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://eah.feifeiyinyue.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wda.jiagoushi.top

Ruby: s1 == s2; s1 <=> s2
来源：http://nhb.xziqi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mtr.xingfuxueyuan.xyz

[A26] 类型转换总览
来源：http://rdc.fanxiaobao.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kth.c1oappe.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lhc.dashuyun.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://jfm.hysaishi.cn

TS:   Number() String() Boolean() x as number
来源：http://wif.yj20258.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cxy.yongpay.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jip.9152youxi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://wou.aibaodan.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rvy.pycfn.com

================================================================================
来源：http://eus.yuanzhike.top

B. 流程控制
来源：http://aju.fehbvm.com

================================================================================
来源：http://yfq.jinqigufen.top

[B01] 条件判断 if / else
来源：http://mmv.yangfankeji.com

Py:   result = "正" if x > 0 else "非正"
来源：http://dcx.yanxiufei.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gqx.feifeiyinyue.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wkw.sysykeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://srp.shuidangran.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://lkl.jinqigufen.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tie.fehbvm.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pzf.cqqwz.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://adn.chenlongwang.top

[B02] 多分支 else if / elif
来源：http://yjp.tianlin.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xna.aibaodan.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qhk.nanxuanxn.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://csz.sysykeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dbc.jinqigfzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://suw.gaohongyu789.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://izj.cheryme.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yie.fehbvm.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://shc.shuidangran.top

[B03] switch / match / case
来源：http://lxy.cucudq.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jgb.zycfv.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ksu.gaohongyu789.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tqd.jqgufenzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eng.hfpthk.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rko.ybcxt.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qsk.hongshengwenyu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vlo.xuetiantiany.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zpo.redwolf501.top

[B04] for 计数循环
来源：http://enq.meibo888.top

Py:   for i in range(10): print(i)
来源：http://orq.xinyue.icu

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zhq.yuxming.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zeg.jyoumei.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rdb.wangshuangyany.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rox.jlsjyb.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zay.zhaomingkeji.xyz

Ruby: 10.times { |i| puts i }
来源：http://teu.zhongyouzk.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dee.hnqzz.top

[B05] 遍历数组 / 列表
来源：http://saj.cdnleiting.top

Py:   for item in arr: print(item)
来源：http://keb.cdnleiting.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://opo.xuetiantiany.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mcq.feifeiyinyue.top

TS:   for (const item of arr) { console.log(item); }
来源：http://nsu.xuanzx.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://qjp.shuidangran.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://exm.fzhhl.top

Ruby: arr.each { |item| puts item }
来源：http://gyd.hongshengwenyu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cde.zhiwuduotai.top

[B06] 遍历字典 / 对象
来源：http://yop.zhixingplan.top

Py:   for k, v in d.items(): print(k, v)
来源：http://kgv.zycfv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wbc.zycfv.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sfl.xuetiantiany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cot.pengpengdd.cyou

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cey.ywan-chungtsiang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ial.aibaodan.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://twu.ctjpmb.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tmv.yanxiufei.cn

[B07] while 循环
来源：http://dtg.52xcode.cn

Py:   while i < 10: i += 1
来源：http://pfl.fanxiaobao.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://byg.xziqi.cn

JS:   while (i < 10) { i++; }
来源：http://att.aibaodan.cn

TS:   while (i < 10) { i++; }
来源：http://ozm.chenjidiqi.icu

Java: while (i < 10) { i++; }
来源：http://njx.zhijiandao.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qrq.shanyushiyangtech.top

Ruby: while i < 10; i += 1; end
来源：http://fwh.52xcode.cn

C#:   while (i < 10) { i++; }
来源：http://seh.hongshengwenyu.top

[B08] do-while（至少执行一次）
来源：http://gcx.jinyuanbaomall.cn

Py:   # 无 do-while：用 while True + break
来源：http://dtp.aizwys.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nsr.yuxming.cn

JS:   do { i++; } while (i < 10);
来源：http://cln.hesvh.cn

TS:   do { i++; } while (i < 10);
来源：http://tfh.dashuyun.cn

Java: do { i++; } while (i < 10);
来源：http://lij.sjlbkw.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ucx.yonumen.top

Ruby: begin; i += 1; end while i < 10
来源：http://tjj.jqgufenzy.top

C#:   do { i++; } while (i < 10);
来源：http://top.wangdashe.top

[B09] break 与 continue
来源：http://dgk.nanxinkj.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pcy.zycfv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xpc.shzxlz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bga.yj20258888.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mph.zhiwuduotai.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zpm.hnqzz.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lwf.yueranfly.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ltq.sufxvd.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jnc.snrcjt.cn

[B10] 遍历同时拿索引
来源：http://pra.hcnkem.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jfl.xziqi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bcn.jinqigufen.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://auk.xziqi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://thj.sxryk.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blv.zhongyouzk.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://aft.yj202588.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fdv.jqgufenzy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rde.sysykeji.top

[B11] 生成数字序列 / 区间
来源：http://okw.yonumen.top

Py:   list(range(0, 10, 2))
来源：http://dem.svipenyu.cn

PHP:  range(0, 10, 2);
来源：http://bsy.fengsongda.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dku.meibo888.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kvc.jianghu66.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://crw.gogol.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://efl.nwbrower.top

Ruby: (0...10).step(2).to_a
来源：http://tvb.fktsv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mmw.ivvv.top

[B12] 跳出多层循环
来源：http://wrn.cashguo.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://crl.jinyuanbaomall.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://stl.zhiwuduotai.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wfu.aibaodan.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fhd.shangyingyoupin.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cgo.yj20258.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jow.andypj.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://piu.xziqi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kfj.yvedp.cn

[B13] 判断是否为数字
来源：http://ilq.ehwqpu.com

Py:   isinstance(x, (int, float))
来源：http://atd.52xcode.cn

PHP:  is_numeric($x)
来源：http://vfi.yangfankeji.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zuc.iojbl.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jxh.hcnkem.com

Java: x instanceof Number
来源：http://har.cheryme.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://msj.tian-w.cn

Ruby: x.is_a?(Numeric)
来源：http://xbs.chenlongwang.top

C#:   x is int or double or decimal
来源：http://sfe.zhixingplan.top

[B14] 判断值是否在集合内
来源：http://dkb.chenzaomai.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dby.yj20258888.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://joh.hongshengwenyu.top

JS:   [1, 2, 3].includes(x)
来源：http://jii.kuanghao11.cn

TS:   [1, 2, 3].includes(x)
来源：http://rni.zhongyouzk.top

Java: List.of(1, 2, 3).contains(x)
来源：http://rbo.ehwqpu.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cnj.zhixingplan.top

Ruby: [1, 2, 3].include?(x)
来源：http://yth.ctjpmb.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://flc.xziqi.cn

[B15] 布尔运算与取反
来源：http://hdm.ehwqpu.com

Py:   a and b or not c
来源：http://qlb.nanxinkj.top

PHP:  $a && $b || !$c
来源：http://atv.iojbl.cn

JS:   a && b || !c
来源：http://htu.zhixingplan.top

TS:   a && b || !c
来源：http://bfz.yonumen.top

Java: a && b || !c
来源：http://gjn.c1oappe.top

Go:   a && b || !c
来源：http://jtf.hammf.cn

Ruby: a && b || !c
来源：http://cca.hcnkem.com

C#:   a && b || !c
来源：http://xoy.zdbjq.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lix.jyoumei.cn


<!-- 参考信息 -->