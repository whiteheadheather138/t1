代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tta.jiagoushi.top

[A07] 数字转字符串
来源：http://wiq.yuanzhike.top

Py:   str(42)
来源：http://wvs.hnqzz.top

PHP:  (string) 42; strval(42)
来源：http://eha.mhx1999.top

JS:   String(42); (42).toString()
来源：http://ybx.ydzc1.top

TS:   String(42)
来源：http://mge.yj202588.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://yag.bjfxy.top

Go:   strconv.Itoa(42)
来源：http://rjh.shuidangran.top

Ruby: 42.to_s
来源：http://fyp.ivvv.top

C#:   42.ToString()
来源：http://hjy.mhx1999.top

[A08] 取整与四舍五入
来源：http://nas.sjlbkw.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vtn.316326.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dbu.tianlin.xyz

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zdg.tanke756.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zte.xylfe.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hdn.0kj1m.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wyy.ywan-chungtsiang.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://mjq.xylfe.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hni.yanxiufei.cn

[A09] 绝对值与最大最小值
来源：http://ets.tanke756.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://olq.nanxinkj.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qkn.xziqi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hco.cucudq.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nrm.meibo888.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://iqk.tian-w.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dgk.xingfuxueyuan.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tde.cashguo.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bki.vqdsnc.cn

[A10] 生成随机数
来源：http://bgu.wangdashe.top

Py:   import random; random.randint(1, 100)
来源：http://cai.aizwys.cn

PHP:  random_int(1, 100);
来源：http://gey.kuanghao11.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://pgv.hcnkem.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://tal.cucudq.cn

Java: new Random().nextInt(100) + 1
来源：http://ecd.ctjpmb.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://and.jyoumei.cn

Ruby: rand(1..100)
来源：http://gcb.ctjpmb.com

C#:   new Random().Next(1, 101)
来源：http://sgk.xziqi.cn

[A11] 条件表达式（三元）
来源：http://fys.nwbrower.top

Py:   "yes" if x > 0 else "no"
来源：http://hlr.jyoumei.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://tqt.jyoumei.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qgk.hfpthk.cn

TS:   x > 0 ? "yes" : "no"
来源：http://vgy.cqqwz.cn

Java: x > 0 ? "yes" : "no"
来源：http://hbb.ydzc1.top

Go:   // 无三元运算符，需用 if 语句
来源：http://mab.fzhhl.top

Ruby: x > 0 ? "yes" : "no"
来源：http://mdd.jlsjyb.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ibt.zhoulong.xyz

[A12] 字符串插值 / 格式化
来源：http://pga.vqdsnc.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://low.yj202588.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uoh.shanyushiyangkeji.top

JS:   `Hello, ${name}!`
来源：http://cmt.jqgufenzy.top

TS:   `Hello, ${name}!`
来源：http://abr.hfpthk.cn

Java: "Hello, %s!".formatted(name)
来源：http://aap.cqqwz.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://quv.vehdjk.com

Ruby: "Hello, #{name}!"
来源：http://gvi.nanxinkj.top

C#:   $"Hello, {name}!"
来源：http://bvk.daxiang520.top

[A13] 多行字符串（练习 \n 转义）
来源：http://hqn.jyoumei.cn

Py:   "第一行\n第二行"
来源：http://stb.pycfn.com

PHP:  "第一行\n第二行"
来源：http://aqz.gaohongyu789.top

JS:   "第一行\n第二行"
来源：http://mmf.gogol.net.cn

TS:   "第一行\n第二行"
来源：http://kon.yanxiufei.cn

Java: "第一行\n第二行"
来源：http://dpz.hnxiangtu.top

Go:   "第一行\n第二行"
来源：http://rma.hongshengwenyu.top

Ruby: "第一行\n第二行"
来源：http://ilm.shanyushiyangkeji.top

C#:   "第一行\n第二行"
来源：http://ytr.redwolf501.top

[A14] 注释写法
来源：http://xmq.tian-w.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://rts.zhoulong.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://ugt.fanxiaobao.xyz

JS:   // 单行；/* 多行 */
来源：http://ujh.havefunace.top

TS:   // 单行；/* 多行 */
来源：http://wgo.sufxvd.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://jor.xziqi.cn

Go:   // 单行；/* 多行 */
来源：http://rep.daria6918.cn

Ruby: # 单行；=begin 多行 =end
来源：http://uno.shzxlz.cn

C#:   // 单行；/* 多行 */
来源：http://zkb.ybcxt.top

[A15] 空值判断与默认值
来源：http://nri.c1oappe.top

Py:   value = data or "默认值"
来源：http://pvp.sysykeji.top

PHP:  $value = $data ?? "默认值";
来源：http://wzn.xingfuxueyuan.xyz

JS:   const value = data ?? "默认值";
来源：http://zqr.smart0.xyz

TS:   const value = data ?? "默认值";
来源：http://kyn.guannengcc.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kix.sufxvd.cn

Go:   if data == "" { data = "默认值" }
来源：http://erh.daria6918.cn

Ruby: value = data || "默认值"
来源：http://poa.yueranfly.top

C#:   var value = data ?? "默认值";
来源：http://niu.ybcxt.top

[A16] 真假值判断规则
来源：http://rtz.nwbrower.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wbk.wangdashe.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dng.hammf.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xag.hnxiangtu.top

TS:   if (!x) {}
来源：http://vug.svipenyu.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cxs.chenlongwang.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ukz.bbcook.cn

Ruby: unless x            # nil 与 false 为假
来源：http://rjd.bjfxy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kik.shuidangran.top

[A17] 位运算
来源：http://vjz.52xcode.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qrt.shanyushiyangtech.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pzu.cqqwz.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gfu.zycfv.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lkf.aibaodan.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nbu.ydzc1.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://olz.fzhhl.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nbr.zycfv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gob.tianlin.xyz

[A18] 字符与 ASCII 码互转
来源：http://vnk.shangyingyoupin.top

Py:   ord("A"); chr(65)
来源：http://als.redwolf501.top

PHP:  ord("A"); chr(65)
来源：http://uyu.bjfxy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uqk.yonumen.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iyc.hcnkem.com

Java: (int) 'A'; (char) 65
来源：http://hry.chenlongwang.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lag.hcnkem.com

Ruby: "A".ord; 65.chr
来源：http://kmz.zhoulong.xyz

C#:   (int)'A'; (char)65
来源：http://soe.zhijiandao.cn

[A19] 交换两个变量
来源：http://sdd.sxryk.cn

Py:   a, b = b, a
来源：http://cnd.tianlin.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://wxm.birdmap.top

JS:   [a, b] = [b, a];
来源：http://nrl.zhoulong.xyz

TS:   [a, b] = [b, a];
来源：http://psu.yfazqb.com

Java: int t = a; a = b; b = t;
来源：http://ljm.shanyushiyangkeji.top

Go:   a, b = b, a
来源：http://wzx.vehdjk.com

Ruby: a, b = b, a
来源：http://xfa.chenzaomai.com

C#:   (a, b) = (b, a);
来源：http://zly.jqgfzy.top

[A20] 读取标准输入
来源：http://ktk.gaohongyu789.top

Py:   name = input("请输入：")
来源：http://mex.daxiang520.top

PHP:  $name = trim(fgets(STDIN));
来源：http://mel.jiagoushi.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vpp.gogol.net.cn

TS:   // Node.js：readline 模块
来源：http://khh.yj202588.top

Java: new Scanner(System.in).nextLine()
来源：http://ngh.tian-w.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://urq.feifeiyinyue.top

Ruby: gets.chomp
来源：http://dts.gotoacloud.top

C#:   Console.ReadLine();
来源：http://isp.zdbjq.cn

[A21] 保留指定小数位输出
来源：http://wci.hfpthk.cn

Py:   f"{3.14159:.2f}"
来源：http://hah.zycfv.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://img.xinyue.icu

JS:   (3.14159).toFixed(2)
来源：http://vbu.yj202588.top

TS:   (3.14159).toFixed(2)
来源：http://gqm.nwbrower.top

Java: String.format("%.2f", 3.14159)
来源：http://xdy.pengpengdd.cyou

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rhi.hywenlv.cn

Ruby: format("%.2f", 3.14159)
来源：http://qbb.xuetiantiany.cn

C#:   3.14159.ToString("F2")
来源：http://yif.c1oappe.top

[A22] 获取字符串长度
来源：http://yev.svipenyu.cn

Py:   len(s)
来源：http://yuk.sufxvd.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dfc.bbcook.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jer.cashguo.top

TS:   s.length
来源：http://rqr.yuanzhike.top

Java: s.length()
来源：http://tfx.ctjpmb.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gsj.ydzc1.top

Ruby: s.length
来源：http://pcm.jinghuilouyu.cn

C#:   s.Length
来源：http://von.cdnleiting.top

[A23] 大小写转换
来源：http://zfk.vehdjk.com

Py:   s.upper(); s.lower(); s.title()
来源：http://elf.hammf.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vga.hnxiangtu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sdf.epnwcf.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sms.cashguo.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jjt.zdqjudy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wsl.uphjek.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pub.meibo888.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ytz.ydjk.org.cn

[A24] 去除首尾空白
来源：http://jqp.hammf.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cfu.daria6918.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vbs.cdnleiting.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tbs.chenzaomai.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yvy.pycfn.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hoa.316326.xyz

Go:   strings.TrimSpace(s)
来源：http://vif.guannengcc.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mdr.ehwqpu.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://uxk.bjfxy.top

[A25] 字符串比较
来源：http://ylv.pengpengdd.cyou

Py:   s1 == s2; s1 != s2
来源：http://ukk.aizwys.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jke.0kj1m.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://czz.9152youxi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pml.52xcode.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nvt.gotoacloud.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://osq.52xcode.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ura.yuxming.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wyw.gotoacloud.top

[A26] 类型转换总览
来源：http://hwi.zhoulong.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dba.0kj1m.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://aqk.bjfxy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://auc.jianghu66.top

TS:   Number() String() Boolean() x as number
来源：http://uio.tianlin.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rmj.cucudq.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ghz.yonumen.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://qif.xuanzx.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zcn.ybcxt.top

================================================================================
来源：http://wnc.sysykeji.top

B. 流程控制
来源：http://idn.c1oappe.top

================================================================================
来源：http://iio.tianlin.xyz

[B01] 条件判断 if / else
来源：http://zwz.yongpay.top

Py:   result = "正" if x > 0 else "非正"
来源：http://xsa.zycfv.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://czf.daria6918.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mir.shuidangran.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://knz.jqgfzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://sny.fktsv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zmz.yj20258888.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kbg.iojbl.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://csm.guowangkeji.top

[B02] 多分支 else if / elif
来源：http://ffr.zhixingplan.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://opw.yuanzhike.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zya.fengsongda.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nxp.zhiwuduotai.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ytz.wangshuangyany.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://klq.fanxiaobao.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gdy.hnqzz.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ayi.jinqigufen.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hyz.fanxiaobao.xyz

[B03] switch / match / case
来源：http://kas.meibo888.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jik.chenlongwang.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ymi.epnwcf.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gux.jianghu66.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qvx.sufxvd.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nhx.xuanzx.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://iuh.daxiang520.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lpe.hywenlv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mxz.shangyingyoupin.top

[B04] for 计数循环
来源：http://ezz.jinghuilouyu.cn

Py:   for i in range(10): print(i)
来源：http://qgj.pengpengdd.cyou

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lfr.iojbl.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lee.shanyushiyangtech.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qaf.fzhhl.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fkb.zhiwuduotai.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://aqc.cucudq.cn

Ruby: 10.times { |i| puts i }
来源：http://drk.sufxvd.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nwp.52xcode.cn

[B05] 遍历数组 / 列表
来源：http://sgn.ydjk.org.cn

Py:   for item in arr: print(item)
来源：http://djo.nanxuanxn.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ibj.zhiwuduotai.top

JS:   for (const item of arr) { console.log(item); }
来源：http://eqq.hywenlv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cvd.fehbvm.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://wsf.jinghuilouyu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zxk.nanxinkj.top

Ruby: arr.each { |item| puts item }
来源：http://gwo.epnwcf.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lde.xinyue.icu

[B06] 遍历字典 / 对象
来源：http://fgl.xingfuxueyuan.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://brq.gaohongyu789.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lvt.nanxuanxn.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ibw.sxryk.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xbj.smart0.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ftk.sysykeji.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kqf.hnxiangtu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://guc.epnwcf.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qds.vqdsnc.cn

[B07] while 循环
来源：http://vqv.fehbvm.com

Py:   while i < 10: i += 1
来源：http://wmd.nanxinkj.top

PHP:  while ($i < 10) { $i++; }
来源：http://xsa.gzhubu.top

JS:   while (i < 10) { i++; }
来源：http://cdh.kuanghao11.cn

TS:   while (i < 10) { i++; }
来源：http://xqp.yfazqb.com

Java: while (i < 10) { i++; }
来源：http://aay.jyoumei.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bsf.smart0.xyz

Ruby: while i < 10; i += 1; end
来源：http://qji.yangfankeji.com

C#:   while (i < 10) { i++; }
来源：http://pns.zhijiandao.cn

[B08] do-while（至少执行一次）
来源：http://bnp.cqqwz.cn

Py:   # 无 do-while：用 while True + break
来源：http://btg.ivvv.top

PHP:  do { $i++; } while ($i < 10);
来源：http://sqe.bbcook.cn

JS:   do { i++; } while (i < 10);
来源：http://cmk.zdqjudy.top

TS:   do { i++; } while (i < 10);
来源：http://vay.nwbrower.top

Java: do { i++; } while (i < 10);
来源：http://rnp.0kj1m.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rnt.jiagoushi.top

Ruby: begin; i += 1; end while i < 10
来源：http://jaf.nanxuanxn.top

C#:   do { i++; } while (i < 10);
来源：http://kzi.hnqzz.top

[B09] break 与 continue
来源：http://nhy.ywan-chungtsiang.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ups.vehdjk.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gay.xylfe.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xcu.hnxiangtu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kvh.daxiang520.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cwe.xuetiantiany.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ysi.xziqi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fwk.ydzc1.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nti.gogol.net.cn

[B10] 遍历同时拿索引
来源：http://ewb.snrcjt.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mth.jlsjyb.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oas.jinyuanbaomall.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ttj.aizwys.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ren.hnqzz.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bmq.hfpthk.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jed.redwolf501.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nik.nanxuanxn.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ywc.xinyue.icu

[B11] 生成数字序列 / 区间
来源：http://jwi.hnqzz.top

Py:   list(range(0, 10, 2))
来源：http://cwj.daxiang520.top

PHP:  range(0, 10, 2);
来源：http://acr.cashguo.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uxq.yj202588.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mos.jqgufenzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jdr.havefunace.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rag.meibo888.top

Ruby: (0...10).step(2).to_a
来源：http://xui.uphjek.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rwx.52xcode.cn

[B12] 跳出多层循环
来源：http://gcu.daria6918.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xmt.fanxiaobao.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://lxl.vqdsnc.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kaj.haohaochexian.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jjf.hysaishi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qop.shuidangran.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kss.zdbjq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rot.mhx1999.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fxr.haohaochexian.top

[B13] 判断是否为数字
来源：http://nes.epnwcf.com

Py:   isinstance(x, (int, float))
来源：http://omh.jinqigufen.top

PHP:  is_numeric($x)
来源：http://qtj.zhengqikj.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zuc.dianchejie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rvj.yangfankeji.com

Java: x instanceof Number
来源：http://hpm.yonumen.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ckg.jqgfzy.top

Ruby: x.is_a?(Numeric)
来源：http://rau.zhaomingkeji.xyz


<!-- 参考信息 -->