代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://wvg.zhijiandao.cn

TS:   x > 0 ? "yes" : "no"
来源：http://iob.jinqigufen.top

Java: x > 0 ? "yes" : "no"
来源：http://oml.aizwys.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://xtr.jinghuilouyu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://sbi.snrcjt.cn

C#:   x > 0 ? "yes" : "no"
来源：http://igv.guannengcc.top

[A12] 字符串插值 / 格式化
来源：http://nfz.yangfankeji.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://egf.hammf.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ylj.ivvv.top

JS:   `Hello, ${name}!`
来源：http://fbz.fehbvm.com

TS:   `Hello, ${name}!`
来源：http://tah.yfazqb.com

Java: "Hello, %s!".formatted(name)
来源：http://xth.jyoumei.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://asp.yvedp.cn

Ruby: "Hello, #{name}!"
来源：http://hrd.sweek.top

C#:   $"Hello, {name}!"
来源：http://gpm.jinqigfzy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://fth.birdmap.top

Py:   "第一行\n第二行"
来源：http://ayn.hywenlv.cn

PHP:  "第一行\n第二行"
来源：http://ytz.uphjek.com

JS:   "第一行\n第二行"
来源：http://vhq.hnqzz.top

TS:   "第一行\n第二行"
来源：http://rgz.jinqigfzy.top

Java: "第一行\n第二行"
来源：http://xha.birdmap.top

Go:   "第一行\n第二行"
来源：http://zbh.bbcook.cn

Ruby: "第一行\n第二行"
来源：http://goy.guannengcc.top

C#:   "第一行\n第二行"
来源：http://xhc.snrcjt.cn

[A14] 注释写法
来源：http://pij.mhx1999.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ncz.yvedp.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://shr.yj202588.top

JS:   // 单行；/* 多行 */
来源：http://uev.tianlin.xyz

TS:   // 单行；/* 多行 */
来源：http://sur.ydzc1.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dfi.birdmap.top

Go:   // 单行；/* 多行 */
来源：http://alh.vehdjk.com

Ruby: # 单行；=begin 多行 =end
来源：http://ozx.0kj1m.cn

C#:   // 单行；/* 多行 */
来源：http://pib.jinqigfzy.top

[A15] 空值判断与默认值
来源：http://yat.zhongyouzk.top

Py:   value = data or "默认值"
来源：http://kmu.smart0.xyz

PHP:  $value = $data ?? "默认值";
来源：http://ivi.guowangkeji.top

JS:   const value = data ?? "默认值";
来源：http://ssk.52xcode.cn

TS:   const value = data ?? "默认值";
来源：http://hum.shangyingyoupin.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://lrz.kuanghao11.cn

Go:   if data == "" { data = "默认值" }
来源：http://xae.chenlongwang.top

Ruby: value = data || "默认值"
来源：http://ynr.ppjwa.cn

C#:   var value = data ?? "默认值";
来源：http://uev.jiagoushi.top

[A16] 真假值判断规则
来源：http://kuw.vqdsnc.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://gcg.zhoulong.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://set.zdbjq.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cjy.fzhhl.top

TS:   if (!x) {}
来源：http://uyn.xingfuxueyuan.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ckc.epnwcf.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://eze.aibaodan.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vgu.nanxinkj.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ttq.daria6918.cn

[A17] 位运算
来源：http://ctp.birdmap.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dje.hcnkem.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jso.sjlbkw.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://msq.shanyushiyangtech.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://niu.hnqzz.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ert.ybcxt.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zuu.0kj1m.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ibw.pycfn.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cvd.ehwqpu.com

[A18] 字符与 ASCII 码互转
来源：http://qle.pycfn.com

Py:   ord("A"); chr(65)
来源：http://etz.yj202588.top

PHP:  ord("A"); chr(65)
来源：http://ijw.iojbl.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wor.52xcode.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://skt.cashguo.top

Java: (int) 'A'; (char) 65
来源：http://trh.nwbrower.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ghp.fktsv.cn

Ruby: "A".ord; 65.chr
来源：http://dfa.epnwcf.com

C#:   (int)'A'; (char)65
来源：http://hoc.bjfxy.top

[A19] 交换两个变量
来源：http://jot.guannengcc.top

Py:   a, b = b, a
来源：http://ugv.pycfn.com

PHP:  [$a, $b] = [$b, $a];
来源：http://dzd.fanxiaobao.xyz

JS:   [a, b] = [b, a];
来源：http://jev.tianlin.xyz

TS:   [a, b] = [b, a];
来源：http://clc.ivvv.top

Java: int t = a; a = b; b = t;
来源：http://qyl.haohaochexian.top

Go:   a, b = b, a
来源：http://kbc.uphjek.com

Ruby: a, b = b, a
来源：http://jcf.meibo888.top

C#:   (a, b) = (b, a);
来源：http://ous.tian-w.cn

[A20] 读取标准输入
来源：http://jgy.xziqi.cn

Py:   name = input("请输入：")
来源：http://jsc.ctjpmb.com

PHP:  $name = trim(fgets(STDIN));
来源：http://zth.yongpay.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wii.ctjpmb.com

TS:   // Node.js：readline 模块
来源：http://vei.yj20258888.top

Java: new Scanner(System.in).nextLine()
来源：http://pwx.gotoacloud.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sbr.yueranfly.top

Ruby: gets.chomp
来源：http://enz.xuetiantiany.cn

C#:   Console.ReadLine();
来源：http://ptt.guannengcc.top

[A21] 保留指定小数位输出
来源：http://mix.xuetiantiany.cn

Py:   f"{3.14159:.2f}"
来源：http://wfm.shzxlz.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://thw.svipenyu.cn

JS:   (3.14159).toFixed(2)
来源：http://fdi.c1oappe.top

TS:   (3.14159).toFixed(2)
来源：http://wfv.ehwqpu.com

Java: String.format("%.2f", 3.14159)
来源：http://khz.jinqigfzy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vjn.meibo888.top

Ruby: format("%.2f", 3.14159)
来源：http://dpt.ivvv.top

C#:   3.14159.ToString("F2")
来源：http://pha.zycfv.cn

[A22] 获取字符串长度
来源：http://nsj.dianchejie.cn

Py:   len(s)
来源：http://uum.9152youxi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pct.hammf.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dea.bjfxy.top

TS:   s.length
来源：http://xsg.shuidangran.top

Java: s.length()
来源：http://npn.smart0.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dnk.shzxlz.cn

Ruby: s.length
来源：http://swl.xinyue.icu

C#:   s.Length
来源：http://kxq.yuanzhike.top

[A23] 大小写转换
来源：http://bgc.fanxiaobao.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://uyc.jinyuanbaomall.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vry.hongshengwenyu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rhv.sufxvd.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ynj.andypj.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://irr.hcnkem.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ake.epnwcf.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xba.nanxuanxn.top

C#:   s.ToUpper(); s.ToLower()
来源：http://iau.tian-w.cn

[A24] 去除首尾空白
来源：http://icx.ydzc1.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fwz.redwolf501.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mgl.tanke756.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uvt.xylfe.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://moe.ydzc1.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xbu.zdbjq.cn

Go:   strings.TrimSpace(s)
来源：http://lsm.cashguo.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ydk.ehwqpu.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hjj.uphjek.com

[A25] 字符串比较
来源：http://jwq.jinyuanbaomall.cn

Py:   s1 == s2; s1 != s2
来源：http://sff.vehdjk.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kij.52xcode.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vnh.jinghuilouyu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yjv.jyoumei.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://btu.shzxlz.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://inp.hesvh.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://exp.gaohongyu789.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yex.fktsv.cn

[A26] 类型转换总览
来源：http://hrr.shuidangran.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vov.xziqi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ulb.xylfe.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tfz.sysykeji.top

TS:   Number() String() Boolean() x as number
来源：http://sll.tarul.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ftb.epnwcf.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dap.zhongyouzk.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://yyr.hcnkem.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ide.cqqwz.cn

================================================================================
来源：http://zbg.andypj.xyz

B. 流程控制
来源：http://ant.jinyuanbaomall.cn

================================================================================
来源：http://swj.zhiwuduotai.top

[B01] 条件判断 if / else
来源：http://cdq.mhx1999.top

Py:   result = "正" if x > 0 else "非正"
来源：http://wkz.havefunace.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xdz.shangyingyoupin.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ypx.shanyushiyangkeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ipw.vqdsnc.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ipn.ctjpmb.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rtw.cdnleiting.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://etm.xuetiantiany.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zmn.haohaochexian.top

[B02] 多分支 else if / elif
来源：http://xpm.xinyue.icu

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://iwu.yongpay.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rbo.hammf.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://imn.fehbvm.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zzz.fanxiaobao.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ltj.smart0.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bih.hammf.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nms.zycfv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jwf.sufxvd.cn

[B03] switch / match / case
来源：http://dfr.yuanzhike.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dpy.xinyue.icu

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ggt.ctjpmb.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kbh.cashguo.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hag.yj20258.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://atu.aibaodan.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qxl.tarul.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qgo.wangdashe.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://flp.jinyuanbaomall.cn

[B04] for 计数循环
来源：http://cdu.zhiwuduotai.top

Py:   for i in range(10): print(i)
来源：http://cmy.yuanzhike.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qpq.jlsjyb.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pga.hnxiangtu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fip.feifeiyinyue.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://spt.snrcjt.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kix.gzhubu.top

Ruby: 10.times { |i| puts i }
来源：http://ywj.tarul.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://thn.xziqi.cn

[B05] 遍历数组 / 列表
来源：http://qlk.sxryk.cn

Py:   for item in arr: print(item)
来源：http://wbo.yangfankeji.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jfn.jyoumei.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xbe.gotoacloud.top

TS:   for (const item of arr) { console.log(item); }
来源：http://akj.xylfe.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xok.gaohongyu789.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jiu.nwbrower.top

Ruby: arr.each { |item| puts item }
来源：http://gco.cucudq.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ric.yuanzhike.top

[B06] 遍历字典 / 对象
来源：http://irz.jinqigufen.top

Py:   for k, v in d.items(): print(k, v)
来源：http://hxf.daxiang520.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://adi.zdqjudy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qzx.nanxuanxn.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://goc.zhixingplan.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://swc.yongpay.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eay.cdnleiting.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tcj.yangfankeji.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hst.kuanghao11.cn

[B07] while 循环
来源：http://tvx.pycfn.com

Py:   while i < 10: i += 1
来源：http://plj.aibaodan.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hnd.meibo888.top

JS:   while (i < 10) { i++; }
来源：http://gps.nwbrower.top

TS:   while (i < 10) { i++; }
来源：http://khj.hnqzz.top

Java: while (i < 10) { i++; }
来源：http://zic.yangfankeji.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mjv.sxryk.cn

Ruby: while i < 10; i += 1; end
来源：http://rbt.cqqwz.cn

C#:   while (i < 10) { i++; }
来源：http://ygj.svipenyu.cn

[B08] do-while（至少执行一次）
来源：http://thg.shuidangran.top

Py:   # 无 do-while：用 while True + break
来源：http://jrn.hywenlv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ikn.chenjidiqi.icu

JS:   do { i++; } while (i < 10);
来源：http://dqb.ywan-chungtsiang.top

TS:   do { i++; } while (i < 10);
来源：http://szq.cheryme.top

Java: do { i++; } while (i < 10);
来源：http://myd.redwolf501.top

Go:   for { i++; if i >= 10 { break } }
来源：http://zmt.snrcjt.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qre.chenjidiqi.icu

C#:   do { i++; } while (i < 10);
来源：http://npb.hcnkem.com

[B09] break 与 continue
来源：http://sfr.feifeiyinyue.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rst.zhongyouzk.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yqj.gogol.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://krt.hammf.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jef.9152youxi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aho.ywan-chungtsiang.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://iuu.tarul.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hrd.xylfe.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mwb.yj20258888.top

[B10] 遍历同时拿索引
来源：http://yxb.dashuyun.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qfq.c1oappe.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qzi.shzxlz.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jkh.yuxming.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qgt.jinghuilouyu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zno.zhixingplan.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xlb.feifeiyinyue.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xhy.hcnkem.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ubq.jlsjyb.cn

[B11] 生成数字序列 / 区间
来源：http://bwm.jlsjyb.cn

Py:   list(range(0, 10, 2))
来源：http://xhj.guannengcc.top

PHP:  range(0, 10, 2);
来源：http://qgh.yfazqb.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wqo.zycfv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://slp.zdqjudy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cxu.daria6918.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://brk.chenzaomai.com

Ruby: (0...10).step(2).to_a
来源：http://odv.cashguo.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jef.shzxlz.cn

[B12] 跳出多层循环
来源：http://elq.52xcode.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://izy.316326.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://dds.pycfn.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rhe.shangyingyoupin.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wzc.shuidangran.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://siy.xinyue.icu

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kie.xziqi.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zvs.hcnkem.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bxq.yueranfly.top

[B13] 判断是否为数字
来源：http://gxo.yuanzhike.top

Py:   isinstance(x, (int, float))
来源：http://hhd.shangyingyoupin.top

PHP:  is_numeric($x)
来源：http://bps.kuanghao11.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cgm.xinyue.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://plj.yfazqb.com

Java: x instanceof Number
来源：http://pmn.zhaomingkeji.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gdh.fktsv.cn

Ruby: x.is_a?(Numeric)
来源：http://faw.fzhhl.top

C#:   x is int or double or decimal
来源：http://zwm.guowangkeji.top

[B14] 判断值是否在集合内
来源：http://wvd.sjlbkw.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ibp.haohaochexian.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xxi.gogol.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://vfi.shanyushiyangtech.top

TS:   [1, 2, 3].includes(x)
来源：http://vzy.daxiang520.top

Java: List.of(1, 2, 3).contains(x)
来源：http://eqk.nanxinkj.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uzg.ppjwa.cn

Ruby: [1, 2, 3].include?(x)
来源：http://usj.jqgufenzy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kya.tian-w.cn

[B15] 布尔运算与取反
来源：http://xgm.zdqjudy.top

Py:   a and b or not c
来源：http://nei.cucudq.cn

PHP:  $a && $b || !$c
来源：http://tlk.zhongyouzk.top

JS:   a && b || !c
来源：http://jzy.yongpay.top

TS:   a && b || !c
来源：http://ydk.zhaomingkeji.xyz

Java: a && b || !c
来源：http://fcz.shangyingyoupin.top

Go:   a && b || !c
来源：http://doe.guannengcc.top

Ruby: a && b || !c
来源：http://oma.yvedp.cn

C#:   a && b || !c
来源：http://cyr.zdqjudy.top

[B16] 卫语句：不满足条件提前返回
来源：http://uzu.fktsv.cn

Py:   if not data: return
来源：http://hvu.redwolf501.top

PHP:  if (!$data) { return; }
来源：http://shf.daxiang520.top

JS:   if (!data) return;
来源：http://prb.sweek.top

TS:   if (!data) return;
来源：http://ntq.kuanghao11.cn

Java: if (data == null) return;
来源：http://jil.vehdjk.com

Go:   if data == nil { return }
来源：http://fcb.zdbjq.cn

Ruby: return if data.nil?
来源：http://ueu.jinghuilouyu.cn

C#:   if (data == null) return;
来源：http://tdn.cucudq.cn

================================================================================
来源：http://kqr.cashguo.top

C. 函数与作用域
来源：http://flr.daxiang520.top

================================================================================
来源：http://vze.iojbl.cn

[C01] 定义函数
来源：http://hee.jiagoushi.top

Py:   def add(a, b): return a + b
来源：http://kgf.uphjek.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mky.jqgufenzy.top

JS:   function add(a, b) { return a + b; }
来源：http://oix.xingfuxueyuan.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mts.hfpthk.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xug.hcnkem.com

Go:   func add(a, b int) int { return a + b }
来源：http://dnp.daria6918.cn

Ruby: def add(a, b); a + b; end
来源：http://ono.bbcook.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zcc.zdbjq.cn


<!-- 参考信息 -->