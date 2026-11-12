代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://awb.yueranfly.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://puf.xuetiantiany.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://avy.jiagoushi.top

Ruby: "42".to_i; "3.14".to_f
来源：http://gzh.yanxiufei.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rtd.cashguo.top

[A07] 数字转字符串
来源：http://ost.chenlongwang.top

Py:   str(42)
来源：http://iah.sjlbkw.cn

PHP:  (string) 42; strval(42)
来源：http://muw.gzhubu.top

JS:   String(42); (42).toString()
来源：http://lvg.yueranfly.top

TS:   String(42)
来源：http://gsq.ehwqpu.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://yev.ctjpmb.com

Go:   strconv.Itoa(42)
来源：http://vev.feifeiyinyue.top

Ruby: 42.to_s
来源：http://qqh.wangdashe.top

C#:   42.ToString()
来源：http://dkk.yanxiufei.cn

[A08] 取整与四舍五入
来源：http://npm.ehwqpu.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cny.meibo888.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nwd.hnxiangtu.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lcd.ydzc1.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://riu.yangfankeji.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vyv.vqdsnc.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zyz.vqdsnc.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://tul.yfazqb.com

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://pun.hnqzz.top

[A09] 绝对值与最大最小值
来源：http://ehu.ctjpmb.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://owy.fengsongda.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fvp.shanyushiyangtech.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://duy.cucudq.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://vko.shuidangran.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://veq.gaohongyu789.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://jbd.dashuyun.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wqu.ywan-chungtsiang.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://vpr.tarul.cn

[A10] 生成随机数
来源：http://uod.uphjek.com

Py:   import random; random.randint(1, 100)
来源：http://wqt.sysykeji.top

PHP:  random_int(1, 100);
来源：http://kix.xylfe.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ufv.mhx1999.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://cdi.smart0.xyz

Java: new Random().nextInt(100) + 1
来源：http://iow.yanxiufei.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ief.vqdsnc.cn

Ruby: rand(1..100)
来源：http://cre.redwolf501.top

C#:   new Random().Next(1, 101)
来源：http://qrg.fengsongda.top

[A11] 条件表达式（三元）
来源：http://lut.sjlbkw.cn

Py:   "yes" if x > 0 else "no"
来源：http://glx.chenlongwang.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://cif.c1oappe.top

JS:   x > 0 ? "yes" : "no"
来源：http://gyr.jinqigufen.top

TS:   x > 0 ? "yes" : "no"
来源：http://lfs.yj202588.top

Java: x > 0 ? "yes" : "no"
来源：http://klh.fanxiaobao.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://emp.shanyushiyangkeji.top

Ruby: x > 0 ? "yes" : "no"
来源：http://hrq.chenjidiqi.icu

C#:   x > 0 ? "yes" : "no"
来源：http://puo.yongpay.top

[A12] 字符串插值 / 格式化
来源：http://bxp.guowangkeji.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://jqr.nanxinkj.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mzc.sjlbkw.cn

JS:   `Hello, ${name}!`
来源：http://tnn.daxiang520.top

TS:   `Hello, ${name}!`
来源：http://qre.yvedp.cn

Java: "Hello, %s!".formatted(name)
来源：http://obg.fengsongda.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hii.uphjek.com

Ruby: "Hello, #{name}!"
来源：http://slg.sjlbkw.cn

C#:   $"Hello, {name}!"
来源：http://fys.zdqjudy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://lvj.c1oappe.top

Py:   "第一行\n第二行"
来源：http://nne.yj20258.top

PHP:  "第一行\n第二行"
来源：http://odd.pengpengdd.cyou

JS:   "第一行\n第二行"
来源：http://cwo.hesvh.cn

TS:   "第一行\n第二行"
来源：http://hws.zdbjq.cn

Java: "第一行\n第二行"
来源：http://oap.bbcook.cn

Go:   "第一行\n第二行"
来源：http://xob.mhx1999.top

Ruby: "第一行\n第二行"
来源：http://ojo.jinghuilouyu.cn

C#:   "第一行\n第二行"
来源：http://uqc.c1oappe.top

[A14] 注释写法
来源：http://bmz.bbcook.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://awr.bbcook.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://fyu.ppjwa.cn

JS:   // 单行；/* 多行 */
来源：http://xbz.zhengqikj.top

TS:   // 单行；/* 多行 */
来源：http://jwe.cdnleiting.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hsv.epnwcf.com

Go:   // 单行；/* 多行 */
来源：http://dlu.shanyushiyangtech.top

Ruby: # 单行；=begin 多行 =end
来源：http://xvu.tanke756.top

C#:   // 单行；/* 多行 */
来源：http://ajg.zhixingplan.top

[A15] 空值判断与默认值
来源：http://qfa.ppjwa.cn

Py:   value = data or "默认值"
来源：http://mfq.birdmap.top

PHP:  $value = $data ?? "默认值";
来源：http://hel.ydzc1.top

JS:   const value = data ?? "默认值";
来源：http://brz.zhixingplan.top

TS:   const value = data ?? "默认值";
来源：http://dub.zhengqikj.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://egi.ctjpmb.com

Go:   if data == "" { data = "默认值" }
来源：http://edx.shzxlz.cn

Ruby: value = data || "默认值"
来源：http://fkk.sxryk.cn

C#:   var value = data ?? "默认值";
来源：http://zmu.jqgufenzy.top

[A16] 真假值判断规则
来源：http://whe.bbcook.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pmb.sufxvd.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://foh.nwbrower.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://qvs.xuanzx.com

TS:   if (!x) {}
来源：http://unl.tarul.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ftc.jinqigfzy.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nob.nanxuanxn.top

Ruby: unless x            # nil 与 false 为假
来源：http://lxf.uphjek.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xoe.yonumen.top

[A17] 位运算
来源：http://qys.hysaishi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qsg.c1oappe.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://adh.hongshengwenyu.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tqs.yuxming.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zlz.zhengqikj.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://adh.jinyuanbaomall.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://apn.vehdjk.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ajd.birdmap.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nzt.tarul.cn

[A18] 字符与 ASCII 码互转
来源：http://yrd.zycfv.cn

Py:   ord("A"); chr(65)
来源：http://ogq.jinqigufen.top

PHP:  ord("A"); chr(65)
来源：http://mem.zhaomingkeji.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://joy.ivvv.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iaj.yj20258.top

Java: (int) 'A'; (char) 65
来源：http://rov.pengpengdd.cyou

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fhp.chenzaomai.com

Ruby: "A".ord; 65.chr
来源：http://upc.nanxuanxn.top

C#:   (int)'A'; (char)65
来源：http://twi.yfazqb.com

[A19] 交换两个变量
来源：http://gvh.wangdashe.top

Py:   a, b = b, a
来源：http://rgc.hfpthk.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://bcs.jinghuilouyu.cn

JS:   [a, b] = [b, a];
来源：http://rlq.kuanghao11.cn

TS:   [a, b] = [b, a];
来源：http://zoe.zhengqikj.top

Java: int t = a; a = b; b = t;
来源：http://cii.yuxming.cn

Go:   a, b = b, a
来源：http://lqv.fanxiaobao.xyz

Ruby: a, b = b, a
来源：http://mts.nanxuanxn.top

C#:   (a, b) = (b, a);
来源：http://sid.bjfxy.top

[A20] 读取标准输入
来源：http://auv.nanxinkj.top

Py:   name = input("请输入：")
来源：http://hkc.daxiang520.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ctj.ybcxt.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ati.jqgfzy.top

TS:   // Node.js：readline 模块
来源：http://ico.zhaomingkeji.xyz

Java: new Scanner(System.in).nextLine()
来源：http://grc.svipenyu.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xlb.shangyingyoupin.top

Ruby: gets.chomp
来源：http://hoc.hammf.cn

C#:   Console.ReadLine();
来源：http://mru.guannengcc.top

[A21] 保留指定小数位输出
来源：http://dzz.zdbjq.cn

Py:   f"{3.14159:.2f}"
来源：http://hrx.zhixingplan.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lxg.shuidangran.top

JS:   (3.14159).toFixed(2)
来源：http://cpz.tarul.cn

TS:   (3.14159).toFixed(2)
来源：http://qax.yj20258.top

Java: String.format("%.2f", 3.14159)
来源：http://ikp.xylfe.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ntg.yueranfly.top

Ruby: format("%.2f", 3.14159)
来源：http://etu.zycfv.cn

C#:   3.14159.ToString("F2")
来源：http://qmh.smart0.xyz

[A22] 获取字符串长度
来源：http://bmz.vqdsnc.cn

Py:   len(s)
来源：http://tgq.tian-w.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://drk.daxiang520.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rnt.hcnkem.com

TS:   s.length
来源：http://xib.yongpay.top

Java: s.length()
来源：http://jmq.hywenlv.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cmm.pycfn.com

Ruby: s.length
来源：http://ksm.gogol.net.cn

C#:   s.Length
来源：http://vvn.52xcode.cn

[A23] 大小写转换
来源：http://ngs.zdqjudy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://dtf.sjlbkw.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mqe.ydjk.org.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pyo.pycfn.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fud.jianghu66.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xba.sysykeji.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://emk.jqgufenzy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rjh.jqgufenzy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://gnu.aizwys.cn

[A24] 去除首尾空白
来源：http://erq.dashuyun.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ctb.nanxuanxn.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://czt.gaohongyu789.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nsx.dianchejie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aac.fanxiaobao.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tmu.xingfuxueyuan.xyz

Go:   strings.TrimSpace(s)
来源：http://tcj.gaohongyu789.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nfs.jinghuilouyu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xbx.yongpay.top

[A25] 字符串比较
来源：http://mrn.fehbvm.com

Py:   s1 == s2; s1 != s2
来源：http://wav.cucudq.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://olg.meibo888.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://eze.jianghu66.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://img.zhixingplan.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dvb.yj202588.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tmb.aizwys.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nwf.sysykeji.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://chm.aizwys.cn

[A26] 类型转换总览
来源：http://bza.hongshengwenyu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lza.jiagoushi.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zdb.feifeiyinyue.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ldm.aibaodan.cn

TS:   Number() String() Boolean() x as number
来源：http://scj.dianchejie.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://awv.ydzc1.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dvc.hnqzz.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://lop.yfazqb.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sec.hnxiangtu.top

================================================================================
来源：http://wca.gzhubu.top

B. 流程控制
来源：http://ovs.nwbrower.top

================================================================================
来源：http://qcu.zhengqikj.top

[B01] 条件判断 if / else
来源：http://yov.gzhubu.top

Py:   result = "正" if x > 0 else "非正"
来源：http://wgm.shangyingyoupin.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zou.zhaomingkeji.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://opy.ydjk.org.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zws.aizwys.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tlv.dashuyun.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zmo.wangshuangyany.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ewg.ywan-chungtsiang.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tjq.jinyuanbaomall.cn

[B02] 多分支 else if / elif
来源：http://hnj.quarkkingdee.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fzr.mhx1999.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bbb.hfpthk.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://flz.sysykeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fbv.vqdsnc.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ltn.sjlbkw.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vyf.hcnkem.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xqv.zhongyouzk.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kit.0kj1m.cn

[B03] switch / match / case
来源：http://rre.kuanghao11.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://znl.shangyingyoupin.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jft.cashguo.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mnu.shuidangran.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mrs.dashuyun.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qrd.yj202588.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uje.xinyue.icu

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zqj.tarul.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yxu.ppjwa.cn

[B04] for 计数循环
来源：http://eut.c1oappe.top

Py:   for i in range(10): print(i)
来源：http://zxf.fzhhl.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://icl.jinyuanbaomall.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lhw.hfpthk.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iyu.daxiang520.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://myy.ehwqpu.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zsh.yj202588.top

Ruby: 10.times { |i| puts i }
来源：http://yyd.yangfankeji.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://llb.yj202588.top

[B05] 遍历数组 / 列表
来源：http://pak.tianlin.xyz

Py:   for item in arr: print(item)
来源：http://vaa.yanxiufei.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qlb.xylfe.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hnn.chenlongwang.top

TS:   for (const item of arr) { console.log(item); }
来源：http://mtw.yj202588.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://utk.xuetiantiany.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://iou.dashuyun.cn

Ruby: arr.each { |item| puts item }
来源：http://cmt.vehdjk.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jyp.hongshengwenyu.top

[B06] 遍历字典 / 对象
来源：http://dcz.52xcode.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zmw.zhixingplan.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jkt.cucudq.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qos.jlsjyb.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hru.zdbjq.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xgh.jinqigufen.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oab.guannengcc.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://aow.shanyushiyangtech.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hdc.shangyingyoupin.top

[B07] while 循环
来源：http://pjf.tarul.cn

Py:   while i < 10: i += 1
来源：http://cya.vehdjk.com

PHP:  while ($i < 10) { $i++; }
来源：http://djc.tanke756.top

JS:   while (i < 10) { i++; }
来源：http://hus.guowangkeji.top

TS:   while (i < 10) { i++; }
来源：http://eqh.jianghu66.top

Java: while (i < 10) { i++; }
来源：http://lia.zdbjq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xtv.xziqi.cn

Ruby: while i < 10; i += 1; end
来源：http://nny.guowangkeji.top

C#:   while (i < 10) { i++; }
来源：http://hdr.wangdashe.top

[B08] do-while（至少执行一次）
来源：http://tzx.cashguo.top

Py:   # 无 do-while：用 while True + break
来源：http://xox.zdqjudy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://cse.zhaomingkeji.xyz

JS:   do { i++; } while (i < 10);
来源：http://nwo.redwolf501.top

TS:   do { i++; } while (i < 10);
来源：http://ncl.ivvv.top

Java: do { i++; } while (i < 10);
来源：http://rkp.fktsv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fqr.smart0.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://vcj.birdmap.top

C#:   do { i++; } while (i < 10);
来源：http://ptb.zhixingplan.top

[B09] break 与 continue
来源：http://naa.uphjek.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://akv.hongshengwenyu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rty.fengsongda.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nbm.svipenyu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nny.daxiang520.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lbl.ctjpmb.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dzg.yfazqb.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://efc.tianlin.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fkn.jinyuanbaomall.cn

[B10] 遍历同时拿索引
来源：http://vmf.epnwcf.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qoh.jinghuilouyu.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zbu.birdmap.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jnn.aizwys.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dsl.hywenlv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qum.hfpthk.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://iug.tianlin.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ssa.0kj1m.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://loh.jyoumei.cn

[B11] 生成数字序列 / 区间
来源：http://oat.hfpthk.cn

Py:   list(range(0, 10, 2))
来源：http://epy.fktsv.cn

PHP:  range(0, 10, 2);
来源：http://ywi.wangshuangyany.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://czt.jiagoushi.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bfb.zdbjq.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://omf.cdnleiting.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hqf.feifeiyinyue.top

Ruby: (0...10).step(2).to_a
来源：http://txf.vqdsnc.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ihd.9152youxi.cn

[B12] 跳出多层循环
来源：http://ldp.chenjidiqi.icu

Py:   # 无标签跳转：抽成函数用 return
来源：http://gbz.snrcjt.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gkx.gotoacloud.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gub.hfpthk.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://aik.guannengcc.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ylk.fengsongda.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bir.shzxlz.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kde.jiagoushi.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://eed.wangshuangyany.cn

[B13] 判断是否为数字
来源：http://hkb.guowangkeji.top

Py:   isinstance(x, (int, float))
来源：http://cex.sufxvd.cn

PHP:  is_numeric($x)
来源：http://pjn.xuanzx.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://okm.meibo888.top


<!-- 参考信息 -->