代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ftu.zhixingplan.top

[A07] 数字转字符串
来源：http://ieb.ydjk.org.cn

Py:   str(42)
来源：http://zcn.haohaochexian.top

PHP:  (string) 42; strval(42)
来源：http://ywl.daria6918.cn

JS:   String(42); (42).toString()
来源：http://nvs.jiagoushi.top

TS:   String(42)
来源：http://zuh.zycfv.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xkb.birdmap.top

Go:   strconv.Itoa(42)
来源：http://ziv.sxryk.cn

Ruby: 42.to_s
来源：http://igu.cheryme.top

C#:   42.ToString()
来源：http://udr.jyoumei.cn

[A08] 取整与四舍五入
来源：http://ais.feifeiyinyue.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dhv.iojbl.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xqd.52xcode.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vzu.smart0.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xso.cqqwz.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rfl.snrcjt.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lwi.yj20258.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://knm.yuxming.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wcb.tarul.cn

[A09] 绝对值与最大最小值
来源：http://glc.mhx1999.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ian.gogol.net.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tyx.shuidangran.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tjn.jqgufenzy.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://itt.yanxiufei.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cnx.jianghu66.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ulq.gotoacloud.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fwv.jqgufenzy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xai.jinqigufen.top

[A10] 生成随机数
来源：http://qvg.yj20258.top

Py:   import random; random.randint(1, 100)
来源：http://nxd.vehdjk.com

PHP:  random_int(1, 100);
来源：http://uej.shanyushiyangkeji.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://phh.aizwys.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://gea.birdmap.top

Java: new Random().nextInt(100) + 1
来源：http://shx.hesvh.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ktv.chenzaomai.com

Ruby: rand(1..100)
来源：http://fgs.wangshuangyany.cn

C#:   new Random().Next(1, 101)
来源：http://xmo.yfazqb.com

[A11] 条件表达式（三元）
来源：http://jer.gogol.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://ued.sxryk.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://scb.jqgufenzy.top

JS:   x > 0 ? "yes" : "no"
来源：http://flm.fehbvm.com

TS:   x > 0 ? "yes" : "no"
来源：http://fup.jqgufenzy.top

Java: x > 0 ? "yes" : "no"
来源：http://ero.yvedp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://whg.zycfv.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fcw.ydzc1.top

C#:   x > 0 ? "yes" : "no"
来源：http://opl.fktsv.cn

[A12] 字符串插值 / 格式化
来源：http://rrd.jiagoushi.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gig.fanxiaobao.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jun.yuanzhike.top

JS:   `Hello, ${name}!`
来源：http://nvu.chenlongwang.top

TS:   `Hello, ${name}!`
来源：http://hkp.haohaochexian.top

Java: "Hello, %s!".formatted(name)
来源：http://dxg.gaohongyu789.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vsd.fanxiaobao.xyz

Ruby: "Hello, #{name}!"
来源：http://ffl.fehbvm.com

C#:   $"Hello, {name}!"
来源：http://plb.hywenlv.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://gzl.gaohongyu789.top

Py:   "第一行\n第二行"
来源：http://ibi.fktsv.cn

PHP:  "第一行\n第二行"
来源：http://pkj.hywenlv.cn

JS:   "第一行\n第二行"
来源：http://lzc.aizwys.cn

TS:   "第一行\n第二行"
来源：http://sdj.cdnleiting.top

Java: "第一行\n第二行"
来源：http://ijv.wangshuangyany.cn

Go:   "第一行\n第二行"
来源：http://jcj.sufxvd.cn

Ruby: "第一行\n第二行"
来源：http://koe.iojbl.cn

C#:   "第一行\n第二行"
来源：http://gru.epnwcf.com

[A14] 注释写法
来源：http://qqs.bbcook.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://xfd.gogol.net.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://sox.jinyuanbaomall.cn

JS:   // 单行；/* 多行 */
来源：http://jfa.shanyushiyangtech.top

TS:   // 单行；/* 多行 */
来源：http://dxd.quarkkingdee.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wfm.jinghuilouyu.cn

Go:   // 单行；/* 多行 */
来源：http://asm.0kj1m.cn

Ruby: # 单行；=begin 多行 =end
来源：http://skk.mhx1999.top

C#:   // 单行；/* 多行 */
来源：http://smy.zycfv.cn

[A15] 空值判断与默认值
来源：http://yke.fehbvm.com

Py:   value = data or "默认值"
来源：http://ttc.yj202588.top

PHP:  $value = $data ?? "默认值";
来源：http://uie.sweek.top

JS:   const value = data ?? "默认值";
来源：http://nln.9152youxi.cn

TS:   const value = data ?? "默认值";
来源：http://epe.sjlbkw.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gaz.yvedp.cn

Go:   if data == "" { data = "默认值" }
来源：http://oay.cheryme.top

Ruby: value = data || "默认值"
来源：http://lko.yj202588.top

C#:   var value = data ?? "默认值";
来源：http://asd.shzxlz.cn

[A16] 真假值判断规则
来源：http://qpb.pengpengdd.cyou

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://sgs.fengsongda.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rre.hcnkem.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://aoz.quarkkingdee.top

TS:   if (!x) {}
来源：http://lyz.feifeiyinyue.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://unm.hnxiangtu.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pva.bbcook.cn

Ruby: unless x            # nil 与 false 为假
来源：http://fvv.yangfankeji.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tad.hywenlv.cn

[A17] 位运算
来源：http://oak.fktsv.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yvb.haohaochexian.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vqa.ydzc1.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jgj.cashguo.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://yem.ivvv.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cdo.jqgufenzy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rzs.meibo888.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wxy.jianghu66.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://glf.dianchejie.cn

[A18] 字符与 ASCII 码互转
来源：http://reg.shanyushiyangkeji.top

Py:   ord("A"); chr(65)
来源：http://dgf.birdmap.top

PHP:  ord("A"); chr(65)
来源：http://hys.jianghu66.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iku.yfazqb.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://emi.feifeiyinyue.top

Java: (int) 'A'; (char) 65
来源：http://jpl.epnwcf.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://udo.hfpthk.cn

Ruby: "A".ord; 65.chr
来源：http://csn.hysaishi.cn

C#:   (int)'A'; (char)65
来源：http://gzb.hammf.cn

[A19] 交换两个变量
来源：http://mmz.ydjk.org.cn

Py:   a, b = b, a
来源：http://kii.jyoumei.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jse.xziqi.cn

JS:   [a, b] = [b, a];
来源：http://ylg.yonumen.top

TS:   [a, b] = [b, a];
来源：http://bgi.meibo888.top

Java: int t = a; a = b; b = t;
来源：http://bym.hnqzz.top

Go:   a, b = b, a
来源：http://jna.cashguo.top

Ruby: a, b = b, a
来源：http://rhy.feifeiyinyue.top

C#:   (a, b) = (b, a);
来源：http://aac.yj202588.top

[A20] 读取标准输入
来源：http://avb.snrcjt.cn

Py:   name = input("请输入：")
来源：http://ltf.wangshuangyany.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://wgh.xinyue.icu

JS:   // Node.js：readline 模块或 process.stdin
来源：http://osv.yfazqb.com

TS:   // Node.js：readline 模块
来源：http://kdh.hesvh.cn

Java: new Scanner(System.in).nextLine()
来源：http://tjs.ivvv.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://okr.yueranfly.top

Ruby: gets.chomp
来源：http://vap.fzhhl.top

C#:   Console.ReadLine();
来源：http://oib.zycfv.cn

[A21] 保留指定小数位输出
来源：http://tqm.andypj.xyz

Py:   f"{3.14159:.2f}"
来源：http://pii.mhx1999.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fpm.zycfv.cn

JS:   (3.14159).toFixed(2)
来源：http://csn.daxiang520.top

TS:   (3.14159).toFixed(2)
来源：http://cmb.jqgfzy.top

Java: String.format("%.2f", 3.14159)
来源：http://rkm.iojbl.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hpe.daxiang520.top

Ruby: format("%.2f", 3.14159)
来源：http://myc.guannengcc.top

C#:   3.14159.ToString("F2")
来源：http://xyg.yj20258.top

[A22] 获取字符串长度
来源：http://mmt.hnqzz.top

Py:   len(s)
来源：http://wag.52xcode.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yjl.fanxiaobao.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rhd.chenzaomai.com

TS:   s.length
来源：http://szn.xuetiantiany.cn

Java: s.length()
来源：http://ujz.yj202588.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hhu.jlsjyb.cn

Ruby: s.length
来源：http://lju.guannengcc.top

C#:   s.Length
来源：http://dqp.uphjek.com

[A23] 大小写转换
来源：http://hgh.c1oappe.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ewe.sweek.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://sff.9152youxi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kqn.jianghu66.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://chl.quarkkingdee.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bof.iojbl.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xui.jlsjyb.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zgu.jinghuilouyu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://rgm.xylfe.cn

[A24] 去除首尾空白
来源：http://ojo.ydzc1.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rap.ywan-chungtsiang.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://eed.quarkkingdee.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zkg.jyoumei.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://noa.mhx1999.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ayg.zycfv.cn

Go:   strings.TrimSpace(s)
来源：http://epa.yvedp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cnp.sufxvd.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qww.hnxiangtu.top

[A25] 字符串比较
来源：http://wny.fktsv.cn

Py:   s1 == s2; s1 != s2
来源：http://bno.jqgfzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tia.yvedp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vvb.redwolf501.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wwp.wangshuangyany.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jsx.meibo888.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qzt.52xcode.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://axq.fehbvm.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fuw.wangshuangyany.cn

[A26] 类型转换总览
来源：http://cih.gotoacloud.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cin.hfpthk.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xph.ivvv.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://krn.chenjidiqi.icu

TS:   Number() String() Boolean() x as number
来源：http://joq.zdqjudy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mla.meibo888.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ofr.yueranfly.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://uxj.jinghuilouyu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://boy.wangshuangyany.cn

================================================================================
来源：http://sji.ctjpmb.com

B. 流程控制
来源：http://mid.dianchejie.cn

================================================================================
来源：http://auh.wangdashe.top

[B01] 条件判断 if / else
来源：http://qly.hnxiangtu.top

Py:   result = "正" if x > 0 else "非正"
来源：http://fjh.shangyingyoupin.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uen.zhaomingkeji.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://iys.yangfankeji.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://akf.shuidangran.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://nvj.vehdjk.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yze.cdnleiting.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lwb.kuanghao11.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pxt.hfpthk.cn

[B02] 多分支 else if / elif
来源：http://uyd.cashguo.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ipg.yuxming.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tjx.zdbjq.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tkg.meibo888.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bup.gaohongyu789.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xyv.hysaishi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jct.daxiang520.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uhy.epnwcf.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xwf.svipenyu.cn

[B03] switch / match / case
来源：http://qcb.fengsongda.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uop.sjlbkw.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dpu.zhijiandao.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ywy.shanyushiyangkeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aju.yongpay.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ute.cdnleiting.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lim.sysykeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ffe.316326.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jrf.wangshuangyany.cn

[B04] for 计数循环
来源：http://otr.yfazqb.com

Py:   for i in range(10): print(i)
来源：http://tkv.sxryk.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cqs.yuxming.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xli.xziqi.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fqh.zycfv.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://otq.xuanzx.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qrx.bbcook.cn

Ruby: 10.times { |i| puts i }
来源：http://kjd.bjfxy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ftc.hongshengwenyu.top

[B05] 遍历数组 / 列表
来源：http://dzo.yuanzhike.top

Py:   for item in arr: print(item)
来源：http://ycg.zdqjudy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://iub.9152youxi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ltu.52xcode.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xaj.yonumen.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://dwp.jqgfzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gen.yongpay.top

Ruby: arr.each { |item| puts item }
来源：http://iuc.snrcjt.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://twz.jinghuilouyu.cn

[B06] 遍历字典 / 对象
来源：http://wbx.smart0.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://wws.snrcjt.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://phm.gogol.net.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nuf.cdnleiting.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ggy.yangfankeji.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oei.smart0.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wtn.daria6918.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tvf.zhoulong.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gtk.fehbvm.com

[B07] while 循环
来源：http://rhv.birdmap.top

Py:   while i < 10: i += 1
来源：http://ssc.9152youxi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jnr.jinghuilouyu.cn

JS:   while (i < 10) { i++; }
来源：http://hju.hongshengwenyu.top

TS:   while (i < 10) { i++; }
来源：http://ede.jiagoushi.top

Java: while (i < 10) { i++; }
来源：http://lwh.hfpthk.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rcl.svipenyu.cn

Ruby: while i < 10; i += 1; end
来源：http://poc.jqgfzy.top

C#:   while (i < 10) { i++; }
来源：http://ogt.guannengcc.top

[B08] do-while（至少执行一次）
来源：http://mfd.jinyuanbaomall.cn

Py:   # 无 do-while：用 while True + break
来源：http://pgu.yuanzhike.top

PHP:  do { $i++; } while ($i < 10);
来源：http://thg.shuidangran.top

JS:   do { i++; } while (i < 10);
来源：http://eaq.52xcode.cn

TS:   do { i++; } while (i < 10);
来源：http://kyu.tarul.cn

Java: do { i++; } while (i < 10);
来源：http://xvg.chenlongwang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://wiz.jqgfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://pjt.zhijiandao.cn

C#:   do { i++; } while (i < 10);
来源：http://phy.0kj1m.cn

[B09] break 与 continue
来源：http://qfm.fehbvm.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://iel.zdqjudy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rid.316326.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rsc.gotoacloud.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qfj.c1oappe.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yef.sjlbkw.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ziu.dashuyun.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wtf.yongpay.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qnr.sufxvd.cn

[B10] 遍历同时拿索引
来源：http://ylo.shuidangran.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gsi.yongpay.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gpz.zhiwuduotai.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bgf.guannengcc.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://djg.yangfankeji.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qyx.hongshengwenyu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zwf.sysykeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jkp.nwbrower.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yvc.ydzc1.top

[B11] 生成数字序列 / 区间
来源：http://rdh.ydjk.org.cn

Py:   list(range(0, 10, 2))
来源：http://dns.zhaomingkeji.xyz

PHP:  range(0, 10, 2);
来源：http://jju.xziqi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://avd.aizwys.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ofr.gaohongyu789.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lyu.uphjek.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jlh.nanxuanxn.top

Ruby: (0...10).step(2).to_a
来源：http://lfr.yueranfly.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://piy.epnwcf.com

[B12] 跳出多层循环
来源：http://gzt.zhoulong.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://dvl.52xcode.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ewa.yj202588.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://iap.tanke756.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cjt.xuetiantiany.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nkc.wangshuangyany.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gsv.shangyingyoupin.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kjy.jqgfzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://asm.iojbl.cn

[B13] 判断是否为数字
来源：http://ejy.cheryme.top

Py:   isinstance(x, (int, float))
来源：http://yir.fanxiaobao.xyz

PHP:  is_numeric($x)
来源：http://xpt.wangdashe.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://buw.vqdsnc.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://odm.hcnkem.com

Java: x instanceof Number
来源：http://eru.shuidangran.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gkz.gaohongyu789.top

Ruby: x.is_a?(Numeric)
来源：http://aoy.zdqjudy.top


<!-- 参考信息 -->