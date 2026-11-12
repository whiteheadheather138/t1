代发 wailian999

[A10] 生成随机数
来源：http://dvy.yj20258.top

Py:   import random; random.randint(1, 100)
来源：http://tnk.chenlongwang.top

PHP:  random_int(1, 100);
来源：http://sgp.wangshuangyany.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wnh.zdbjq.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ioi.yfazqb.com

Java: new Random().nextInt(100) + 1
来源：http://qjj.hywenlv.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gdd.zdqjudy.top

Ruby: rand(1..100)
来源：http://ojq.pycfn.com

C#:   new Random().Next(1, 101)
来源：http://swf.hfpthk.cn

[A11] 条件表达式（三元）
来源：http://eqn.yj20258.top

Py:   "yes" if x > 0 else "no"
来源：http://buh.quarkkingdee.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://rsx.yj20258888.top

JS:   x > 0 ? "yes" : "no"
来源：http://ogl.hywenlv.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rxp.guannengcc.top

Java: x > 0 ? "yes" : "no"
来源：http://yml.andypj.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://znv.ydjk.org.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://mzy.nanxinkj.top

C#:   x > 0 ? "yes" : "no"
来源：http://cqm.guowangkeji.top

[A12] 字符串插值 / 格式化
来源：http://rkr.fehbvm.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hro.gaohongyu789.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yzv.yj20258888.top

JS:   `Hello, ${name}!`
来源：http://edz.ppjwa.cn

TS:   `Hello, ${name}!`
来源：http://ayt.gaohongyu789.top

Java: "Hello, %s!".formatted(name)
来源：http://gdn.zhoulong.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://etg.xylfe.cn

Ruby: "Hello, #{name}!"
来源：http://hmx.fzhhl.top

C#:   $"Hello, {name}!"
来源：http://cdk.jinghuilouyu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://phm.shanyushiyangkeji.top

Py:   "第一行\n第二行"
来源：http://nqy.bbcook.cn

PHP:  "第一行\n第二行"
来源：http://mkb.tianlin.xyz

JS:   "第一行\n第二行"
来源：http://imm.gogol.net.cn

TS:   "第一行\n第二行"
来源：http://fop.ydjk.org.cn

Java: "第一行\n第二行"
来源：http://cvj.epnwcf.com

Go:   "第一行\n第二行"
来源：http://qnp.nanxuanxn.top

Ruby: "第一行\n第二行"
来源：http://ogz.iojbl.cn

C#:   "第一行\n第二行"
来源：http://pzw.sjlbkw.cn

[A14] 注释写法
来源：http://iey.redwolf501.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ksw.ywan-chungtsiang.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://zgw.zhixingplan.top

JS:   // 单行；/* 多行 */
来源：http://buk.mhx1999.top

TS:   // 单行；/* 多行 */
来源：http://fws.yuanzhike.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nrl.sweek.top

Go:   // 单行；/* 多行 */
来源：http://lur.aibaodan.cn

Ruby: # 单行；=begin 多行 =end
来源：http://gup.chenzaomai.com

C#:   // 单行；/* 多行 */
来源：http://qkr.pycfn.com

[A15] 空值判断与默认值
来源：http://lli.hammf.cn

Py:   value = data or "默认值"
来源：http://koh.zhiwuduotai.top

PHP:  $value = $data ?? "默认值";
来源：http://wbc.havefunace.top

JS:   const value = data ?? "默认值";
来源：http://rrr.havefunace.top

TS:   const value = data ?? "默认值";
来源：http://lby.shanyushiyangtech.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bbe.fanxiaobao.xyz

Go:   if data == "" { data = "默认值" }
来源：http://gmu.yangfankeji.com

Ruby: value = data || "默认值"
来源：http://xgo.smart0.xyz

C#:   var value = data ?? "默认值";
来源：http://uzc.shanyushiyangtech.top

[A16] 真假值判断规则
来源：http://xlj.havefunace.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mdn.hnqzz.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zzs.fktsv.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ttp.shanyushiyangtech.top

TS:   if (!x) {}
来源：http://som.yuxming.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://twx.kuanghao11.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xig.jqgfzy.top

Ruby: unless x            # nil 与 false 为假
来源：http://cul.epnwcf.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ria.pengpengdd.cyou

[A17] 位运算
来源：http://juq.aibaodan.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dmf.wangshuangyany.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://irl.birdmap.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://twg.zhengqikj.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qsi.jqgufenzy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zso.ywan-chungtsiang.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zzs.zdqjudy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hga.hywenlv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://czn.yj202588.top

[A18] 字符与 ASCII 码互转
来源：http://tun.sjlbkw.cn

Py:   ord("A"); chr(65)
来源：http://pct.hfpthk.cn

PHP:  ord("A"); chr(65)
来源：http://xcy.hongshengwenyu.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ina.nanxinkj.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://beo.birdmap.top

Java: (int) 'A'; (char) 65
来源：http://sen.jlsjyb.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nnl.bbcook.cn

Ruby: "A".ord; 65.chr
来源：http://xja.tianlin.xyz

C#:   (int)'A'; (char)65
来源：http://jwy.9152youxi.cn

[A19] 交换两个变量
来源：http://lvp.yonumen.top

Py:   a, b = b, a
来源：http://jun.aibaodan.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ajq.meibo888.top

JS:   [a, b] = [b, a];
来源：http://ujd.yongpay.top

TS:   [a, b] = [b, a];
来源：http://oxq.sufxvd.cn

Java: int t = a; a = b; b = t;
来源：http://tlu.shangyingyoupin.top

Go:   a, b = b, a
来源：http://qst.sweek.top

Ruby: a, b = b, a
来源：http://uvj.yuanzhike.top

C#:   (a, b) = (b, a);
来源：http://rcq.bjfxy.top

[A20] 读取标准输入
来源：http://hlo.vqdsnc.cn

Py:   name = input("请输入：")
来源：http://enp.shangyingyoupin.top

PHP:  $name = trim(fgets(STDIN));
来源：http://neu.zhongyouzk.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wbz.smart0.xyz

TS:   // Node.js：readline 模块
来源：http://mwr.cashguo.top

Java: new Scanner(System.in).nextLine()
来源：http://hxc.zhoulong.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://epy.xingfuxueyuan.xyz

Ruby: gets.chomp
来源：http://ifw.jiagoushi.top

C#:   Console.ReadLine();
来源：http://eoy.vqdsnc.cn

[A21] 保留指定小数位输出
来源：http://tzk.bjfxy.top

Py:   f"{3.14159:.2f}"
来源：http://gum.hcnkem.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://aro.zycfv.cn

JS:   (3.14159).toFixed(2)
来源：http://lnz.fzhhl.top

TS:   (3.14159).toFixed(2)
来源：http://wsv.shzxlz.cn

Java: String.format("%.2f", 3.14159)
来源：http://zbc.tianlin.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qgt.guowangkeji.top

Ruby: format("%.2f", 3.14159)
来源：http://lyh.zhaomingkeji.xyz

C#:   3.14159.ToString("F2")
来源：http://fod.daria6918.cn

[A22] 获取字符串长度
来源：http://dcg.cqqwz.cn

Py:   len(s)
来源：http://efw.yuxming.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gvb.andypj.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://akh.jyoumei.cn

TS:   s.length
来源：http://xur.aibaodan.cn

Java: s.length()
来源：http://vqc.wangshuangyany.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zxj.haohaochexian.top

Ruby: s.length
来源：http://bgv.yfazqb.com

C#:   s.Length
来源：http://qcn.hesvh.cn

[A23] 大小写转换
来源：http://kgr.gotoacloud.top

Py:   s.upper(); s.lower(); s.title()
来源：http://bme.pengpengdd.cyou

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rvg.smart0.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ssh.yj202588.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://upn.uphjek.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qci.tarul.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://uzb.pycfn.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pcd.redwolf501.top

C#:   s.ToUpper(); s.ToLower()
来源：http://xkc.jinqigfzy.top

[A24] 去除首尾空白
来源：http://due.tianlin.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cvv.jqgufenzy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nez.ybcxt.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ivq.iojbl.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rqp.jinghuilouyu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ekt.hfpthk.cn

Go:   strings.TrimSpace(s)
来源：http://ebz.chenjidiqi.icu

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ghp.ivvv.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wrf.52xcode.cn

[A25] 字符串比较
来源：http://ogx.tanke756.top

Py:   s1 == s2; s1 != s2
来源：http://wsr.sweek.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://yyg.sysykeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://oyy.dianchejie.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://eje.tarul.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cax.yj202588.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://eho.yj20258.top

Ruby: s1 == s2; s1 <=> s2
来源：http://jmh.gogol.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ysn.xuetiantiany.cn

[A26] 类型转换总览
来源：http://kcn.ehwqpu.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://rke.redwolf501.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kkm.ctjpmb.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://itm.bjfxy.top

TS:   Number() String() Boolean() x as number
来源：http://kvn.ywan-chungtsiang.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rxn.yonumen.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zrp.yj20258888.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ywm.chenlongwang.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fec.ydzc1.top

================================================================================
来源：http://wts.pycfn.com

B. 流程控制
来源：http://baa.nanxuanxn.top

================================================================================
来源：http://lqt.jinyuanbaomall.cn

[B01] 条件判断 if / else
来源：http://ebr.ydzc1.top

Py:   result = "正" if x > 0 else "非正"
来源：http://hql.pycfn.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://erp.shuidangran.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lum.shanyushiyangkeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fdd.c1oappe.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://hrz.guowangkeji.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gjt.bjfxy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oyn.bbcook.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ixq.yanxiufei.cn

[B02] 多分支 else if / elif
来源：http://rpr.tarul.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qqj.guannengcc.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://jsp.tanke756.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fwh.c1oappe.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rkc.haohaochexian.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lys.shanyushiyangkeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qej.wangdashe.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rcu.fzhhl.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ral.yonumen.top

[B03] switch / match / case
来源：http://bse.svipenyu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ooo.zhengqikj.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ukl.gogol.net.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mqp.redwolf501.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bpv.zhixingplan.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://enh.ydzc1.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zck.shangyingyoupin.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uck.cashguo.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://izq.fengsongda.top

[B04] for 计数循环
来源：http://vqq.ydzc1.top

Py:   for i in range(10): print(i)
来源：http://gdm.aizwys.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rrv.hcnkem.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tks.yuxming.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ohm.gaohongyu789.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sdz.aibaodan.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://the.nanxuanxn.top

Ruby: 10.times { |i| puts i }
来源：http://wat.guannengcc.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://twe.yvedp.cn

[B05] 遍历数组 / 列表
来源：http://elg.tianlin.xyz

Py:   for item in arr: print(item)
来源：http://pnw.fehbvm.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://oqb.yonumen.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ops.52xcode.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://hzh.svipenyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://xth.yangfankeji.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ese.52xcode.cn

Ruby: arr.each { |item| puts item }
来源：http://utp.yfazqb.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mdo.hcnkem.com

[B06] 遍历字典 / 对象
来源：http://ssf.jinqigfzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://gcz.vehdjk.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xfw.jlsjyb.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jop.jqgfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cxx.fktsv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ini.uphjek.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fod.xinyue.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lde.bbcook.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fer.havefunace.top

[B07] while 循环
来源：http://ckv.feifeiyinyue.top

Py:   while i < 10: i += 1
来源：http://vzm.meibo888.top

PHP:  while ($i < 10) { $i++; }
来源：http://vtj.hnqzz.top

JS:   while (i < 10) { i++; }
来源：http://nqy.xuetiantiany.cn

TS:   while (i < 10) { i++; }
来源：http://dxs.ctjpmb.com

Java: while (i < 10) { i++; }
来源：http://nom.chenlongwang.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qkb.gotoacloud.top

Ruby: while i < 10; i += 1; end
来源：http://txd.ivvv.top

C#:   while (i < 10) { i++; }
来源：http://gzc.jlsjyb.cn

[B08] do-while（至少执行一次）
来源：http://ddc.yj20258888.top

Py:   # 无 do-while：用 while True + break
来源：http://svx.yj20258.top

PHP:  do { $i++; } while ($i < 10);
来源：http://sks.jianghu66.top

JS:   do { i++; } while (i < 10);
来源：http://klc.birdmap.top

TS:   do { i++; } while (i < 10);
来源：http://pap.shangyingyoupin.top

Java: do { i++; } while (i < 10);
来源：http://zmz.316326.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://ivj.bjfxy.top

Ruby: begin; i += 1; end while i < 10
来源：http://lig.hnxiangtu.top

C#:   do { i++; } while (i < 10);
来源：http://vfh.bjfxy.top

[B09] break 与 continue
来源：http://nza.wangshuangyany.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lkr.zhengqikj.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hvy.mhx1999.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ckx.shangyingyoupin.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://grg.feifeiyinyue.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://okl.xuanzx.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://aim.smart0.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hic.wangdashe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tuj.hongshengwenyu.top

[B10] 遍历同时拿索引
来源：http://zzq.hammf.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bdy.zdqjudy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pci.daxiang520.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hrg.ywan-chungtsiang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mfx.jinqigufen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jgu.fktsv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zni.wangshuangyany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tbh.yangfankeji.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pld.haohaochexian.top

[B11] 生成数字序列 / 区间
来源：http://upb.yj202588.top

Py:   list(range(0, 10, 2))
来源：http://mlu.jqgufenzy.top

PHP:  range(0, 10, 2);
来源：http://baw.ctjpmb.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wpz.tian-w.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://srz.svipenyu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://odj.zhengqikj.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://olw.bbcook.cn

Ruby: (0...10).step(2).to_a
来源：http://ynl.sjlbkw.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://epn.dianchejie.cn

[B12] 跳出多层循环
来源：http://vfr.chenjidiqi.icu

Py:   # 无标签跳转：抽成函数用 return
来源：http://lph.ctjpmb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://ekz.fehbvm.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cqn.pycfn.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jwx.nanxinkj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mxz.yonumen.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nwy.c1oappe.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tjv.jyoumei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dmq.cqqwz.cn

[B13] 判断是否为数字
来源：http://gdo.tarul.cn

Py:   isinstance(x, (int, float))
来源：http://mcs.ivvv.top

PHP:  is_numeric($x)
来源：http://zar.hammf.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hbh.chenjidiqi.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lvn.fengsongda.top

Java: x instanceof Number
来源：http://rzp.hesvh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://etx.uphjek.com

Ruby: x.is_a?(Numeric)
来源：http://snu.zycfv.cn

C#:   x is int or double or decimal
来源：http://sgo.yuxming.cn

[B14] 判断值是否在集合内
来源：http://gvv.jinqigfzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vae.xingfuxueyuan.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kya.redwolf501.top

JS:   [1, 2, 3].includes(x)
来源：http://ves.tianlin.xyz

TS:   [1, 2, 3].includes(x)
来源：http://zbk.ppjwa.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ens.hysaishi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bzw.ivvv.top

Ruby: [1, 2, 3].include?(x)
来源：http://cvw.quarkkingdee.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zkw.guowangkeji.top

[B15] 布尔运算与取反
来源：http://enk.epnwcf.com

Py:   a and b or not c
来源：http://pwa.ywan-chungtsiang.top

PHP:  $a && $b || !$c
来源：http://ees.ehwqpu.com

JS:   a && b || !c
来源：http://rxv.xziqi.cn

TS:   a && b || !c
来源：http://wdn.uphjek.com

Java: a && b || !c
来源：http://zis.hfpthk.cn

Go:   a && b || !c
来源：http://ewa.tanke756.top

Ruby: a && b || !c
来源：http://lgo.tian-w.cn

C#:   a && b || !c
来源：http://lda.aizwys.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dof.guannengcc.top

Py:   if not data: return
来源：http://kzn.316326.xyz

PHP:  if (!$data) { return; }
来源：http://jhc.zhiwuduotai.top

JS:   if (!data) return;
来源：http://qdi.iojbl.cn

TS:   if (!data) return;
来源：http://axz.pycfn.com

Java: if (data == null) return;
来源：http://xro.zhengqikj.top

Go:   if data == nil { return }
来源：http://rnw.hongshengwenyu.top

Ruby: return if data.nil?
来源：http://pax.zdbjq.cn

C#:   if (data == null) return;
来源：http://gky.52xcode.cn


<!-- 参考信息 -->