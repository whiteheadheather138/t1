代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://awf.hammf.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dht.pengpengdd.cyou

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hxa.shuidangran.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kez.hcnkem.com

[A10] 生成随机数
来源：http://dbm.hywenlv.cn

Py:   import random; random.randint(1, 100)
来源：http://fvj.uphjek.com

PHP:  random_int(1, 100);
来源：http://ccs.bbcook.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jnc.xuetiantiany.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rnb.gotoacloud.top

Java: new Random().nextInt(100) + 1
来源：http://nac.svipenyu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://zqm.pycfn.com

Ruby: rand(1..100)
来源：http://fsq.smart0.xyz

C#:   new Random().Next(1, 101)
来源：http://azj.daxiang520.top

[A11] 条件表达式（三元）
来源：http://uoz.tian-w.cn

Py:   "yes" if x > 0 else "no"
来源：http://vbq.zhaomingkeji.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://ffu.c1oappe.top

JS:   x > 0 ? "yes" : "no"
来源：http://pqg.shzxlz.cn

TS:   x > 0 ? "yes" : "no"
来源：http://thp.andypj.xyz

Java: x > 0 ? "yes" : "no"
来源：http://osu.zdbjq.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://mql.xylfe.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tsl.sweek.top

C#:   x > 0 ? "yes" : "no"
来源：http://kdi.dianchejie.cn

[A12] 字符串插值 / 格式化
来源：http://cht.xuetiantiany.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lgz.uphjek.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rwy.shanyushiyangtech.top

JS:   `Hello, ${name}!`
来源：http://lom.jqgufenzy.top

TS:   `Hello, ${name}!`
来源：http://aus.pycfn.com

Java: "Hello, %s!".formatted(name)
来源：http://tkt.bjfxy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dta.52xcode.cn

Ruby: "Hello, #{name}!"
来源：http://ngi.xingfuxueyuan.xyz

C#:   $"Hello, {name}!"
来源：http://vhp.tanke756.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ixs.cqqwz.cn

Py:   "第一行\n第二行"
来源：http://zva.gzhubu.top

PHP:  "第一行\n第二行"
来源：http://aqi.aibaodan.cn

JS:   "第一行\n第二行"
来源：http://jcp.nanxinkj.top

TS:   "第一行\n第二行"
来源：http://xqr.nwbrower.top

Java: "第一行\n第二行"
来源：http://hee.xziqi.cn

Go:   "第一行\n第二行"
来源：http://mmf.fengsongda.top

Ruby: "第一行\n第二行"
来源：http://dia.daria6918.cn

C#:   "第一行\n第二行"
来源：http://hdq.hysaishi.cn

[A14] 注释写法
来源：http://ytz.hesvh.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://fma.birdmap.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://yha.ivvv.top

JS:   // 单行；/* 多行 */
来源：http://cte.hfpthk.cn

TS:   // 单行；/* 多行 */
来源：http://vne.316326.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gco.xinyue.icu

Go:   // 单行；/* 多行 */
来源：http://cnt.gogol.net.cn

Ruby: # 单行；=begin 多行 =end
来源：http://goi.yj20258.top

C#:   // 单行；/* 多行 */
来源：http://gtv.yj202588.top

[A15] 空值判断与默认值
来源：http://wau.sweek.top

Py:   value = data or "默认值"
来源：http://imi.daria6918.cn

PHP:  $value = $data ?? "默认值";
来源：http://ozx.yuanzhike.top

JS:   const value = data ?? "默认值";
来源：http://fol.pengpengdd.cyou

TS:   const value = data ?? "默认值";
来源：http://tex.zhixingplan.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://upb.jyoumei.cn

Go:   if data == "" { data = "默认值" }
来源：http://jzr.zhongyouzk.top

Ruby: value = data || "默认值"
来源：http://why.smart0.xyz

C#:   var value = data ?? "默认值";
来源：http://bsu.pycfn.com

[A16] 真假值判断规则
来源：http://lcg.ydzc1.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://znh.hfpthk.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ulx.birdmap.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cfz.tianlin.xyz

TS:   if (!x) {}
来源：http://boq.jinyuanbaomall.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xvf.gzhubu.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ekr.birdmap.top

Ruby: unless x            # nil 与 false 为假
来源：http://pno.sjlbkw.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rge.9152youxi.cn

[A17] 位运算
来源：http://bej.dianchejie.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ybv.316326.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jmx.sufxvd.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oki.shanyushiyangkeji.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nro.smart0.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fub.fehbvm.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ubi.iojbl.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xhn.jqgfzy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://olt.ivvv.top

[A18] 字符与 ASCII 码互转
来源：http://tii.sxryk.cn

Py:   ord("A"); chr(65)
来源：http://fuh.fehbvm.com

PHP:  ord("A"); chr(65)
来源：http://nce.hcnkem.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hyh.zycfv.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ycz.zhengqikj.top

Java: (int) 'A'; (char) 65
来源：http://vcs.tianlin.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://isr.hnqzz.top

Ruby: "A".ord; 65.chr
来源：http://rkz.ybcxt.top

C#:   (int)'A'; (char)65
来源：http://edw.ybcxt.top

[A19] 交换两个变量
来源：http://mxh.nanxuanxn.top

Py:   a, b = b, a
来源：http://ryn.zhoulong.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://oqk.pengpengdd.cyou

JS:   [a, b] = [b, a];
来源：http://vmy.yfazqb.com

TS:   [a, b] = [b, a];
来源：http://dnl.9152youxi.cn

Java: int t = a; a = b; b = t;
来源：http://jaf.svipenyu.cn

Go:   a, b = b, a
来源：http://tqp.cheryme.top

Ruby: a, b = b, a
来源：http://zee.daxiang520.top

C#:   (a, b) = (b, a);
来源：http://yth.hywenlv.cn

[A20] 读取标准输入
来源：http://bio.hammf.cn

Py:   name = input("请输入：")
来源：http://gdm.guannengcc.top

PHP:  $name = trim(fgets(STDIN));
来源：http://vsf.zycfv.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://sfr.epnwcf.com

TS:   // Node.js：readline 模块
来源：http://xcx.fengsongda.top

Java: new Scanner(System.in).nextLine()
来源：http://jbg.wangshuangyany.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yii.dianchejie.cn

Ruby: gets.chomp
来源：http://xoa.yfazqb.com

C#:   Console.ReadLine();
来源：http://gkf.xuanzx.com

[A21] 保留指定小数位输出
来源：http://uld.yvedp.cn

Py:   f"{3.14159:.2f}"
来源：http://tlj.gaohongyu789.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gab.shanyushiyangtech.top

JS:   (3.14159).toFixed(2)
来源：http://ccb.jinqigufen.top

TS:   (3.14159).toFixed(2)
来源：http://ahv.gotoacloud.top

Java: String.format("%.2f", 3.14159)
来源：http://bvw.zycfv.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://enq.dashuyun.cn

Ruby: format("%.2f", 3.14159)
来源：http://jkn.ydjk.org.cn

C#:   3.14159.ToString("F2")
来源：http://yui.yuxming.cn

[A22] 获取字符串长度
来源：http://msb.pycfn.com

Py:   len(s)
来源：http://ytl.jlsjyb.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://eeh.yuxming.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://anh.vehdjk.com

TS:   s.length
来源：http://fkb.andypj.xyz

Java: s.length()
来源：http://ovc.shzxlz.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nmk.jiagoushi.top

Ruby: s.length
来源：http://lvx.cucudq.cn

C#:   s.Length
来源：http://cgy.feifeiyinyue.top

[A23] 大小写转换
来源：http://ksy.gzhubu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://nbr.nwbrower.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://tko.ybcxt.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hvo.ydjk.org.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://iep.pengpengdd.cyou

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zmr.yj202588.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://axw.xylfe.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tha.havefunace.top

C#:   s.ToUpper(); s.ToLower()
来源：http://hav.316326.xyz

[A24] 去除首尾空白
来源：http://eid.nwbrower.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://duk.jianghu66.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mll.jinqigfzy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oat.jianghu66.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tkg.xylfe.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bsb.zhiwuduotai.top

Go:   strings.TrimSpace(s)
来源：http://kjw.jinyuanbaomall.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://try.cqqwz.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zqj.redwolf501.top

[A25] 字符串比较
来源：http://yhz.jinyuanbaomall.cn

Py:   s1 == s2; s1 != s2
来源：http://wpi.wangdashe.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ceq.jinghuilouyu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kih.feifeiyinyue.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://omd.cucudq.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gnc.fanxiaobao.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kxs.yj202588.top

Ruby: s1 == s2; s1 <=> s2
来源：http://wsg.meibo888.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pyw.jiagoushi.top

[A26] 类型转换总览
来源：http://vlm.yuanzhike.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tqk.aizwys.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tsq.xuanzx.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://grn.chenjidiqi.icu

TS:   Number() String() Boolean() x as number
来源：http://kqz.yuxming.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zpn.jinqigufen.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hwm.zhongyouzk.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://zak.yongpay.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yau.zhijiandao.cn

================================================================================
来源：http://hss.shanyushiyangkeji.top

B. 流程控制
来源：http://wga.yanxiufei.cn

================================================================================
来源：http://gec.ydzc1.top

[B01] 条件判断 if / else
来源：http://uiy.tarul.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://kmg.aibaodan.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://eyu.pengpengdd.cyou

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qmm.zhiwuduotai.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dcf.fzhhl.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://rxk.ppjwa.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xhr.shanyushiyangtech.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dgf.uphjek.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mcp.fehbvm.com

[B02] 多分支 else if / elif
来源：http://fto.kuanghao11.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zxu.tanke756.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mcp.jinyuanbaomall.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://llr.yangfankeji.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uin.bbcook.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pjz.gotoacloud.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tja.yj20258888.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://any.hnxiangtu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ydd.hongshengwenyu.top

[B03] switch / match / case
来源：http://ifb.smart0.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bct.shangyingyoupin.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pln.shanyushiyangtech.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gzu.hywenlv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vxu.pengpengdd.cyou

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lap.yangfankeji.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rns.cqqwz.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zxc.birdmap.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jdz.sysykeji.top

[B04] for 计数循环
来源：http://gtv.fehbvm.com

Py:   for i in range(10): print(i)
来源：http://kbc.hongshengwenyu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zzn.cqqwz.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pcc.epnwcf.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://izw.c1oappe.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ohj.xuanzx.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jmf.fktsv.cn

Ruby: 10.times { |i| puts i }
来源：http://cnb.jinqigufen.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gpx.yj20258888.top

[B05] 遍历数组 / 列表
来源：http://dbc.yonumen.top

Py:   for item in arr: print(item)
来源：http://dpd.jinqigufen.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vjc.yueranfly.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hab.redwolf501.top

TS:   for (const item of arr) { console.log(item); }
来源：http://cog.ehwqpu.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://mdn.chenjidiqi.icu

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xqx.guowangkeji.top

Ruby: arr.each { |item| puts item }
来源：http://tsk.chenlongwang.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mrh.zhoulong.xyz

[B06] 遍历字典 / 对象
来源：http://duf.hongshengwenyu.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ttq.xingfuxueyuan.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://eyg.yongpay.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eel.quarkkingdee.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://aoa.epnwcf.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gkh.meibo888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://agg.meibo888.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xea.xuetiantiany.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cht.sweek.top

[B07] while 循环
来源：http://ljz.pengpengdd.cyou

Py:   while i < 10: i += 1
来源：http://pga.iojbl.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xbg.shanyushiyangkeji.top

JS:   while (i < 10) { i++; }
来源：http://zeb.daxiang520.top

TS:   while (i < 10) { i++; }
来源：http://lqo.tanke756.top

Java: while (i < 10) { i++; }
来源：http://gih.fktsv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ukc.guowangkeji.top

Ruby: while i < 10; i += 1; end
来源：http://rcc.cdnleiting.top

C#:   while (i < 10) { i++; }
来源：http://yei.aizwys.cn

[B08] do-while（至少执行一次）
来源：http://fbi.sxryk.cn

Py:   # 无 do-while：用 while True + break
来源：http://dne.pycfn.com

PHP:  do { $i++; } while ($i < 10);
来源：http://wtt.jinghuilouyu.cn

JS:   do { i++; } while (i < 10);
来源：http://fji.ydjk.org.cn

TS:   do { i++; } while (i < 10);
来源：http://gyt.tarul.cn

Java: do { i++; } while (i < 10);
来源：http://fpc.jyoumei.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://uvk.cqqwz.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mqt.feifeiyinyue.top

C#:   do { i++; } while (i < 10);
来源：http://cvn.sxryk.cn

[B09] break 与 continue
来源：http://qte.tarul.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kks.xylfe.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rso.hnqzz.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tma.c1oappe.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kul.hywenlv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yxb.vehdjk.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dpb.chenlongwang.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pzt.nwbrower.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fbe.hnqzz.top

[B10] 遍历同时拿索引
来源：http://ece.fengsongda.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gpc.ybcxt.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://klc.cashguo.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://anf.tian-w.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yjf.uphjek.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qao.fengsongda.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://war.daxiang520.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wvv.meibo888.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ktw.sweek.top

[B11] 生成数字序列 / 区间
来源：http://mua.havefunace.top

Py:   list(range(0, 10, 2))
来源：http://deu.jqgfzy.top

PHP:  range(0, 10, 2);
来源：http://awn.sweek.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rwk.zhaomingkeji.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pxc.ydzc1.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gqf.zhixingplan.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fqy.sjlbkw.cn

Ruby: (0...10).step(2).to_a
来源：http://vmb.aibaodan.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pry.ybcxt.top

[B12] 跳出多层循环
来源：http://kxp.jyoumei.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://duk.xingfuxueyuan.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://jon.jiagoushi.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xef.shuidangran.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://utk.hywenlv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cqf.mhx1999.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://liw.hesvh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ovg.wangdashe.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qdl.yuanzhike.top

[B13] 判断是否为数字
来源：http://knr.ehwqpu.com

Py:   isinstance(x, (int, float))
来源：http://mku.tarul.cn

PHP:  is_numeric($x)
来源：http://tvq.shuidangran.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://opu.cqqwz.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fvh.gogol.net.cn

Java: x instanceof Number
来源：http://cik.xingfuxueyuan.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jxf.haohaochexian.top

Ruby: x.is_a?(Numeric)
来源：http://oyy.zhongyouzk.top

C#:   x is int or double or decimal
来源：http://euy.bjfxy.top

[B14] 判断值是否在集合内
来源：http://rck.ppjwa.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mhc.sysykeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rpk.haohaochexian.top

JS:   [1, 2, 3].includes(x)
来源：http://vtt.zhiwuduotai.top

TS:   [1, 2, 3].includes(x)
来源：http://fcm.pycfn.com

Java: List.of(1, 2, 3).contains(x)
来源：http://nrr.cqqwz.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vvp.52xcode.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lqe.nanxinkj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lvb.shanyushiyangtech.top

[B15] 布尔运算与取反
来源：http://inv.wangdashe.top

Py:   a and b or not c
来源：http://goh.yvedp.cn

PHP:  $a && $b || !$c
来源：http://ayc.gotoacloud.top

JS:   a && b || !c
来源：http://clv.ivvv.top

TS:   a && b || !c
来源：http://oss.nwbrower.top

Java: a && b || !c
来源：http://puw.xingfuxueyuan.xyz

Go:   a && b || !c
来源：http://tnj.tanke756.top

Ruby: a && b || !c
来源：http://gsw.svipenyu.cn

C#:   a && b || !c
来源：http://dcb.sxryk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vfl.tarul.cn

Py:   if not data: return
来源：http://hnb.316326.xyz

PHP:  if (!$data) { return; }
来源：http://cno.52xcode.cn

JS:   if (!data) return;
来源：http://wkl.aibaodan.cn

TS:   if (!data) return;
来源：http://dfz.xuanzx.com


<!-- 参考信息 -->