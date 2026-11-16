代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wnv.ywan-chungtsiang.top

[A07] 数字转字符串
来源：http://qed.cheryme.top

Py:   str(42)
来源：http://rat.dashuyun.cn

PHP:  (string) 42; strval(42)
来源：http://lmu.ydjk.org.cn

JS:   String(42); (42).toString()
来源：http://sry.dianchejie.cn

TS:   String(42)
来源：http://lgd.hesvh.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zdg.pengpengdd.cyou

Go:   strconv.Itoa(42)
来源：http://ybz.fktsv.cn

Ruby: 42.to_s
来源：http://ilu.xingfuxueyuan.xyz

C#:   42.ToString()
来源：http://dis.yj202588.top

[A08] 取整与四舍五入
来源：http://htr.yueranfly.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dcl.ppjwa.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://dqb.zhongyouzk.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qcr.yueranfly.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lld.hnqzz.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://toh.mhx1999.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rxg.hesvh.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://iij.fktsv.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mdt.zhongyouzk.top

[A09] 绝对值与最大最小值
来源：http://frm.jianghu66.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pkm.ehwqpu.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bwn.fanxiaobao.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jnh.nanxuanxn.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://krq.aizwys.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://djq.guannengcc.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://aso.9152youxi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ztr.nanxinkj.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://stu.zdbjq.cn

[A10] 生成随机数
来源：http://lzx.ctjpmb.com

Py:   import random; random.randint(1, 100)
来源：http://mvl.ydjk.org.cn

PHP:  random_int(1, 100);
来源：http://rzx.zdbjq.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rpt.birdmap.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://vpd.zhoulong.xyz

Java: new Random().nextInt(100) + 1
来源：http://jrt.cheryme.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mtp.ybcxt.top

Ruby: rand(1..100)
来源：http://tgu.kuanghao11.cn

C#:   new Random().Next(1, 101)
来源：http://iht.fehbvm.com

[A11] 条件表达式（三元）
来源：http://pcv.fzhhl.top

Py:   "yes" if x > 0 else "no"
来源：http://chd.smart0.xyz

PHP:  $x > 0 ? "yes" : "no"
来源：http://snf.zdbjq.cn

JS:   x > 0 ? "yes" : "no"
来源：http://tar.hammf.cn

TS:   x > 0 ? "yes" : "no"
来源：http://waq.jinyuanbaomall.cn

Java: x > 0 ? "yes" : "no"
来源：http://pkp.epnwcf.com

Go:   // 无三元运算符，需用 if 语句
来源：http://ucz.havefunace.top

Ruby: x > 0 ? "yes" : "no"
来源：http://esr.zdbjq.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ucy.aizwys.cn

[A12] 字符串插值 / 格式化
来源：http://pml.dashuyun.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://tgw.uphjek.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://flk.fanxiaobao.xyz

JS:   `Hello, ${name}!`
来源：http://ggz.daxiang520.top

TS:   `Hello, ${name}!`
来源：http://jnp.zhengqikj.top

Java: "Hello, %s!".formatted(name)
来源：http://tdz.pycfn.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qhj.zhengqikj.top

Ruby: "Hello, #{name}!"
来源：http://hzo.zhoulong.xyz

C#:   $"Hello, {name}!"
来源：http://nho.vehdjk.com

[A13] 多行字符串（练习 \n 转义）
来源：http://vaz.mhx1999.top

Py:   "第一行\n第二行"
来源：http://lbh.hysaishi.cn

PHP:  "第一行\n第二行"
来源：http://ysa.xuetiantiany.cn

JS:   "第一行\n第二行"
来源：http://jei.shuidangran.top

TS:   "第一行\n第二行"
来源：http://dgi.ehwqpu.com

Java: "第一行\n第二行"
来源：http://krq.shanyushiyangtech.top

Go:   "第一行\n第二行"
来源：http://zop.shuidangran.top

Ruby: "第一行\n第二行"
来源：http://mpg.316326.xyz

C#:   "第一行\n第二行"
来源：http://lsl.zhaomingkeji.xyz

[A14] 注释写法
来源：http://iqh.ybcxt.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://cit.ppjwa.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://sfi.sjlbkw.cn

JS:   // 单行；/* 多行 */
来源：http://fwp.chenzaomai.com

TS:   // 单行；/* 多行 */
来源：http://bls.52xcode.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dbn.haohaochexian.top

Go:   // 单行；/* 多行 */
来源：http://cik.bjfxy.top

Ruby: # 单行；=begin 多行 =end
来源：http://bzq.xinyue.icu

C#:   // 单行；/* 多行 */
来源：http://ymr.sjlbkw.cn

[A15] 空值判断与默认值
来源：http://wkm.shangyingyoupin.top

Py:   value = data or "默认值"
来源：http://vmh.vehdjk.com

PHP:  $value = $data ?? "默认值";
来源：http://hlp.hnxiangtu.top

JS:   const value = data ?? "默认值";
来源：http://ukc.bjfxy.top

TS:   const value = data ?? "默认值";
来源：http://lbd.tanke756.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xhs.xylfe.cn

Go:   if data == "" { data = "默认值" }
来源：http://lkg.hnqzz.top

Ruby: value = data || "默认值"
来源：http://jli.epnwcf.com

C#:   var value = data ?? "默认值";
来源：http://fyp.haohaochexian.top

[A16] 真假值判断规则
来源：http://bgz.shanyushiyangtech.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qhh.quarkkingdee.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bav.ehwqpu.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ocb.c1oappe.top

TS:   if (!x) {}
来源：http://tjp.cdnleiting.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uaq.0kj1m.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rxv.ydjk.org.cn

Ruby: unless x            # nil 与 false 为假
来源：http://pxf.jinghuilouyu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vvf.zycfv.cn

[A17] 位运算
来源：http://bvs.hysaishi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xud.0kj1m.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qgt.sufxvd.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xow.tian-w.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rst.tian-w.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pff.cheryme.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kub.mhx1999.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://awz.mhx1999.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hqq.ywan-chungtsiang.top

[A18] 字符与 ASCII 码互转
来源：http://mjn.hfpthk.cn

Py:   ord("A"); chr(65)
来源：http://swn.ppjwa.cn

PHP:  ord("A"); chr(65)
来源：http://ngb.fengsongda.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fsn.chenzaomai.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jjh.pycfn.com

Java: (int) 'A'; (char) 65
来源：http://fqw.zhixingplan.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://aaj.ywan-chungtsiang.top

Ruby: "A".ord; 65.chr
来源：http://tse.andypj.xyz

C#:   (int)'A'; (char)65
来源：http://twg.gzhubu.top

[A19] 交换两个变量
来源：http://spv.zhoulong.xyz

Py:   a, b = b, a
来源：http://qrk.ywan-chungtsiang.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ryy.wangdashe.top

JS:   [a, b] = [b, a];
来源：http://owg.jlsjyb.cn

TS:   [a, b] = [b, a];
来源：http://eru.chenlongwang.top

Java: int t = a; a = b; b = t;
来源：http://stk.shangyingyoupin.top

Go:   a, b = b, a
来源：http://yrb.yj20258888.top

Ruby: a, b = b, a
来源：http://mwa.ehwqpu.com

C#:   (a, b) = (b, a);
来源：http://lpk.xingfuxueyuan.xyz

[A20] 读取标准输入
来源：http://fyn.yj20258.top

Py:   name = input("请输入：")
来源：http://idr.yj20258.top

PHP:  $name = trim(fgets(STDIN));
来源：http://jek.yuxming.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dcp.nwbrower.top

TS:   // Node.js：readline 模块
来源：http://ybg.epnwcf.com

Java: new Scanner(System.in).nextLine()
来源：http://uqv.mhx1999.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gxd.0kj1m.cn

Ruby: gets.chomp
来源：http://zwz.guannengcc.top

C#:   Console.ReadLine();
来源：http://soa.316326.xyz

[A21] 保留指定小数位输出
来源：http://eqj.yj20258888.top

Py:   f"{3.14159:.2f}"
来源：http://pvu.sxryk.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://grq.hcnkem.com

JS:   (3.14159).toFixed(2)
来源：http://tij.andypj.xyz

TS:   (3.14159).toFixed(2)
来源：http://blj.pycfn.com

Java: String.format("%.2f", 3.14159)
来源：http://ubk.yonumen.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pya.mhx1999.top

Ruby: format("%.2f", 3.14159)
来源：http://uuv.fktsv.cn

C#:   3.14159.ToString("F2")
来源：http://kql.nanxinkj.top

[A22] 获取字符串长度
来源：http://ssi.hcnkem.com

Py:   len(s)
来源：http://jvo.zycfv.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://uqu.shuidangran.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bjq.quarkkingdee.top

TS:   s.length
来源：http://efd.yangfankeji.com

Java: s.length()
来源：http://gnu.vehdjk.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wml.havefunace.top

Ruby: s.length
来源：http://mlj.kuanghao11.cn

C#:   s.Length
来源：http://frm.ehwqpu.com

[A23] 大小写转换
来源：http://flg.andypj.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://hbz.yueranfly.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://otj.zdbjq.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dky.xingfuxueyuan.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ajy.guowangkeji.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ubw.meibo888.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://huy.cashguo.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://eaz.hnqzz.top

C#:   s.ToUpper(); s.ToLower()
来源：http://shf.aibaodan.cn

[A24] 去除首尾空白
来源：http://asj.chenjidiqi.icu

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xnx.gogol.net.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xrd.hammf.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xit.nanxuanxn.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aff.daxiang520.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://svw.mhx1999.top

Go:   strings.TrimSpace(s)
来源：http://oxl.xuetiantiany.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dui.316326.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dkg.jinqigfzy.top

[A25] 字符串比较
来源：http://fye.birdmap.top

Py:   s1 == s2; s1 != s2
来源：http://tii.dashuyun.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tkl.zdqjudy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lrg.pengpengdd.cyou

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://alt.chenzaomai.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://njk.sysykeji.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nao.mhx1999.top

Ruby: s1 == s2; s1 <=> s2
来源：http://vpu.zycfv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wfc.andypj.xyz

[A26] 类型转换总览
来源：http://sqh.hfpthk.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zwz.hongshengwenyu.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bfr.jiagoushi.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cxv.hnxiangtu.top

TS:   Number() String() Boolean() x as number
来源：http://eht.sysykeji.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wum.fktsv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://psu.cqqwz.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jik.cucudq.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nks.fzhhl.top

================================================================================
来源：http://qnj.ehwqpu.com

B. 流程控制
来源：http://pud.yueranfly.top

================================================================================
来源：http://vys.gzhubu.top

[B01] 条件判断 if / else
来源：http://lic.snrcjt.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bpn.guowangkeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://edq.sjlbkw.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xcv.vqdsnc.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xek.yongpay.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://leq.shanyushiyangtech.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cnv.jqgufenzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kvj.cheryme.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tlb.quarkkingdee.top

[B02] 多分支 else if / elif
来源：http://tbu.52xcode.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vjg.jinghuilouyu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ouk.gzhubu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tfs.hongshengwenyu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tqh.yuanzhike.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hcs.yj20258888.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://brw.jlsjyb.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ttk.quarkkingdee.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sii.gotoacloud.top

[B03] switch / match / case
来源：http://fjq.yfazqb.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hqs.svipenyu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yok.9152youxi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sdu.yonumen.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://btc.hywenlv.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dvs.gotoacloud.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kpu.cqqwz.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mgx.zhoulong.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ikb.zhaomingkeji.xyz

[B04] for 计数循环
来源：http://hcf.aibaodan.cn

Py:   for i in range(10): print(i)
来源：http://efi.ywan-chungtsiang.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://buk.hywenlv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zov.yueranfly.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://doz.yj20258888.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eku.tanke756.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lkf.ppjwa.cn

Ruby: 10.times { |i| puts i }
来源：http://wax.jianghu66.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mpp.gogol.net.cn

[B05] 遍历数组 / 列表
来源：http://hae.shanyushiyangtech.top

Py:   for item in arr: print(item)
来源：http://drc.fanxiaobao.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zcz.gotoacloud.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hbv.yvedp.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cgy.quarkkingdee.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fmf.0kj1m.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://omu.jlsjyb.cn

Ruby: arr.each { |item| puts item }
来源：http://dtn.xinyue.icu

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uff.sweek.top

[B06] 遍历字典 / 对象
来源：http://lhq.cdnleiting.top

Py:   for k, v in d.items(): print(k, v)
来源：http://nqu.zhoulong.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qfm.yj20258888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hxm.316326.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tgt.yvedp.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dye.sufxvd.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gvw.hfpthk.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zzv.redwolf501.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hli.guowangkeji.top

[B07] while 循环
来源：http://eed.zhengqikj.top

Py:   while i < 10: i += 1
来源：http://qqf.sufxvd.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ivh.bbcook.cn

JS:   while (i < 10) { i++; }
来源：http://kfc.chenzaomai.com

TS:   while (i < 10) { i++; }
来源：http://ahz.haohaochexian.top

Java: while (i < 10) { i++; }
来源：http://dsv.iojbl.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xkf.quarkkingdee.top

Ruby: while i < 10; i += 1; end
来源：http://rqa.shanyushiyangkeji.top

C#:   while (i < 10) { i++; }
来源：http://keq.havefunace.top

[B08] do-while（至少执行一次）
来源：http://wjl.ywan-chungtsiang.top

Py:   # 无 do-while：用 while True + break
来源：http://ysh.ybcxt.top

PHP:  do { $i++; } while ($i < 10);
来源：http://nwo.fzhhl.top

JS:   do { i++; } while (i < 10);
来源：http://hkw.zycfv.cn

TS:   do { i++; } while (i < 10);
来源：http://vnm.pengpengdd.cyou

Java: do { i++; } while (i < 10);
来源：http://iyz.c1oappe.top

Go:   for { i++; if i >= 10 { break } }
来源：http://wqj.xuetiantiany.cn

Ruby: begin; i += 1; end while i < 10
来源：http://mkt.nwbrower.top

C#:   do { i++; } while (i < 10);
来源：http://wwu.hammf.cn

[B09] break 与 continue
来源：http://ibk.epnwcf.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wnm.zycfv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://erk.zhengqikj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pqb.hywenlv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pqh.pycfn.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lma.fengsongda.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zxz.9152youxi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rwx.xuanzx.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://drv.jinyuanbaomall.cn

[B10] 遍历同时拿索引
来源：http://mpc.vqdsnc.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tht.xuetiantiany.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ayl.zhaomingkeji.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hjv.guowangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uhr.zdqjudy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xfy.zhengqikj.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://azr.yuanzhike.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zwa.fengsongda.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mhb.jinqigufen.top

[B11] 生成数字序列 / 区间
来源：http://dgh.jlsjyb.cn

Py:   list(range(0, 10, 2))
来源：http://rhl.yj20258888.top

PHP:  range(0, 10, 2);
来源：http://lmb.316326.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xcr.hywenlv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ntk.ywan-chungtsiang.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tjs.pycfn.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rsr.dashuyun.cn

Ruby: (0...10).step(2).to_a
来源：http://xto.wangdashe.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ngj.vqdsnc.cn

[B12] 跳出多层循环
来源：http://yzv.mhx1999.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://plf.vehdjk.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://eez.shuidangran.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lnw.sysykeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rwk.ppjwa.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://end.pengpengdd.cyou

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zdu.chenzaomai.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ozc.yongpay.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sxq.jlsjyb.cn

[B13] 判断是否为数字
来源：http://izi.tanke756.top

Py:   isinstance(x, (int, float))
来源：http://sau.ctjpmb.com

PHP:  is_numeric($x)
来源：http://wgm.yfazqb.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://azc.guowangkeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://taj.hysaishi.cn

Java: x instanceof Number
来源：http://sbd.daxiang520.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dei.fehbvm.com

Ruby: x.is_a?(Numeric)
来源：http://ozj.yj20258.top


<!-- 参考信息 -->