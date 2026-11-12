代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://qac.hnqzz.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ytb.gzhubu.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ozl.fengsongda.top

Ruby: "42".to_i; "3.14".to_f
来源：http://bbc.iojbl.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gzs.hnqzz.top

[A07] 数字转字符串
来源：http://odd.dashuyun.cn

Py:   str(42)
来源：http://izd.shuidangran.top

PHP:  (string) 42; strval(42)
来源：http://alr.chenjidiqi.icu

JS:   String(42); (42).toString()
来源：http://vht.yfazqb.com

TS:   String(42)
来源：http://zgr.hammf.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ouf.andypj.xyz

Go:   strconv.Itoa(42)
来源：http://ueg.yj20258888.top

Ruby: 42.to_s
来源：http://yfr.ivvv.top

C#:   42.ToString()
来源：http://apc.hcnkem.com

[A08] 取整与四舍五入
来源：http://cii.birdmap.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ygv.wangdashe.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ysp.gzhubu.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://luc.yueranfly.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xri.svipenyu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ttx.xylfe.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ehj.jinqigufen.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://awb.yueranfly.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://kbr.yvedp.cn

[A09] 绝对值与最大最小值
来源：http://mxm.zhixingplan.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://fzc.zhoulong.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fsz.kuanghao11.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ite.cheryme.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cja.ybcxt.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wzr.sxryk.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fiq.quarkkingdee.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://eeq.cdnleiting.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jxn.iojbl.cn

[A10] 生成随机数
来源：http://jni.jqgufenzy.top

Py:   import random; random.randint(1, 100)
来源：http://iwt.316326.xyz

PHP:  random_int(1, 100);
来源：http://wdg.xingfuxueyuan.xyz

JS:   Math.floor(Math.random() * 100) + 1
来源：http://muq.xylfe.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://bxz.zhixingplan.top

Java: new Random().nextInt(100) + 1
来源：http://rol.wangshuangyany.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://thk.shzxlz.cn

Ruby: rand(1..100)
来源：http://ccc.hywenlv.cn

C#:   new Random().Next(1, 101)
来源：http://itj.jianghu66.top

[A11] 条件表达式（三元）
来源：http://tdc.jinqigufen.top

Py:   "yes" if x > 0 else "no"
来源：http://eot.gaohongyu789.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://jcq.yueranfly.top

JS:   x > 0 ? "yes" : "no"
来源：http://jbe.kuanghao11.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dyr.kuanghao11.cn

Java: x > 0 ? "yes" : "no"
来源：http://cri.iojbl.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://asy.zhijiandao.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://uhq.sysykeji.top

C#:   x > 0 ? "yes" : "no"
来源：http://bie.meibo888.top

[A12] 字符串插值 / 格式化
来源：http://vve.hongshengwenyu.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://axf.xylfe.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://dxl.yuanzhike.top

JS:   `Hello, ${name}!`
来源：http://dwu.xuetiantiany.cn

TS:   `Hello, ${name}!`
来源：http://ymw.bjfxy.top

Java: "Hello, %s!".formatted(name)
来源：http://psw.svipenyu.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://eqe.chenlongwang.top

Ruby: "Hello, #{name}!"
来源：http://lac.jianghu66.top

C#:   $"Hello, {name}!"
来源：http://clo.cashguo.top

[A13] 多行字符串（练习 \n 转义）
来源：http://asg.tarul.cn

Py:   "第一行\n第二行"
来源：http://dhi.ydzc1.top

PHP:  "第一行\n第二行"
来源：http://ore.ydzc1.top

JS:   "第一行\n第二行"
来源：http://rfy.svipenyu.cn

TS:   "第一行\n第二行"
来源：http://iaw.haohaochexian.top

Java: "第一行\n第二行"
来源：http://azi.daxiang520.top

Go:   "第一行\n第二行"
来源：http://vli.fengsongda.top

Ruby: "第一行\n第二行"
来源：http://qag.cucudq.cn

C#:   "第一行\n第二行"
来源：http://rmq.shzxlz.cn

[A14] 注释写法
来源：http://dxz.sjlbkw.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://bzb.ydjk.org.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hdx.ywan-chungtsiang.top

JS:   // 单行；/* 多行 */
来源：http://isi.redwolf501.top

TS:   // 单行；/* 多行 */
来源：http://nkk.fanxiaobao.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cnn.svipenyu.cn

Go:   // 单行；/* 多行 */
来源：http://wuh.hongshengwenyu.top

Ruby: # 单行；=begin 多行 =end
来源：http://lur.yuxming.cn

C#:   // 单行；/* 多行 */
来源：http://tre.cqqwz.cn

[A15] 空值判断与默认值
来源：http://ave.snrcjt.cn

Py:   value = data or "默认值"
来源：http://uci.cheryme.top

PHP:  $value = $data ?? "默认值";
来源：http://jfd.aizwys.cn

JS:   const value = data ?? "默认值";
来源：http://gji.yanxiufei.cn

TS:   const value = data ?? "默认值";
来源：http://vwj.zhiwuduotai.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://res.0kj1m.cn

Go:   if data == "" { data = "默认值" }
来源：http://ywy.sweek.top

Ruby: value = data || "默认值"
来源：http://bbk.jinyuanbaomall.cn

C#:   var value = data ?? "默认值";
来源：http://gpv.zhiwuduotai.top

[A16] 真假值判断规则
来源：http://hwa.gzhubu.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kok.smart0.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dyz.52xcode.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wsj.jyoumei.cn

TS:   if (!x) {}
来源：http://qud.xylfe.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hsh.sufxvd.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yaw.aibaodan.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vss.ehwqpu.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zuh.zhoulong.xyz

[A17] 位运算
来源：http://xlq.svipenyu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://suj.aibaodan.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ihz.gotoacloud.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ikl.yj20258888.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://iee.tian-w.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zen.xingfuxueyuan.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://agx.jianghu66.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vxn.hywenlv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gnn.zdbjq.cn

[A18] 字符与 ASCII 码互转
来源：http://mxe.zhongyouzk.top

Py:   ord("A"); chr(65)
来源：http://ssa.hfpthk.cn

PHP:  ord("A"); chr(65)
来源：http://xvj.ppjwa.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://liz.pengpengdd.cyou

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tdi.pycfn.com

Java: (int) 'A'; (char) 65
来源：http://azg.dashuyun.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dsb.ctjpmb.com

Ruby: "A".ord; 65.chr
来源：http://obf.kuanghao11.cn

C#:   (int)'A'; (char)65
来源：http://upo.bbcook.cn

[A19] 交换两个变量
来源：http://tzp.epnwcf.com

Py:   a, b = b, a
来源：http://djc.ctjpmb.com

PHP:  [$a, $b] = [$b, $a];
来源：http://thw.jqgfzy.top

JS:   [a, b] = [b, a];
来源：http://qvj.sjlbkw.cn

TS:   [a, b] = [b, a];
来源：http://xpf.jyoumei.cn

Java: int t = a; a = b; b = t;
来源：http://wep.guannengcc.top

Go:   a, b = b, a
来源：http://kej.yj202588.top

Ruby: a, b = b, a
来源：http://iuw.nanxinkj.top

C#:   (a, b) = (b, a);
来源：http://mpj.hesvh.cn

[A20] 读取标准输入
来源：http://uvs.fanxiaobao.xyz

Py:   name = input("请输入：")
来源：http://rkj.jyoumei.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ggy.zhiwuduotai.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vsu.sxryk.cn

TS:   // Node.js：readline 模块
来源：http://aoc.snrcjt.cn

Java: new Scanner(System.in).nextLine()
来源：http://vct.fengsongda.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ooi.chenlongwang.top

Ruby: gets.chomp
来源：http://lae.aibaodan.cn

C#:   Console.ReadLine();
来源：http://irr.snrcjt.cn

[A21] 保留指定小数位输出
来源：http://ljs.52xcode.cn

Py:   f"{3.14159:.2f}"
来源：http://urg.yanxiufei.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xsp.snrcjt.cn

JS:   (3.14159).toFixed(2)
来源：http://ada.wangdashe.top

TS:   (3.14159).toFixed(2)
来源：http://qql.jinqigfzy.top

Java: String.format("%.2f", 3.14159)
来源：http://beh.gotoacloud.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bsv.xylfe.cn

Ruby: format("%.2f", 3.14159)
来源：http://mrv.guowangkeji.top

C#:   3.14159.ToString("F2")
来源：http://wgg.zhaomingkeji.xyz

[A22] 获取字符串长度
来源：http://fop.cashguo.top

Py:   len(s)
来源：http://oza.52xcode.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qns.quarkkingdee.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ros.sufxvd.cn

TS:   s.length
来源：http://olr.yj20258.top

Java: s.length()
来源：http://tyd.yonumen.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://amo.ctjpmb.com

Ruby: s.length
来源：http://jjn.0kj1m.cn

C#:   s.Length
来源：http://nft.vehdjk.com

[A23] 大小写转换
来源：http://lhf.meibo888.top

Py:   s.upper(); s.lower(); s.title()
来源：http://fyy.ydjk.org.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ael.hesvh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sdp.jinyuanbaomall.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zii.gaohongyu789.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kpj.zhoulong.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nhw.tian-w.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jcr.cqqwz.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fvx.shanyushiyangtech.top

[A24] 去除首尾空白
来源：http://abb.meibo888.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vdz.ivvv.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xvs.ctjpmb.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fpr.feifeiyinyue.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pwo.cdnleiting.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ajt.sysykeji.top

Go:   strings.TrimSpace(s)
来源：http://aba.cashguo.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ahc.gzhubu.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tkv.vqdsnc.cn

[A25] 字符串比较
来源：http://dqj.xinyue.icu

Py:   s1 == s2; s1 != s2
来源：http://htk.hysaishi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hrs.jqgufenzy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gxy.9152youxi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://siw.dianchejie.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jmv.guowangkeji.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pvx.hcnkem.com

Ruby: s1 == s2; s1 <=> s2
来源：http://pat.hongshengwenyu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fgk.chenzaomai.com

[A26] 类型转换总览
来源：http://pbv.yuanzhike.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://otd.wangshuangyany.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nsg.smart0.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lte.jinghuilouyu.cn

TS:   Number() String() Boolean() x as number
来源：http://orm.yongpay.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lor.fengsongda.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dpe.vqdsnc.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ltq.yonumen.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://oyw.daria6918.cn

================================================================================
来源：http://plg.fzhhl.top

B. 流程控制
来源：http://ogn.tarul.cn

================================================================================
来源：http://raa.zhixingplan.top

[B01] 条件判断 if / else
来源：http://rrs.chenjidiqi.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://suu.wangshuangyany.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fgf.yueranfly.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ifu.nanxinkj.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mst.chenlongwang.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://fjz.jinghuilouyu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gof.yongpay.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fyr.hnqzz.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pfl.guannengcc.top

[B02] 多分支 else if / elif
来源：http://pcq.smart0.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bho.pengpengdd.cyou

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://abu.yueranfly.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ygy.zdbjq.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ags.cdnleiting.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cit.fengsongda.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lnp.feifeiyinyue.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bom.c1oappe.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vwh.gogol.net.cn

[B03] switch / match / case
来源：http://fnj.hesvh.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jtu.ydjk.org.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qcs.vehdjk.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qlj.hongshengwenyu.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://deg.zhoulong.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fgw.xuanzx.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zxp.9152youxi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yvr.yueranfly.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qnr.jinghuilouyu.cn

[B04] for 计数循环
来源：http://iqu.daria6918.cn

Py:   for i in range(10): print(i)
来源：http://kfj.shanyushiyangtech.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xao.ydjk.org.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hqe.feifeiyinyue.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://klx.fktsv.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sxv.cashguo.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gci.haohaochexian.top

Ruby: 10.times { |i| puts i }
来源：http://hco.dianchejie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://utz.xinyue.icu

[B05] 遍历数组 / 列表
来源：http://kzc.birdmap.top

Py:   for item in arr: print(item)
来源：http://vlh.tian-w.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ceg.dianchejie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://rpz.birdmap.top

TS:   for (const item of arr) { console.log(item); }
来源：http://fyy.hnqzz.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://cbx.meibo888.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rwj.xylfe.cn

Ruby: arr.each { |item| puts item }
来源：http://snp.aibaodan.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://erm.zhoulong.xyz

[B06] 遍历字典 / 对象
来源：http://avj.yj20258888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://oia.guowangkeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kkw.gotoacloud.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zhe.yongpay.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://awy.c1oappe.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gft.quarkkingdee.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://msn.zycfv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rca.yanxiufei.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gvp.jqgufenzy.top

[B07] while 循环
来源：http://rqd.zhengqikj.top

Py:   while i < 10: i += 1
来源：http://gxs.yj20258.top

PHP:  while ($i < 10) { $i++; }
来源：http://hpd.jlsjyb.cn

JS:   while (i < 10) { i++; }
来源：http://tnn.zhijiandao.cn

TS:   while (i < 10) { i++; }
来源：http://kky.yanxiufei.cn

Java: while (i < 10) { i++; }
来源：http://tbi.bbcook.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://cis.daxiang520.top

Ruby: while i < 10; i += 1; end
来源：http://mel.jinyuanbaomall.cn

C#:   while (i < 10) { i++; }
来源：http://aam.yongpay.top

[B08] do-while（至少执行一次）
来源：http://sdx.fktsv.cn

Py:   # 无 do-while：用 while True + break
来源：http://vdt.jqgufenzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ktk.shangyingyoupin.top

JS:   do { i++; } while (i < 10);
来源：http://ekj.9152youxi.cn

TS:   do { i++; } while (i < 10);
来源：http://kxv.feifeiyinyue.top

Java: do { i++; } while (i < 10);
来源：http://ccc.jiagoushi.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ejh.hcnkem.com

Ruby: begin; i += 1; end while i < 10
来源：http://sxc.xylfe.cn

C#:   do { i++; } while (i < 10);
来源：http://eps.kuanghao11.cn

[B09] break 与 continue
来源：http://ifo.ydjk.org.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nbt.cdnleiting.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sii.jqgfzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vdl.jqgufenzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ciu.0kj1m.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cuy.hammf.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gkg.52xcode.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zgq.nwbrower.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eoc.bbcook.cn

[B10] 遍历同时拿索引
来源：http://dtt.chenjidiqi.icu

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kbc.shzxlz.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ctj.ppjwa.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ida.vehdjk.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ygl.daria6918.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lkj.shzxlz.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rwu.chenlongwang.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iba.zhongyouzk.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vjy.fktsv.cn

[B11] 生成数字序列 / 区间
来源：http://mqs.jyoumei.cn

Py:   list(range(0, 10, 2))
来源：http://vyo.xinyue.icu

PHP:  range(0, 10, 2);
来源：http://yqf.chenlongwang.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zrx.wangdashe.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rla.sxryk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://twu.ctjpmb.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gti.sweek.top

Ruby: (0...10).step(2).to_a
来源：http://jhv.havefunace.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wvo.cdnleiting.top

[B12] 跳出多层循环
来源：http://hbx.fengsongda.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://fhy.tian-w.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dwg.jinghuilouyu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cge.hnxiangtu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wwe.316326.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bdj.jinghuilouyu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ntk.dianchejie.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wmn.smart0.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dml.gogol.net.cn

[B13] 判断是否为数字
来源：http://ywb.ydzc1.top

Py:   isinstance(x, (int, float))
来源：http://vnj.fanxiaobao.xyz

PHP:  is_numeric($x)
来源：http://txl.fengsongda.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tbw.zdbjq.cn


<!-- 参考信息 -->