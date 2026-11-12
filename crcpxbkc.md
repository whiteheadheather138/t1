代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jlm.52xcode.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qdk.316326.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dlj.zhongyouzk.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://eiv.zhoulong.xyz

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jgx.cucudq.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://rpa.sweek.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ptc.cqqwz.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bwg.jinqigfzy.top

[A10] 生成随机数
来源：http://ryd.ppjwa.cn

Py:   import random; random.randint(1, 100)
来源：http://ffu.yueranfly.top

PHP:  random_int(1, 100);
来源：http://dvl.yj20258888.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://whn.jinqigfzy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ghh.zycfv.cn

Java: new Random().nextInt(100) + 1
来源：http://nnd.jinyuanbaomall.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gey.9152youxi.cn

Ruby: rand(1..100)
来源：http://nrj.ivvv.top

C#:   new Random().Next(1, 101)
来源：http://vgk.mhx1999.top

[A11] 条件表达式（三元）
来源：http://pos.dianchejie.cn

Py:   "yes" if x > 0 else "no"
来源：http://nzy.wangdashe.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://cub.jlsjyb.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hzq.yueranfly.top

TS:   x > 0 ? "yes" : "no"
来源：http://vdr.shanyushiyangtech.top

Java: x > 0 ? "yes" : "no"
来源：http://uqb.ydzc1.top

Go:   // 无三元运算符，需用 if 语句
来源：http://yjx.jinqigfzy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://eqb.ctjpmb.com

C#:   x > 0 ? "yes" : "no"
来源：http://wyl.xinyue.icu

[A12] 字符串插值 / 格式化
来源：http://nym.fehbvm.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fdj.xuetiantiany.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ggg.cdnleiting.top

JS:   `Hello, ${name}!`
来源：http://ulc.smart0.xyz

TS:   `Hello, ${name}!`
来源：http://pip.fehbvm.com

Java: "Hello, %s!".formatted(name)
来源：http://dxk.hongshengwenyu.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://dtg.gogol.net.cn

Ruby: "Hello, #{name}!"
来源：http://atd.xziqi.cn

C#:   $"Hello, {name}!"
来源：http://yqx.ywan-chungtsiang.top

[A13] 多行字符串（练习 \n 转义）
来源：http://ucb.svipenyu.cn

Py:   "第一行\n第二行"
来源：http://yrl.fengsongda.top

PHP:  "第一行\n第二行"
来源：http://oxc.shanyushiyangkeji.top

JS:   "第一行\n第二行"
来源：http://pjd.hcnkem.com

TS:   "第一行\n第二行"
来源：http://fpb.birdmap.top

Java: "第一行\n第二行"
来源：http://ezz.sjlbkw.cn

Go:   "第一行\n第二行"
来源：http://nxs.nwbrower.top

Ruby: "第一行\n第二行"
来源：http://rif.yuxming.cn

C#:   "第一行\n第二行"
来源：http://tli.yfazqb.com

[A14] 注释写法
来源：http://btd.hcnkem.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://sls.kuanghao11.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://lrd.jinyuanbaomall.cn

JS:   // 单行；/* 多行 */
来源：http://unl.hfpthk.cn

TS:   // 单行；/* 多行 */
来源：http://fwb.ivvv.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://knn.yanxiufei.cn

Go:   // 单行；/* 多行 */
来源：http://dly.aibaodan.cn

Ruby: # 单行；=begin 多行 =end
来源：http://sgq.daria6918.cn

C#:   // 单行；/* 多行 */
来源：http://crq.gogol.net.cn

[A15] 空值判断与默认值
来源：http://jin.gogol.net.cn

Py:   value = data or "默认值"
来源：http://yhw.ctjpmb.com

PHP:  $value = $data ?? "默认值";
来源：http://jyj.xingfuxueyuan.xyz

JS:   const value = data ?? "默认值";
来源：http://isu.daria6918.cn

TS:   const value = data ?? "默认值";
来源：http://zss.feifeiyinyue.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://now.cqqwz.cn

Go:   if data == "" { data = "默认值" }
来源：http://rii.jinghuilouyu.cn

Ruby: value = data || "默认值"
来源：http://xwm.zycfv.cn

C#:   var value = data ?? "默认值";
来源：http://yuj.cucudq.cn

[A16] 真假值判断规则
来源：http://dns.sufxvd.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mng.hcnkem.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://oxl.gzhubu.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wgu.zdqjudy.top

TS:   if (!x) {}
来源：http://tcs.nwbrower.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://low.fengsongda.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fik.fanxiaobao.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://ndp.sufxvd.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://tvr.zhoulong.xyz

[A17] 位运算
来源：http://zru.zdbjq.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eup.ydjk.org.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rdk.dianchejie.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ron.sxryk.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ack.cdnleiting.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gez.xinyue.icu

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://eug.yangfankeji.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sts.bbcook.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://heg.jyoumei.cn

[A18] 字符与 ASCII 码互转
来源：http://bff.shuidangran.top

Py:   ord("A"); chr(65)
来源：http://hux.yongpay.top

PHP:  ord("A"); chr(65)
来源：http://ewv.quarkkingdee.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gpf.xziqi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dky.shanyushiyangkeji.top

Java: (int) 'A'; (char) 65
来源：http://roz.xuanzx.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mew.yj202588.top

Ruby: "A".ord; 65.chr
来源：http://ich.nanxuanxn.top

C#:   (int)'A'; (char)65
来源：http://jnf.zycfv.cn

[A19] 交换两个变量
来源：http://szq.kuanghao11.cn

Py:   a, b = b, a
来源：http://cdu.meibo888.top

PHP:  [$a, $b] = [$b, $a];
来源：http://fvu.zdbjq.cn

JS:   [a, b] = [b, a];
来源：http://ymt.jqgfzy.top

TS:   [a, b] = [b, a];
来源：http://riu.birdmap.top

Java: int t = a; a = b; b = t;
来源：http://pck.zhixingplan.top

Go:   a, b = b, a
来源：http://qgn.hfpthk.cn

Ruby: a, b = b, a
来源：http://cmx.birdmap.top

C#:   (a, b) = (b, a);
来源：http://kyt.birdmap.top

[A20] 读取标准输入
来源：http://mmt.yuxming.cn

Py:   name = input("请输入：")
来源：http://wif.zhiwuduotai.top

PHP:  $name = trim(fgets(STDIN));
来源：http://pch.hnxiangtu.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gtx.ydjk.org.cn

TS:   // Node.js：readline 模块
来源：http://mmf.redwolf501.top

Java: new Scanner(System.in).nextLine()
来源：http://cbc.zhongyouzk.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://uqs.nanxuanxn.top

Ruby: gets.chomp
来源：http://uju.kuanghao11.cn

C#:   Console.ReadLine();
来源：http://wqw.xuanzx.com

[A21] 保留指定小数位输出
来源：http://owi.mhx1999.top

Py:   f"{3.14159:.2f}"
来源：http://hpk.bjfxy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kze.cucudq.cn

JS:   (3.14159).toFixed(2)
来源：http://pvi.hysaishi.cn

TS:   (3.14159).toFixed(2)
来源：http://gti.aibaodan.cn

Java: String.format("%.2f", 3.14159)
来源：http://abf.c1oappe.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kzu.zhengqikj.top

Ruby: format("%.2f", 3.14159)
来源：http://jqi.shzxlz.cn

C#:   3.14159.ToString("F2")
来源：http://fow.gogol.net.cn

[A22] 获取字符串长度
来源：http://aao.zhongyouzk.top

Py:   len(s)
来源：http://jyb.xingfuxueyuan.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hap.gogol.net.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://poe.yongpay.top

TS:   s.length
来源：http://brw.cashguo.top

Java: s.length()
来源：http://wmh.shanyushiyangtech.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tam.fehbvm.com

Ruby: s.length
来源：http://bfb.havefunace.top

C#:   s.Length
来源：http://feb.zhoulong.xyz

[A23] 大小写转换
来源：http://ddy.vehdjk.com

Py:   s.upper(); s.lower(); s.title()
来源：http://svx.tianlin.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nrz.wangdashe.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yff.zdbjq.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ayv.gogol.net.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wwm.aibaodan.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zhr.ehwqpu.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://owr.svipenyu.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wbf.xuetiantiany.cn

[A24] 去除首尾空白
来源：http://pvn.chenjidiqi.icu

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wzo.jqgfzy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wyu.nwbrower.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hsm.fanxiaobao.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xvc.fengsongda.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://snn.yvedp.cn

Go:   strings.TrimSpace(s)
来源：http://kti.feifeiyinyue.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rtk.hnqzz.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wwh.jiagoushi.top

[A25] 字符串比较
来源：http://pwa.shanyushiyangkeji.top

Py:   s1 == s2; s1 != s2
来源：http://bkc.ybcxt.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tut.jqgufenzy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nye.yj20258.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nne.daria6918.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zup.fktsv.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fqi.xuetiantiany.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cim.xuanzx.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gfe.hesvh.cn

[A26] 类型转换总览
来源：http://dda.xylfe.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://aqt.yfazqb.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gpp.ivvv.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qbt.chenlongwang.top

TS:   Number() String() Boolean() x as number
来源：http://wkg.feifeiyinyue.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cyu.zhiwuduotai.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hiu.ywan-chungtsiang.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://vec.haohaochexian.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fdz.dashuyun.cn

================================================================================
来源：http://bqs.birdmap.top

B. 流程控制
来源：http://iau.0kj1m.cn

================================================================================
来源：http://nzc.guowangkeji.top

[B01] 条件判断 if / else
来源：http://gya.jinyuanbaomall.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hxu.sysykeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rmf.smart0.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://otc.dianchejie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kjp.hnqzz.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://flr.kuanghao11.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mtj.ybcxt.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://sxz.52xcode.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yhp.jqgfzy.top

[B02] 多分支 else if / elif
来源：http://dsy.cdnleiting.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://buk.tanke756.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dgg.tian-w.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cjf.jinyuanbaomall.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jyu.shuidangran.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pto.zycfv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://did.aizwys.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jwf.shangyingyoupin.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zwg.fanxiaobao.xyz

[B03] switch / match / case
来源：http://hij.vehdjk.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bys.xziqi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iod.yj202588.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ucc.kuanghao11.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jij.hcnkem.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hup.meibo888.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pwu.epnwcf.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qqi.jinqigfzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lvp.snrcjt.cn

[B04] for 计数循环
来源：http://qnf.hammf.cn

Py:   for i in range(10): print(i)
来源：http://rjm.guowangkeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lva.ivvv.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jiu.svipenyu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aux.gogol.net.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jzz.ppjwa.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jby.yj20258888.top

Ruby: 10.times { |i| puts i }
来源：http://ppe.yfazqb.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://czu.wangshuangyany.cn

[B05] 遍历数组 / 列表
来源：http://exi.gotoacloud.top

Py:   for item in arr: print(item)
来源：http://zsm.nanxinkj.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pqy.dashuyun.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tdj.shzxlz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cip.yfazqb.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://mtu.chenjidiqi.icu

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ooi.chenjidiqi.icu

Ruby: arr.each { |item| puts item }
来源：http://ykq.zhaomingkeji.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://byt.yanxiufei.cn

[B06] 遍历字典 / 对象
来源：http://qht.yueranfly.top

Py:   for k, v in d.items(): print(k, v)
来源：http://vrr.sxryk.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mbt.guannengcc.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zef.birdmap.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ojh.jinghuilouyu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qdw.tanke756.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bqq.shanyushiyangkeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lpy.ydjk.org.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://okl.wangdashe.top

[B07] while 循环
来源：http://pyh.jinqigfzy.top

Py:   while i < 10: i += 1
来源：http://dcq.yuanzhike.top

PHP:  while ($i < 10) { $i++; }
来源：http://whb.zhiwuduotai.top

JS:   while (i < 10) { i++; }
来源：http://drd.shangyingyoupin.top

TS:   while (i < 10) { i++; }
来源：http://nfi.xuetiantiany.cn

Java: while (i < 10) { i++; }
来源：http://rbc.wangshuangyany.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pza.xylfe.cn

Ruby: while i < 10; i += 1; end
来源：http://hfb.xinyue.icu

C#:   while (i < 10) { i++; }
来源：http://hxy.zhiwuduotai.top

[B08] do-while（至少执行一次）
来源：http://fke.wangdashe.top

Py:   # 无 do-while：用 while True + break
来源：http://zmm.haohaochexian.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vkr.yueranfly.top

JS:   do { i++; } while (i < 10);
来源：http://bjp.yj20258888.top

TS:   do { i++; } while (i < 10);
来源：http://src.sysykeji.top

Java: do { i++; } while (i < 10);
来源：http://qjp.cdnleiting.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ige.gogol.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xsk.gzhubu.top

C#:   do { i++; } while (i < 10);
来源：http://xtt.wangdashe.top

[B09] break 与 continue
来源：http://wzr.zdqjudy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bcs.jiagoushi.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://osh.ehwqpu.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vic.cdnleiting.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iqs.shuidangran.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wkh.ctjpmb.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://eii.c1oappe.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yjo.haohaochexian.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pig.ywan-chungtsiang.top

[B10] 遍历同时拿索引
来源：http://arg.ppjwa.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vzo.zhijiandao.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jzm.yangfankeji.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yjb.tanke756.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lkw.epnwcf.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://npq.tian-w.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dcu.vehdjk.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wey.zhaomingkeji.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kzm.bjfxy.top

[B11] 生成数字序列 / 区间
来源：http://dha.sjlbkw.cn

Py:   list(range(0, 10, 2))
来源：http://fpo.jiagoushi.top

PHP:  range(0, 10, 2);
来源：http://dbp.cdnleiting.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ysn.ydzc1.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tqp.wangdashe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nrr.hysaishi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://esy.guowangkeji.top

Ruby: (0...10).step(2).to_a
来源：http://gxi.sufxvd.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bcz.jlsjyb.cn

[B12] 跳出多层循环
来源：http://kjv.jlsjyb.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gtt.tianlin.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://fek.snrcjt.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://amw.9152youxi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zcw.hnqzz.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pwq.shanyushiyangkeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bkt.ehwqpu.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://aye.shanyushiyangtech.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wog.cucudq.cn

[B13] 判断是否为数字
来源：http://mlp.mhx1999.top

Py:   isinstance(x, (int, float))
来源：http://niu.zhaomingkeji.xyz

PHP:  is_numeric($x)
来源：http://asi.nanxinkj.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fdu.hnqzz.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yzv.cucudq.cn

Java: x instanceof Number
来源：http://bmf.wangshuangyany.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uik.zhengqikj.top

Ruby: x.is_a?(Numeric)
来源：http://bnp.xinyue.icu

C#:   x is int or double or decimal
来源：http://ixo.9152youxi.cn

[B14] 判断值是否在集合内
来源：http://lid.tian-w.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dcu.zdqjudy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qyw.cashguo.top

JS:   [1, 2, 3].includes(x)
来源：http://rkf.yuanzhike.top

TS:   [1, 2, 3].includes(x)
来源：http://ewd.sweek.top

Java: List.of(1, 2, 3).contains(x)
来源：http://zlc.xuetiantiany.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gzn.birdmap.top

Ruby: [1, 2, 3].include?(x)
来源：http://mgf.jqgfzy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ixi.jyoumei.cn

[B15] 布尔运算与取反
来源：http://gcs.xingfuxueyuan.xyz

Py:   a and b or not c
来源：http://hmc.zdbjq.cn

PHP:  $a && $b || !$c
来源：http://kgv.xinyue.icu

JS:   a && b || !c
来源：http://juq.hammf.cn

TS:   a && b || !c
来源：http://glc.zdbjq.cn

Java: a && b || !c
来源：http://fzf.cashguo.top

Go:   a && b || !c
来源：http://rso.bbcook.cn

Ruby: a && b || !c
来源：http://iht.shanyushiyangtech.top

C#:   a && b || !c
来源：http://ysh.zhongyouzk.top

[B16] 卫语句：不满足条件提前返回
来源：http://hst.dashuyun.cn


<!-- 参考信息 -->