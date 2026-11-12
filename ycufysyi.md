代发 wailian999

Ruby: 42.to_s
来源：http://dcl.shzxlz.cn

C#:   42.ToString()
来源：http://lgy.redwolf501.top

[A08] 取整与四舍五入
来源：http://pwj.yj202588.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qkz.nwbrower.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dsj.daria6918.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://irk.chenlongwang.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lnb.gaohongyu789.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://dyk.jinqigufen.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://eep.sysykeji.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://zdw.ydzc1.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://akt.hysaishi.cn

[A09] 绝对值与最大最小值
来源：http://wfk.ydzc1.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wrk.sweek.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dba.xingfuxueyuan.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ubb.birdmap.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://clu.yj202588.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hbl.yfazqb.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pwb.jinqigfzy.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://uex.bjfxy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fvg.ywan-chungtsiang.top

[A10] 生成随机数
来源：http://ats.hesvh.cn

Py:   import random; random.randint(1, 100)
来源：http://yvt.sweek.top

PHP:  random_int(1, 100);
来源：http://hla.sysykeji.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kku.jyoumei.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bgp.zdqjudy.top

Java: new Random().nextInt(100) + 1
来源：http://ayo.hnxiangtu.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fod.xylfe.cn

Ruby: rand(1..100)
来源：http://fel.haohaochexian.top

C#:   new Random().Next(1, 101)
来源：http://dmn.ydjk.org.cn

[A11] 条件表达式（三元）
来源：http://thy.haohaochexian.top

Py:   "yes" if x > 0 else "no"
来源：http://tfz.zhongyouzk.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://kyg.yonumen.top

JS:   x > 0 ? "yes" : "no"
来源：http://hqs.hysaishi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dud.zhijiandao.cn

Java: x > 0 ? "yes" : "no"
来源：http://wzg.iojbl.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hdo.jinqigfzy.top

Ruby: x > 0 ? "yes" : "no"
来源：http://zfw.gzhubu.top

C#:   x > 0 ? "yes" : "no"
来源：http://cgn.hcnkem.com

[A12] 字符串插值 / 格式化
来源：http://eii.yj20258.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://vpl.yongpay.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://yxz.xuanzx.com

JS:   `Hello, ${name}!`
来源：http://wyo.hfpthk.cn

TS:   `Hello, ${name}!`
来源：http://ywq.52xcode.cn

Java: "Hello, %s!".formatted(name)
来源：http://xck.zhiwuduotai.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hwd.yonumen.top

Ruby: "Hello, #{name}!"
来源：http://fah.xingfuxueyuan.xyz

C#:   $"Hello, {name}!"
来源：http://gkk.shanyushiyangkeji.top

[A13] 多行字符串（练习 \n 转义）
来源：http://myu.xuanzx.com

Py:   "第一行\n第二行"
来源：http://ngu.xingfuxueyuan.xyz

PHP:  "第一行\n第二行"
来源：http://vib.cqqwz.cn

JS:   "第一行\n第二行"
来源：http://ndv.ppjwa.cn

TS:   "第一行\n第二行"
来源：http://jvf.yanxiufei.cn

Java: "第一行\n第二行"
来源：http://zbv.jqgfzy.top

Go:   "第一行\n第二行"
来源：http://cgz.zhaomingkeji.xyz

Ruby: "第一行\n第二行"
来源：http://bbp.xziqi.cn

C#:   "第一行\n第二行"
来源：http://wxh.vqdsnc.cn

[A14] 注释写法
来源：http://ohl.cashguo.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://gbk.zhoulong.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://twp.jyoumei.cn

JS:   // 单行；/* 多行 */
来源：http://shv.shangyingyoupin.top

TS:   // 单行；/* 多行 */
来源：http://kay.andypj.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vtu.ppjwa.cn

Go:   // 单行；/* 多行 */
来源：http://fwf.iojbl.cn

Ruby: # 单行；=begin 多行 =end
来源：http://dsi.hongshengwenyu.top

C#:   // 单行；/* 多行 */
来源：http://pue.zdqjudy.top

[A15] 空值判断与默认值
来源：http://eqh.ctjpmb.com

Py:   value = data or "默认值"
来源：http://jjs.hesvh.cn

PHP:  $value = $data ?? "默认值";
来源：http://tig.redwolf501.top

JS:   const value = data ?? "默认值";
来源：http://fod.jianghu66.top

TS:   const value = data ?? "默认值";
来源：http://wte.jinghuilouyu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wha.zdbjq.cn

Go:   if data == "" { data = "默认值" }
来源：http://mum.zhijiandao.cn

Ruby: value = data || "默认值"
来源：http://mst.guannengcc.top

C#:   var value = data ?? "默认值";
来源：http://xow.yj202588.top

[A16] 真假值判断规则
来源：http://hty.jinqigufen.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yhg.dianchejie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://duw.shanyushiyangtech.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nnl.wangdashe.top

TS:   if (!x) {}
来源：http://bob.nanxinkj.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gjf.316326.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://eik.9152youxi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vcf.0kj1m.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ugz.52xcode.cn

[A17] 位运算
来源：http://fou.hfpthk.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qkq.hfpthk.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://sbn.jianghu66.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jrl.smart0.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://enb.hnqzz.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uau.xuanzx.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pcg.epnwcf.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://khz.zhixingplan.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ehx.gogol.net.cn

[A18] 字符与 ASCII 码互转
来源：http://zpb.ydjk.org.cn

Py:   ord("A"); chr(65)
来源：http://cuw.jlsjyb.cn

PHP:  ord("A"); chr(65)
来源：http://oip.xinyue.icu

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dll.yongpay.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cbs.xinyue.icu

Java: (int) 'A'; (char) 65
来源：http://skv.shuidangran.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://drk.sufxvd.cn

Ruby: "A".ord; 65.chr
来源：http://ajm.wangshuangyany.cn

C#:   (int)'A'; (char)65
来源：http://vou.fanxiaobao.xyz

[A19] 交换两个变量
来源：http://hwc.dianchejie.cn

Py:   a, b = b, a
来源：http://hrt.chenzaomai.com

PHP:  [$a, $b] = [$b, $a];
来源：http://cuw.hnxiangtu.top

JS:   [a, b] = [b, a];
来源：http://gil.wangshuangyany.cn

TS:   [a, b] = [b, a];
来源：http://spq.xuanzx.com

Java: int t = a; a = b; b = t;
来源：http://wyz.jinqigufen.top

Go:   a, b = b, a
来源：http://ubk.hysaishi.cn

Ruby: a, b = b, a
来源：http://mhj.jlsjyb.cn

C#:   (a, b) = (b, a);
来源：http://yva.bbcook.cn

[A20] 读取标准输入
来源：http://tgj.9152youxi.cn

Py:   name = input("请输入：")
来源：http://gql.gzhubu.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ete.hesvh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://auo.vehdjk.com

TS:   // Node.js：readline 模块
来源：http://hie.vqdsnc.cn

Java: new Scanner(System.in).nextLine()
来源：http://jry.jyoumei.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://afz.xuanzx.com

Ruby: gets.chomp
来源：http://iej.hesvh.cn

C#:   Console.ReadLine();
来源：http://eut.yj20258.top

[A21] 保留指定小数位输出
来源：http://ttu.ywan-chungtsiang.top

Py:   f"{3.14159:.2f}"
来源：http://ltu.xuetiantiany.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://woc.hywenlv.cn

JS:   (3.14159).toFixed(2)
来源：http://bhp.yj202588.top

TS:   (3.14159).toFixed(2)
来源：http://kfd.kuanghao11.cn

Java: String.format("%.2f", 3.14159)
来源：http://vgt.redwolf501.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ptn.guowangkeji.top

Ruby: format("%.2f", 3.14159)
来源：http://xvf.haohaochexian.top

C#:   3.14159.ToString("F2")
来源：http://hwa.quarkkingdee.top

[A22] 获取字符串长度
来源：http://bxv.jinyuanbaomall.cn

Py:   len(s)
来源：http://owg.c1oappe.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sfa.daxiang520.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kxk.ivvv.top

TS:   s.length
来源：http://xvh.svipenyu.cn

Java: s.length()
来源：http://ssl.chenzaomai.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tqo.xuetiantiany.cn

Ruby: s.length
来源：http://ura.zdqjudy.top

C#:   s.Length
来源：http://nli.fanxiaobao.xyz

[A23] 大小写转换
来源：http://ggs.xziqi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wlj.aizwys.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://nng.xylfe.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://eot.tanke756.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://axg.aibaodan.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ood.quarkkingdee.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wye.fengsongda.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uet.nanxuanxn.top

C#:   s.ToUpper(); s.ToLower()
来源：http://tsf.cqqwz.cn

[A24] 去除首尾空白
来源：http://rdy.andypj.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://laa.gzhubu.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://isf.yfazqb.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eqv.ppjwa.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uyt.jinqigfzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ugq.gaohongyu789.top

Go:   strings.TrimSpace(s)
来源：http://tuh.ydjk.org.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cef.tian-w.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://viv.fengsongda.top

[A25] 字符串比较
来源：http://ugd.svipenyu.cn

Py:   s1 == s2; s1 != s2
来源：http://xgc.wangshuangyany.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://akv.guannengcc.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uwg.cashguo.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qmh.ehwqpu.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rqa.yonumen.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gmx.hnqzz.top

Ruby: s1 == s2; s1 <=> s2
来源：http://fsi.316326.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://gza.nwbrower.top

[A26] 类型转换总览
来源：http://htb.hnxiangtu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kwd.yj20258888.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uis.hammf.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pqf.daria6918.cn

TS:   Number() String() Boolean() x as number
来源：http://ibl.hesvh.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yva.aibaodan.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bra.sufxvd.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://qrv.hnxiangtu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rgw.yanxiufei.cn

================================================================================
来源：http://rtj.jinghuilouyu.cn

B. 流程控制
来源：http://lxi.bjfxy.top

================================================================================
来源：http://oju.pycfn.com

[B01] 条件判断 if / else
来源：http://mve.smart0.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://gxu.chenzaomai.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hqt.andypj.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gnt.zdbjq.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ljf.haohaochexian.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://rib.zhixingplan.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zme.havefunace.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vcr.shzxlz.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ruj.jinqigufen.top

[B02] 多分支 else if / elif
来源：http://omm.yfazqb.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ona.jinqigfzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lhb.daria6918.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://erb.smart0.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zol.vqdsnc.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lfr.zhoulong.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pfq.cqqwz.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mim.jiagoushi.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jpc.xinyue.icu

[B03] switch / match / case
来源：http://mns.ctjpmb.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gfx.xinyue.icu

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cmj.svipenyu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hvc.ywan-chungtsiang.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wuc.dianchejie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://atc.xinyue.icu

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cvy.fanxiaobao.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lbw.cqqwz.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tdr.gaohongyu789.top

[B04] for 计数循环
来源：http://xru.jqgfzy.top

Py:   for i in range(10): print(i)
来源：http://qhk.jinghuilouyu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sld.fktsv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jmq.sysykeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kos.fengsongda.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://thh.gotoacloud.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nkh.yj202588.top

Ruby: 10.times { |i| puts i }
来源：http://uix.jinghuilouyu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ydz.c1oappe.top

[B05] 遍历数组 / 列表
来源：http://cqy.zdqjudy.top

Py:   for item in arr: print(item)
来源：http://vww.c1oappe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vsv.fengsongda.top

JS:   for (const item of arr) { console.log(item); }
来源：http://msn.daria6918.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sjl.ctjpmb.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://ccw.nanxinkj.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rhy.snrcjt.cn

Ruby: arr.each { |item| puts item }
来源：http://rqo.cqqwz.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uqa.jqgufenzy.top

[B06] 遍历字典 / 对象
来源：http://qsx.ehwqpu.com

Py:   for k, v in d.items(): print(k, v)
来源：http://nqe.yuxming.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://krf.sxryk.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hkv.sweek.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://reh.uphjek.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cfu.sjlbkw.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mco.yangfankeji.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://feq.zhijiandao.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://juy.dashuyun.cn

[B07] while 循环
来源：http://udl.hfpthk.cn

Py:   while i < 10: i += 1
来源：http://ojp.yfazqb.com

PHP:  while ($i < 10) { $i++; }
来源：http://swx.fktsv.cn

JS:   while (i < 10) { i++; }
来源：http://lqv.0kj1m.cn

TS:   while (i < 10) { i++; }
来源：http://rcu.gzhubu.top

Java: while (i < 10) { i++; }
来源：http://rdr.jianghu66.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://czx.zhijiandao.cn

Ruby: while i < 10; i += 1; end
来源：http://lvy.tarul.cn

C#:   while (i < 10) { i++; }
来源：http://znb.nwbrower.top

[B08] do-while（至少执行一次）
来源：http://laz.ydjk.org.cn

Py:   # 无 do-while：用 while True + break
来源：http://djz.tarul.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://lzl.feifeiyinyue.top

JS:   do { i++; } while (i < 10);
来源：http://nzv.yfazqb.com

TS:   do { i++; } while (i < 10);
来源：http://csr.fzhhl.top

Java: do { i++; } while (i < 10);
来源：http://xfv.jinyuanbaomall.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dnm.52xcode.cn

Ruby: begin; i += 1; end while i < 10
来源：http://etr.yangfankeji.com

C#:   do { i++; } while (i < 10);
来源：http://vpg.yonumen.top

[B09] break 与 continue
来源：http://seq.ehwqpu.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wjf.ydjk.org.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yuv.havefunace.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lzn.zhiwuduotai.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://onr.birdmap.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ofa.fanxiaobao.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://die.fktsv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dot.cucudq.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fsl.jqgfzy.top

[B10] 遍历同时拿索引
来源：http://jxx.jiagoushi.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://veo.nanxuanxn.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://myi.dianchejie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://seu.xylfe.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://smj.haohaochexian.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tpq.shzxlz.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rgm.chenlongwang.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://osz.jqgfzy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fpj.cashguo.top

[B11] 生成数字序列 / 区间
来源：http://nuk.jyoumei.cn

Py:   list(range(0, 10, 2))
来源：http://myh.zhengqikj.top

PHP:  range(0, 10, 2);
来源：http://xww.sysykeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fmv.chenzaomai.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wxx.wangdashe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mli.cqqwz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fgt.ehwqpu.com

Ruby: (0...10).step(2).to_a
来源：http://nza.quarkkingdee.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vlt.yvedp.cn

[B12] 跳出多层循环
来源：http://rbr.chenzaomai.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://xws.ppjwa.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://wlj.chenlongwang.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://izi.shuidangran.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wja.aibaodan.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://eeg.sjlbkw.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wan.yj202588.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sfl.ybcxt.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nyl.snrcjt.cn

[B13] 判断是否为数字
来源：http://htl.vqdsnc.cn

Py:   isinstance(x, (int, float))
来源：http://nam.hywenlv.cn

PHP:  is_numeric($x)
来源：http://mak.jiagoushi.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jto.sysykeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://raf.bbcook.cn

Java: x instanceof Number
来源：http://xem.zhoulong.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qmz.zdqjudy.top

Ruby: x.is_a?(Numeric)
来源：http://ulm.ivvv.top

C#:   x is int or double or decimal
来源：http://rlt.gotoacloud.top

[B14] 判断值是否在集合内
来源：http://egd.yj202588.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://elr.52xcode.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mqt.snrcjt.cn

JS:   [1, 2, 3].includes(x)
来源：http://bcv.316326.xyz

TS:   [1, 2, 3].includes(x)
来源：http://bkv.gogol.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ljh.yangfankeji.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kpy.zdbjq.cn


<!-- 参考信息 -->