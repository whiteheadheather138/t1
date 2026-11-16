代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://oxz.jyoumei.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://axr.zhengqikj.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ern.quarkkingdee.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://uqg.9152youxi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ssh.snrcjt.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://yvp.ywan-chungtsiang.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qyl.shanyushiyangkeji.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dxu.uphjek.com

[A10] 生成随机数
来源：http://apo.nanxinkj.top

Py:   import random; random.randint(1, 100)
来源：http://obc.gaohongyu789.top

PHP:  random_int(1, 100);
来源：http://qrz.smart0.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lck.zycfv.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dds.epnwcf.com

Java: new Random().nextInt(100) + 1
来源：http://pal.cucudq.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vwz.dianchejie.cn

Ruby: rand(1..100)
来源：http://zct.uphjek.com

C#:   new Random().Next(1, 101)
来源：http://vpu.bbcook.cn

[A11] 条件表达式（三元）
来源：http://gyd.cqqwz.cn

Py:   "yes" if x > 0 else "no"
来源：http://sgs.sufxvd.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://qkr.aizwys.cn

JS:   x > 0 ? "yes" : "no"
来源：http://hva.nwbrower.top

TS:   x > 0 ? "yes" : "no"
来源：http://riv.316326.xyz

Java: x > 0 ? "yes" : "no"
来源：http://sgn.fktsv.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://klp.andypj.xyz

Ruby: x > 0 ? "yes" : "no"
来源：http://vls.yj202588.top

C#:   x > 0 ? "yes" : "no"
来源：http://tqk.xinyue.icu

[A12] 字符串插值 / 格式化
来源：http://rfd.ywan-chungtsiang.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kop.316326.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wwd.nwbrower.top

JS:   `Hello, ${name}!`
来源：http://rol.ehwqpu.com

TS:   `Hello, ${name}!`
来源：http://bdt.haohaochexian.top

Java: "Hello, %s!".formatted(name)
来源：http://ggf.52xcode.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://cje.fzhhl.top

Ruby: "Hello, #{name}!"
来源：http://xex.wangshuangyany.cn

C#:   $"Hello, {name}!"
来源：http://uuh.sysykeji.top

[A13] 多行字符串（练习 \n 转义）
来源：http://lgo.ctjpmb.com

Py:   "第一行\n第二行"
来源：http://sni.mhx1999.top

PHP:  "第一行\n第二行"
来源：http://fsg.zdqjudy.top

JS:   "第一行\n第二行"
来源：http://aiq.guowangkeji.top

TS:   "第一行\n第二行"
来源：http://wox.gzhubu.top

Java: "第一行\n第二行"
来源：http://jny.epnwcf.com

Go:   "第一行\n第二行"
来源：http://hnn.fengsongda.top

Ruby: "第一行\n第二行"
来源：http://tkj.gzhubu.top

C#:   "第一行\n第二行"
来源：http://gzg.zhongyouzk.top

[A14] 注释写法
来源：http://fvw.nanxinkj.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://muq.jlsjyb.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://quk.sweek.top

JS:   // 单行；/* 多行 */
来源：http://eow.yj20258.top

TS:   // 单行；/* 多行 */
来源：http://uuu.xuetiantiany.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fmm.dianchejie.cn

Go:   // 单行；/* 多行 */
来源：http://gmf.yuanzhike.top

Ruby: # 单行；=begin 多行 =end
来源：http://wuh.mhx1999.top

C#:   // 单行；/* 多行 */
来源：http://onz.uphjek.com

[A15] 空值判断与默认值
来源：http://zyd.jinqigufen.top

Py:   value = data or "默认值"
来源：http://njc.xziqi.cn

PHP:  $value = $data ?? "默认值";
来源：http://zql.jinghuilouyu.cn

JS:   const value = data ?? "默认值";
来源：http://xkd.daxiang520.top

TS:   const value = data ?? "默认值";
来源：http://trp.wangdashe.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jqm.0kj1m.cn

Go:   if data == "" { data = "默认值" }
来源：http://xvl.zycfv.cn

Ruby: value = data || "默认值"
来源：http://tdr.nwbrower.top

C#:   var value = data ?? "默认值";
来源：http://ifh.gaohongyu789.top

[A16] 真假值判断规则
来源：http://den.fanxiaobao.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ggl.chenzaomai.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ipz.sxryk.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xwe.zhaomingkeji.xyz

TS:   if (!x) {}
来源：http://cnr.jlsjyb.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://inq.xziqi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hqv.fehbvm.com

Ruby: unless x            # nil 与 false 为假
来源：http://rlo.yuanzhike.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://otg.xziqi.cn

[A17] 位运算
来源：http://qkd.nanxuanxn.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://icp.aizwys.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wuu.havefunace.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vjc.hammf.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nle.pycfn.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cyd.tarul.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://duy.xinyue.icu

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://shh.tanke756.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wyk.zdqjudy.top

[A18] 字符与 ASCII 码互转
来源：http://ezq.pycfn.com

Py:   ord("A"); chr(65)
来源：http://vea.kuanghao11.cn

PHP:  ord("A"); chr(65)
来源：http://lbm.hywenlv.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://djn.xziqi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ifv.gotoacloud.top

Java: (int) 'A'; (char) 65
来源：http://zsl.jlsjyb.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://drm.nanxinkj.top

Ruby: "A".ord; 65.chr
来源：http://wir.iojbl.cn

C#:   (int)'A'; (char)65
来源：http://men.zhongyouzk.top

[A19] 交换两个变量
来源：http://ekg.pengpengdd.cyou

Py:   a, b = b, a
来源：http://xbv.xuetiantiany.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ovk.fehbvm.com

JS:   [a, b] = [b, a];
来源：http://cnr.sufxvd.cn

TS:   [a, b] = [b, a];
来源：http://hcp.zdqjudy.top

Java: int t = a; a = b; b = t;
来源：http://itr.jinqigfzy.top

Go:   a, b = b, a
来源：http://fcr.tian-w.cn

Ruby: a, b = b, a
来源：http://vgz.vqdsnc.cn

C#:   (a, b) = (b, a);
来源：http://ztn.havefunace.top

[A20] 读取标准输入
来源：http://cwf.ivvv.top

Py:   name = input("请输入：")
来源：http://aem.kuanghao11.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xft.cdnleiting.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nmt.yueranfly.top

TS:   // Node.js：readline 模块
来源：http://nqj.hysaishi.cn

Java: new Scanner(System.in).nextLine()
来源：http://pjc.mhx1999.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vam.fanxiaobao.xyz

Ruby: gets.chomp
来源：http://hrw.tanke756.top

C#:   Console.ReadLine();
来源：http://pbo.zhoulong.xyz

[A21] 保留指定小数位输出
来源：http://rkh.hywenlv.cn

Py:   f"{3.14159:.2f}"
来源：http://mnc.xinyue.icu

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qwq.c1oappe.top

JS:   (3.14159).toFixed(2)
来源：http://idb.epnwcf.com

TS:   (3.14159).toFixed(2)
来源：http://xwj.zhiwuduotai.top

Java: String.format("%.2f", 3.14159)
来源：http://bjh.zhixingplan.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hbr.fengsongda.top

Ruby: format("%.2f", 3.14159)
来源：http://kpj.andypj.xyz

C#:   3.14159.ToString("F2")
来源：http://oyf.shuidangran.top

[A22] 获取字符串长度
来源：http://ktv.chenlongwang.top

Py:   len(s)
来源：http://ltp.shzxlz.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://iff.zhoulong.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qzo.jyoumei.cn

TS:   s.length
来源：http://wyr.hcnkem.com

Java: s.length()
来源：http://chu.tianlin.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jtu.zhoulong.xyz

Ruby: s.length
来源：http://vlo.gogol.net.cn

C#:   s.Length
来源：http://ait.ydjk.org.cn

[A23] 大小写转换
来源：http://cxv.jyoumei.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rpf.52xcode.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ixi.chenzaomai.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://igt.jianghu66.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://kpi.dianchejie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bos.zhongyouzk.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bwg.cdnleiting.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mnu.nwbrower.top

C#:   s.ToUpper(); s.ToLower()
来源：http://job.svipenyu.cn

[A24] 去除首尾空白
来源：http://fuo.shzxlz.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://uyl.fzhhl.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jgr.bbcook.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wtg.quarkkingdee.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://inz.quarkkingdee.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qhu.gzhubu.top

Go:   strings.TrimSpace(s)
来源：http://uwl.bbcook.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bdb.hnxiangtu.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rac.hcnkem.com

[A25] 字符串比较
来源：http://wiq.jinqigfzy.top

Py:   s1 == s2; s1 != s2
来源：http://vjh.hfpthk.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ncp.uphjek.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lpc.wangdashe.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zud.smart0.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fnl.aibaodan.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cnk.tarul.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cyb.jiagoushi.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wtc.shangyingyoupin.top

[A26] 类型转换总览
来源：http://abe.yongpay.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fgu.tianlin.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hmt.pengpengdd.cyou

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fqe.iojbl.cn

TS:   Number() String() Boolean() x as number
来源：http://ltf.aibaodan.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ywp.jinqigufen.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wua.ppjwa.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rln.chenjidiqi.icu

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xyc.snrcjt.cn

================================================================================
来源：http://mfe.zhoulong.xyz

B. 流程控制
来源：http://ntv.ctjpmb.com

================================================================================
来源：http://gzl.nwbrower.top

[B01] 条件判断 if / else
来源：http://imk.yj202588.top

Py:   result = "正" if x > 0 else "非正"
来源：http://xoo.hnxiangtu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zke.fengsongda.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zvu.gotoacloud.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kct.meibo888.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://dgm.aizwys.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lhg.tanke756.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lzt.gotoacloud.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://eal.zhongyouzk.top

[B02] 多分支 else if / elif
来源：http://qro.dianchejie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://edn.c1oappe.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gcg.yvedp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qkp.sweek.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bzo.yanxiufei.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jjc.jinqigfzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ltd.zhijiandao.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://smx.jinqigfzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jsr.cashguo.top

[B03] switch / match / case
来源：http://ugy.redwolf501.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vyt.fengsongda.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zof.pycfn.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zyx.jinqigufen.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xsq.bbcook.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://twp.shangyingyoupin.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cue.jinyuanbaomall.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jxm.fanxiaobao.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ywz.0kj1m.cn

[B04] for 计数循环
来源：http://lbt.hfpthk.cn

Py:   for i in range(10): print(i)
来源：http://ust.birdmap.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vel.hongshengwenyu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mij.shanyushiyangtech.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://naf.bbcook.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mlj.yvedp.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fjw.smart0.xyz

Ruby: 10.times { |i| puts i }
来源：http://dws.fengsongda.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://bwf.aizwys.cn

[B05] 遍历数组 / 列表
来源：http://trd.aizwys.cn

Py:   for item in arr: print(item)
来源：http://bgv.ctjpmb.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mzp.yuxming.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://grx.shanyushiyangtech.top

TS:   for (const item of arr) { console.log(item); }
来源：http://bse.tanke756.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://vgj.shzxlz.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jdx.jyoumei.cn

Ruby: arr.each { |item| puts item }
来源：http://tnx.jianghu66.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wpw.zhixingplan.top

[B06] 遍历字典 / 对象
来源：http://bmp.zhoulong.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://seq.jinghuilouyu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lar.gaohongyu789.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fpe.ivvv.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yah.hcnkem.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://eht.shanyushiyangtech.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bpb.hcnkem.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ghu.0kj1m.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nhh.quarkkingdee.top

[B07] while 循环
来源：http://ykj.xziqi.cn

Py:   while i < 10: i += 1
来源：http://kmp.cqqwz.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hra.jinghuilouyu.cn

JS:   while (i < 10) { i++; }
来源：http://ocs.zhoulong.xyz

TS:   while (i < 10) { i++; }
来源：http://jsg.jqgufenzy.top

Java: while (i < 10) { i++; }
来源：http://qxv.yfazqb.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vfr.andypj.xyz

Ruby: while i < 10; i += 1; end
来源：http://idd.aizwys.cn

C#:   while (i < 10) { i++; }
来源：http://oek.shanyushiyangtech.top

[B08] do-while（至少执行一次）
来源：http://olh.daxiang520.top

Py:   # 无 do-while：用 while True + break
来源：http://dxc.nanxinkj.top

PHP:  do { $i++; } while ($i < 10);
来源：http://fxm.hongshengwenyu.top

JS:   do { i++; } while (i < 10);
来源：http://oye.zhongyouzk.top

TS:   do { i++; } while (i < 10);
来源：http://eeq.ivvv.top

Java: do { i++; } while (i < 10);
来源：http://ewg.tianlin.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://dde.sweek.top

Ruby: begin; i += 1; end while i < 10
来源：http://voh.vehdjk.com

C#:   do { i++; } while (i < 10);
来源：http://bka.gaohongyu789.top

[B09] break 与 continue
来源：http://nta.xziqi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wty.yonumen.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://izh.cqqwz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://apb.yongpay.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://snv.xuanzx.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://icx.gotoacloud.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bef.chenzaomai.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qzk.0kj1m.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://trd.zycfv.cn

[B10] 遍历同时拿索引
来源：http://zvt.tarul.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ulp.daria6918.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vol.ydzc1.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://seb.zhaomingkeji.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fzt.zhiwuduotai.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://juk.uphjek.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fqw.9152youxi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eew.xuetiantiany.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jms.yongpay.top

[B11] 生成数字序列 / 区间
来源：http://uja.cheryme.top

Py:   list(range(0, 10, 2))
来源：http://rmp.ydzc1.top

PHP:  range(0, 10, 2);
来源：http://jjv.yueranfly.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fhr.ivvv.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xxx.meibo888.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xbj.sxryk.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jvz.smart0.xyz

Ruby: (0...10).step(2).to_a
来源：http://zjd.aizwys.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rpi.yongpay.top

[B12] 跳出多层循环
来源：http://nze.shanyushiyangkeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://hkw.52xcode.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ulr.shanyushiyangtech.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sqa.zhaomingkeji.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ybq.aizwys.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://upy.daxiang520.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sne.zdqjudy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yew.tanke756.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wic.gzhubu.top

[B13] 判断是否为数字
来源：http://lpw.tian-w.cn

Py:   isinstance(x, (int, float))
来源：http://zbw.jyoumei.cn

PHP:  is_numeric($x)
来源：http://eea.kuanghao11.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dgz.aibaodan.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://maf.jinyuanbaomall.cn

Java: x instanceof Number
来源：http://wcy.ppjwa.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sco.shangyingyoupin.top

Ruby: x.is_a?(Numeric)
来源：http://sgp.feifeiyinyue.top

C#:   x is int or double or decimal
来源：http://fmu.hesvh.cn

[B14] 判断值是否在集合内
来源：http://ubf.sufxvd.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bhs.shuidangran.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jdq.haohaochexian.top

JS:   [1, 2, 3].includes(x)
来源：http://vza.xziqi.cn

TS:   [1, 2, 3].includes(x)
来源：http://wnz.yuxming.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sql.jiagoushi.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hkg.cashguo.top

Ruby: [1, 2, 3].include?(x)
来源：http://fdg.ctjpmb.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qwx.wangshuangyany.cn

[B15] 布尔运算与取反
来源：http://egz.xylfe.cn

Py:   a and b or not c
来源：http://kox.shanyushiyangkeji.top

PHP:  $a && $b || !$c
来源：http://ukx.zhengqikj.top

JS:   a && b || !c
来源：http://okd.guowangkeji.top

TS:   a && b || !c
来源：http://syc.haohaochexian.top

Java: a && b || !c
来源：http://hwn.hammf.cn

Go:   a && b || !c
来源：http://egr.yuanzhike.top

Ruby: a && b || !c
来源：http://zit.cashguo.top

C#:   a && b || !c
来源：http://qnn.xuanzx.com

[B16] 卫语句：不满足条件提前返回
来源：http://fop.zdbjq.cn


<!-- 参考信息 -->