代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://onr.ybcxt.top

Java: new Random().nextInt(100) + 1
来源：http://dgs.hnqzz.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fik.tian-w.cn

Ruby: rand(1..100)
来源：http://vlh.birdmap.top

C#:   new Random().Next(1, 101)
来源：http://wsi.zdqjudy.top

[A11] 条件表达式（三元）
来源：http://xwg.jinghuilouyu.cn

Py:   "yes" if x > 0 else "no"
来源：http://ojl.shuidangran.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://nnw.shuidangran.top

JS:   x > 0 ? "yes" : "no"
来源：http://syn.zhixingplan.top

TS:   x > 0 ? "yes" : "no"
来源：http://yce.nwbrower.top

Java: x > 0 ? "yes" : "no"
来源：http://bnt.tian-w.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://shf.tarul.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://nap.andypj.xyz

C#:   x > 0 ? "yes" : "no"
来源：http://wxu.xylfe.cn

[A12] 字符串插值 / 格式化
来源：http://cqp.tanke756.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://snv.jinqigfzy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mmp.tanke756.top

JS:   `Hello, ${name}!`
来源：http://ozx.tianlin.xyz

TS:   `Hello, ${name}!`
来源：http://bvv.zhiwuduotai.top

Java: "Hello, %s!".formatted(name)
来源：http://tbs.zhijiandao.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fgb.uphjek.com

Ruby: "Hello, #{name}!"
来源：http://yho.xuanzx.com

C#:   $"Hello, {name}!"
来源：http://qac.aibaodan.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ilz.daxiang520.top

Py:   "第一行\n第二行"
来源：http://qul.fanxiaobao.xyz

PHP:  "第一行\n第二行"
来源：http://gog.yvedp.cn

JS:   "第一行\n第二行"
来源：http://gdj.guowangkeji.top

TS:   "第一行\n第二行"
来源：http://arn.ydjk.org.cn

Java: "第一行\n第二行"
来源：http://ppv.tianlin.xyz

Go:   "第一行\n第二行"
来源：http://sqi.havefunace.top

Ruby: "第一行\n第二行"
来源：http://iah.shanyushiyangkeji.top

C#:   "第一行\n第二行"
来源：http://zpf.xylfe.cn

[A14] 注释写法
来源：http://qoc.jianghu66.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://qcv.chenlongwang.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ytt.cdnleiting.top

JS:   // 单行；/* 多行 */
来源：http://tyj.zdqjudy.top

TS:   // 单行；/* 多行 */
来源：http://veh.sxryk.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yzt.shanyushiyangkeji.top

Go:   // 单行；/* 多行 */
来源：http://xhz.tianlin.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://qlj.yfazqb.com

C#:   // 单行；/* 多行 */
来源：http://yqv.yongpay.top

[A15] 空值判断与默认值
来源：http://dpv.jinghuilouyu.cn

Py:   value = data or "默认值"
来源：http://lci.0kj1m.cn

PHP:  $value = $data ?? "默认值";
来源：http://gtt.aibaodan.cn

JS:   const value = data ?? "默认值";
来源：http://znj.ydjk.org.cn

TS:   const value = data ?? "默认值";
来源：http://qvy.guowangkeji.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jdo.shanyushiyangkeji.top

Go:   if data == "" { data = "默认值" }
来源：http://kjo.shanyushiyangtech.top

Ruby: value = data || "默认值"
来源：http://hvq.jinqigufen.top

C#:   var value = data ?? "默认值";
来源：http://cww.yj20258.top

[A16] 真假值判断规则
来源：http://nuk.zhongyouzk.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xoq.cucudq.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rnk.yj202588.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xkd.hysaishi.cn

TS:   if (!x) {}
来源：http://roj.xingfuxueyuan.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yye.tianlin.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://beu.shzxlz.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jnz.yuxming.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tns.zhongyouzk.top

[A17] 位运算
来源：http://jab.tianlin.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bst.wangshuangyany.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zil.9152youxi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bhb.gaohongyu789.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ddb.shanyushiyangkeji.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xkl.hnqzz.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hrh.zdqjudy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rrw.chenjidiqi.icu

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xgs.shuidangran.top

[A18] 字符与 ASCII 码互转
来源：http://zzz.hnqzz.top

Py:   ord("A"); chr(65)
来源：http://ilb.shanyushiyangkeji.top

PHP:  ord("A"); chr(65)
来源：http://eqx.jinqigfzy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gzd.zycfv.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://awh.yvedp.cn

Java: (int) 'A'; (char) 65
来源：http://ipl.wangshuangyany.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cyb.cqqwz.cn

Ruby: "A".ord; 65.chr
来源：http://bir.andypj.xyz

C#:   (int)'A'; (char)65
来源：http://ifp.shanyushiyangkeji.top

[A19] 交换两个变量
来源：http://caa.xylfe.cn

Py:   a, b = b, a
来源：http://mwq.yvedp.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ofg.jqgufenzy.top

JS:   [a, b] = [b, a];
来源：http://rcb.zhongyouzk.top

TS:   [a, b] = [b, a];
来源：http://bpd.tian-w.cn

Java: int t = a; a = b; b = t;
来源：http://syu.zhoulong.xyz

Go:   a, b = b, a
来源：http://jsh.yonumen.top

Ruby: a, b = b, a
来源：http://heu.zhijiandao.cn

C#:   (a, b) = (b, a);
来源：http://fgk.sufxvd.cn

[A20] 读取标准输入
来源：http://vjv.haohaochexian.top

Py:   name = input("请输入：")
来源：http://sud.gaohongyu789.top

PHP:  $name = trim(fgets(STDIN));
来源：http://jgw.feifeiyinyue.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wgq.mhx1999.top

TS:   // Node.js：readline 模块
来源：http://hjc.cucudq.cn

Java: new Scanner(System.in).nextLine()
来源：http://nny.fanxiaobao.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xxh.fengsongda.top

Ruby: gets.chomp
来源：http://uwn.yuanzhike.top

C#:   Console.ReadLine();
来源：http://gig.wangshuangyany.cn

[A21] 保留指定小数位输出
来源：http://nev.ctjpmb.com

Py:   f"{3.14159:.2f}"
来源：http://ugn.gotoacloud.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://iwj.yj20258888.top

JS:   (3.14159).toFixed(2)
来源：http://ikt.xziqi.cn

TS:   (3.14159).toFixed(2)
来源：http://bjl.xingfuxueyuan.xyz

Java: String.format("%.2f", 3.14159)
来源：http://edc.sjlbkw.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qzx.nanxinkj.top

Ruby: format("%.2f", 3.14159)
来源：http://hrj.zhaomingkeji.xyz

C#:   3.14159.ToString("F2")
来源：http://tac.nanxuanxn.top

[A22] 获取字符串长度
来源：http://ztg.0kj1m.cn

Py:   len(s)
来源：http://qzl.tianlin.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xyd.ppjwa.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ifx.sysykeji.top

TS:   s.length
来源：http://vwr.hesvh.cn

Java: s.length()
来源：http://adh.chenjidiqi.icu

Go:   len(s); utf8.RuneCountInString(s)
来源：http://skb.haohaochexian.top

Ruby: s.length
来源：http://ljr.yuxming.cn

C#:   s.Length
来源：http://daa.jqgfzy.top

[A23] 大小写转换
来源：http://obh.fengsongda.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ddv.chenlongwang.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nce.jinyuanbaomall.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://msl.fzhhl.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mur.wangshuangyany.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lcd.jiagoushi.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mjw.bbcook.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://spf.haohaochexian.top

C#:   s.ToUpper(); s.ToLower()
来源：http://rwx.jinqigfzy.top

[A24] 去除首尾空白
来源：http://giv.316326.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://amm.gzhubu.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pry.yuanzhike.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dxo.kuanghao11.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://woy.nanxuanxn.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xsw.tian-w.cn

Go:   strings.TrimSpace(s)
来源：http://phb.hammf.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cfu.jqgfzy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tkt.yj202588.top

[A25] 字符串比较
来源：http://drt.yj20258.top

Py:   s1 == s2; s1 != s2
来源：http://xqa.shangyingyoupin.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://otu.xuetiantiany.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yda.sufxvd.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ado.epnwcf.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xrr.zhiwuduotai.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fff.dashuyun.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://bdr.jqgufenzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://eww.ctjpmb.com

[A26] 类型转换总览
来源：http://wep.wangshuangyany.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jew.feifeiyinyue.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vnn.hnxiangtu.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xhr.hfpthk.cn

TS:   Number() String() Boolean() x as number
来源：http://hou.52xcode.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fwm.jinqigfzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wkt.hesvh.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://paj.bbcook.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dqv.cdnleiting.top

================================================================================
来源：http://ohk.tarul.cn

B. 流程控制
来源：http://ujv.bbcook.cn

================================================================================
来源：http://tcm.dashuyun.cn

[B01] 条件判断 if / else
来源：http://fkg.dianchejie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://lrd.tarul.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qhl.shangyingyoupin.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xni.quarkkingdee.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://clr.dianchejie.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wge.jinqigfzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jvn.sufxvd.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lgg.52xcode.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gnf.nanxuanxn.top

[B02] 多分支 else if / elif
来源：http://nce.xylfe.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fom.yuanzhike.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://oyr.ehwqpu.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rek.yj20258888.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wff.nanxuanxn.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ckr.jinqigfzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fwt.yvedp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jru.bbcook.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ocp.gogol.net.cn

[B03] switch / match / case
来源：http://zce.zhaomingkeji.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://iby.chenlongwang.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zhj.ybcxt.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xys.zhiwuduotai.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ztz.hfpthk.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jio.svipenyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tym.sweek.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tpy.316326.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qce.dianchejie.cn

[B04] for 计数循环
来源：http://muh.hywenlv.cn

Py:   for i in range(10): print(i)
来源：http://zmq.kuanghao11.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yxt.sxryk.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gwu.kuanghao11.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zna.aizwys.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ouy.nanxinkj.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vna.nwbrower.top

Ruby: 10.times { |i| puts i }
来源：http://ahs.yanxiufei.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zje.chenzaomai.com

[B05] 遍历数组 / 列表
来源：http://lef.9152youxi.cn

Py:   for item in arr: print(item)
来源：http://esm.jyoumei.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nxu.dianchejie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hds.gzhubu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://dmx.hnqzz.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://wuq.hcnkem.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jpf.cdnleiting.top

Ruby: arr.each { |item| puts item }
来源：http://xjc.nwbrower.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cfs.hywenlv.cn

[B06] 遍历字典 / 对象
来源：http://sxj.zdqjudy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://emc.cdnleiting.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bun.aizwys.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ecm.yuanzhike.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://afe.zhoulong.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rpi.cashguo.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wyh.cqqwz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://snf.zhoulong.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ztk.jianghu66.top

[B07] while 循环
来源：http://cia.fehbvm.com

Py:   while i < 10: i += 1
来源：http://air.shanyushiyangkeji.top

PHP:  while ($i < 10) { $i++; }
来源：http://nnb.yanxiufei.cn

JS:   while (i < 10) { i++; }
来源：http://kkj.gogol.net.cn

TS:   while (i < 10) { i++; }
来源：http://bkn.gzhubu.top

Java: while (i < 10) { i++; }
来源：http://zff.zycfv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pmf.mhx1999.top

Ruby: while i < 10; i += 1; end
来源：http://ciq.yanxiufei.cn

C#:   while (i < 10) { i++; }
来源：http://jcc.sjlbkw.cn

[B08] do-while（至少执行一次）
来源：http://mmt.jqgufenzy.top

Py:   # 无 do-while：用 while True + break
来源：http://uxm.gogol.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ucn.guannengcc.top

JS:   do { i++; } while (i < 10);
来源：http://kst.cheryme.top

TS:   do { i++; } while (i < 10);
来源：http://srs.aizwys.cn

Java: do { i++; } while (i < 10);
来源：http://lsg.pengpengdd.cyou

Go:   for { i++; if i >= 10 { break } }
来源：http://ewi.zdqjudy.top

Ruby: begin; i += 1; end while i < 10
来源：http://hcc.fzhhl.top

C#:   do { i++; } while (i < 10);
来源：http://bbz.zhijiandao.cn

[B09] break 与 continue
来源：http://bis.nanxuanxn.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://agi.ehwqpu.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://swf.vqdsnc.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qzr.tanke756.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zho.pycfn.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gqg.zdqjudy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hzk.birdmap.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lvk.jyoumei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eaa.svipenyu.cn

[B10] 遍历同时拿索引
来源：http://wmm.wangdashe.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wau.ywan-chungtsiang.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dhk.fengsongda.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ped.kuanghao11.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://odp.tanke756.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rpy.dianchejie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://orl.fanxiaobao.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ioh.epnwcf.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://igc.fanxiaobao.xyz

[B11] 生成数字序列 / 区间
来源：http://evn.chenzaomai.com

Py:   list(range(0, 10, 2))
来源：http://ebj.uphjek.com

PHP:  range(0, 10, 2);
来源：http://hnf.xinyue.icu

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rdn.tianlin.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cvg.shangyingyoupin.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nlz.ppjwa.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wxg.uphjek.com

Ruby: (0...10).step(2).to_a
来源：http://akq.jyoumei.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yny.jlsjyb.cn

[B12] 跳出多层循环
来源：http://sac.52xcode.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vlt.gotoacloud.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ctj.gotoacloud.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ryd.aizwys.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://axi.zycfv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jmm.mhx1999.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://juq.tian-w.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yaz.jqgufenzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://brf.yonumen.top

[B13] 判断是否为数字
来源：http://syf.316326.xyz

Py:   isinstance(x, (int, float))
来源：http://oft.hnxiangtu.top

PHP:  is_numeric($x)
来源：http://nog.epnwcf.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nre.gotoacloud.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://scf.mhx1999.top

Java: x instanceof Number
来源：http://ebo.epnwcf.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wnn.nanxuanxn.top

Ruby: x.is_a?(Numeric)
来源：http://lar.zhaomingkeji.xyz

C#:   x is int or double or decimal
来源：http://unj.aizwys.cn

[B14] 判断值是否在集合内
来源：http://uyt.yj20258888.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tgr.xziqi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ahx.cheryme.top

JS:   [1, 2, 3].includes(x)
来源：http://gno.yj202588.top

TS:   [1, 2, 3].includes(x)
来源：http://kxg.fanxiaobao.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://bjt.hysaishi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xsh.yuanzhike.top

Ruby: [1, 2, 3].include?(x)
来源：http://otu.xingfuxueyuan.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://iml.cheryme.top

[B15] 布尔运算与取反
来源：http://aig.gzhubu.top

Py:   a and b or not c
来源：http://llu.jinghuilouyu.cn

PHP:  $a && $b || !$c
来源：http://ujp.ehwqpu.com

JS:   a && b || !c
来源：http://zix.tianlin.xyz

TS:   a && b || !c
来源：http://ioz.yfazqb.com

Java: a && b || !c
来源：http://jxh.xinyue.icu

Go:   a && b || !c
来源：http://fuv.c1oappe.top

Ruby: a && b || !c
来源：http://yva.dashuyun.cn

C#:   a && b || !c
来源：http://vyo.iojbl.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xhk.yuxming.cn

Py:   if not data: return
来源：http://bxf.c1oappe.top

PHP:  if (!$data) { return; }
来源：http://gzh.daxiang520.top

JS:   if (!data) return;
来源：http://wbo.ctjpmb.com

TS:   if (!data) return;
来源：http://itb.gaohongyu789.top

Java: if (data == null) return;
来源：http://yai.jinqigufen.top

Go:   if data == nil { return }
来源：http://vpb.shzxlz.cn

Ruby: return if data.nil?
来源：http://bcf.yanxiufei.cn

C#:   if (data == null) return;
来源：http://yoq.hysaishi.cn

================================================================================
来源：http://ryh.bbcook.cn

C. 函数与作用域
来源：http://mwh.pengpengdd.cyou

================================================================================
来源：http://uqc.chenjidiqi.icu

[C01] 定义函数
来源：http://pxw.gogol.net.cn


<!-- 参考信息 -->