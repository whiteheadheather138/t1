代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://skj.yj202588.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://elq.chenzaomai.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://xay.yuxming.cn

[A09] 绝对值与最大最小值
来源：http://ydl.svipenyu.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pdk.tarul.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xpo.redwolf501.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vcn.c1oappe.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tju.tarul.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wbo.cucudq.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gqn.jqgfzy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ovg.feifeiyinyue.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xxf.yfazqb.com

[A10] 生成随机数
来源：http://zez.zhoulong.xyz

Py:   import random; random.randint(1, 100)
来源：http://nbx.xziqi.cn

PHP:  random_int(1, 100);
来源：http://tvc.chenzaomai.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://khz.xuetiantiany.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://njv.mhx1999.top

Java: new Random().nextInt(100) + 1
来源：http://inu.hfpthk.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cyi.hysaishi.cn

Ruby: rand(1..100)
来源：http://kpi.wangdashe.top

C#:   new Random().Next(1, 101)
来源：http://gjg.hcnkem.com

[A11] 条件表达式（三元）
来源：http://clt.zhixingplan.top

Py:   "yes" if x > 0 else "no"
来源：http://gkn.hesvh.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://rxy.cheryme.top

JS:   x > 0 ? "yes" : "no"
来源：http://hga.birdmap.top

TS:   x > 0 ? "yes" : "no"
来源：http://ews.dianchejie.cn

Java: x > 0 ? "yes" : "no"
来源：http://ard.birdmap.top

Go:   // 无三元运算符，需用 if 语句
来源：http://fby.chenzaomai.com

Ruby: x > 0 ? "yes" : "no"
来源：http://zpi.jianghu66.top

C#:   x > 0 ? "yes" : "no"
来源：http://xwo.yfazqb.com

[A12] 字符串插值 / 格式化
来源：http://mlj.zhoulong.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://itx.shanyushiyangkeji.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://kat.yongpay.top

JS:   `Hello, ${name}!`
来源：http://vzq.meibo888.top

TS:   `Hello, ${name}!`
来源：http://vwu.fzhhl.top

Java: "Hello, %s!".formatted(name)
来源：http://pag.havefunace.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gar.cucudq.cn

Ruby: "Hello, #{name}!"
来源：http://pys.sweek.top

C#:   $"Hello, {name}!"
来源：http://tej.hongshengwenyu.top

[A13] 多行字符串（练习 \n 转义）
来源：http://wtn.ehwqpu.com

Py:   "第一行\n第二行"
来源：http://xmt.yfazqb.com

PHP:  "第一行\n第二行"
来源：http://ydm.birdmap.top

JS:   "第一行\n第二行"
来源：http://awd.hysaishi.cn

TS:   "第一行\n第二行"
来源：http://tyo.dianchejie.cn

Java: "第一行\n第二行"
来源：http://imq.chenzaomai.com

Go:   "第一行\n第二行"
来源：http://rqo.hnqzz.top

Ruby: "第一行\n第二行"
来源：http://uvc.zhixingplan.top

C#:   "第一行\n第二行"
来源：http://fyg.wangshuangyany.cn

[A14] 注释写法
来源：http://ibf.daria6918.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://tin.jinghuilouyu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://byz.mhx1999.top

JS:   // 单行；/* 多行 */
来源：http://amc.jianghu66.top

TS:   // 单行；/* 多行 */
来源：http://fot.bjfxy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://nom.yongpay.top

Go:   // 单行；/* 多行 */
来源：http://gdu.fzhhl.top

Ruby: # 单行；=begin 多行 =end
来源：http://tie.shanyushiyangtech.top

C#:   // 单行；/* 多行 */
来源：http://tab.hnxiangtu.top

[A15] 空值判断与默认值
来源：http://bya.ydzc1.top

Py:   value = data or "默认值"
来源：http://jbp.jianghu66.top

PHP:  $value = $data ?? "默认值";
来源：http://iag.daxiang520.top

JS:   const value = data ?? "默认值";
来源：http://epp.fktsv.cn

TS:   const value = data ?? "默认值";
来源：http://jci.sxryk.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ejb.yuanzhike.top

Go:   if data == "" { data = "默认值" }
来源：http://vnp.ppjwa.cn

Ruby: value = data || "默认值"
来源：http://tts.chenzaomai.com

C#:   var value = data ?? "默认值";
来源：http://ksy.xziqi.cn

[A16] 真假值判断规则
来源：http://izl.hnqzz.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ynh.hfpthk.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xyd.xziqi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sae.feifeiyinyue.top

TS:   if (!x) {}
来源：http://xyl.hywenlv.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wsp.havefunace.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://jxa.9152youxi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gpr.guowangkeji.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pqc.hcnkem.com

[A17] 位运算
来源：http://bcs.guowangkeji.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qzu.zhoulong.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fpo.yj20258.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://snl.jinqigufen.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gaa.jyoumei.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gex.sweek.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jsy.jinqigfzy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xuo.fanxiaobao.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qrm.zdqjudy.top

[A18] 字符与 ASCII 码互转
来源：http://qlj.jinqigufen.top

Py:   ord("A"); chr(65)
来源：http://xnr.jqgfzy.top

PHP:  ord("A"); chr(65)
来源：http://ifh.xziqi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jls.ybcxt.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://klh.cqqwz.cn

Java: (int) 'A'; (char) 65
来源：http://myn.yvedp.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ddm.ywan-chungtsiang.top

Ruby: "A".ord; 65.chr
来源：http://wlc.xingfuxueyuan.xyz

C#:   (int)'A'; (char)65
来源：http://zfx.yonumen.top

[A19] 交换两个变量
来源：http://aye.birdmap.top

Py:   a, b = b, a
来源：http://kel.redwolf501.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ahd.gaohongyu789.top

JS:   [a, b] = [b, a];
来源：http://uno.zhongyouzk.top

TS:   [a, b] = [b, a];
来源：http://aby.zhixingplan.top

Java: int t = a; a = b; b = t;
来源：http://lnb.sjlbkw.cn

Go:   a, b = b, a
来源：http://oaq.sjlbkw.cn

Ruby: a, b = b, a
来源：http://hmz.aizwys.cn

C#:   (a, b) = (b, a);
来源：http://zny.hnqzz.top

[A20] 读取标准输入
来源：http://nak.pycfn.com

Py:   name = input("请输入：")
来源：http://xgi.wangshuangyany.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://sjm.cheryme.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://eah.sufxvd.cn

TS:   // Node.js：readline 模块
来源：http://cod.jlsjyb.cn

Java: new Scanner(System.in).nextLine()
来源：http://lra.sxryk.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ogk.ctjpmb.com

Ruby: gets.chomp
来源：http://rgb.ydzc1.top

C#:   Console.ReadLine();
来源：http://wst.feifeiyinyue.top

[A21] 保留指定小数位输出
来源：http://xam.ydzc1.top

Py:   f"{3.14159:.2f}"
来源：http://nit.fanxiaobao.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hgk.ppjwa.cn

JS:   (3.14159).toFixed(2)
来源：http://fpp.shangyingyoupin.top

TS:   (3.14159).toFixed(2)
来源：http://lou.gzhubu.top

Java: String.format("%.2f", 3.14159)
来源：http://bon.yanxiufei.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xtr.sjlbkw.cn

Ruby: format("%.2f", 3.14159)
来源：http://zeq.vqdsnc.cn

C#:   3.14159.ToString("F2")
来源：http://icu.nwbrower.top

[A22] 获取字符串长度
来源：http://jmd.ivvv.top

Py:   len(s)
来源：http://tch.jinyuanbaomall.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mgs.nwbrower.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dud.sjlbkw.cn

TS:   s.length
来源：http://odv.gaohongyu789.top

Java: s.length()
来源：http://otw.havefunace.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mcz.pengpengdd.cyou

Ruby: s.length
来源：http://ods.fehbvm.com

C#:   s.Length
来源：http://pqk.zhoulong.xyz

[A23] 大小写转换
来源：http://pro.tarul.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://syv.ivvv.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mao.hysaishi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ues.fehbvm.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://svq.cashguo.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dwi.nanxuanxn.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://box.yfazqb.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cis.cdnleiting.top

C#:   s.ToUpper(); s.ToLower()
来源：http://miq.shangyingyoupin.top

[A24] 去除首尾空白
来源：http://ffl.redwolf501.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lbj.wangshuangyany.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bvv.xingfuxueyuan.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://asl.9152youxi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eck.xuetiantiany.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wod.zhengqikj.top

Go:   strings.TrimSpace(s)
来源：http://yur.tian-w.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hqn.ydjk.org.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jxt.jianghu66.top

[A25] 字符串比较
来源：http://cpq.mhx1999.top

Py:   s1 == s2; s1 != s2
来源：http://zym.cashguo.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lcy.hnxiangtu.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://glj.haohaochexian.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ttq.zhoulong.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sbh.hnxiangtu.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://iyn.guowangkeji.top

Ruby: s1 == s2; s1 <=> s2
来源：http://nqi.nanxuanxn.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fyf.chenlongwang.top

[A26] 类型转换总览
来源：http://hwu.hysaishi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qkj.shanyushiyangkeji.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qiu.zhijiandao.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://geb.yj20258888.top

TS:   Number() String() Boolean() x as number
来源：http://ehb.zhixingplan.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://geo.jqgfzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yww.gaohongyu789.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://lyl.nanxinkj.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fwb.vehdjk.com

================================================================================
来源：http://siw.chenzaomai.com

B. 流程控制
来源：http://kzl.feifeiyinyue.top

================================================================================
来源：http://kvu.quarkkingdee.top

[B01] 条件判断 if / else
来源：http://kcq.fanxiaobao.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://xkd.guowangkeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kvn.yj20258.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cpr.316326.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tld.bbcook.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ydo.jinyuanbaomall.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rqd.meibo888.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mxx.havefunace.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qqu.pengpengdd.cyou

[B02] 多分支 else if / elif
来源：http://mve.tarul.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vak.fktsv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zax.yanxiufei.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hvf.chenjidiqi.icu

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bxl.dianchejie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dpw.zhongyouzk.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hsi.ctjpmb.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xki.zdqjudy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://noq.haohaochexian.top

[B03] switch / match / case
来源：http://aqd.tarul.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nwf.aibaodan.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ekm.shanyushiyangtech.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://frt.redwolf501.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dpz.hongshengwenyu.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://azb.xuetiantiany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jcv.mhx1999.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nfb.hongshengwenyu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vsz.cashguo.top

[B04] for 计数循环
来源：http://wuh.ydzc1.top

Py:   for i in range(10): print(i)
来源：http://bta.chenjidiqi.icu

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://muv.fehbvm.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qgk.jyoumei.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://npl.vehdjk.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gva.gaohongyu789.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mhq.iojbl.cn

Ruby: 10.times { |i| puts i }
来源：http://fnv.quarkkingdee.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fjg.jqgfzy.top

[B05] 遍历数组 / 列表
来源：http://wet.sweek.top

Py:   for item in arr: print(item)
来源：http://jam.xylfe.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://shl.jlsjyb.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://zma.yuanzhike.top

TS:   for (const item of arr) { console.log(item); }
来源：http://zjq.gzhubu.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://vfe.fanxiaobao.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kwx.yvedp.cn

Ruby: arr.each { |item| puts item }
来源：http://bey.xuanzx.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://btw.cqqwz.cn

[B06] 遍历字典 / 对象
来源：http://lpv.fktsv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rip.feifeiyinyue.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mje.jiagoushi.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zam.gzhubu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://puc.xuanzx.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://esj.uphjek.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ibs.yongpay.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://enq.vqdsnc.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://joc.zhoulong.xyz

[B07] while 循环
来源：http://ceg.fktsv.cn

Py:   while i < 10: i += 1
来源：http://pma.9152youxi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dge.zhongyouzk.top

JS:   while (i < 10) { i++; }
来源：http://dvz.daria6918.cn

TS:   while (i < 10) { i++; }
来源：http://wdo.tianlin.xyz

Java: while (i < 10) { i++; }
来源：http://dfg.jqgufenzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zto.fehbvm.com

Ruby: while i < 10; i += 1; end
来源：http://iyy.yongpay.top

C#:   while (i < 10) { i++; }
来源：http://uqs.vehdjk.com

[B08] do-while（至少执行一次）
来源：http://ytw.quarkkingdee.top

Py:   # 无 do-while：用 while True + break
来源：http://jap.hcnkem.com

PHP:  do { $i++; } while ($i < 10);
来源：http://lkh.pengpengdd.cyou

JS:   do { i++; } while (i < 10);
来源：http://bee.shanyushiyangkeji.top

TS:   do { i++; } while (i < 10);
来源：http://zan.fehbvm.com

Java: do { i++; } while (i < 10);
来源：http://ptc.tian-w.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dvj.hnqzz.top

Ruby: begin; i += 1; end while i < 10
来源：http://imj.gogol.net.cn

C#:   do { i++; } while (i < 10);
来源：http://ydm.xuanzx.com

[B09] break 与 continue
来源：http://bme.dashuyun.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mnx.aibaodan.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qeu.guowangkeji.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blz.jinqigfzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://adm.aibaodan.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zku.aibaodan.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ego.ybcxt.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ibo.dianchejie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ecj.aibaodan.cn

[B10] 遍历同时拿索引
来源：http://nqg.52xcode.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qvi.yangfankeji.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qtx.yongpay.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wxf.svipenyu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nnd.tanke756.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://drl.chenzaomai.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rns.hfpthk.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tbf.xuetiantiany.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qmf.316326.xyz

[B11] 生成数字序列 / 区间
来源：http://npe.cdnleiting.top

Py:   list(range(0, 10, 2))
来源：http://hnh.wangshuangyany.cn

PHP:  range(0, 10, 2);
来源：http://rpz.xinyue.icu

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fyh.hongshengwenyu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aei.zdqjudy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://srp.hnqzz.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kab.shangyingyoupin.top

Ruby: (0...10).step(2).to_a
来源：http://jfq.dashuyun.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rur.epnwcf.com

[B12] 跳出多层循环
来源：http://nmx.zhixingplan.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://oty.jinqigfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://zlo.sysykeji.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jyw.cucudq.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kpa.yonumen.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://eyq.birdmap.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://leh.wangdashe.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fdt.ctjpmb.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rhl.hesvh.cn

[B13] 判断是否为数字
来源：http://wqn.mhx1999.top

Py:   isinstance(x, (int, float))
来源：http://yiu.shuidangran.top

PHP:  is_numeric($x)
来源：http://tbw.zhongyouzk.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bop.hnqzz.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zya.jinqigufen.top

Java: x instanceof Number
来源：http://nli.ydzc1.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xbj.hysaishi.cn

Ruby: x.is_a?(Numeric)
来源：http://qoe.chenlongwang.top

C#:   x is int or double or decimal
来源：http://qeg.bbcook.cn

[B14] 判断值是否在集合内
来源：http://wfc.haohaochexian.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://aox.zhijiandao.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://axw.hfpthk.cn

JS:   [1, 2, 3].includes(x)
来源：http://sgy.gotoacloud.top

TS:   [1, 2, 3].includes(x)
来源：http://wci.ehwqpu.com

Java: List.of(1, 2, 3).contains(x)
来源：http://ygc.52xcode.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nzd.hysaishi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sjj.fengsongda.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yjw.dashuyun.cn

[B15] 布尔运算与取反
来源：http://ogc.aizwys.cn

Py:   a and b or not c
来源：http://hye.jinqigufen.top

PHP:  $a && $b || !$c
来源：http://ghb.ybcxt.top

JS:   a && b || !c
来源：http://fsr.pengpengdd.cyou

TS:   a && b || !c
来源：http://mlv.sweek.top

Java: a && b || !c
来源：http://xbv.sjlbkw.cn


<!-- 参考信息 -->