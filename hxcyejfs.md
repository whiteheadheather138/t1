代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://ypm.cucudq.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tgj.guannengcc.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://sil.chenzaomai.com

Ruby: "42".to_i; "3.14".to_f
来源：http://lcx.xylfe.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rtd.yj20258888.top

[A07] 数字转字符串
来源：http://ewr.yj20258.top

Py:   str(42)
来源：http://jcv.mhx1999.top

PHP:  (string) 42; strval(42)
来源：http://jvs.yongpay.top

JS:   String(42); (42).toString()
来源：http://yju.bbcook.cn

TS:   String(42)
来源：http://ysa.cheryme.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://pje.jinghuilouyu.cn

Go:   strconv.Itoa(42)
来源：http://byv.zhongyouzk.top

Ruby: 42.to_s
来源：http://szu.tanke756.top

C#:   42.ToString()
来源：http://qco.zhiwuduotai.top

[A08] 取整与四舍五入
来源：http://mbx.snrcjt.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cwj.fehbvm.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hhy.xuanzx.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://uvu.aibaodan.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://akb.zhixingplan.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rrw.daria6918.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mws.sxryk.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xzk.guowangkeji.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yqq.vqdsnc.cn

[A09] 绝对值与最大最小值
来源：http://ash.ctjpmb.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pvk.iojbl.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nep.sweek.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fdr.fzhhl.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bma.yangfankeji.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://nsx.birdmap.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pzv.yvedp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://imj.hywenlv.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rom.sjlbkw.cn

[A10] 生成随机数
来源：http://wqy.zhaomingkeji.xyz

Py:   import random; random.randint(1, 100)
来源：http://enw.jlsjyb.cn

PHP:  random_int(1, 100);
来源：http://kfx.shuidangran.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nhk.zhixingplan.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://oed.hammf.cn

Java: new Random().nextInt(100) + 1
来源：http://lnh.dianchejie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rzs.tianlin.xyz

Ruby: rand(1..100)
来源：http://pqt.kuanghao11.cn

C#:   new Random().Next(1, 101)
来源：http://bzq.zhixingplan.top

[A11] 条件表达式（三元）
来源：http://can.shzxlz.cn

Py:   "yes" if x > 0 else "no"
来源：http://ftz.gzhubu.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://kav.gogol.net.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ccw.zhijiandao.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ayn.wangshuangyany.cn

Java: x > 0 ? "yes" : "no"
来源：http://lpm.sjlbkw.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://bav.redwolf501.top

Ruby: x > 0 ? "yes" : "no"
来源：http://irp.wangshuangyany.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fxe.epnwcf.com

[A12] 字符串插值 / 格式化
来源：http://pvv.uphjek.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gbv.havefunace.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://jxq.ydjk.org.cn

JS:   `Hello, ${name}!`
来源：http://msf.andypj.xyz

TS:   `Hello, ${name}!`
来源：http://rnj.hnxiangtu.top

Java: "Hello, %s!".formatted(name)
来源：http://djv.daria6918.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://eqo.aizwys.cn

Ruby: "Hello, #{name}!"
来源：http://ocp.aibaodan.cn

C#:   $"Hello, {name}!"
来源：http://qps.smart0.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://wkz.shanyushiyangtech.top

Py:   "第一行\n第二行"
来源：http://upm.fehbvm.com

PHP:  "第一行\n第二行"
来源：http://rcb.wangdashe.top

JS:   "第一行\n第二行"
来源：http://flf.sysykeji.top

TS:   "第一行\n第二行"
来源：http://eao.bbcook.cn

Java: "第一行\n第二行"
来源：http://adj.haohaochexian.top

Go:   "第一行\n第二行"
来源：http://jlj.shuidangran.top

Ruby: "第一行\n第二行"
来源：http://ven.yanxiufei.cn

C#:   "第一行\n第二行"
来源：http://pne.redwolf501.top

[A14] 注释写法
来源：http://skv.cheryme.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://wyo.0kj1m.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://soj.hesvh.cn

JS:   // 单行；/* 多行 */
来源：http://mst.yuxming.cn

TS:   // 单行；/* 多行 */
来源：http://nyr.shangyingyoupin.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lwe.tianlin.xyz

Go:   // 单行；/* 多行 */
来源：http://cfd.jinqigufen.top

Ruby: # 单行；=begin 多行 =end
来源：http://wpd.0kj1m.cn

C#:   // 单行；/* 多行 */
来源：http://abd.fengsongda.top

[A15] 空值判断与默认值
来源：http://ljs.shanyushiyangkeji.top

Py:   value = data or "默认值"
来源：http://pzy.nwbrower.top

PHP:  $value = $data ?? "默认值";
来源：http://zgd.zdbjq.cn

JS:   const value = data ?? "默认值";
来源：http://xgz.dianchejie.cn

TS:   const value = data ?? "默认值";
来源：http://pif.52xcode.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hed.ywan-chungtsiang.top

Go:   if data == "" { data = "默认值" }
来源：http://psd.quarkkingdee.top

Ruby: value = data || "默认值"
来源：http://jkv.yongpay.top

C#:   var value = data ?? "默认值";
来源：http://nuf.shanyushiyangtech.top

[A16] 真假值判断规则
来源：http://xge.pycfn.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cgv.xuanzx.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dcf.tarul.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gfp.wangdashe.top

TS:   if (!x) {}
来源：http://hcw.yj20258888.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kzd.aizwys.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vgv.vqdsnc.cn

Ruby: unless x            # nil 与 false 为假
来源：http://cug.wangdashe.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bmw.gzhubu.top

[A17] 位运算
来源：http://jth.52xcode.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fma.tianlin.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wuy.fanxiaobao.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kbv.gogol.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gkr.ivvv.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qxh.ctjpmb.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vlo.gogol.net.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dlz.yfazqb.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bnh.chenzaomai.com

[A18] 字符与 ASCII 码互转
来源：http://prq.nwbrower.top

Py:   ord("A"); chr(65)
来源：http://yrv.c1oappe.top

PHP:  ord("A"); chr(65)
来源：http://mzm.bjfxy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://myz.quarkkingdee.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ntd.yvedp.cn

Java: (int) 'A'; (char) 65
来源：http://zvb.redwolf501.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nhj.wangdashe.top

Ruby: "A".ord; 65.chr
来源：http://rzc.aizwys.cn

C#:   (int)'A'; (char)65
来源：http://cit.zhaomingkeji.xyz

[A19] 交换两个变量
来源：http://ght.uphjek.com

Py:   a, b = b, a
来源：http://pkh.jinyuanbaomall.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://utg.ehwqpu.com

JS:   [a, b] = [b, a];
来源：http://jpe.vehdjk.com

TS:   [a, b] = [b, a];
来源：http://vma.yj202588.top

Java: int t = a; a = b; b = t;
来源：http://nbm.yj20258888.top

Go:   a, b = b, a
来源：http://jrj.aibaodan.cn

Ruby: a, b = b, a
来源：http://bmb.dashuyun.cn

C#:   (a, b) = (b, a);
来源：http://jsx.mhx1999.top

[A20] 读取标准输入
来源：http://lxm.cucudq.cn

Py:   name = input("请输入：")
来源：http://adc.chenjidiqi.icu

PHP:  $name = trim(fgets(STDIN));
来源：http://fsf.guannengcc.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gje.zhiwuduotai.top

TS:   // Node.js：readline 模块
来源：http://mtp.uphjek.com

Java: new Scanner(System.in).nextLine()
来源：http://pos.chenzaomai.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sis.gaohongyu789.top

Ruby: gets.chomp
来源：http://fgf.zhijiandao.cn

C#:   Console.ReadLine();
来源：http://dic.jianghu66.top

[A21] 保留指定小数位输出
来源：http://owz.ywan-chungtsiang.top

Py:   f"{3.14159:.2f}"
来源：http://djw.jianghu66.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lon.xinyue.icu

JS:   (3.14159).toFixed(2)
来源：http://ime.hongshengwenyu.top

TS:   (3.14159).toFixed(2)
来源：http://tar.ppjwa.cn

Java: String.format("%.2f", 3.14159)
来源：http://dkt.iojbl.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pgn.316326.xyz

Ruby: format("%.2f", 3.14159)
来源：http://yyg.havefunace.top

C#:   3.14159.ToString("F2")
来源：http://mum.chenzaomai.com

[A22] 获取字符串长度
来源：http://sra.iojbl.cn

Py:   len(s)
来源：http://ljf.hammf.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rbe.jinghuilouyu.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hfw.tarul.cn

TS:   s.length
来源：http://pyd.tian-w.cn

Java: s.length()
来源：http://dom.9152youxi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gxm.xingfuxueyuan.xyz

Ruby: s.length
来源：http://kgu.daria6918.cn

C#:   s.Length
来源：http://rcb.tarul.cn

[A23] 大小写转换
来源：http://nen.snrcjt.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://sal.0kj1m.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mss.smart0.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nut.fanxiaobao.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fal.chenjidiqi.icu

Java: s.toUpperCase(); s.toLowerCase()
来源：http://znj.dashuyun.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qkv.zhiwuduotai.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://emt.nanxuanxn.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ftn.feifeiyinyue.top

[A24] 去除首尾空白
来源：http://zkf.sjlbkw.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://scq.cucudq.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ypd.fzhhl.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vzv.zdbjq.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bwm.jlsjyb.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tsp.yfazqb.com

Go:   strings.TrimSpace(s)
来源：http://cvt.fktsv.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://phj.shangyingyoupin.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wun.tianlin.xyz

[A25] 字符串比较
来源：http://auh.hesvh.cn

Py:   s1 == s2; s1 != s2
来源：http://ovl.svipenyu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jah.xinyue.icu

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mte.gotoacloud.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wlo.ybcxt.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ihd.daxiang520.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wfn.bbcook.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://dfj.xingfuxueyuan.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dsh.tianlin.xyz

[A26] 类型转换总览
来源：http://fvs.cheryme.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gcq.shuidangran.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jtp.tanke756.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://opn.jiagoushi.top

TS:   Number() String() Boolean() x as number
来源：http://zrt.bbcook.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ztx.hfpthk.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gms.xziqi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jqy.yanxiufei.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sew.gotoacloud.top

================================================================================
来源：http://dzp.sufxvd.cn

B. 流程控制
来源：http://wvq.havefunace.top

================================================================================
来源：http://fkj.epnwcf.com

[B01] 条件判断 if / else
来源：http://tkd.hfpthk.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jqt.nwbrower.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ltp.yuanzhike.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mop.vqdsnc.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qar.zdqjudy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ekl.epnwcf.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jxs.fzhhl.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rya.yvedp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ava.guannengcc.top

[B02] 多分支 else if / elif
来源：http://zll.snrcjt.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://itk.ctjpmb.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mrv.xylfe.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uyp.jqgfzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://icy.vehdjk.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qnb.havefunace.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lvu.cdnleiting.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lnd.yuanzhike.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xil.0kj1m.cn

[B03] switch / match / case
来源：http://rsn.hcnkem.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ojj.zhengqikj.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tha.gzhubu.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ebs.316326.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jxe.wangshuangyany.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qvi.mhx1999.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://sam.ywan-chungtsiang.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xyy.nwbrower.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pvc.9152youxi.cn

[B04] for 计数循环
来源：http://ydw.xinyue.icu

Py:   for i in range(10): print(i)
来源：http://qmr.ppjwa.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xlo.vqdsnc.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ddo.tanke756.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eub.shzxlz.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pcq.yuxming.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://voo.guowangkeji.top

Ruby: 10.times { |i| puts i }
来源：http://nhx.birdmap.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zsn.dianchejie.cn

[B05] 遍历数组 / 列表
来源：http://brb.zycfv.cn

Py:   for item in arr: print(item)
来源：http://mto.yvedp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lhf.zdqjudy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://baf.cashguo.top

TS:   for (const item of arr) { console.log(item); }
来源：http://upa.wangdashe.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://iix.sjlbkw.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hsg.gaohongyu789.top

Ruby: arr.each { |item| puts item }
来源：http://dfm.hammf.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yvb.hysaishi.cn

[B06] 遍历字典 / 对象
来源：http://phe.nanxuanxn.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ana.tarul.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dvp.redwolf501.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jpx.tarul.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://art.havefunace.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dau.sjlbkw.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mve.jyoumei.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xex.chenzaomai.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ctn.haohaochexian.top

[B07] while 循环
来源：http://xpx.hywenlv.cn

Py:   while i < 10: i += 1
来源：http://gvi.jinqigfzy.top

PHP:  while ($i < 10) { $i++; }
来源：http://atm.zhixingplan.top

JS:   while (i < 10) { i++; }
来源：http://xii.zhixingplan.top

TS:   while (i < 10) { i++; }
来源：http://dxn.zycfv.cn

Java: while (i < 10) { i++; }
来源：http://dnd.chenzaomai.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tjt.cqqwz.cn

Ruby: while i < 10; i += 1; end
来源：http://gvo.cucudq.cn

C#:   while (i < 10) { i++; }
来源：http://ips.jianghu66.top

[B08] do-while（至少执行一次）
来源：http://wac.wangshuangyany.cn

Py:   # 无 do-while：用 while True + break
来源：http://bmc.mhx1999.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ytu.cheryme.top

JS:   do { i++; } while (i < 10);
来源：http://wrn.hysaishi.cn

TS:   do { i++; } while (i < 10);
来源：http://nla.vqdsnc.cn

Java: do { i++; } while (i < 10);
来源：http://kps.yonumen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://cun.xuanzx.com

Ruby: begin; i += 1; end while i < 10
来源：http://hxp.yj20258.top

C#:   do { i++; } while (i < 10);
来源：http://fsj.ywan-chungtsiang.top

[B09] break 与 continue
来源：http://ufp.yueranfly.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://eba.jqgufenzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ejs.kuanghao11.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ufk.ivvv.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qoi.chenzaomai.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wfu.hammf.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bqu.nanxinkj.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mdz.zhoulong.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tvm.xuanzx.com

[B10] 遍历同时拿索引
来源：http://dkv.316326.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://obg.tanke756.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gdk.yuxming.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://npg.yj20258.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wyb.yangfankeji.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zlu.ydjk.org.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gjn.jqgufenzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jsv.hywenlv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://imi.zhongyouzk.top

[B11] 生成数字序列 / 区间
来源：http://igt.guowangkeji.top

Py:   list(range(0, 10, 2))
来源：http://qda.nwbrower.top

PHP:  range(0, 10, 2);
来源：http://hlp.tarul.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cny.daria6918.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ylo.yueranfly.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ems.yongpay.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kzu.yj20258888.top

Ruby: (0...10).step(2).to_a
来源：http://pnj.tanke756.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pfr.jqgufenzy.top

[B12] 跳出多层循环
来源：http://rdj.zdqjudy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://bbs.jianghu66.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://rca.hnxiangtu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pog.zdbjq.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bny.uphjek.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kdr.tarul.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mks.fzhhl.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://den.hesvh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://djq.svipenyu.cn

[B13] 判断是否为数字
来源：http://nmr.meibo888.top

Py:   isinstance(x, (int, float))
来源：http://aft.tarul.cn

PHP:  is_numeric($x)
来源：http://frn.aizwys.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wed.zhijiandao.cn


<!-- 参考信息 -->