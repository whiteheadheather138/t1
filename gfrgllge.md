代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://raa.shanyushiyangtech.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cyz.hfpthk.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xvz.yangfankeji.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tub.pengpengdd.cyou

[A10] 生成随机数
来源：http://sef.shzxlz.cn

Py:   import random; random.randint(1, 100)
来源：http://axm.zhixingplan.top

PHP:  random_int(1, 100);
来源：http://gug.ydzc1.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://uhh.yangfankeji.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bcq.yfazqb.com

Java: new Random().nextInt(100) + 1
来源：http://dap.zdbjq.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mta.yuanzhike.top

Ruby: rand(1..100)
来源：http://zsz.jlsjyb.cn

C#:   new Random().Next(1, 101)
来源：http://zlt.zdbjq.cn

[A11] 条件表达式（三元）
来源：http://jgx.yj20258888.top

Py:   "yes" if x > 0 else "no"
来源：http://fin.xingfuxueyuan.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://bqi.sysykeji.top

JS:   x > 0 ? "yes" : "no"
来源：http://wfh.havefunace.top

TS:   x > 0 ? "yes" : "no"
来源：http://peu.shanyushiyangkeji.top

Java: x > 0 ? "yes" : "no"
来源：http://hcd.gaohongyu789.top

Go:   // 无三元运算符，需用 if 语句
来源：http://qjg.sjlbkw.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://kej.snrcjt.cn

C#:   x > 0 ? "yes" : "no"
来源：http://sae.zhongyouzk.top

[A12] 字符串插值 / 格式化
来源：http://nvs.hesvh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lax.ehwqpu.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ugz.ydjk.org.cn

JS:   `Hello, ${name}!`
来源：http://udl.zhijiandao.cn

TS:   `Hello, ${name}!`
来源：http://kyj.yj202588.top

Java: "Hello, %s!".formatted(name)
来源：http://frw.hysaishi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jbt.mhx1999.top

Ruby: "Hello, #{name}!"
来源：http://cgv.xuanzx.com

C#:   $"Hello, {name}!"
来源：http://ugk.shzxlz.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://axb.smart0.xyz

Py:   "第一行\n第二行"
来源：http://phm.guannengcc.top

PHP:  "第一行\n第二行"
来源：http://bmp.svipenyu.cn

JS:   "第一行\n第二行"
来源：http://lgm.chenjidiqi.icu

TS:   "第一行\n第二行"
来源：http://vpm.jinghuilouyu.cn

Java: "第一行\n第二行"
来源：http://rcv.shanyushiyangkeji.top

Go:   "第一行\n第二行"
来源：http://cbq.zhengqikj.top

Ruby: "第一行\n第二行"
来源：http://axo.tanke756.top

C#:   "第一行\n第二行"
来源：http://gjy.smart0.xyz

[A14] 注释写法
来源：http://dpi.ydzc1.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://mlc.hfpthk.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xoo.sysykeji.top

JS:   // 单行；/* 多行 */
来源：http://wpl.dashuyun.cn

TS:   // 单行；/* 多行 */
来源：http://hxz.zhiwuduotai.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rsl.hcnkem.com

Go:   // 单行；/* 多行 */
来源：http://vjp.316326.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://sgw.fehbvm.com

C#:   // 单行；/* 多行 */
来源：http://dvb.gotoacloud.top

[A15] 空值判断与默认值
来源：http://php.zdqjudy.top

Py:   value = data or "默认值"
来源：http://tdy.yueranfly.top

PHP:  $value = $data ?? "默认值";
来源：http://fxl.zdbjq.cn

JS:   const value = data ?? "默认值";
来源：http://czy.ywan-chungtsiang.top

TS:   const value = data ?? "默认值";
来源：http://qcc.cdnleiting.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ngu.uphjek.com

Go:   if data == "" { data = "默认值" }
来源：http://bww.sjlbkw.cn

Ruby: value = data || "默认值"
来源：http://jsj.smart0.xyz

C#:   var value = data ?? "默认值";
来源：http://rzz.svipenyu.cn

[A16] 真假值判断规则
来源：http://wsk.xylfe.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vnj.vehdjk.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wqu.jlsjyb.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://luu.yuanzhike.top

TS:   if (!x) {}
来源：http://ear.ivvv.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://urv.tian-w.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pau.jinyuanbaomall.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lox.jqgfzy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vje.mhx1999.top

[A17] 位运算
来源：http://qre.vqdsnc.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baw.havefunace.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://eta.ywan-chungtsiang.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kax.ppjwa.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wjw.yangfankeji.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://glz.havefunace.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://okm.pengpengdd.cyou

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ebd.snrcjt.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gon.ivvv.top

[A18] 字符与 ASCII 码互转
来源：http://xba.chenjidiqi.icu

Py:   ord("A"); chr(65)
来源：http://cvt.xziqi.cn

PHP:  ord("A"); chr(65)
来源：http://dbd.52xcode.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://etg.aizwys.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://swq.yanxiufei.cn

Java: (int) 'A'; (char) 65
来源：http://cvi.guannengcc.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hak.guowangkeji.top

Ruby: "A".ord; 65.chr
来源：http://bmy.yvedp.cn

C#:   (int)'A'; (char)65
来源：http://mvj.yvedp.cn

[A19] 交换两个变量
来源：http://ifb.zhiwuduotai.top

Py:   a, b = b, a
来源：http://kxh.yuxming.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://yjq.xingfuxueyuan.xyz

JS:   [a, b] = [b, a];
来源：http://kao.fktsv.cn

TS:   [a, b] = [b, a];
来源：http://pwd.zdqjudy.top

Java: int t = a; a = b; b = t;
来源：http://tjf.yanxiufei.cn

Go:   a, b = b, a
来源：http://imu.tianlin.xyz

Ruby: a, b = b, a
来源：http://yar.dianchejie.cn

C#:   (a, b) = (b, a);
来源：http://bce.guowangkeji.top

[A20] 读取标准输入
来源：http://kif.zhaomingkeji.xyz

Py:   name = input("请输入：")
来源：http://dtd.vehdjk.com

PHP:  $name = trim(fgets(STDIN));
来源：http://efy.fktsv.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dse.redwolf501.top

TS:   // Node.js：readline 模块
来源：http://epp.daxiang520.top

Java: new Scanner(System.in).nextLine()
来源：http://tpj.cucudq.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lan.jqgfzy.top

Ruby: gets.chomp
来源：http://zep.vqdsnc.cn

C#:   Console.ReadLine();
来源：http://xyt.gogol.net.cn

[A21] 保留指定小数位输出
来源：http://iab.andypj.xyz

Py:   f"{3.14159:.2f}"
来源：http://oqf.smart0.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://aws.ydjk.org.cn

JS:   (3.14159).toFixed(2)
来源：http://tgg.jqgfzy.top

TS:   (3.14159).toFixed(2)
来源：http://otl.yongpay.top

Java: String.format("%.2f", 3.14159)
来源：http://rsv.0kj1m.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://eij.zhijiandao.cn

Ruby: format("%.2f", 3.14159)
来源：http://cey.svipenyu.cn

C#:   3.14159.ToString("F2")
来源：http://rjv.xziqi.cn

[A22] 获取字符串长度
来源：http://cim.guannengcc.top

Py:   len(s)
来源：http://moh.sweek.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nih.andypj.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dga.uphjek.com

TS:   s.length
来源：http://ffk.tarul.cn

Java: s.length()
来源：http://lto.nwbrower.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fdk.chenjidiqi.icu

Ruby: s.length
来源：http://vmi.chenzaomai.com

C#:   s.Length
来源：http://sce.guannengcc.top

[A23] 大小写转换
来源：http://non.guannengcc.top

Py:   s.upper(); s.lower(); s.title()
来源：http://wfl.zycfv.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ato.ehwqpu.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://srj.ehwqpu.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://vnf.fzhhl.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zil.ybcxt.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://iri.guannengcc.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://oln.zhengqikj.top

C#:   s.ToUpper(); s.ToLower()
来源：http://rsv.c1oappe.top

[A24] 去除首尾空白
来源：http://sht.yanxiufei.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mco.xingfuxueyuan.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fus.wangdashe.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nxe.tanke756.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gst.ydzc1.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cnh.hfpthk.cn

Go:   strings.TrimSpace(s)
来源：http://hav.yonumen.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wux.xuanzx.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xsv.dianchejie.cn

[A25] 字符串比较
来源：http://lzt.kuanghao11.cn

Py:   s1 == s2; s1 != s2
来源：http://bui.c1oappe.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wgd.ppjwa.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://azr.shangyingyoupin.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jut.dashuyun.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://vem.cashguo.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ptg.sjlbkw.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pqp.chenlongwang.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kos.xingfuxueyuan.xyz

[A26] 类型转换总览
来源：http://fuc.zhixingplan.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ryc.quarkkingdee.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xui.fzhhl.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yeb.daxiang520.top

TS:   Number() String() Boolean() x as number
来源：http://vty.ehwqpu.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sqn.birdmap.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rkz.jinqigufen.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://iil.hnqzz.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ojz.cucudq.cn

================================================================================
来源：http://ppo.cucudq.cn

B. 流程控制
来源：http://cqh.fktsv.cn

================================================================================
来源：http://qfd.ywan-chungtsiang.top

[B01] 条件判断 if / else
来源：http://ayw.cdnleiting.top

Py:   result = "正" if x > 0 else "非正"
来源：http://coz.kuanghao11.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tbj.daria6918.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yoz.uphjek.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tgg.meibo888.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://fgr.zhongyouzk.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zhy.cqqwz.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gew.xziqi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://aqr.yfazqb.com

[B02] 多分支 else if / elif
来源：http://ubu.haohaochexian.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mqz.yuanzhike.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://quj.daria6918.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wrs.snrcjt.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vek.xinyue.icu

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://isw.shangyingyoupin.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gar.hnxiangtu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://egx.nwbrower.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://obo.ywan-chungtsiang.top

[B03] switch / match / case
来源：http://wef.0kj1m.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cdl.xylfe.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ekz.hongshengwenyu.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jfi.gaohongyu789.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://viw.gogol.net.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kel.cdnleiting.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fda.haohaochexian.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kpu.smart0.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bmp.hywenlv.cn

[B04] for 计数循环
来源：http://qzz.nwbrower.top

Py:   for i in range(10): print(i)
来源：http://kee.jlsjyb.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zwi.hammf.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hjp.nanxinkj.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ztt.zhoulong.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://alt.yj20258.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://iwd.vqdsnc.cn

Ruby: 10.times { |i| puts i }
来源：http://xif.snrcjt.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nnf.yj20258.top

[B05] 遍历数组 / 列表
来源：http://hza.zdqjudy.top

Py:   for item in arr: print(item)
来源：http://gra.hnqzz.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mpv.hnxiangtu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hwn.snrcjt.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://gqy.havefunace.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ise.redwolf501.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qix.sjlbkw.cn

Ruby: arr.each { |item| puts item }
来源：http://acv.dianchejie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gjq.jinqigfzy.top

[B06] 遍历字典 / 对象
来源：http://jks.shangyingyoupin.top

Py:   for k, v in d.items(): print(k, v)
来源：http://djm.cdnleiting.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lgh.feifeiyinyue.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zin.aibaodan.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dir.tanke756.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qyz.wangshuangyany.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yjh.zycfv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vkr.jinyuanbaomall.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kjg.tanke756.top

[B07] while 循环
来源：http://jco.hcnkem.com

Py:   while i < 10: i += 1
来源：http://obe.sweek.top

PHP:  while ($i < 10) { $i++; }
来源：http://bck.ppjwa.cn

JS:   while (i < 10) { i++; }
来源：http://zme.yueranfly.top

TS:   while (i < 10) { i++; }
来源：http://aze.gzhubu.top

Java: while (i < 10) { i++; }
来源：http://orf.gaohongyu789.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zgz.zycfv.cn

Ruby: while i < 10; i += 1; end
来源：http://ngo.zhengqikj.top

C#:   while (i < 10) { i++; }
来源：http://hve.quarkkingdee.top

[B08] do-while（至少执行一次）
来源：http://odd.smart0.xyz

Py:   # 无 do-while：用 while True + break
来源：http://tgw.sweek.top

PHP:  do { $i++; } while ($i < 10);
来源：http://dyd.hongshengwenyu.top

JS:   do { i++; } while (i < 10);
来源：http://itn.wangdashe.top

TS:   do { i++; } while (i < 10);
来源：http://ipq.jianghu66.top

Java: do { i++; } while (i < 10);
来源：http://cut.tanke756.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ukc.yueranfly.top

Ruby: begin; i += 1; end while i < 10
来源：http://umy.wangdashe.top

C#:   do { i++; } while (i < 10);
来源：http://tmg.bjfxy.top

[B09] break 与 continue
来源：http://zhn.cheryme.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://anp.chenlongwang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lma.sufxvd.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://olt.guannengcc.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oek.fanxiaobao.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://abp.tanke756.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://krf.ydjk.org.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ztn.jinqigfzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dzy.iojbl.cn

[B10] 遍历同时拿索引
来源：http://uoa.zycfv.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hsf.sweek.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bgc.uphjek.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://edj.ivvv.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://itn.chenjidiqi.icu

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kyx.jinqigfzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hhx.iojbl.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nev.aibaodan.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ztj.yonumen.top

[B11] 生成数字序列 / 区间
来源：http://gnl.meibo888.top

Py:   list(range(0, 10, 2))
来源：http://jxb.gogol.net.cn

PHP:  range(0, 10, 2);
来源：http://sjh.tianlin.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hbz.jinyuanbaomall.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ldr.jinghuilouyu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wjs.xziqi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://aix.daxiang520.top

Ruby: (0...10).step(2).to_a
来源：http://pod.redwolf501.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://amg.yj20258.top

[B12] 跳出多层循环
来源：http://fbs.yonumen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ago.zycfv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qct.vqdsnc.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ram.zdbjq.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bua.haohaochexian.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dnc.sysykeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dev.316326.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wpx.daria6918.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vjk.hesvh.cn

[B13] 判断是否为数字
来源：http://ynh.vehdjk.com

Py:   isinstance(x, (int, float))
来源：http://cmr.svipenyu.cn

PHP:  is_numeric($x)
来源：http://cdr.jiagoushi.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fdg.ydzc1.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iwx.sufxvd.cn

Java: x instanceof Number
来源：http://fcy.feifeiyinyue.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://iif.haohaochexian.top

Ruby: x.is_a?(Numeric)
来源：http://ncp.jiagoushi.top

C#:   x is int or double or decimal
来源：http://wlh.dashuyun.cn

[B14] 判断值是否在集合内
来源：http://tyg.cucudq.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wob.sufxvd.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kul.gogol.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://nxv.hongshengwenyu.top

TS:   [1, 2, 3].includes(x)
来源：http://lts.jianghu66.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mhb.ydzc1.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gfl.yangfankeji.com

Ruby: [1, 2, 3].include?(x)
来源：http://vnv.chenzaomai.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mci.jyoumei.cn

[B15] 布尔运算与取反
来源：http://rop.daxiang520.top

Py:   a and b or not c
来源：http://khv.9152youxi.cn

PHP:  $a && $b || !$c
来源：http://hzb.yfazqb.com

JS:   a && b || !c
来源：http://hul.zhiwuduotai.top

TS:   a && b || !c
来源：http://zbl.dianchejie.cn

Java: a && b || !c
来源：http://sor.nanxinkj.top

Go:   a && b || !c
来源：http://etk.birdmap.top

Ruby: a && b || !c
来源：http://gpt.hcnkem.com

C#:   a && b || !c
来源：http://cum.vqdsnc.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vhp.zdbjq.cn

Py:   if not data: return
来源：http://iyx.cqqwz.cn

PHP:  if (!$data) { return; }
来源：http://zve.guannengcc.top

JS:   if (!data) return;
来源：http://kjg.hywenlv.cn

TS:   if (!data) return;
来源：http://dlx.ywan-chungtsiang.top


<!-- 参考信息 -->