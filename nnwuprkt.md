代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://maz.dashuyun.cn

Java: new Random().nextInt(100) + 1
来源：http://udk.aibaodan.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rtk.shangyingyoupin.top

Ruby: rand(1..100)
来源：http://wpq.9152youxi.cn

C#:   new Random().Next(1, 101)
来源：http://dqj.ctjpmb.com

[A11] 条件表达式（三元）
来源：http://vxa.zhengqikj.top

Py:   "yes" if x > 0 else "no"
来源：http://ron.wangdashe.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://ava.birdmap.top

JS:   x > 0 ? "yes" : "no"
来源：http://txy.cashguo.top

TS:   x > 0 ? "yes" : "no"
来源：http://vkn.epnwcf.com

Java: x > 0 ? "yes" : "no"
来源：http://kmj.jinqigufen.top

Go:   // 无三元运算符，需用 if 语句
来源：http://ckg.fzhhl.top

Ruby: x > 0 ? "yes" : "no"
来源：http://qar.yueranfly.top

C#:   x > 0 ? "yes" : "no"
来源：http://jut.gzhubu.top

[A12] 字符串插值 / 格式化
来源：http://ult.vqdsnc.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qic.shzxlz.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rpm.xziqi.cn

JS:   `Hello, ${name}!`
来源：http://jwz.fehbvm.com

TS:   `Hello, ${name}!`
来源：http://xny.xinyue.icu

Java: "Hello, %s!".formatted(name)
来源：http://sal.jinghuilouyu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bev.jlsjyb.cn

Ruby: "Hello, #{name}!"
来源：http://lmq.xuetiantiany.cn

C#:   $"Hello, {name}!"
来源：http://arc.andypj.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://wyp.zdqjudy.top

Py:   "第一行\n第二行"
来源：http://ubf.sxryk.cn

PHP:  "第一行\n第二行"
来源：http://run.jlsjyb.cn

JS:   "第一行\n第二行"
来源：http://msb.ybcxt.top

TS:   "第一行\n第二行"
来源：http://scf.nwbrower.top

Java: "第一行\n第二行"
来源：http://oco.9152youxi.cn

Go:   "第一行\n第二行"
来源：http://tqf.yuanzhike.top

Ruby: "第一行\n第二行"
来源：http://fja.zhixingplan.top

C#:   "第一行\n第二行"
来源：http://zgx.yangfankeji.com

[A14] 注释写法
来源：http://wum.yueranfly.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://hxl.chenzaomai.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://rxa.pengpengdd.cyou

JS:   // 单行；/* 多行 */
来源：http://uih.yueranfly.top

TS:   // 单行；/* 多行 */
来源：http://lyk.zycfv.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://drr.vqdsnc.cn

Go:   // 单行；/* 多行 */
来源：http://dpk.zhijiandao.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rzv.shanyushiyangkeji.top

C#:   // 单行；/* 多行 */
来源：http://chn.feifeiyinyue.top

[A15] 空值判断与默认值
来源：http://mrt.cheryme.top

Py:   value = data or "默认值"
来源：http://llp.shanyushiyangkeji.top

PHP:  $value = $data ?? "默认值";
来源：http://squ.yonumen.top

JS:   const value = data ?? "默认值";
来源：http://wdk.pengpengdd.cyou

TS:   const value = data ?? "默认值";
来源：http://fgp.dashuyun.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wju.jqgufenzy.top

Go:   if data == "" { data = "默认值" }
来源：http://gdc.chenlongwang.top

Ruby: value = data || "默认值"
来源：http://ots.jinqigufen.top

C#:   var value = data ?? "默认值";
来源：http://ytf.uphjek.com

[A16] 真假值判断规则
来源：http://wfw.vqdsnc.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kbg.wangshuangyany.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://csf.ehwqpu.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wgq.tianlin.xyz

TS:   if (!x) {}
来源：http://wvh.svipenyu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lsa.hnxiangtu.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ato.hongshengwenyu.top

Ruby: unless x            # nil 与 false 为假
来源：http://qmg.cashguo.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ttt.hesvh.cn

[A17] 位运算
来源：http://wza.52xcode.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xrm.zdqjudy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zpy.snrcjt.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oif.hysaishi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kfa.cashguo.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wkl.havefunace.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fhu.svipenyu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tyq.shanyushiyangtech.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gvz.yuanzhike.top

[A18] 字符与 ASCII 码互转
来源：http://mxr.yangfankeji.com

Py:   ord("A"); chr(65)
来源：http://jel.316326.xyz

PHP:  ord("A"); chr(65)
来源：http://hza.xuetiantiany.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dpt.yanxiufei.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://few.epnwcf.com

Java: (int) 'A'; (char) 65
来源：http://zsm.ydjk.org.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jzb.cdnleiting.top

Ruby: "A".ord; 65.chr
来源：http://nsc.jinyuanbaomall.cn

C#:   (int)'A'; (char)65
来源：http://iag.guannengcc.top

[A19] 交换两个变量
来源：http://bna.tian-w.cn

Py:   a, b = b, a
来源：http://uig.jinqigfzy.top

PHP:  [$a, $b] = [$b, $a];
来源：http://vqy.chenjidiqi.icu

JS:   [a, b] = [b, a];
来源：http://rfj.yj202588.top

TS:   [a, b] = [b, a];
来源：http://gkw.pycfn.com

Java: int t = a; a = b; b = t;
来源：http://kxb.yj20258.top

Go:   a, b = b, a
来源：http://qca.gaohongyu789.top

Ruby: a, b = b, a
来源：http://yxp.ywan-chungtsiang.top

C#:   (a, b) = (b, a);
来源：http://jdw.xziqi.cn

[A20] 读取标准输入
来源：http://dxj.ybcxt.top

Py:   name = input("请输入：")
来源：http://llm.xuetiantiany.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://tev.yj202588.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://scc.9152youxi.cn

TS:   // Node.js：readline 模块
来源：http://iqr.shzxlz.cn

Java: new Scanner(System.in).nextLine()
来源：http://gso.hywenlv.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gxv.feifeiyinyue.top

Ruby: gets.chomp
来源：http://hxi.haohaochexian.top

C#:   Console.ReadLine();
来源：http://ser.shangyingyoupin.top

[A21] 保留指定小数位输出
来源：http://rhs.zhoulong.xyz

Py:   f"{3.14159:.2f}"
来源：http://fmj.pengpengdd.cyou

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hrp.pycfn.com

JS:   (3.14159).toFixed(2)
来源：http://xly.sufxvd.cn

TS:   (3.14159).toFixed(2)
来源：http://ysy.zdqjudy.top

Java: String.format("%.2f", 3.14159)
来源：http://sxt.ppjwa.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fim.aizwys.cn

Ruby: format("%.2f", 3.14159)
来源：http://ezm.nanxinkj.top

C#:   3.14159.ToString("F2")
来源：http://mro.jyoumei.cn

[A22] 获取字符串长度
来源：http://wrg.tarul.cn

Py:   len(s)
来源：http://jsd.yj202588.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gcp.fehbvm.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wzg.yongpay.top

TS:   s.length
来源：http://yfl.ehwqpu.com

Java: s.length()
来源：http://ojg.yangfankeji.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pud.wangdashe.top

Ruby: s.length
来源：http://qjj.chenlongwang.top

C#:   s.Length
来源：http://mup.c1oappe.top

[A23] 大小写转换
来源：http://wmh.yj202588.top

Py:   s.upper(); s.lower(); s.title()
来源：http://lkm.sufxvd.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://spo.xziqi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tth.uphjek.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xme.yangfankeji.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bzd.zhongyouzk.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ycs.jinqigufen.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vuh.zhijiandao.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://irw.gotoacloud.top

[A24] 去除首尾空白
来源：http://gjd.aizwys.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ffb.sysykeji.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://aya.sweek.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qeh.zdqjudy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jqf.svipenyu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xim.sysykeji.top

Go:   strings.TrimSpace(s)
来源：http://ecg.bjfxy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ttf.chenlongwang.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tbs.pengpengdd.cyou

[A25] 字符串比较
来源：http://smj.gotoacloud.top

Py:   s1 == s2; s1 != s2
来源：http://yuz.yongpay.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ilk.pycfn.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qqr.hnxiangtu.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gmz.hammf.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://imt.tianlin.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hog.tarul.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pxx.tarul.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ido.kuanghao11.cn

[A26] 类型转换总览
来源：http://orz.gaohongyu789.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rce.shuidangran.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://twm.yj202588.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vzt.hongshengwenyu.top

TS:   Number() String() Boolean() x as number
来源：http://foi.9152youxi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qcd.ivvv.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ntc.quarkkingdee.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://hqc.wangdashe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://oij.ivvv.top

================================================================================
来源：http://vaa.andypj.xyz

B. 流程控制
来源：http://cte.pengpengdd.cyou

================================================================================
来源：http://kxw.ppjwa.cn

[B01] 条件判断 if / else
来源：http://fzy.zhengqikj.top

Py:   result = "正" if x > 0 else "非正"
来源：http://hng.jyoumei.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dye.dianchejie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://iks.hysaishi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ucd.aizwys.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fue.vqdsnc.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://uug.jqgufenzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://amy.yfazqb.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://aqi.yueranfly.top

[B02] 多分支 else if / elif
来源：http://cab.dashuyun.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jae.andypj.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ifc.jinqigufen.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yrn.vqdsnc.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nvt.daxiang520.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bjw.tianlin.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xda.yj20258888.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bov.wangshuangyany.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vhu.pengpengdd.cyou

[B03] switch / match / case
来源：http://bmt.c1oappe.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xyt.zycfv.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://upi.wangshuangyany.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jwt.nanxinkj.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wxu.zhaomingkeji.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ptr.ivvv.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://auj.zhaomingkeji.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://pwh.ywan-chungtsiang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ubk.iojbl.cn

[B04] for 计数循环
来源：http://vcy.tian-w.cn

Py:   for i in range(10): print(i)
来源：http://eqo.ybcxt.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://oqh.guowangkeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rga.uphjek.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ods.guannengcc.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dvr.ctjpmb.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kyh.snrcjt.cn

Ruby: 10.times { |i| puts i }
来源：http://qvi.yueranfly.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://edn.vqdsnc.cn

[B05] 遍历数组 / 列表
来源：http://eku.52xcode.cn

Py:   for item in arr: print(item)
来源：http://knm.cucudq.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ngl.yongpay.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ukz.jinqigufen.top

TS:   for (const item of arr) { console.log(item); }
来源：http://lvu.vqdsnc.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ajq.epnwcf.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kcg.zhengqikj.top

Ruby: arr.each { |item| puts item }
来源：http://wch.yfazqb.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vrx.redwolf501.top

[B06] 遍历字典 / 对象
来源：http://nrm.guannengcc.top

Py:   for k, v in d.items(): print(k, v)
来源：http://cpa.shuidangran.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://soq.52xcode.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ptg.yvedp.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bae.daxiang520.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cme.sjlbkw.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vxx.jiagoushi.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rzf.cdnleiting.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iad.yuxming.cn

[B07] while 循环
来源：http://fve.ywan-chungtsiang.top

Py:   while i < 10: i += 1
来源：http://iae.ywan-chungtsiang.top

PHP:  while ($i < 10) { $i++; }
来源：http://vlg.ctjpmb.com

JS:   while (i < 10) { i++; }
来源：http://grq.hywenlv.cn

TS:   while (i < 10) { i++; }
来源：http://bti.dianchejie.cn

Java: while (i < 10) { i++; }
来源：http://iyi.ctjpmb.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qsk.jiagoushi.top

Ruby: while i < 10; i += 1; end
来源：http://fkr.andypj.xyz

C#:   while (i < 10) { i++; }
来源：http://xlr.zhixingplan.top

[B08] do-while（至少执行一次）
来源：http://ioh.tanke756.top

Py:   # 无 do-while：用 while True + break
来源：http://enk.andypj.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://nzn.ehwqpu.com

JS:   do { i++; } while (i < 10);
来源：http://enp.yj20258888.top

TS:   do { i++; } while (i < 10);
来源：http://cwn.9152youxi.cn

Java: do { i++; } while (i < 10);
来源：http://cre.snrcjt.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://idk.bjfxy.top

Ruby: begin; i += 1; end while i < 10
来源：http://xnl.cucudq.cn

C#:   do { i++; } while (i < 10);
来源：http://ahd.jinghuilouyu.cn

[B09] break 与 continue
来源：http://uwz.gogol.net.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zyb.quarkkingdee.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eof.ybcxt.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://thl.jlsjyb.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bjx.yuxming.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zem.zhoulong.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nbc.ydjk.org.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lfn.shuidangran.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yfu.hammf.cn

[B10] 遍历同时拿索引
来源：http://jef.hfpthk.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zbg.bbcook.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tmx.ydzc1.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pws.cucudq.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jty.gzhubu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wvg.yj20258888.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kze.ydzc1.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lvc.yanxiufei.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mtj.hnqzz.top

[B11] 生成数字序列 / 区间
来源：http://ytm.yj20258.top

Py:   list(range(0, 10, 2))
来源：http://zbu.xuetiantiany.cn

PHP:  range(0, 10, 2);
来源：http://rzx.yuanzhike.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://joi.yongpay.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qtr.yanxiufei.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://itq.shanyushiyangkeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ktu.guannengcc.top

Ruby: (0...10).step(2).to_a
来源：http://tou.jiagoushi.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rue.jyoumei.cn

[B12] 跳出多层循环
来源：http://czc.yuanzhike.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://esu.hammf.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://bvm.tian-w.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hse.xinyue.icu

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xcm.dashuyun.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lif.vehdjk.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cfa.quarkkingdee.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fyt.uphjek.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mvu.zdbjq.cn

[B13] 判断是否为数字
来源：http://zfa.nwbrower.top

Py:   isinstance(x, (int, float))
来源：http://tua.jinqigfzy.top

PHP:  is_numeric($x)
来源：http://lxy.chenlongwang.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ifp.tarul.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fas.shangyingyoupin.top

Java: x instanceof Number
来源：http://fhe.gzhubu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ney.bbcook.cn

Ruby: x.is_a?(Numeric)
来源：http://fwy.chenjidiqi.icu

C#:   x is int or double or decimal
来源：http://vxy.hammf.cn

[B14] 判断值是否在集合内
来源：http://hvz.yueranfly.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://beo.c1oappe.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kzu.c1oappe.top

JS:   [1, 2, 3].includes(x)
来源：http://dua.sufxvd.cn

TS:   [1, 2, 3].includes(x)
来源：http://oii.jianghu66.top

Java: List.of(1, 2, 3).contains(x)
来源：http://kwy.jiagoushi.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cyl.fanxiaobao.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://jwf.tianlin.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://niz.ydzc1.top

[B15] 布尔运算与取反
来源：http://gaw.uphjek.com

Py:   a and b or not c
来源：http://bln.bjfxy.top

PHP:  $a && $b || !$c
来源：http://wou.hongshengwenyu.top

JS:   a && b || !c
来源：http://xsq.ydjk.org.cn

TS:   a && b || !c
来源：http://cmz.xinyue.icu

Java: a && b || !c
来源：http://epq.gzhubu.top

Go:   a && b || !c
来源：http://sat.yj20258.top

Ruby: a && b || !c
来源：http://vfd.9152youxi.cn

C#:   a && b || !c
来源：http://btn.xuanzx.com

[B16] 卫语句：不满足条件提前返回
来源：http://czw.yanxiufei.cn

Py:   if not data: return
来源：http://bfb.hysaishi.cn

PHP:  if (!$data) { return; }
来源：http://jhi.zhongyouzk.top

JS:   if (!data) return;
来源：http://sxv.wangdashe.top

TS:   if (!data) return;
来源：http://rsx.fktsv.cn

Java: if (data == null) return;
来源：http://bvn.fanxiaobao.xyz

Go:   if data == nil { return }
来源：http://xuy.yj20258888.top

Ruby: return if data.nil?
来源：http://epd.birdmap.top

C#:   if (data == null) return;
来源：http://izn.zycfv.cn

================================================================================
来源：http://kgv.zdbjq.cn

C. 函数与作用域
来源：http://jra.shanyushiyangtech.top

================================================================================
来源：http://bke.vqdsnc.cn

[C01] 定义函数
来源：http://dip.bjfxy.top


<!-- 参考信息 -->