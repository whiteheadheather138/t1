代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://pwc.haohaochexian.top

[A11] 条件表达式（三元）
来源：http://nlk.xylfe.cn

Py:   "yes" if x > 0 else "no"
来源：http://njd.zhiwuduotai.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://yat.jiagoushi.top

JS:   x > 0 ? "yes" : "no"
来源：http://dzd.shuidangran.top

TS:   x > 0 ? "yes" : "no"
来源：http://lea.chenjidiqi.icu

Java: x > 0 ? "yes" : "no"
来源：http://pqj.bbcook.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://tga.jianghu66.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ijq.havefunace.top

C#:   x > 0 ? "yes" : "no"
来源：http://lcj.ydzc1.top

[A12] 字符串插值 / 格式化
来源：http://ocv.pengpengdd.cyou

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://oac.ydzc1.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://akx.andypj.xyz

JS:   `Hello, ${name}!`
来源：http://gov.nanxuanxn.top

TS:   `Hello, ${name}!`
来源：http://kfy.tarul.cn

Java: "Hello, %s!".formatted(name)
来源：http://nbq.cashguo.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wps.hysaishi.cn

Ruby: "Hello, #{name}!"
来源：http://fol.sufxvd.cn

C#:   $"Hello, {name}!"
来源：http://pxd.chenzaomai.com

[A13] 多行字符串（练习 \n 转义）
来源：http://amo.shangyingyoupin.top

Py:   "第一行\n第二行"
来源：http://xdm.hywenlv.cn

PHP:  "第一行\n第二行"
来源：http://pve.hesvh.cn

JS:   "第一行\n第二行"
来源：http://yub.jqgfzy.top

TS:   "第一行\n第二行"
来源：http://uej.jinqigufen.top

Java: "第一行\n第二行"
来源：http://zth.hnqzz.top

Go:   "第一行\n第二行"
来源：http://mui.sjlbkw.cn

Ruby: "第一行\n第二行"
来源：http://adq.yonumen.top

C#:   "第一行\n第二行"
来源：http://gmn.zycfv.cn

[A14] 注释写法
来源：http://zec.fengsongda.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://cch.c1oappe.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://duf.zhixingplan.top

JS:   // 单行；/* 多行 */
来源：http://hpf.xylfe.cn

TS:   // 单行；/* 多行 */
来源：http://bjp.feifeiyinyue.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bqk.cheryme.top

Go:   // 单行；/* 多行 */
来源：http://hfb.hammf.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qfx.316326.xyz

C#:   // 单行；/* 多行 */
来源：http://qia.jqgufenzy.top

[A15] 空值判断与默认值
来源：http://lpa.cucudq.cn

Py:   value = data or "默认值"
来源：http://wvp.jinqigufen.top

PHP:  $value = $data ?? "默认值";
来源：http://var.quarkkingdee.top

JS:   const value = data ?? "默认值";
来源：http://wpk.zdqjudy.top

TS:   const value = data ?? "默认值";
来源：http://axc.tanke756.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yey.redwolf501.top

Go:   if data == "" { data = "默认值" }
来源：http://wyi.ivvv.top

Ruby: value = data || "默认值"
来源：http://vpb.snrcjt.cn

C#:   var value = data ?? "默认值";
来源：http://gfa.jinghuilouyu.cn

[A16] 真假值判断规则
来源：http://ifn.ydjk.org.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ivz.shangyingyoupin.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hkd.chenjidiqi.icu

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gbs.aibaodan.cn

TS:   if (!x) {}
来源：http://cfb.hywenlv.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qgb.chenzaomai.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://juo.zhijiandao.cn

Ruby: unless x            # nil 与 false 为假
来源：http://opy.yj20258888.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ixj.fanxiaobao.xyz

[A17] 位运算
来源：http://smx.aizwys.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lhr.jlsjyb.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zqa.ydjk.org.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://edz.haohaochexian.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bzr.0kj1m.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bnd.uphjek.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://val.daria6918.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vha.zhaomingkeji.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iym.fanxiaobao.xyz

[A18] 字符与 ASCII 码互转
来源：http://ijg.cucudq.cn

Py:   ord("A"); chr(65)
来源：http://had.hammf.cn

PHP:  ord("A"); chr(65)
来源：http://tit.daria6918.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qbs.yj202588.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bvy.fktsv.cn

Java: (int) 'A'; (char) 65
来源：http://dus.feifeiyinyue.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fjh.jlsjyb.cn

Ruby: "A".ord; 65.chr
来源：http://gxf.gotoacloud.top

C#:   (int)'A'; (char)65
来源：http://ixb.yj202588.top

[A19] 交换两个变量
来源：http://kxb.birdmap.top

Py:   a, b = b, a
来源：http://wux.zhaomingkeji.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://iot.andypj.xyz

JS:   [a, b] = [b, a];
来源：http://qwm.sjlbkw.cn

TS:   [a, b] = [b, a];
来源：http://uoq.sysykeji.top

Java: int t = a; a = b; b = t;
来源：http://knq.yueranfly.top

Go:   a, b = b, a
来源：http://aak.nanxinkj.top

Ruby: a, b = b, a
来源：http://lrm.snrcjt.cn

C#:   (a, b) = (b, a);
来源：http://mqt.ydjk.org.cn

[A20] 读取标准输入
来源：http://jly.jqgfzy.top

Py:   name = input("请输入：")
来源：http://qwb.ivvv.top

PHP:  $name = trim(fgets(STDIN));
来源：http://fbw.chenjidiqi.icu

JS:   // Node.js：readline 模块或 process.stdin
来源：http://utz.aizwys.cn

TS:   // Node.js：readline 模块
来源：http://aru.yj20258888.top

Java: new Scanner(System.in).nextLine()
来源：http://hgq.zhaomingkeji.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pqh.jqgufenzy.top

Ruby: gets.chomp
来源：http://whj.yj202588.top

C#:   Console.ReadLine();
来源：http://lug.zycfv.cn

[A21] 保留指定小数位输出
来源：http://uvm.xziqi.cn

Py:   f"{3.14159:.2f}"
来源：http://znr.fanxiaobao.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tlq.zhiwuduotai.top

JS:   (3.14159).toFixed(2)
来源：http://qie.cdnleiting.top

TS:   (3.14159).toFixed(2)
来源：http://npr.yj20258.top

Java: String.format("%.2f", 3.14159)
来源：http://qvx.svipenyu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yby.yj20258.top

Ruby: format("%.2f", 3.14159)
来源：http://ljv.smart0.xyz

C#:   3.14159.ToString("F2")
来源：http://owt.yanxiufei.cn

[A22] 获取字符串长度
来源：http://kak.fengsongda.top

Py:   len(s)
来源：http://qow.andypj.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jce.wangdashe.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ctv.quarkkingdee.top

TS:   s.length
来源：http://wey.xingfuxueyuan.xyz

Java: s.length()
来源：http://nom.shangyingyoupin.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rmj.gogol.net.cn

Ruby: s.length
来源：http://mwx.quarkkingdee.top

C#:   s.Length
来源：http://kpt.shuidangran.top

[A23] 大小写转换
来源：http://eyh.ctjpmb.com

Py:   s.upper(); s.lower(); s.title()
来源：http://piv.quarkkingdee.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fcf.ywan-chungtsiang.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jpu.svipenyu.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vfh.yvedp.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jny.shangyingyoupin.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nag.hammf.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://awy.cheryme.top

C#:   s.ToUpper(); s.ToLower()
来源：http://emk.fengsongda.top

[A24] 去除首尾空白
来源：http://lyx.yuxming.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ust.hnqzz.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lah.xinyue.icu

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vvc.aibaodan.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bby.aizwys.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ldl.shanyushiyangtech.top

Go:   strings.TrimSpace(s)
来源：http://cnp.sxryk.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rxi.birdmap.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://agv.52xcode.cn

[A25] 字符串比较
来源：http://vin.jqgfzy.top

Py:   s1 == s2; s1 != s2
来源：http://emy.daxiang520.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://woe.9152youxi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uvc.hammf.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ytc.fzhhl.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cbg.jlsjyb.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dzy.cheryme.top

Ruby: s1 == s2; s1 <=> s2
来源：http://byl.chenlongwang.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lsn.yueranfly.top

[A26] 类型转换总览
来源：http://atj.sweek.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lxe.jqgufenzy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ayi.jinqigfzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qbh.ivvv.top

TS:   Number() String() Boolean() x as number
来源：http://gjm.nanxuanxn.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cwh.hcnkem.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gsp.zhijiandao.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nyo.shanyushiyangtech.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ago.redwolf501.top

================================================================================
来源：http://ywc.shanyushiyangkeji.top

B. 流程控制
来源：http://lty.ybcxt.top

================================================================================
来源：http://qpf.fehbvm.com

[B01] 条件判断 if / else
来源：http://ipx.zhongyouzk.top

Py:   result = "正" if x > 0 else "非正"
来源：http://xeh.hesvh.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mhl.ehwqpu.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://avr.xinyue.icu

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uyl.ywan-chungtsiang.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://pre.ivvv.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fdj.yueranfly.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rca.yangfankeji.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fjg.ywan-chungtsiang.top

[B02] 多分支 else if / elif
来源：http://xoh.ehwqpu.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uet.jiagoushi.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lxe.ywan-chungtsiang.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://krn.tarul.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xui.zhongyouzk.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tye.xuanzx.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hhw.yuanzhike.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jum.ydjk.org.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ttl.zhixingplan.top

[B03] switch / match / case
来源：http://xaj.zhiwuduotai.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cfv.dianchejie.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vzr.zhengqikj.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uid.zycfv.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rjh.ybcxt.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sba.ydjk.org.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://stp.zycfv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wmq.shuidangran.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cuf.wangshuangyany.cn

[B04] for 计数循环
来源：http://nuz.ehwqpu.com

Py:   for i in range(10): print(i)
来源：http://ryn.jqgufenzy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pon.yj20258888.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hoa.fanxiaobao.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lgy.ivvv.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ict.pengpengdd.cyou

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kwy.chenlongwang.top

Ruby: 10.times { |i| puts i }
来源：http://kmp.chenlongwang.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sde.yonumen.top

[B05] 遍历数组 / 列表
来源：http://qtm.gzhubu.top

Py:   for item in arr: print(item)
来源：http://eiu.vqdsnc.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fpn.jinghuilouyu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://auf.zhijiandao.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yrr.gzhubu.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fkh.hnxiangtu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ese.shzxlz.cn

Ruby: arr.each { |item| puts item }
来源：http://nvg.fengsongda.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://knr.jiagoushi.top

[B06] 遍历字典 / 对象
来源：http://nrp.bjfxy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ffm.nwbrower.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gml.fengsongda.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hak.zdbjq.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cyv.yj202588.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ety.yongpay.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eqh.dashuyun.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://boy.cheryme.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://soa.yonumen.top

[B07] while 循环
来源：http://wic.316326.xyz

Py:   while i < 10: i += 1
来源：http://fbs.hfpthk.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dwc.hfpthk.cn

JS:   while (i < 10) { i++; }
来源：http://fnz.jinghuilouyu.cn

TS:   while (i < 10) { i++; }
来源：http://dtm.svipenyu.cn

Java: while (i < 10) { i++; }
来源：http://cyv.bjfxy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wwd.zdbjq.cn

Ruby: while i < 10; i += 1; end
来源：http://sxi.daxiang520.top

C#:   while (i < 10) { i++; }
来源：http://hct.svipenyu.cn

[B08] do-while（至少执行一次）
来源：http://tpi.daria6918.cn

Py:   # 无 do-while：用 while True + break
来源：http://hdl.yuxming.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://etf.ctjpmb.com

JS:   do { i++; } while (i < 10);
来源：http://uyx.xuanzx.com

TS:   do { i++; } while (i < 10);
来源：http://qgt.9152youxi.cn

Java: do { i++; } while (i < 10);
来源：http://kze.fktsv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nlj.yueranfly.top

Ruby: begin; i += 1; end while i < 10
来源：http://dqt.hammf.cn

C#:   do { i++; } while (i < 10);
来源：http://eab.c1oappe.top

[B09] break 与 continue
来源：http://xdy.hongshengwenyu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://glo.xuetiantiany.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cbb.ppjwa.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bml.chenlongwang.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ges.zycfv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vmy.aibaodan.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wnd.iojbl.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dvv.9152youxi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mox.hnxiangtu.top

[B10] 遍历同时拿索引
来源：http://unv.uphjek.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://geh.ydjk.org.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zwc.cashguo.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://niv.zhijiandao.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://htz.yj20258.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://okx.xuetiantiany.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hne.hywenlv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fqk.sufxvd.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zmf.daria6918.cn

[B11] 生成数字序列 / 区间
来源：http://jzs.vehdjk.com

Py:   list(range(0, 10, 2))
来源：http://gvf.xziqi.cn

PHP:  range(0, 10, 2);
来源：http://sqp.yfazqb.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zur.meibo888.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zpg.ywan-chungtsiang.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://osn.pycfn.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gvt.nanxinkj.top

Ruby: (0...10).step(2).to_a
来源：http://map.c1oappe.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://czj.cheryme.top

[B12] 跳出多层循环
来源：http://sex.fengsongda.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://iyj.tanke756.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://gsj.tianlin.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://okz.shzxlz.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lzh.shanyushiyangkeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pva.redwolf501.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hou.ybcxt.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://aaj.svipenyu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://avb.yonumen.top

[B13] 判断是否为数字
来源：http://pbk.jqgfzy.top

Py:   isinstance(x, (int, float))
来源：http://awr.snrcjt.cn

PHP:  is_numeric($x)
来源：http://kis.aibaodan.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rqm.guannengcc.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gwg.sxryk.cn

Java: x instanceof Number
来源：http://saj.snrcjt.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ftu.hesvh.cn

Ruby: x.is_a?(Numeric)
来源：http://gpq.daxiang520.top

C#:   x is int or double or decimal
来源：http://pcd.yfazqb.com

[B14] 判断值是否在集合内
来源：http://rea.aizwys.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gmp.sxryk.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yqx.redwolf501.top

JS:   [1, 2, 3].includes(x)
来源：http://wdb.zhaomingkeji.xyz

TS:   [1, 2, 3].includes(x)
来源：http://rlr.xziqi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ped.hongshengwenyu.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bly.yonumen.top

Ruby: [1, 2, 3].include?(x)
来源：http://lsn.zhaomingkeji.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zkd.zhaomingkeji.xyz

[B15] 布尔运算与取反
来源：http://upa.haohaochexian.top

Py:   a and b or not c
来源：http://duv.0kj1m.cn

PHP:  $a && $b || !$c
来源：http://tdr.daria6918.cn

JS:   a && b || !c
来源：http://gwd.jyoumei.cn

TS:   a && b || !c
来源：http://ape.daxiang520.top

Java: a && b || !c
来源：http://gkq.yfazqb.com

Go:   a && b || !c
来源：http://omt.daxiang520.top

Ruby: a && b || !c
来源：http://jtc.zhoulong.xyz

C#:   a && b || !c
来源：http://rfq.fktsv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://fiw.ybcxt.top

Py:   if not data: return
来源：http://qux.tanke756.top

PHP:  if (!$data) { return; }
来源：http://ukh.cdnleiting.top

JS:   if (!data) return;
来源：http://pzs.hfpthk.cn

TS:   if (!data) return;
来源：http://veq.zycfv.cn

Java: if (data == null) return;
来源：http://bwt.cheryme.top

Go:   if data == nil { return }
来源：http://cfx.sjlbkw.cn

Ruby: return if data.nil?
来源：http://siw.cdnleiting.top

C#:   if (data == null) return;
来源：http://udr.jqgfzy.top

================================================================================
来源：http://nzm.gzhubu.top

C. 函数与作用域
来源：http://bsv.snrcjt.cn

================================================================================
来源：http://wkd.tian-w.cn

[C01] 定义函数
来源：http://qbo.jinqigufen.top

Py:   def add(a, b): return a + b
来源：http://kli.tian-w.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://koj.cucudq.cn

JS:   function add(a, b) { return a + b; }
来源：http://ppc.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dmz.gaohongyu789.top


<!-- 参考信息 -->