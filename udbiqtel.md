代发 wailian999

Java: 7 / 2; 7 % 2
来源：http://sph.svipenyu.cn

Go:   7 / 2; 7 % 2
来源：http://fyr.hammf.cn

Ruby: 7 / 2; 7 % 2
来源：http://lsh.zhaomingkeji.xyz

C#:   7 / 2; 7 % 2
来源：http://wgb.hesvh.cn

[A06] 字符串转数字
来源：http://zhe.sufxvd.cn

Py:   int("42"); float("3.14")
来源：http://owi.yuanzhike.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wll.bjfxy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wnt.yangfankeji.com

TS:   parseInt("42", 10); Number("42")
来源：http://pct.fanxiaobao.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kgb.yueranfly.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yhb.yuanzhike.top

Ruby: "42".to_i; "3.14".to_f
来源：http://puw.jinqigufen.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fzq.havefunace.top

[A07] 数字转字符串
来源：http://uvj.gzhubu.top

Py:   str(42)
来源：http://rnd.jinqigfzy.top

PHP:  (string) 42; strval(42)
来源：http://hmq.redwolf501.top

JS:   String(42); (42).toString()
来源：http://deu.hongshengwenyu.top

TS:   String(42)
来源：http://kxb.zdbjq.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zci.jianghu66.top

Go:   strconv.Itoa(42)
来源：http://bth.guowangkeji.top

Ruby: 42.to_s
来源：http://tox.zycfv.cn

C#:   42.ToString()
来源：http://cza.haohaochexian.top

[A08] 取整与四舍五入
来源：http://iou.cheryme.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mbh.jqgfzy.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rnt.hongshengwenyu.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://njl.hnxiangtu.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rha.hesvh.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://sax.yuanzhike.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cqq.sweek.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://lpo.zhengqikj.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://viq.gotoacloud.top

[A09] 绝对值与最大最小值
来源：http://smd.hammf.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nnw.jinqigfzy.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://igc.birdmap.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://iho.cucudq.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://agt.gaohongyu789.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://iug.jinqigufen.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ecj.cashguo.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://uuz.sweek.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://swd.hnqzz.top

[A10] 生成随机数
来源：http://lom.xziqi.cn

Py:   import random; random.randint(1, 100)
来源：http://vnn.ywan-chungtsiang.top

PHP:  random_int(1, 100);
来源：http://loh.nanxinkj.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sew.pengpengdd.cyou

TS:   Math.floor(Math.random() * 100) + 1
来源：http://saq.guowangkeji.top

Java: new Random().nextInt(100) + 1
来源：http://mqt.fanxiaobao.xyz

Go:   rand.Intn(100) + 1               // math/rand
来源：http://bxp.0kj1m.cn

Ruby: rand(1..100)
来源：http://dad.dashuyun.cn

C#:   new Random().Next(1, 101)
来源：http://zkh.fengsongda.top

[A11] 条件表达式（三元）
来源：http://kzn.dianchejie.cn

Py:   "yes" if x > 0 else "no"
来源：http://dqa.nwbrower.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://pam.fzhhl.top

JS:   x > 0 ? "yes" : "no"
来源：http://eax.zhoulong.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://dpp.cqqwz.cn

Java: x > 0 ? "yes" : "no"
来源：http://daz.sjlbkw.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ylw.wangshuangyany.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://vsd.yj20258888.top

C#:   x > 0 ? "yes" : "no"
来源：http://wdd.fanxiaobao.xyz

[A12] 字符串插值 / 格式化
来源：http://iiz.snrcjt.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mga.fktsv.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://sls.daria6918.cn

JS:   `Hello, ${name}!`
来源：http://zyc.jqgufenzy.top

TS:   `Hello, ${name}!`
来源：http://qtw.wangdashe.top

Java: "Hello, %s!".formatted(name)
来源：http://adh.zhongyouzk.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://prt.nwbrower.top

Ruby: "Hello, #{name}!"
来源：http://how.guowangkeji.top

C#:   $"Hello, {name}!"
来源：http://bgt.smart0.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://wgw.cashguo.top

Py:   "第一行\n第二行"
来源：http://cwy.guowangkeji.top

PHP:  "第一行\n第二行"
来源：http://cme.316326.xyz

JS:   "第一行\n第二行"
来源：http://zhy.hammf.cn

TS:   "第一行\n第二行"
来源：http://ije.xinyue.icu

Java: "第一行\n第二行"
来源：http://ovo.daxiang520.top

Go:   "第一行\n第二行"
来源：http://hxq.xziqi.cn

Ruby: "第一行\n第二行"
来源：http://caz.zhongyouzk.top

C#:   "第一行\n第二行"
来源：http://ydj.daxiang520.top

[A14] 注释写法
来源：http://llr.wangshuangyany.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://eno.jyoumei.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://psc.cucudq.cn

JS:   // 单行；/* 多行 */
来源：http://xep.shanyushiyangkeji.top

TS:   // 单行；/* 多行 */
来源：http://oya.ydzc1.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://par.shanyushiyangkeji.top

Go:   // 单行；/* 多行 */
来源：http://kri.wangdashe.top

Ruby: # 单行；=begin 多行 =end
来源：http://dym.hesvh.cn

C#:   // 单行；/* 多行 */
来源：http://xlp.yuxming.cn

[A15] 空值判断与默认值
来源：http://css.tian-w.cn

Py:   value = data or "默认值"
来源：http://jtw.gzhubu.top

PHP:  $value = $data ?? "默认值";
来源：http://pgx.jqgfzy.top

JS:   const value = data ?? "默认值";
来源：http://ogk.cashguo.top

TS:   const value = data ?? "默认值";
来源：http://irm.hammf.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://obs.yvedp.cn

Go:   if data == "" { data = "默认值" }
来源：http://lue.kuanghao11.cn

Ruby: value = data || "默认值"
来源：http://wgl.andypj.xyz

C#:   var value = data ?? "默认值";
来源：http://kch.xuanzx.com

[A16] 真假值判断规则
来源：http://poq.hnqzz.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nnl.ivvv.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hyn.fanxiaobao.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wdc.jinqigfzy.top

TS:   if (!x) {}
来源：http://wsr.wangshuangyany.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://sgz.pycfn.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nvr.sweek.top

Ruby: unless x            # nil 与 false 为假
来源：http://kgo.fehbvm.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://aqh.jinghuilouyu.cn

[A17] 位运算
来源：http://mlk.zhiwuduotai.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xcb.jinyuanbaomall.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jcv.chenlongwang.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ccl.nanxinkj.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jct.xuanzx.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gnu.fehbvm.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lnk.hywenlv.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wti.gogol.net.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pib.iojbl.cn

[A18] 字符与 ASCII 码互转
来源：http://mlb.yongpay.top

Py:   ord("A"); chr(65)
来源：http://ckk.jinyuanbaomall.cn

PHP:  ord("A"); chr(65)
来源：http://moa.hfpthk.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kvn.chenlongwang.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://llv.cheryme.top

Java: (int) 'A'; (char) 65
来源：http://qul.yuxming.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://flz.meibo888.top

Ruby: "A".ord; 65.chr
来源：http://clu.zdbjq.cn

C#:   (int)'A'; (char)65
来源：http://xbq.zhixingplan.top

[A19] 交换两个变量
来源：http://mbw.jinghuilouyu.cn

Py:   a, b = b, a
来源：http://iwb.svipenyu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://wrt.andypj.xyz

JS:   [a, b] = [b, a];
来源：http://sps.zhiwuduotai.top

TS:   [a, b] = [b, a];
来源：http://nfj.cashguo.top

Java: int t = a; a = b; b = t;
来源：http://mzw.fehbvm.com

Go:   a, b = b, a
来源：http://dth.zhengqikj.top

Ruby: a, b = b, a
来源：http://hdv.shanyushiyangkeji.top

C#:   (a, b) = (b, a);
来源：http://wnj.tianlin.xyz

[A20] 读取标准输入
来源：http://acb.nanxinkj.top

Py:   name = input("请输入：")
来源：http://kfe.sjlbkw.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://fxo.yongpay.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cfq.meibo888.top

TS:   // Node.js：readline 模块
来源：http://stm.ivvv.top

Java: new Scanner(System.in).nextLine()
来源：http://nev.shangyingyoupin.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gqn.nwbrower.top

Ruby: gets.chomp
来源：http://ldr.cheryme.top

C#:   Console.ReadLine();
来源：http://zcd.redwolf501.top

[A21] 保留指定小数位输出
来源：http://zst.ehwqpu.com

Py:   f"{3.14159:.2f}"
来源：http://tgk.jinqigfzy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wwj.yongpay.top

JS:   (3.14159).toFixed(2)
来源：http://jce.gaohongyu789.top

TS:   (3.14159).toFixed(2)
来源：http://ocg.vehdjk.com

Java: String.format("%.2f", 3.14159)
来源：http://bkw.smart0.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nrh.316326.xyz

Ruby: format("%.2f", 3.14159)
来源：http://psq.fktsv.cn

C#:   3.14159.ToString("F2")
来源：http://qtb.guannengcc.top

[A22] 获取字符串长度
来源：http://mxr.hfpthk.cn

Py:   len(s)
来源：http://oqx.wangdashe.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sps.pycfn.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hvj.epnwcf.com

TS:   s.length
来源：http://rdt.shanyushiyangkeji.top

Java: s.length()
来源：http://nhf.yueranfly.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hnb.kuanghao11.cn

Ruby: s.length
来源：http://kgr.xziqi.cn

C#:   s.Length
来源：http://hlj.yangfankeji.com

[A23] 大小写转换
来源：http://xdq.daxiang520.top

Py:   s.upper(); s.lower(); s.title()
来源：http://hsr.aibaodan.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ojs.redwolf501.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://aug.xziqi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jqr.hfpthk.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gik.fzhhl.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vhv.dashuyun.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://npg.zycfv.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://cbo.fehbvm.com

[A24] 去除首尾空白
来源：http://nxu.hywenlv.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nza.sysykeji.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mhp.guowangkeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pjy.hnxiangtu.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lfy.jinyuanbaomall.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wyk.epnwcf.com

Go:   strings.TrimSpace(s)
来源：http://ohw.shuidangran.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://imu.gogol.net.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mlq.dashuyun.cn

[A25] 字符串比较
来源：http://pec.uphjek.com

Py:   s1 == s2; s1 != s2
来源：http://vya.zycfv.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://irv.iojbl.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wfq.hnqzz.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xxh.ywan-chungtsiang.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://tuk.vehdjk.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xvx.cdnleiting.top

Ruby: s1 == s2; s1 <=> s2
来源：http://fum.9152youxi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mar.cucudq.cn

[A26] 类型转换总览
来源：http://mmi.fktsv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pbr.zhijiandao.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://erm.jianghu66.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bsl.sjlbkw.cn

TS:   Number() String() Boolean() x as number
来源：http://xny.fktsv.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kmc.chenlongwang.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hcr.kuanghao11.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://plt.9152youxi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gag.wangshuangyany.cn

================================================================================
来源：http://mcd.bbcook.cn

B. 流程控制
来源：http://xej.wangshuangyany.cn

================================================================================
来源：http://agx.nanxinkj.top

[B01] 条件判断 if / else
来源：http://iuv.chenzaomai.com

Py:   result = "正" if x > 0 else "非正"
来源：http://agc.cdnleiting.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gch.jqgfzy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hxt.hammf.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pnf.fzhhl.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://hbl.xziqi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ujj.yongpay.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ros.zycfv.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lja.0kj1m.cn

[B02] 多分支 else if / elif
来源：http://ksg.nwbrower.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wdy.yj20258.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bqf.yj202588.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ecu.sweek.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ccf.jianghu66.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sqp.aizwys.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ghw.fengsongda.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nvv.316326.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vqb.hywenlv.cn

[B03] switch / match / case
来源：http://apz.mhx1999.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tdu.jinghuilouyu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jgm.jiagoushi.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uyi.jinghuilouyu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eri.ivvv.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://aqg.chenlongwang.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dng.birdmap.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://och.jiagoushi.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://twu.ivvv.top

[B04] for 计数循环
来源：http://fzl.hammf.cn

Py:   for i in range(10): print(i)
来源：http://yuj.316326.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://umv.shanyushiyangtech.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kup.wangdashe.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yrz.52xcode.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vyh.sjlbkw.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://quf.tanke756.top

Ruby: 10.times { |i| puts i }
来源：http://rsl.xylfe.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ljp.hesvh.cn

[B05] 遍历数组 / 列表
来源：http://nek.xuetiantiany.cn

Py:   for item in arr: print(item)
来源：http://jnr.fehbvm.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dkz.jyoumei.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qrv.shuidangran.top

TS:   for (const item of arr) { console.log(item); }
来源：http://edo.316326.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://ndw.aizwys.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qpi.wangdashe.top

Ruby: arr.each { |item| puts item }
来源：http://rvo.mhx1999.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xrf.0kj1m.cn

[B06] 遍历字典 / 对象
来源：http://ueg.ehwqpu.com

Py:   for k, v in d.items(): print(k, v)
来源：http://hbk.gogol.net.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qqs.xuanzx.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mbr.jianghu66.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fsj.xziqi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lqp.52xcode.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://swt.hnqzz.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vni.zycfv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://doc.ctjpmb.com

[B07] while 循环
来源：http://rgg.yj20258.top

Py:   while i < 10: i += 1
来源：http://yva.cheryme.top

PHP:  while ($i < 10) { $i++; }
来源：http://bub.cdnleiting.top

JS:   while (i < 10) { i++; }
来源：http://jjy.9152youxi.cn

TS:   while (i < 10) { i++; }
来源：http://pcc.dianchejie.cn

Java: while (i < 10) { i++; }
来源：http://twy.xuetiantiany.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cxy.jqgufenzy.top

Ruby: while i < 10; i += 1; end
来源：http://iqg.jinyuanbaomall.cn

C#:   while (i < 10) { i++; }
来源：http://ouz.meibo888.top

[B08] do-while（至少执行一次）
来源：http://msr.mhx1999.top

Py:   # 无 do-while：用 while True + break
来源：http://czw.yuanzhike.top

PHP:  do { $i++; } while ($i < 10);
来源：http://obd.bjfxy.top

JS:   do { i++; } while (i < 10);
来源：http://lov.aibaodan.cn

TS:   do { i++; } while (i < 10);
来源：http://org.yfazqb.com

Java: do { i++; } while (i < 10);
来源：http://meb.ydjk.org.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ivh.cdnleiting.top

Ruby: begin; i += 1; end while i < 10
来源：http://pwb.fktsv.cn

C#:   do { i++; } while (i < 10);
来源：http://upe.zhongyouzk.top

[B09] break 与 continue
来源：http://cyi.hywenlv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zkw.chenjidiqi.icu

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hgo.sufxvd.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zel.shangyingyoupin.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://del.ybcxt.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iiy.andypj.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cfk.guannengcc.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zrk.xingfuxueyuan.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ctk.epnwcf.com

[B10] 遍历同时拿索引
来源：http://qop.ehwqpu.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ldq.xingfuxueyuan.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xbl.yfazqb.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ldh.jinqigufen.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yhx.ppjwa.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xei.fehbvm.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hnn.yj202588.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qts.yvedp.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wjo.jinyuanbaomall.cn

[B11] 生成数字序列 / 区间
来源：http://ziw.yj202588.top

Py:   list(range(0, 10, 2))
来源：http://rnl.fzhhl.top

PHP:  range(0, 10, 2);
来源：http://uut.pengpengdd.cyou

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fov.cdnleiting.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://msv.smart0.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lsh.dianchejie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ieb.ywan-chungtsiang.top

Ruby: (0...10).step(2).to_a
来源：http://idw.kuanghao11.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uue.zhengqikj.top

[B12] 跳出多层循环
来源：http://fbv.svipenyu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ulu.316326.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://ere.jianghu66.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blm.jianghu66.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tik.ydjk.org.cn


<!-- 参考信息 -->