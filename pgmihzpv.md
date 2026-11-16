代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dhh.iojbl.cn

Java: new Random().nextInt(100) + 1
来源：http://ore.fzhhl.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://usb.zhixingplan.top

Ruby: rand(1..100)
来源：http://luy.jiagoushi.top

C#:   new Random().Next(1, 101)
来源：http://kci.tanke756.top

[A11] 条件表达式（三元）
来源：http://ief.c1oappe.top

Py:   "yes" if x > 0 else "no"
来源：http://igt.fzhhl.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://wyk.chenzaomai.com

JS:   x > 0 ? "yes" : "no"
来源：http://fai.hesvh.cn

TS:   x > 0 ? "yes" : "no"
来源：http://oak.ydzc1.top

Java: x > 0 ? "yes" : "no"
来源：http://rnn.jinyuanbaomall.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ahl.chenzaomai.com

Ruby: x > 0 ? "yes" : "no"
来源：http://bva.yj20258.top

C#:   x > 0 ? "yes" : "no"
来源：http://zjj.cheryme.top

[A12] 字符串插值 / 格式化
来源：http://gnv.fzhhl.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://zka.xylfe.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mfa.andypj.xyz

JS:   `Hello, ${name}!`
来源：http://hsg.9152youxi.cn

TS:   `Hello, ${name}!`
来源：http://igj.sysykeji.top

Java: "Hello, %s!".formatted(name)
来源：http://cmg.hesvh.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pjb.shuidangran.top

Ruby: "Hello, #{name}!"
来源：http://szv.xziqi.cn

C#:   $"Hello, {name}!"
来源：http://slp.316326.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://coj.sysykeji.top

Py:   "第一行\n第二行"
来源：http://ofm.sxryk.cn

PHP:  "第一行\n第二行"
来源：http://cey.shzxlz.cn

JS:   "第一行\n第二行"
来源：http://bpg.vqdsnc.cn

TS:   "第一行\n第二行"
来源：http://ypw.feifeiyinyue.top

Java: "第一行\n第二行"
来源：http://mps.yuanzhike.top

Go:   "第一行\n第二行"
来源：http://ikm.ppjwa.cn

Ruby: "第一行\n第二行"
来源：http://cjh.kuanghao11.cn

C#:   "第一行\n第二行"
来源：http://xjy.quarkkingdee.top

[A14] 注释写法
来源：http://yjj.cashguo.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ile.zycfv.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wdy.hnqzz.top

JS:   // 单行；/* 多行 */
来源：http://ikw.ydzc1.top

TS:   // 单行；/* 多行 */
来源：http://zxs.hcnkem.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://eop.ctjpmb.com

Go:   // 单行；/* 多行 */
来源：http://gcu.ybcxt.top

Ruby: # 单行；=begin 多行 =end
来源：http://wfe.shangyingyoupin.top

C#:   // 单行；/* 多行 */
来源：http://yps.andypj.xyz

[A15] 空值判断与默认值
来源：http://ert.havefunace.top

Py:   value = data or "默认值"
来源：http://vyw.havefunace.top

PHP:  $value = $data ?? "默认值";
来源：http://rex.zdqjudy.top

JS:   const value = data ?? "默认值";
来源：http://own.dashuyun.cn

TS:   const value = data ?? "默认值";
来源：http://qej.yonumen.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dvq.hnqzz.top

Go:   if data == "" { data = "默认值" }
来源：http://mvf.xuanzx.com

Ruby: value = data || "默认值"
来源：http://okc.xuetiantiany.cn

C#:   var value = data ?? "默认值";
来源：http://jkz.hfpthk.cn

[A16] 真假值判断规则
来源：http://fnb.yj20258.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cwt.wangdashe.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wyl.bjfxy.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dkh.jinqigufen.top

TS:   if (!x) {}
来源：http://wnp.yangfankeji.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://avx.shangyingyoupin.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dvw.aibaodan.cn

Ruby: unless x            # nil 与 false 为假
来源：http://wym.chenlongwang.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xjc.feifeiyinyue.top

[A17] 位运算
来源：http://smf.hnqzz.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lqt.jinghuilouyu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nof.jyoumei.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wqy.hesvh.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pyb.bbcook.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fvn.nanxuanxn.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ira.haohaochexian.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://igb.yonumen.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oql.sjlbkw.cn

[A18] 字符与 ASCII 码互转
来源：http://tqg.ivvv.top

Py:   ord("A"); chr(65)
来源：http://uji.yanxiufei.cn

PHP:  ord("A"); chr(65)
来源：http://civ.yueranfly.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wbz.hywenlv.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cle.birdmap.top

Java: (int) 'A'; (char) 65
来源：http://kgo.zhiwuduotai.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qnt.52xcode.cn

Ruby: "A".ord; 65.chr
来源：http://lob.shangyingyoupin.top

C#:   (int)'A'; (char)65
来源：http://otp.tianlin.xyz

[A19] 交换两个变量
来源：http://vpz.zdbjq.cn

Py:   a, b = b, a
来源：http://acn.cucudq.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jax.hfpthk.cn

JS:   [a, b] = [b, a];
来源：http://kpp.ywan-chungtsiang.top

TS:   [a, b] = [b, a];
来源：http://azb.hnxiangtu.top

Java: int t = a; a = b; b = t;
来源：http://bea.vehdjk.com

Go:   a, b = b, a
来源：http://opa.jinqigfzy.top

Ruby: a, b = b, a
来源：http://jca.ctjpmb.com

C#:   (a, b) = (b, a);
来源：http://hql.birdmap.top

[A20] 读取标准输入
来源：http://dvx.fanxiaobao.xyz

Py:   name = input("请输入：")
来源：http://fls.shanyushiyangtech.top

PHP:  $name = trim(fgets(STDIN));
来源：http://tlx.hongshengwenyu.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tgd.vehdjk.com

TS:   // Node.js：readline 模块
来源：http://eld.ydjk.org.cn

Java: new Scanner(System.in).nextLine()
来源：http://kps.jyoumei.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tdr.feifeiyinyue.top

Ruby: gets.chomp
来源：http://omk.yangfankeji.com

C#:   Console.ReadLine();
来源：http://epn.chenzaomai.com

[A21] 保留指定小数位输出
来源：http://xuf.cheryme.top

Py:   f"{3.14159:.2f}"
来源：http://bbu.aizwys.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rbs.zhixingplan.top

JS:   (3.14159).toFixed(2)
来源：http://pxh.jinqigufen.top

TS:   (3.14159).toFixed(2)
来源：http://ylq.c1oappe.top

Java: String.format("%.2f", 3.14159)
来源：http://kot.hfpthk.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yts.sufxvd.cn

Ruby: format("%.2f", 3.14159)
来源：http://mcf.jinghuilouyu.cn

C#:   3.14159.ToString("F2")
来源：http://okc.ybcxt.top

[A22] 获取字符串长度
来源：http://ecp.zhongyouzk.top

Py:   len(s)
来源：http://wkr.xuetiantiany.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://otv.gogol.net.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://drn.jinqigfzy.top

TS:   s.length
来源：http://gxh.meibo888.top

Java: s.length()
来源：http://zsg.mhx1999.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ssd.chenzaomai.com

Ruby: s.length
来源：http://gvn.zdqjudy.top

C#:   s.Length
来源：http://xzx.hammf.cn

[A23] 大小写转换
来源：http://emu.shangyingyoupin.top

Py:   s.upper(); s.lower(); s.title()
来源：http://etm.uphjek.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fvu.yueranfly.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vkk.tian-w.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ese.hfpthk.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mzs.ehwqpu.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://oxp.meibo888.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wjt.hnqzz.top

C#:   s.ToUpper(); s.ToLower()
来源：http://mes.0kj1m.cn

[A24] 去除首尾空白
来源：http://vqp.ppjwa.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nbk.iojbl.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://oqp.zhijiandao.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qps.meibo888.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mmo.jinghuilouyu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://uor.haohaochexian.top

Go:   strings.TrimSpace(s)
来源：http://uki.vqdsnc.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yho.vehdjk.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ucd.shanyushiyangtech.top

[A25] 字符串比较
来源：http://mlc.xylfe.cn

Py:   s1 == s2; s1 != s2
来源：http://gaq.hesvh.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://oll.tarul.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://usg.chenlongwang.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dgz.316326.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uty.jinqigufen.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bvd.yuanzhike.top

Ruby: s1 == s2; s1 <=> s2
来源：http://gip.pengpengdd.cyou

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qlm.fzhhl.top

[A26] 类型转换总览
来源：http://pbu.redwolf501.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://duk.tanke756.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://odu.xuanzx.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://aza.hammf.cn

TS:   Number() String() Boolean() x as number
来源：http://xrm.dianchejie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tkp.hywenlv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fyv.ydjk.org.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://oxa.jlsjyb.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vxu.vehdjk.com

================================================================================
来源：http://vsr.shanyushiyangkeji.top

B. 流程控制
来源：http://ned.jinqigufen.top

================================================================================
来源：http://mon.zhoulong.xyz

[B01] 条件判断 if / else
来源：http://uej.316326.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://djv.sjlbkw.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kui.wangshuangyany.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xkt.fehbvm.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kmx.sweek.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://doa.guowangkeji.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nye.xziqi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lsk.kuanghao11.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ihp.52xcode.cn

[B02] 多分支 else if / elif
来源：http://wax.haohaochexian.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://deu.xinyue.icu

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ohw.hnqzz.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qhk.fktsv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tst.yfazqb.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ivb.hammf.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bsw.jlsjyb.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zjt.316326.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ihr.shzxlz.cn

[B03] switch / match / case
来源：http://cwn.yj20258.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ufl.ctjpmb.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://abt.quarkkingdee.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cwv.jqgufenzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xxc.meibo888.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qmn.nwbrower.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wzg.tanke756.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://osb.chenlongwang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://eod.hcnkem.com

[B04] for 计数循环
来源：http://ddj.cucudq.cn

Py:   for i in range(10): print(i)
来源：http://bpu.snrcjt.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fjp.jlsjyb.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sjd.sysykeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xee.havefunace.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xor.ydjk.org.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vue.bjfxy.top

Ruby: 10.times { |i| puts i }
来源：http://wlk.yfazqb.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uyo.gaohongyu789.top

[B05] 遍历数组 / 列表
来源：http://bkm.smart0.xyz

Py:   for item in arr: print(item)
来源：http://zmt.chenzaomai.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://iit.shuidangran.top

JS:   for (const item of arr) { console.log(item); }
来源：http://qqv.nanxuanxn.top

TS:   for (const item of arr) { console.log(item); }
来源：http://njh.jinqigufen.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ims.shangyingyoupin.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gag.52xcode.cn

Ruby: arr.each { |item| puts item }
来源：http://yqr.sysykeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nbr.xylfe.cn

[B06] 遍历字典 / 对象
来源：http://dwi.chenjidiqi.icu

Py:   for k, v in d.items(): print(k, v)
来源：http://jxz.zhijiandao.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cde.zhixingplan.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://oer.feifeiyinyue.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bvr.yongpay.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pgg.ybcxt.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gut.xinyue.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ykw.c1oappe.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tiy.guowangkeji.top

[B07] while 循环
来源：http://onl.nanxinkj.top

Py:   while i < 10: i += 1
来源：http://wcf.jinqigufen.top

PHP:  while ($i < 10) { $i++; }
来源：http://kuc.gogol.net.cn

JS:   while (i < 10) { i++; }
来源：http://tdl.andypj.xyz

TS:   while (i < 10) { i++; }
来源：http://fcg.cucudq.cn

Java: while (i < 10) { i++; }
来源：http://wea.jinyuanbaomall.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uez.xylfe.cn

Ruby: while i < 10; i += 1; end
来源：http://iod.nanxuanxn.top

C#:   while (i < 10) { i++; }
来源：http://fnf.yvedp.cn

[B08] do-while（至少执行一次）
来源：http://dny.birdmap.top

Py:   # 无 do-while：用 while True + break
来源：http://cgz.aibaodan.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://yxq.zhoulong.xyz

JS:   do { i++; } while (i < 10);
来源：http://xwv.birdmap.top

TS:   do { i++; } while (i < 10);
来源：http://xck.jinghuilouyu.cn

Java: do { i++; } while (i < 10);
来源：http://mla.ctjpmb.com

Go:   for { i++; if i >= 10 { break } }
来源：http://pfg.jiagoushi.top

Ruby: begin; i += 1; end while i < 10
来源：http://juc.tian-w.cn

C#:   do { i++; } while (i < 10);
来源：http://mbu.dashuyun.cn

[B09] break 与 continue
来源：http://llb.hammf.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ioq.bjfxy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eap.yfazqb.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wgq.hywenlv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zxh.jinqigfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eku.gotoacloud.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gcx.iojbl.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://awe.ydzc1.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wzb.hesvh.cn

[B10] 遍历同时拿索引
来源：http://qyl.feifeiyinyue.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ltq.yongpay.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jbg.wangshuangyany.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ydf.smart0.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ndm.gotoacloud.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pof.yj20258888.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://opa.xziqi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yzu.yangfankeji.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ucq.redwolf501.top

[B11] 生成数字序列 / 区间
来源：http://tet.aibaodan.cn

Py:   list(range(0, 10, 2))
来源：http://vgz.shangyingyoupin.top

PHP:  range(0, 10, 2);
来源：http://wzx.dianchejie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://anz.yueranfly.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eeh.cqqwz.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gef.yueranfly.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kgm.hywenlv.cn

Ruby: (0...10).step(2).to_a
来源：http://inw.jinqigufen.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ofr.jyoumei.cn

[B12] 跳出多层循环
来源：http://maa.ybcxt.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://gxl.smart0.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://wxe.epnwcf.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cca.xziqi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jat.nwbrower.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kjq.yvedp.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ncv.daxiang520.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tgq.xuanzx.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://yaq.yangfankeji.com

[B13] 判断是否为数字
来源：http://inf.xziqi.cn

Py:   isinstance(x, (int, float))
来源：http://eye.ybcxt.top

PHP:  is_numeric($x)
来源：http://dqa.hywenlv.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fiv.fzhhl.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xcd.zhongyouzk.top

Java: x instanceof Number
来源：http://ork.fengsongda.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rxe.gotoacloud.top

Ruby: x.is_a?(Numeric)
来源：http://aco.hywenlv.cn

C#:   x is int or double or decimal
来源：http://idu.chenjidiqi.icu

[B14] 判断值是否在集合内
来源：http://qqf.ybcxt.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wdb.zhengqikj.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://aaj.meibo888.top

JS:   [1, 2, 3].includes(x)
来源：http://pem.52xcode.cn

TS:   [1, 2, 3].includes(x)
来源：http://kxf.wangdashe.top

Java: List.of(1, 2, 3).contains(x)
来源：http://wdc.zdbjq.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ofc.yonumen.top

Ruby: [1, 2, 3].include?(x)
来源：http://ztm.quarkkingdee.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nos.jinghuilouyu.cn

[B15] 布尔运算与取反
来源：http://tgy.jyoumei.cn

Py:   a and b or not c
来源：http://exw.tianlin.xyz

PHP:  $a && $b || !$c
来源：http://axl.shanyushiyangtech.top

JS:   a && b || !c
来源：http://srh.iojbl.cn

TS:   a && b || !c
来源：http://olj.andypj.xyz

Java: a && b || !c
来源：http://oof.0kj1m.cn

Go:   a && b || !c
来源：http://ijo.jlsjyb.cn

Ruby: a && b || !c
来源：http://xgl.jinghuilouyu.cn

C#:   a && b || !c
来源：http://tob.aizwys.cn

[B16] 卫语句：不满足条件提前返回
来源：http://iyz.andypj.xyz

Py:   if not data: return
来源：http://azf.gaohongyu789.top

PHP:  if (!$data) { return; }
来源：http://elx.cashguo.top

JS:   if (!data) return;
来源：http://vpi.ctjpmb.com

TS:   if (!data) return;
来源：http://wxy.yueranfly.top

Java: if (data == null) return;
来源：http://lzg.zhixingplan.top

Go:   if data == nil { return }
来源：http://not.shuidangran.top

Ruby: return if data.nil?
来源：http://yid.wangshuangyany.cn

C#:   if (data == null) return;
来源：http://aul.guowangkeji.top

================================================================================
来源：http://uov.zhongyouzk.top

C. 函数与作用域
来源：http://elh.yvedp.cn

================================================================================
来源：http://xwv.jqgufenzy.top

[C01] 定义函数
来源：http://cqu.zhaomingkeji.xyz


<!-- 参考信息 -->