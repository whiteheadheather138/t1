代发 wailian999

JS:   String(42); (42).toString()
来源：http://mjg.cqqwz.cn

TS:   String(42)
来源：http://pkz.vehdjk.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://bqo.sjlbkw.cn

Go:   strconv.Itoa(42)
来源：http://oup.feifeiyinyue.top

Ruby: 42.to_s
来源：http://lns.xinyue.icu

C#:   42.ToString()
来源：http://azi.316326.xyz

[A08] 取整与四舍五入
来源：http://zop.hammf.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qju.jinyuanbaomall.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://bxk.quarkkingdee.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ibb.fanxiaobao.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yqn.tian-w.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nrz.ehwqpu.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yqu.tanke756.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ewi.zhiwuduotai.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jir.ivvv.top

[A09] 绝对值与最大最小值
来源：http://yel.yueranfly.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lsd.52xcode.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hsa.sysykeji.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fmf.wangshuangyany.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://sct.yvedp.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://emx.svipenyu.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://eiq.hcnkem.com

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://qul.0kj1m.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://uwa.gogol.net.cn

[A10] 生成随机数
来源：http://moj.cqqwz.cn

Py:   import random; random.randint(1, 100)
来源：http://dxm.jiagoushi.top

PHP:  random_int(1, 100);
来源：http://jjt.quarkkingdee.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lla.jqgufenzy.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hrz.nanxinkj.top

Java: new Random().nextInt(100) + 1
来源：http://hmc.shangyingyoupin.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://nzr.zdbjq.cn

Ruby: rand(1..100)
来源：http://byu.zdqjudy.top

C#:   new Random().Next(1, 101)
来源：http://caw.xylfe.cn

[A11] 条件表达式（三元）
来源：http://zob.shzxlz.cn

Py:   "yes" if x > 0 else "no"
来源：http://tjf.pycfn.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://xax.hcnkem.com

JS:   x > 0 ? "yes" : "no"
来源：http://kfx.bbcook.cn

TS:   x > 0 ? "yes" : "no"
来源：http://fee.dianchejie.cn

Java: x > 0 ? "yes" : "no"
来源：http://kcz.aizwys.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://cda.pycfn.com

Ruby: x > 0 ? "yes" : "no"
来源：http://ley.shangyingyoupin.top

C#:   x > 0 ? "yes" : "no"
来源：http://pxv.hongshengwenyu.top

[A12] 字符串插值 / 格式化
来源：http://dsn.pengpengdd.cyou

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vfh.ywan-chungtsiang.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jes.xuanzx.com

JS:   `Hello, ${name}!`
来源：http://yuh.snrcjt.cn

TS:   `Hello, ${name}!`
来源：http://rrm.uphjek.com

Java: "Hello, %s!".formatted(name)
来源：http://wlp.jlsjyb.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://acq.chenjidiqi.icu

Ruby: "Hello, #{name}!"
来源：http://wpb.svipenyu.cn

C#:   $"Hello, {name}!"
来源：http://vwm.pengpengdd.cyou

[A13] 多行字符串（练习 \n 转义）
来源：http://xue.hongshengwenyu.top

Py:   "第一行\n第二行"
来源：http://iwm.hesvh.cn

PHP:  "第一行\n第二行"
来源：http://axg.hcnkem.com

JS:   "第一行\n第二行"
来源：http://cqa.bjfxy.top

TS:   "第一行\n第二行"
来源：http://uyc.hammf.cn

Java: "第一行\n第二行"
来源：http://iwf.vehdjk.com

Go:   "第一行\n第二行"
来源：http://brv.yvedp.cn

Ruby: "第一行\n第二行"
来源：http://wdn.hfpthk.cn

C#:   "第一行\n第二行"
来源：http://imm.hongshengwenyu.top

[A14] 注释写法
来源：http://ovo.nanxuanxn.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ihr.snrcjt.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://xjk.52xcode.cn

JS:   // 单行；/* 多行 */
来源：http://btk.wangshuangyany.cn

TS:   // 单行；/* 多行 */
来源：http://dak.sysykeji.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://oul.jinyuanbaomall.cn

Go:   // 单行；/* 多行 */
来源：http://joq.yfazqb.com

Ruby: # 单行；=begin 多行 =end
来源：http://xxs.smart0.xyz

C#:   // 单行；/* 多行 */
来源：http://evw.shangyingyoupin.top

[A15] 空值判断与默认值
来源：http://ecm.daxiang520.top

Py:   value = data or "默认值"
来源：http://val.fehbvm.com

PHP:  $value = $data ?? "默认值";
来源：http://iui.xinyue.icu

JS:   const value = data ?? "默认值";
来源：http://rqx.tian-w.cn

TS:   const value = data ?? "默认值";
来源：http://mje.yfazqb.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://bzx.ydjk.org.cn

Go:   if data == "" { data = "默认值" }
来源：http://qoh.snrcjt.cn

Ruby: value = data || "默认值"
来源：http://iew.zhixingplan.top

C#:   var value = data ?? "默认值";
来源：http://nhy.wangshuangyany.cn

[A16] 真假值判断规则
来源：http://vpo.jianghu66.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://liw.gotoacloud.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://euz.nanxuanxn.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://khm.wangshuangyany.cn

TS:   if (!x) {}
来源：http://jtc.bjfxy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dms.yj20258.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://pwh.jinqigfzy.top

Ruby: unless x            # nil 与 false 为假
来源：http://elk.cheryme.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rip.zhixingplan.top

[A17] 位运算
来源：http://nar.havefunace.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lvv.316326.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xfn.zhijiandao.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zlj.zycfv.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vhp.yj20258888.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jhv.dashuyun.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fzh.feifeiyinyue.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://edn.yj20258.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tgn.snrcjt.cn

[A18] 字符与 ASCII 码互转
来源：http://dsx.sufxvd.cn

Py:   ord("A"); chr(65)
来源：http://uig.jianghu66.top

PHP:  ord("A"); chr(65)
来源：http://pfu.smart0.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kzq.yj20258.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ath.iojbl.cn

Java: (int) 'A'; (char) 65
来源：http://cux.gaohongyu789.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ttz.hammf.cn

Ruby: "A".ord; 65.chr
来源：http://qap.sufxvd.cn

C#:   (int)'A'; (char)65
来源：http://nml.havefunace.top

[A19] 交换两个变量
来源：http://akz.jianghu66.top

Py:   a, b = b, a
来源：http://hnm.ehwqpu.com

PHP:  [$a, $b] = [$b, $a];
来源：http://vwc.meibo888.top

JS:   [a, b] = [b, a];
来源：http://osn.chenzaomai.com

TS:   [a, b] = [b, a];
来源：http://mab.hywenlv.cn

Java: int t = a; a = b; b = t;
来源：http://osq.bjfxy.top

Go:   a, b = b, a
来源：http://fxi.iojbl.cn

Ruby: a, b = b, a
来源：http://cjn.haohaochexian.top

C#:   (a, b) = (b, a);
来源：http://tan.chenlongwang.top

[A20] 读取标准输入
来源：http://ezg.ivvv.top

Py:   name = input("请输入：")
来源：http://cew.316326.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://iyo.nanxinkj.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wcd.nanxuanxn.top

TS:   // Node.js：readline 模块
来源：http://mow.hfpthk.cn

Java: new Scanner(System.in).nextLine()
来源：http://ipi.hcnkem.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cfq.tanke756.top

Ruby: gets.chomp
来源：http://gvm.sxryk.cn

C#:   Console.ReadLine();
来源：http://eir.nanxuanxn.top

[A21] 保留指定小数位输出
来源：http://ucx.ybcxt.top

Py:   f"{3.14159:.2f}"
来源：http://mcc.xuetiantiany.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kcs.yanxiufei.cn

JS:   (3.14159).toFixed(2)
来源：http://djs.zdqjudy.top

TS:   (3.14159).toFixed(2)
来源：http://jns.tarul.cn

Java: String.format("%.2f", 3.14159)
来源：http://bqj.fehbvm.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://our.hesvh.cn

Ruby: format("%.2f", 3.14159)
来源：http://sql.tianlin.xyz

C#:   3.14159.ToString("F2")
来源：http://lzx.zhongyouzk.top

[A22] 获取字符串长度
来源：http://ymb.xinyue.icu

Py:   len(s)
来源：http://ntv.xinyue.icu

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ngh.yj20258888.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nbc.gaohongyu789.top

TS:   s.length
来源：http://wly.svipenyu.cn

Java: s.length()
来源：http://lmb.yanxiufei.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rzf.epnwcf.com

Ruby: s.length
来源：http://jyf.cashguo.top

C#:   s.Length
来源：http://njf.birdmap.top

[A23] 大小写转换
来源：http://uag.jianghu66.top

Py:   s.upper(); s.lower(); s.title()
来源：http://nkd.sweek.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://sct.wangshuangyany.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://lks.jianghu66.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tbi.zdqjudy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jqt.fengsongda.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bij.ywan-chungtsiang.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mop.redwolf501.top

C#:   s.ToUpper(); s.ToLower()
来源：http://kxh.fehbvm.com

[A24] 去除首尾空白
来源：http://cvs.zhengqikj.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zlh.xziqi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mjj.dashuyun.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xvh.ywan-chungtsiang.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gek.gaohongyu789.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xiw.jianghu66.top

Go:   strings.TrimSpace(s)
来源：http://qar.xuanzx.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mpj.yvedp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gzq.dianchejie.cn

[A25] 字符串比较
来源：http://umy.jianghu66.top

Py:   s1 == s2; s1 != s2
来源：http://mej.kuanghao11.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mfe.quarkkingdee.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mjo.yongpay.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gyk.cqqwz.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xdo.epnwcf.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://jyg.zdqjudy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://yrc.zhoulong.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pqc.shzxlz.cn

[A26] 类型转换总览
来源：http://dsw.hfpthk.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kgb.pengpengdd.cyou

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fgt.ywan-chungtsiang.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tal.jinqigfzy.top

TS:   Number() String() Boolean() x as number
来源：http://bai.nanxuanxn.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fya.dianchejie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wlh.zhixingplan.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://inw.ydzc1.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vah.hesvh.cn

================================================================================
来源：http://wme.zhixingplan.top

B. 流程控制
来源：http://cij.tian-w.cn

================================================================================
来源：http://ssd.dashuyun.cn

[B01] 条件判断 if / else
来源：http://mtf.hesvh.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bqf.yongpay.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://exg.shanyushiyangtech.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://esz.wangshuangyany.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://aei.birdmap.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://cli.cashguo.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vef.yj20258.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nxn.guannengcc.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zlk.kuanghao11.cn

[B02] 多分支 else if / elif
来源：http://prs.andypj.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://inr.ydzc1.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ghm.hywenlv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lrc.guannengcc.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bbb.kuanghao11.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ncc.fktsv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hku.shangyingyoupin.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fbd.yangfankeji.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nmb.iojbl.cn

[B03] switch / match / case
来源：http://trs.shangyingyoupin.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ckb.fehbvm.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xrj.sxryk.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ykt.bbcook.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mlw.epnwcf.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vxm.yuxming.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dgv.wangdashe.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xwr.yvedp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ing.ctjpmb.com

[B04] for 计数循环
来源：http://hau.aibaodan.cn

Py:   for i in range(10): print(i)
来源：http://mvx.ydzc1.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fxi.jinghuilouyu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dzm.zhiwuduotai.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yrq.hnxiangtu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zje.snrcjt.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://omu.hfpthk.cn

Ruby: 10.times { |i| puts i }
来源：http://tav.yj202588.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mwn.uphjek.com

[B05] 遍历数组 / 列表
来源：http://jpk.vehdjk.com

Py:   for item in arr: print(item)
来源：http://pgl.xingfuxueyuan.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yha.shanyushiyangtech.top

JS:   for (const item of arr) { console.log(item); }
来源：http://jen.haohaochexian.top

TS:   for (const item of arr) { console.log(item); }
来源：http://olh.uphjek.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://kvm.chenjidiqi.icu

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vqk.snrcjt.cn

Ruby: arr.each { |item| puts item }
来源：http://yuu.guowangkeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lqz.gaohongyu789.top

[B06] 遍历字典 / 对象
来源：http://blx.birdmap.top

Py:   for k, v in d.items(): print(k, v)
来源：http://jkg.shzxlz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wel.hnqzz.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jmh.zhongyouzk.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qsy.shanyushiyangtech.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://axn.vehdjk.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vji.epnwcf.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wop.316326.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://khr.daxiang520.top

[B07] while 循环
来源：http://jll.yj202588.top

Py:   while i < 10: i += 1
来源：http://mdw.yonumen.top

PHP:  while ($i < 10) { $i++; }
来源：http://rmd.yvedp.cn

JS:   while (i < 10) { i++; }
来源：http://csm.andypj.xyz

TS:   while (i < 10) { i++; }
来源：http://kon.sjlbkw.cn

Java: while (i < 10) { i++; }
来源：http://frp.gaohongyu789.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://adj.chenzaomai.com

Ruby: while i < 10; i += 1; end
来源：http://kpk.cucudq.cn

C#:   while (i < 10) { i++; }
来源：http://xhm.fanxiaobao.xyz

[B08] do-while（至少执行一次）
来源：http://eek.ehwqpu.com

Py:   # 无 do-while：用 while True + break
来源：http://pbo.uphjek.com

PHP:  do { $i++; } while ($i < 10);
来源：http://ite.jinqigufen.top

JS:   do { i++; } while (i < 10);
来源：http://sxu.tarul.cn

TS:   do { i++; } while (i < 10);
来源：http://dcy.zdbjq.cn

Java: do { i++; } while (i < 10);
来源：http://tbw.fanxiaobao.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://csb.smart0.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://uyv.hysaishi.cn

C#:   do { i++; } while (i < 10);
来源：http://str.jianghu66.top

[B09] break 与 continue
来源：http://sjh.yangfankeji.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://aet.hcnkem.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gds.tarul.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ath.c1oappe.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pll.yanxiufei.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ogw.yj20258.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://eda.svipenyu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xvk.cashguo.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ast.xuetiantiany.cn

[B10] 遍历同时拿索引
来源：http://tnk.shzxlz.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ege.snrcjt.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yyj.ivvv.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dzi.chenlongwang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iux.tianlin.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ral.zdqjudy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jjq.zycfv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ivt.cdnleiting.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fwn.cdnleiting.top

[B11] 生成数字序列 / 区间
来源：http://vgj.gotoacloud.top

Py:   list(range(0, 10, 2))
来源：http://ujq.zhiwuduotai.top

PHP:  range(0, 10, 2);
来源：http://twz.bbcook.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nei.gaohongyu789.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fls.daria6918.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://alj.dianchejie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jkd.chenlongwang.top

Ruby: (0...10).step(2).to_a
来源：http://fxp.bjfxy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uhb.kuanghao11.cn

[B12] 跳出多层循环
来源：http://cqo.xinyue.icu

Py:   # 无标签跳转：抽成函数用 return
来源：http://cau.ctjpmb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://fzx.andypj.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jkc.jinqigfzy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://izj.yuxming.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wga.birdmap.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vcq.sysykeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uea.xylfe.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zwa.52xcode.cn

[B13] 判断是否为数字
来源：http://lko.zhiwuduotai.top

Py:   isinstance(x, (int, float))
来源：http://vfa.yanxiufei.cn

PHP:  is_numeric($x)
来源：http://nre.dianchejie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ldj.zhiwuduotai.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nvb.yuanzhike.top

Java: x instanceof Number
来源：http://iam.tarul.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qui.ehwqpu.com

Ruby: x.is_a?(Numeric)
来源：http://njc.zhaomingkeji.xyz

C#:   x is int or double or decimal
来源：http://ier.gotoacloud.top

[B14] 判断值是否在集合内
来源：http://fgm.hnxiangtu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qfu.tian-w.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mls.yj20258.top


<!-- 参考信息 -->