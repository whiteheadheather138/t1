代发 wailian999

[A10] 生成随机数
来源：http://kum.xuetiantiany.cn

Py:   import random; random.randint(1, 100)
来源：http://khv.fehbvm.com

PHP:  random_int(1, 100);
来源：http://unr.bbcook.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://iov.sweek.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xfw.chenlongwang.top

Java: new Random().nextInt(100) + 1
来源：http://kkc.yueranfly.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dut.cdnleiting.top

Ruby: rand(1..100)
来源：http://glb.yangfankeji.com

C#:   new Random().Next(1, 101)
来源：http://ddu.fehbvm.com

[A11] 条件表达式（三元）
来源：http://npw.zhijiandao.cn

Py:   "yes" if x > 0 else "no"
来源：http://xxy.ybcxt.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ywq.yongpay.top

JS:   x > 0 ? "yes" : "no"
来源：http://ptd.dashuyun.cn

TS:   x > 0 ? "yes" : "no"
来源：http://sft.wangshuangyany.cn

Java: x > 0 ? "yes" : "no"
来源：http://dlt.kuanghao11.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ecg.jqgufenzy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://jzo.52xcode.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xeu.0kj1m.cn

[A12] 字符串插值 / 格式化
来源：http://dvn.meibo888.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fvb.tian-w.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fyo.9152youxi.cn

JS:   `Hello, ${name}!`
来源：http://cnv.tanke756.top

TS:   `Hello, ${name}!`
来源：http://ibw.jinghuilouyu.cn

Java: "Hello, %s!".formatted(name)
来源：http://gzq.jianghu66.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jdb.chenjidiqi.icu

Ruby: "Hello, #{name}!"
来源：http://jxx.snrcjt.cn

C#:   $"Hello, {name}!"
来源：http://whz.hnqzz.top

[A13] 多行字符串（练习 \n 转义）
来源：http://qlu.yueranfly.top

Py:   "第一行\n第二行"
来源：http://rde.xinyue.icu

PHP:  "第一行\n第二行"
来源：http://zgu.jinqigufen.top

JS:   "第一行\n第二行"
来源：http://pmm.tarul.cn

TS:   "第一行\n第二行"
来源：http://blm.nwbrower.top

Java: "第一行\n第二行"
来源：http://qfd.jinyuanbaomall.cn

Go:   "第一行\n第二行"
来源：http://udi.vehdjk.com

Ruby: "第一行\n第二行"
来源：http://lsq.xinyue.icu

C#:   "第一行\n第二行"
来源：http://hzx.xinyue.icu

[A14] 注释写法
来源：http://kny.yj202588.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://hzb.zhengqikj.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://wox.guannengcc.top

JS:   // 单行；/* 多行 */
来源：http://kiu.xinyue.icu

TS:   // 单行；/* 多行 */
来源：http://qhr.xinyue.icu

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jsz.jinqigufen.top

Go:   // 单行；/* 多行 */
来源：http://kdu.iojbl.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qaq.sjlbkw.cn

C#:   // 单行；/* 多行 */
来源：http://rsr.epnwcf.com

[A15] 空值判断与默认值
来源：http://hew.gaohongyu789.top

Py:   value = data or "默认值"
来源：http://suo.c1oappe.top

PHP:  $value = $data ?? "默认值";
来源：http://gcd.ywan-chungtsiang.top

JS:   const value = data ?? "默认值";
来源：http://ygo.jqgufenzy.top

TS:   const value = data ?? "默认值";
来源：http://tpj.dashuyun.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xwi.chenlongwang.top

Go:   if data == "" { data = "默认值" }
来源：http://fzt.tian-w.cn

Ruby: value = data || "默认值"
来源：http://zwb.jinyuanbaomall.cn

C#:   var value = data ?? "默认值";
来源：http://lnl.havefunace.top

[A16] 真假值判断规则
来源：http://pbj.pengpengdd.cyou

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://osi.xingfuxueyuan.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ssz.wangshuangyany.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://jve.svipenyu.cn

TS:   if (!x) {}
来源：http://vpq.cheryme.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uos.smart0.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://acr.cucudq.cn

Ruby: unless x            # nil 与 false 为假
来源：http://tcm.hywenlv.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://czt.guowangkeji.top

[A17] 位运算
来源：http://aeu.aizwys.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bdc.aizwys.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dns.316326.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fjj.hnxiangtu.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dty.xingfuxueyuan.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vnj.zhixingplan.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ulu.snrcjt.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://daw.epnwcf.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ith.xuanzx.com

[A18] 字符与 ASCII 码互转
来源：http://iai.fzhhl.top

Py:   ord("A"); chr(65)
来源：http://lwi.tarul.cn

PHP:  ord("A"); chr(65)
来源：http://pzb.gogol.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fvx.cqqwz.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yrv.yongpay.top

Java: (int) 'A'; (char) 65
来源：http://lon.uphjek.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ofu.yangfankeji.com

Ruby: "A".ord; 65.chr
来源：http://qxz.ivvv.top

C#:   (int)'A'; (char)65
来源：http://yuq.jinqigufen.top

[A19] 交换两个变量
来源：http://fai.chenlongwang.top

Py:   a, b = b, a
来源：http://pwd.yfazqb.com

PHP:  [$a, $b] = [$b, $a];
来源：http://wsa.ydjk.org.cn

JS:   [a, b] = [b, a];
来源：http://wbn.jqgufenzy.top

TS:   [a, b] = [b, a];
来源：http://exe.sjlbkw.cn

Java: int t = a; a = b; b = t;
来源：http://buj.yonumen.top

Go:   a, b = b, a
来源：http://djy.hywenlv.cn

Ruby: a, b = b, a
来源：http://dcc.tarul.cn

C#:   (a, b) = (b, a);
来源：http://pwf.wangdashe.top

[A20] 读取标准输入
来源：http://slp.yvedp.cn

Py:   name = input("请输入：")
来源：http://nvf.pycfn.com

PHP:  $name = trim(fgets(STDIN));
来源：http://pxi.wangdashe.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ixt.xziqi.cn

TS:   // Node.js：readline 模块
来源：http://puz.zhiwuduotai.top

Java: new Scanner(System.in).nextLine()
来源：http://oik.zhijiandao.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://npq.nwbrower.top

Ruby: gets.chomp
来源：http://mcd.zhixingplan.top

C#:   Console.ReadLine();
来源：http://ckq.jqgfzy.top

[A21] 保留指定小数位输出
来源：http://dti.havefunace.top

Py:   f"{3.14159:.2f}"
来源：http://qyj.sufxvd.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dhr.chenzaomai.com

JS:   (3.14159).toFixed(2)
来源：http://tna.ybcxt.top

TS:   (3.14159).toFixed(2)
来源：http://imn.tianlin.xyz

Java: String.format("%.2f", 3.14159)
来源：http://sax.sysykeji.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vot.shangyingyoupin.top

Ruby: format("%.2f", 3.14159)
来源：http://ggh.zhongyouzk.top

C#:   3.14159.ToString("F2")
来源：http://uru.yangfankeji.com

[A22] 获取字符串长度
来源：http://zjm.ywan-chungtsiang.top

Py:   len(s)
来源：http://qhg.nwbrower.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vmg.fengsongda.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sbe.hongshengwenyu.top

TS:   s.length
来源：http://yjd.hnxiangtu.top

Java: s.length()
来源：http://xqr.ivvv.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qeb.tarul.cn

Ruby: s.length
来源：http://tjs.yanxiufei.cn

C#:   s.Length
来源：http://rlx.hammf.cn

[A23] 大小写转换
来源：http://mcy.gzhubu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://wav.yj20258888.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://asj.gotoacloud.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dgg.daria6918.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nvj.ywan-chungtsiang.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fkt.zhengqikj.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://clp.shangyingyoupin.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pab.wangdashe.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ben.ehwqpu.com

[A24] 去除首尾空白
来源：http://dkz.yj202588.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fiv.havefunace.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pwe.zhijiandao.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gza.gzhubu.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zfr.hammf.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bwj.hongshengwenyu.top

Go:   strings.TrimSpace(s)
来源：http://eto.nanxuanxn.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tdx.zhongyouzk.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jle.xinyue.icu

[A25] 字符串比较
来源：http://ehe.nwbrower.top

Py:   s1 == s2; s1 != s2
来源：http://vsw.birdmap.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tef.jinqigfzy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yyr.andypj.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xvv.xylfe.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bzu.ehwqpu.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yuj.wangshuangyany.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://zxx.vqdsnc.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ofk.shuidangran.top

[A26] 类型转换总览
来源：http://hjs.shangyingyoupin.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dgr.yj202588.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xbb.sysykeji.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://obc.zhijiandao.cn

TS:   Number() String() Boolean() x as number
来源：http://zya.zdqjudy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ghr.ivvv.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hvv.havefunace.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://aia.fanxiaobao.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://frh.andypj.xyz

================================================================================
来源：http://tbi.uphjek.com

B. 流程控制
来源：http://tih.bbcook.cn

================================================================================
来源：http://pnt.uphjek.com

[B01] 条件判断 if / else
来源：http://cvn.hywenlv.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mnq.sufxvd.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wpi.shanyushiyangkeji.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://uxu.ctjpmb.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://roj.9152youxi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://aif.hfpthk.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jzr.nanxuanxn.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qky.xylfe.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tkc.cheryme.top

[B02] 多分支 else if / elif
来源：http://xzh.xylfe.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qgp.zycfv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://aef.zhongyouzk.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eit.vehdjk.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zvg.chenzaomai.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xmh.dianchejie.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://szl.jinghuilouyu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://iun.shanyushiyangtech.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hco.nanxinkj.top

[B03] switch / match / case
来源：http://zgw.ybcxt.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ouk.xuanzx.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rre.gotoacloud.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ynr.sxryk.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uwq.yonumen.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fgp.yj202588.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hkc.9152youxi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://asn.gaohongyu789.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hfz.bjfxy.top

[B04] for 计数循环
来源：http://pce.kuanghao11.cn

Py:   for i in range(10): print(i)
来源：http://qdl.fehbvm.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://kdk.tianlin.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://syh.ydjk.org.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mdq.yangfankeji.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kbz.guannengcc.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://quv.sufxvd.cn

Ruby: 10.times { |i| puts i }
来源：http://gye.zhongyouzk.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cop.hywenlv.cn

[B05] 遍历数组 / 列表
来源：http://ezf.jlsjyb.cn

Py:   for item in arr: print(item)
来源：http://pqn.pengpengdd.cyou

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://aob.cashguo.top

JS:   for (const item of arr) { console.log(item); }
来源：http://zku.fehbvm.com

TS:   for (const item of arr) { console.log(item); }
来源：http://ine.bbcook.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://bhr.nanxinkj.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jek.shzxlz.cn

Ruby: arr.each { |item| puts item }
来源：http://btp.zhijiandao.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://apy.shangyingyoupin.top

[B06] 遍历字典 / 对象
来源：http://lou.aizwys.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ffu.hysaishi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mve.jinqigfzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fpv.jqgfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hhx.sjlbkw.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://onz.gzhubu.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ixf.shangyingyoupin.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://eqq.gaohongyu789.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rlj.zhengqikj.top

[B07] while 循环
来源：http://wdu.hesvh.cn

Py:   while i < 10: i += 1
来源：http://zbr.hongshengwenyu.top

PHP:  while ($i < 10) { $i++; }
来源：http://jtj.jinqigfzy.top

JS:   while (i < 10) { i++; }
来源：http://xiz.jianghu66.top

TS:   while (i < 10) { i++; }
来源：http://rec.jinqigufen.top

Java: while (i < 10) { i++; }
来源：http://drg.gogol.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pls.ybcxt.top

Ruby: while i < 10; i += 1; end
来源：http://mpf.fehbvm.com

C#:   while (i < 10) { i++; }
来源：http://chm.vqdsnc.cn

[B08] do-while（至少执行一次）
来源：http://jfj.chenzaomai.com

Py:   # 无 do-while：用 while True + break
来源：http://hry.sufxvd.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://lil.yj20258888.top

JS:   do { i++; } while (i < 10);
来源：http://aov.zdqjudy.top

TS:   do { i++; } while (i < 10);
来源：http://hyc.ppjwa.cn

Java: do { i++; } while (i < 10);
来源：http://tpz.havefunace.top

Go:   for { i++; if i >= 10 { break } }
来源：http://eun.sxryk.cn

Ruby: begin; i += 1; end while i < 10
来源：http://oop.hysaishi.cn

C#:   do { i++; } while (i < 10);
来源：http://bhb.zhijiandao.cn

[B09] break 与 continue
来源：http://xev.hysaishi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ujj.yonumen.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://htm.shangyingyoupin.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qfc.hnxiangtu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://amy.chenjidiqi.icu

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vvw.ybcxt.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nfz.jlsjyb.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://aqn.cheryme.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qpy.hesvh.cn

[B10] 遍历同时拿索引
来源：http://gyp.vehdjk.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://axn.pycfn.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yas.sufxvd.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://muq.aibaodan.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lll.zhaomingkeji.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ulo.gogol.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yyt.sysykeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xmw.svipenyu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kae.ivvv.top

[B11] 生成数字序列 / 区间
来源：http://xbx.chenlongwang.top

Py:   list(range(0, 10, 2))
来源：http://hyp.redwolf501.top

PHP:  range(0, 10, 2);
来源：http://ouv.fktsv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nge.yongpay.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://npy.dianchejie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://myd.bjfxy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lya.jinghuilouyu.cn

Ruby: (0...10).step(2).to_a
来源：http://esi.iojbl.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vey.daxiang520.top

[B12] 跳出多层循环
来源：http://rxj.nanxinkj.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xky.yfazqb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://asb.shuidangran.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://buo.hfpthk.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://iyv.snrcjt.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://igg.snrcjt.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blg.zhoulong.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hyh.hfpthk.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hnz.xuetiantiany.cn

[B13] 判断是否为数字
来源：http://xpk.chenzaomai.com

Py:   isinstance(x, (int, float))
来源：http://vhk.jyoumei.cn

PHP:  is_numeric($x)
来源：http://yfq.vqdsnc.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ydp.aizwys.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aps.fengsongda.top

Java: x instanceof Number
来源：http://ajl.jiagoushi.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lcr.zhiwuduotai.top

Ruby: x.is_a?(Numeric)
来源：http://bxk.uphjek.com

C#:   x is int or double or decimal
来源：http://ryj.jinqigufen.top

[B14] 判断值是否在集合内
来源：http://ydl.yj20258888.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jkf.bjfxy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xgm.ywan-chungtsiang.top

JS:   [1, 2, 3].includes(x)
来源：http://lok.yangfankeji.com

TS:   [1, 2, 3].includes(x)
来源：http://wfq.kuanghao11.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ngs.wangdashe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wxk.zhiwuduotai.top

Ruby: [1, 2, 3].include?(x)
来源：http://vfx.ydzc1.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wil.jqgufenzy.top

[B15] 布尔运算与取反
来源：http://qsd.zhiwuduotai.top

Py:   a and b or not c
来源：http://aat.ivvv.top

PHP:  $a && $b || !$c
来源：http://yvk.wangdashe.top

JS:   a && b || !c
来源：http://euq.shangyingyoupin.top

TS:   a && b || !c
来源：http://qku.yonumen.top

Java: a && b || !c
来源：http://bps.quarkkingdee.top

Go:   a && b || !c
来源：http://kwe.tian-w.cn

Ruby: a && b || !c
来源：http://iam.yongpay.top

C#:   a && b || !c
来源：http://jzu.ydjk.org.cn

[B16] 卫语句：不满足条件提前返回
来源：http://myr.hesvh.cn

Py:   if not data: return
来源：http://iln.chenzaomai.com

PHP:  if (!$data) { return; }
来源：http://ial.gogol.net.cn

JS:   if (!data) return;
来源：http://ebn.c1oappe.top

TS:   if (!data) return;
来源：http://odz.birdmap.top

Java: if (data == null) return;
来源：http://crp.gogol.net.cn

Go:   if data == nil { return }
来源：http://hwk.iojbl.cn

Ruby: return if data.nil?
来源：http://obb.chenjidiqi.icu

C#:   if (data == null) return;
来源：http://pyg.jinghuilouyu.cn


<!-- 参考信息 -->