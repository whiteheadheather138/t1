代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lej.daxiang520.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://toe.shzxlz.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vjh.shanyushiyangkeji.top

[A09] 绝对值与最大最小值
来源：http://yqq.haohaochexian.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jzj.sufxvd.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://exe.yfazqb.com

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rca.hesvh.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://owj.yj202588.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zol.ivvv.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ill.zycfv.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mra.hesvh.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://aix.dianchejie.cn

[A10] 生成随机数
来源：http://lfz.ppjwa.cn

Py:   import random; random.randint(1, 100)
来源：http://eqn.jiagoushi.top

PHP:  random_int(1, 100);
来源：http://cgf.hnxiangtu.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zhw.hesvh.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bow.zdbjq.cn

Java: new Random().nextInt(100) + 1
来源：http://dxx.tarul.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rgy.ivvv.top

Ruby: rand(1..100)
来源：http://cvo.epnwcf.com

C#:   new Random().Next(1, 101)
来源：http://tli.pycfn.com

[A11] 条件表达式（三元）
来源：http://uik.gogol.net.cn

Py:   "yes" if x > 0 else "no"
来源：http://iaw.xingfuxueyuan.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://nzd.xziqi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://pdp.yj202588.top

TS:   x > 0 ? "yes" : "no"
来源：http://pwb.tarul.cn

Java: x > 0 ? "yes" : "no"
来源：http://eup.nwbrower.top

Go:   // 无三元运算符，需用 if 语句
来源：http://fcu.guannengcc.top

Ruby: x > 0 ? "yes" : "no"
来源：http://flv.gzhubu.top

C#:   x > 0 ? "yes" : "no"
来源：http://aop.haohaochexian.top

[A12] 字符串插值 / 格式化
来源：http://qcc.kuanghao11.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://kdq.9152youxi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ouh.gzhubu.top

JS:   `Hello, ${name}!`
来源：http://xbl.zdbjq.cn

TS:   `Hello, ${name}!`
来源：http://swm.havefunace.top

Java: "Hello, %s!".formatted(name)
来源：http://awz.gotoacloud.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://akl.sysykeji.top

Ruby: "Hello, #{name}!"
来源：http://qkv.ctjpmb.com

C#:   $"Hello, {name}!"
来源：http://oxn.havefunace.top

[A13] 多行字符串（练习 \n 转义）
来源：http://zsn.bjfxy.top

Py:   "第一行\n第二行"
来源：http://iuv.feifeiyinyue.top

PHP:  "第一行\n第二行"
来源：http://jes.jqgfzy.top

JS:   "第一行\n第二行"
来源：http://wvn.sweek.top

TS:   "第一行\n第二行"
来源：http://ekr.fehbvm.com

Java: "第一行\n第二行"
来源：http://oef.yongpay.top

Go:   "第一行\n第二行"
来源：http://tiq.havefunace.top

Ruby: "第一行\n第二行"
来源：http://mnj.nanxinkj.top

C#:   "第一行\n第二行"
来源：http://oyh.tianlin.xyz

[A14] 注释写法
来源：http://mqp.tianlin.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://kwu.pycfn.com

PHP:  // 或 # 单行；/* 多行 */
来源：http://xlq.chenzaomai.com

JS:   // 单行；/* 多行 */
来源：http://njj.zhiwuduotai.top

TS:   // 单行；/* 多行 */
来源：http://nac.zhixingplan.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yuw.xziqi.cn

Go:   // 单行；/* 多行 */
来源：http://snh.yangfankeji.com

Ruby: # 单行；=begin 多行 =end
来源：http://zft.smart0.xyz

C#:   // 单行；/* 多行 */
来源：http://ipg.jlsjyb.cn

[A15] 空值判断与默认值
来源：http://vtj.pycfn.com

Py:   value = data or "默认值"
来源：http://uuy.yangfankeji.com

PHP:  $value = $data ?? "默认值";
来源：http://gzi.gaohongyu789.top

JS:   const value = data ?? "默认值";
来源：http://ceg.bjfxy.top

TS:   const value = data ?? "默认值";
来源：http://zrs.tianlin.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wtj.jinqigfzy.top

Go:   if data == "" { data = "默认值" }
来源：http://mfz.ehwqpu.com

Ruby: value = data || "默认值"
来源：http://yrf.redwolf501.top

C#:   var value = data ?? "默认值";
来源：http://qiq.wangshuangyany.cn

[A16] 真假值判断规则
来源：http://eri.sxryk.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ehu.9152youxi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ctm.hongshengwenyu.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gqd.shanyushiyangkeji.top

TS:   if (!x) {}
来源：http://vzz.guannengcc.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xje.shanyushiyangtech.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dfb.ydjk.org.cn

Ruby: unless x            # nil 与 false 为假
来源：http://lcl.uphjek.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hyt.jiagoushi.top

[A17] 位运算
来源：http://ivk.cdnleiting.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uaj.sjlbkw.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qgi.tianlin.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ife.dianchejie.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wkv.hammf.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vkk.zhongyouzk.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qiw.yj20258.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ogd.52xcode.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://afs.xingfuxueyuan.xyz

[A18] 字符与 ASCII 码互转
来源：http://voj.haohaochexian.top

Py:   ord("A"); chr(65)
来源：http://cwu.zhaomingkeji.xyz

PHP:  ord("A"); chr(65)
来源：http://fwn.dianchejie.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wqf.birdmap.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://flv.cucudq.cn

Java: (int) 'A'; (char) 65
来源：http://dga.redwolf501.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://isw.nanxuanxn.top

Ruby: "A".ord; 65.chr
来源：http://tne.aizwys.cn

C#:   (int)'A'; (char)65
来源：http://zet.zdbjq.cn

[A19] 交换两个变量
来源：http://isi.yonumen.top

Py:   a, b = b, a
来源：http://hly.guowangkeji.top

PHP:  [$a, $b] = [$b, $a];
来源：http://njw.yfazqb.com

JS:   [a, b] = [b, a];
来源：http://erj.nwbrower.top

TS:   [a, b] = [b, a];
来源：http://axe.mhx1999.top

Java: int t = a; a = b; b = t;
来源：http://tfz.jianghu66.top

Go:   a, b = b, a
来源：http://iyk.feifeiyinyue.top

Ruby: a, b = b, a
来源：http://fcc.kuanghao11.cn

C#:   (a, b) = (b, a);
来源：http://znk.iojbl.cn

[A20] 读取标准输入
来源：http://idm.ctjpmb.com

Py:   name = input("请输入：")
来源：http://tau.yj20258888.top

PHP:  $name = trim(fgets(STDIN));
来源：http://bmc.chenzaomai.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mat.fzhhl.top

TS:   // Node.js：readline 模块
来源：http://heg.shzxlz.cn

Java: new Scanner(System.in).nextLine()
来源：http://lge.guowangkeji.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gnw.tian-w.cn

Ruby: gets.chomp
来源：http://eyv.fanxiaobao.xyz

C#:   Console.ReadLine();
来源：http://edv.zhengqikj.top

[A21] 保留指定小数位输出
来源：http://nrs.yuanzhike.top

Py:   f"{3.14159:.2f}"
来源：http://amg.snrcjt.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hkx.nanxuanxn.top

JS:   (3.14159).toFixed(2)
来源：http://mec.yfazqb.com

TS:   (3.14159).toFixed(2)
来源：http://row.yanxiufei.cn

Java: String.format("%.2f", 3.14159)
来源：http://crt.pycfn.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hup.cashguo.top

Ruby: format("%.2f", 3.14159)
来源：http://tpa.hcnkem.com

C#:   3.14159.ToString("F2")
来源：http://vuk.uphjek.com

[A22] 获取字符串长度
来源：http://phl.hywenlv.cn

Py:   len(s)
来源：http://uas.kuanghao11.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dau.zhixingplan.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lof.bjfxy.top

TS:   s.length
来源：http://zmd.hnqzz.top

Java: s.length()
来源：http://vis.guowangkeji.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jyg.pengpengdd.cyou

Ruby: s.length
来源：http://qna.aizwys.cn

C#:   s.Length
来源：http://css.sjlbkw.cn

[A23] 大小写转换
来源：http://mdk.wangshuangyany.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xti.hywenlv.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qtq.yj20258.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uqe.andypj.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://epf.shangyingyoupin.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ibp.yuanzhike.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://txz.hnxiangtu.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://bnw.cdnleiting.top

C#:   s.ToUpper(); s.ToLower()
来源：http://llj.ppjwa.cn

[A24] 去除首尾空白
来源：http://imq.xuetiantiany.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tbl.sxryk.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sno.shanyushiyangtech.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ags.dashuyun.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vno.shuidangran.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://owv.snrcjt.cn

Go:   strings.TrimSpace(s)
来源：http://mml.yj20258.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dqj.gzhubu.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vmr.zhixingplan.top

[A25] 字符串比较
来源：http://xqx.yueranfly.top

Py:   s1 == s2; s1 != s2
来源：http://cay.tian-w.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rtn.jqgufenzy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://upy.tarul.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pox.ivvv.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xpo.bjfxy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://whw.havefunace.top

Ruby: s1 == s2; s1 <=> s2
来源：http://sxw.xinyue.icu

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gpf.smart0.xyz

[A26] 类型转换总览
来源：http://ltt.epnwcf.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oaf.zhixingplan.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bjo.yongpay.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kul.daria6918.cn

TS:   Number() String() Boolean() x as number
来源：http://tdp.ctjpmb.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yjm.52xcode.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://uqs.shuidangran.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://xzu.9152youxi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lmx.yuanzhike.top

================================================================================
来源：http://xxa.xingfuxueyuan.xyz

B. 流程控制
来源：http://ypu.hammf.cn

================================================================================
来源：http://hgl.yj202588.top

[B01] 条件判断 if / else
来源：http://wci.nanxuanxn.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ndn.aibaodan.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://noi.jinyuanbaomall.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://phb.tian-w.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://erd.ehwqpu.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://amu.fengsongda.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cxq.fzhhl.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jio.tianlin.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xko.svipenyu.cn

[B02] 多分支 else if / elif
来源：http://jqy.jianghu66.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rkl.jqgufenzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wkc.meibo888.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lvg.zycfv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://egb.yueranfly.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ulk.jianghu66.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jah.zhiwuduotai.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nvj.pengpengdd.cyou

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tgn.gaohongyu789.top

[B03] switch / match / case
来源：http://pmn.shuidangran.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yib.ybcxt.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mgk.guowangkeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://taq.ybcxt.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pba.fzhhl.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nln.0kj1m.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://euw.sjlbkw.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kjy.meibo888.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yay.xziqi.cn

[B04] for 计数循环
来源：http://tuz.nanxinkj.top

Py:   for i in range(10): print(i)
来源：http://zaw.tanke756.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xwx.gzhubu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ruy.cucudq.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iyt.sweek.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gtt.guowangkeji.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vpo.ydzc1.top

Ruby: 10.times { |i| puts i }
来源：http://ujd.xuetiantiany.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rng.shuidangran.top

[B05] 遍历数组 / 列表
来源：http://bnc.guowangkeji.top

Py:   for item in arr: print(item)
来源：http://emy.daria6918.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ptj.nanxinkj.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vot.tanke756.top

TS:   for (const item of arr) { console.log(item); }
来源：http://jga.jqgufenzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://gps.xuetiantiany.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jsy.zhixingplan.top

Ruby: arr.each { |item| puts item }
来源：http://fap.birdmap.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rbt.yanxiufei.cn

[B06] 遍历字典 / 对象
来源：http://kcs.hongshengwenyu.top

Py:   for k, v in d.items(): print(k, v)
来源：http://rtp.zhijiandao.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cik.yuxming.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://olj.kuanghao11.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://frn.hammf.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://whg.tarul.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qrm.hnqzz.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fzt.wangshuangyany.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zag.aizwys.cn

[B07] while 循环
来源：http://scg.ctjpmb.com

Py:   while i < 10: i += 1
来源：http://wht.tian-w.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xoj.vqdsnc.cn

JS:   while (i < 10) { i++; }
来源：http://srk.zhixingplan.top

TS:   while (i < 10) { i++; }
来源：http://pdd.zhixingplan.top

Java: while (i < 10) { i++; }
来源：http://hjr.hnxiangtu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xfw.fzhhl.top

Ruby: while i < 10; i += 1; end
来源：http://ymb.ppjwa.cn

C#:   while (i < 10) { i++; }
来源：http://zqk.uphjek.com

[B08] do-while（至少执行一次）
来源：http://tqj.gaohongyu789.top

Py:   # 无 do-while：用 while True + break
来源：http://cbr.fengsongda.top

PHP:  do { $i++; } while ($i < 10);
来源：http://wmo.sweek.top

JS:   do { i++; } while (i < 10);
来源：http://qgx.vehdjk.com

TS:   do { i++; } while (i < 10);
来源：http://ins.zhongyouzk.top

Java: do { i++; } while (i < 10);
来源：http://nfy.chenlongwang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hev.zhoulong.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://nzp.gzhubu.top

C#:   do { i++; } while (i < 10);
来源：http://ozo.xziqi.cn

[B09] break 与 continue
来源：http://ygo.zhaomingkeji.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://iyo.nwbrower.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://opt.tianlin.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xfo.jinghuilouyu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ytk.epnwcf.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ctx.hesvh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lql.c1oappe.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rmg.jyoumei.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ree.yj20258.top

[B10] 遍历同时拿索引
来源：http://qde.xziqi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sin.hnxiangtu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://djv.dianchejie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ynp.sysykeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lez.ppjwa.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gyc.tian-w.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fzb.cqqwz.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ksa.ydjk.org.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wwu.xuanzx.com

[B11] 生成数字序列 / 区间
来源：http://xzi.52xcode.cn

Py:   list(range(0, 10, 2))
来源：http://zyw.smart0.xyz

PHP:  range(0, 10, 2);
来源：http://ifp.zdqjudy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kbi.jinqigufen.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wev.hnxiangtu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bxz.jqgfzy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ips.jianghu66.top

Ruby: (0...10).step(2).to_a
来源：http://xtz.ivvv.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qlc.yj202588.top

[B12] 跳出多层循环
来源：http://uva.yuanzhike.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://yst.yongpay.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://wci.52xcode.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://msa.fzhhl.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ucf.tarul.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pew.cucudq.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kxt.yj20258.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://otb.sweek.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://znh.ydzc1.top

[B13] 判断是否为数字
来源：http://bnw.jlsjyb.cn

Py:   isinstance(x, (int, float))
来源：http://ahu.sxryk.cn

PHP:  is_numeric($x)
来源：http://quf.jqgufenzy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pkv.quarkkingdee.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bjj.aibaodan.cn

Java: x instanceof Number
来源：http://jjd.yangfankeji.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sli.zhengqikj.top

Ruby: x.is_a?(Numeric)
来源：http://ejf.aizwys.cn

C#:   x is int or double or decimal
来源：http://vxi.zhaomingkeji.xyz

[B14] 判断值是否在集合内
来源：http://fda.hnxiangtu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://thh.xuanzx.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fjt.quarkkingdee.top

JS:   [1, 2, 3].includes(x)
来源：http://czt.fanxiaobao.xyz

TS:   [1, 2, 3].includes(x)
来源：http://rtb.cheryme.top

Java: List.of(1, 2, 3).contains(x)
来源：http://xym.jinqigfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xlf.tanke756.top

Ruby: [1, 2, 3].include?(x)
来源：http://itp.xziqi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bqh.iojbl.cn

[B15] 布尔运算与取反
来源：http://xtn.fehbvm.com

Py:   a and b or not c
来源：http://vxa.hongshengwenyu.top

PHP:  $a && $b || !$c
来源：http://syf.xylfe.cn

JS:   a && b || !c
来源：http://ndh.yj202588.top

TS:   a && b || !c
来源：http://hdt.jinyuanbaomall.cn

Java: a && b || !c
来源：http://ycp.hnqzz.top


<!-- 参考信息 -->