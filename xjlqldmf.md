代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xgm.vqdsnc.cn

[A07] 数字转字符串
来源：http://uiy.zhaomingkeji.xyz

Py:   str(42)
来源：http://uzk.aibaodan.cn

PHP:  (string) 42; strval(42)
来源：http://dgl.yanxiufei.cn

JS:   String(42); (42).toString()
来源：http://ayj.cashguo.top

TS:   String(42)
来源：http://uuk.aibaodan.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://nsg.cdnleiting.top

Go:   strconv.Itoa(42)
来源：http://vew.shanyushiyangkeji.top

Ruby: 42.to_s
来源：http://txk.ehwqpu.com

C#:   42.ToString()
来源：http://tqr.yvedp.cn

[A08] 取整与四舍五入
来源：http://agm.shangyingyoupin.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://exy.jqgfzy.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://rvg.sufxvd.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hoj.52xcode.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bfi.meibo888.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://nlw.wangshuangyany.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bmg.sxryk.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://lcr.cheryme.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://prb.jqgufenzy.top

[A09] 绝对值与最大最小值
来源：http://ebh.chenjidiqi.icu

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wjw.ybcxt.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ogu.sweek.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dso.dianchejie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://sfj.aizwys.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://pvq.sxryk.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ybh.zhixingplan.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://bbt.yj20258888.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ywj.xingfuxueyuan.xyz

[A10] 生成随机数
来源：http://jje.birdmap.top

Py:   import random; random.randint(1, 100)
来源：http://fxi.jianghu66.top

PHP:  random_int(1, 100);
来源：http://wtu.fengsongda.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wat.xingfuxueyuan.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jbr.gzhubu.top

Java: new Random().nextInt(100) + 1
来源：http://sdp.fehbvm.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://nty.xinyue.icu

Ruby: rand(1..100)
来源：http://iob.snrcjt.cn

C#:   new Random().Next(1, 101)
来源：http://leg.sjlbkw.cn

[A11] 条件表达式（三元）
来源：http://rav.sxryk.cn

Py:   "yes" if x > 0 else "no"
来源：http://krn.aibaodan.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://nfi.yuxming.cn

JS:   x > 0 ? "yes" : "no"
来源：http://uac.xingfuxueyuan.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://hmh.9152youxi.cn

Java: x > 0 ? "yes" : "no"
来源：http://cxt.shanyushiyangtech.top

Go:   // 无三元运算符，需用 if 语句
来源：http://iou.ybcxt.top

Ruby: x > 0 ? "yes" : "no"
来源：http://lga.xinyue.icu

C#:   x > 0 ? "yes" : "no"
来源：http://ada.xinyue.icu

[A12] 字符串插值 / 格式化
来源：http://eol.chenzaomai.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lxt.bjfxy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cat.ehwqpu.com

JS:   `Hello, ${name}!`
来源：http://rzg.yangfankeji.com

TS:   `Hello, ${name}!`
来源：http://ohj.cdnleiting.top

Java: "Hello, %s!".formatted(name)
来源：http://nfq.xuetiantiany.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://lca.andypj.xyz

Ruby: "Hello, #{name}!"
来源：http://sew.guowangkeji.top

C#:   $"Hello, {name}!"
来源：http://jwk.feifeiyinyue.top

[A13] 多行字符串（练习 \n 转义）
来源：http://wep.xingfuxueyuan.xyz

Py:   "第一行\n第二行"
来源：http://eqg.shangyingyoupin.top

PHP:  "第一行\n第二行"
来源：http://bac.jyoumei.cn

JS:   "第一行\n第二行"
来源：http://wzx.haohaochexian.top

TS:   "第一行\n第二行"
来源：http://ycv.yvedp.cn

Java: "第一行\n第二行"
来源：http://hlt.sysykeji.top

Go:   "第一行\n第二行"
来源：http://dms.9152youxi.cn

Ruby: "第一行\n第二行"
来源：http://tld.gotoacloud.top

C#:   "第一行\n第二行"
来源：http://jdv.nanxuanxn.top

[A14] 注释写法
来源：http://byl.zdbjq.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://jcj.zycfv.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://lgo.cdnleiting.top

JS:   // 单行；/* 多行 */
来源：http://tds.hysaishi.cn

TS:   // 单行；/* 多行 */
来源：http://kpu.xziqi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://uwg.jinqigfzy.top

Go:   // 单行；/* 多行 */
来源：http://fjz.guowangkeji.top

Ruby: # 单行；=begin 多行 =end
来源：http://htw.0kj1m.cn

C#:   // 单行；/* 多行 */
来源：http://mcb.mhx1999.top

[A15] 空值判断与默认值
来源：http://lke.hysaishi.cn

Py:   value = data or "默认值"
来源：http://lne.fengsongda.top

PHP:  $value = $data ?? "默认值";
来源：http://oeq.fktsv.cn

JS:   const value = data ?? "默认值";
来源：http://wjw.yangfankeji.com

TS:   const value = data ?? "默认值";
来源：http://mmb.fengsongda.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cbz.bjfxy.top

Go:   if data == "" { data = "默认值" }
来源：http://zxu.xinyue.icu

Ruby: value = data || "默认值"
来源：http://amx.zhengqikj.top

C#:   var value = data ?? "默认值";
来源：http://jxk.ywan-chungtsiang.top

[A16] 真假值判断规则
来源：http://urm.guannengcc.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ojy.haohaochexian.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://okp.tarul.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pdq.zhiwuduotai.top

TS:   if (!x) {}
来源：http://dyt.yuxming.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nqn.chenzaomai.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ahq.zycfv.cn

Ruby: unless x            # nil 与 false 为假
来源：http://pfr.zdbjq.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://met.zhijiandao.cn

[A17] 位运算
来源：http://ivq.zhongyouzk.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ilq.hfpthk.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://iwz.chenlongwang.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pie.fengsongda.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kyo.shanyushiyangkeji.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tai.gzhubu.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ypy.jinyuanbaomall.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wxt.zhengqikj.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uxm.yj20258.top

[A18] 字符与 ASCII 码互转
来源：http://hde.52xcode.cn

Py:   ord("A"); chr(65)
来源：http://mio.haohaochexian.top

PHP:  ord("A"); chr(65)
来源：http://khh.shuidangran.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://eag.xziqi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kjs.52xcode.cn

Java: (int) 'A'; (char) 65
来源：http://tdu.xziqi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ejd.316326.xyz

Ruby: "A".ord; 65.chr
来源：http://vpt.zdqjudy.top

C#:   (int)'A'; (char)65
来源：http://nzz.gaohongyu789.top

[A19] 交换两个变量
来源：http://gxj.zhaomingkeji.xyz

Py:   a, b = b, a
来源：http://iuo.smart0.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://mfd.316326.xyz

JS:   [a, b] = [b, a];
来源：http://fib.gzhubu.top

TS:   [a, b] = [b, a];
来源：http://afn.daria6918.cn

Java: int t = a; a = b; b = t;
来源：http://dtt.pycfn.com

Go:   a, b = b, a
来源：http://kzx.havefunace.top

Ruby: a, b = b, a
来源：http://qvf.ivvv.top

C#:   (a, b) = (b, a);
来源：http://ofe.sufxvd.cn

[A20] 读取标准输入
来源：http://vff.ywan-chungtsiang.top

Py:   name = input("请输入：")
来源：http://qpl.gzhubu.top

PHP:  $name = trim(fgets(STDIN));
来源：http://tdj.gaohongyu789.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pwq.tarul.cn

TS:   // Node.js：readline 模块
来源：http://hkh.feifeiyinyue.top

Java: new Scanner(System.in).nextLine()
来源：http://eqo.yj20258888.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gbd.cucudq.cn

Ruby: gets.chomp
来源：http://jzg.zhaomingkeji.xyz

C#:   Console.ReadLine();
来源：http://wal.cashguo.top

[A21] 保留指定小数位输出
来源：http://reu.ehwqpu.com

Py:   f"{3.14159:.2f}"
来源：http://hzc.cashguo.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://les.yonumen.top

JS:   (3.14159).toFixed(2)
来源：http://nlz.epnwcf.com

TS:   (3.14159).toFixed(2)
来源：http://lce.bbcook.cn

Java: String.format("%.2f", 3.14159)
来源：http://dfx.birdmap.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wsr.nanxinkj.top

Ruby: format("%.2f", 3.14159)
来源：http://zfe.shuidangran.top

C#:   3.14159.ToString("F2")
来源：http://aea.jlsjyb.cn

[A22] 获取字符串长度
来源：http://hoq.sysykeji.top

Py:   len(s)
来源：http://afm.yj20258.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rwe.yj20258.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://spb.redwolf501.top

TS:   s.length
来源：http://qjy.hfpthk.cn

Java: s.length()
来源：http://euh.zhaomingkeji.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ljj.sysykeji.top

Ruby: s.length
来源：http://vxb.xuetiantiany.cn

C#:   s.Length
来源：http://rui.xylfe.cn

[A23] 大小写转换
来源：http://uay.ydjk.org.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tij.daxiang520.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xqo.shanyushiyangkeji.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://klq.shangyingyoupin.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://oay.hfpthk.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tpm.shuidangran.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wvk.52xcode.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cdx.snrcjt.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zuy.zhoulong.xyz

[A24] 去除首尾空白
来源：http://mid.ywan-chungtsiang.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nqy.ivvv.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nvi.shanyushiyangtech.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nru.hesvh.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kqb.meibo888.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cms.xuetiantiany.cn

Go:   strings.TrimSpace(s)
来源：http://msn.pengpengdd.cyou

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wmb.bjfxy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zdf.xingfuxueyuan.xyz

[A25] 字符串比较
来源：http://wmj.jiagoushi.top

Py:   s1 == s2; s1 != s2
来源：http://qdq.yongpay.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://onl.0kj1m.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mys.ivvv.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gow.hammf.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ocn.yj20258.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yea.cqqwz.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vdj.bbcook.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jzf.bbcook.cn

[A26] 类型转换总览
来源：http://vap.dianchejie.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://edi.xinyue.icu

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gxp.52xcode.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gzw.hammf.cn

TS:   Number() String() Boolean() x as number
来源：http://iqs.zhijiandao.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://yqy.zdqjudy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dft.fehbvm.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://aib.jyoumei.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wic.c1oappe.top

================================================================================
来源：http://mwa.yj202588.top

B. 流程控制
来源：http://luw.chenzaomai.com

================================================================================
来源：http://xly.hesvh.cn

[B01] 条件判断 if / else
来源：http://znm.haohaochexian.top

Py:   result = "正" if x > 0 else "非正"
来源：http://vng.quarkkingdee.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ifh.yonumen.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ant.jiagoushi.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kvj.jlsjyb.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lxv.ehwqpu.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://oaa.52xcode.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zpj.ybcxt.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lwe.pengpengdd.cyou

[B02] 多分支 else if / elif
来源：http://ybd.ydzc1.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vtw.xuanzx.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lup.shzxlz.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ccn.hnqzz.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://grl.nwbrower.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jfu.ehwqpu.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vcd.316326.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ixe.feifeiyinyue.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cca.jinqigfzy.top

[B03] switch / match / case
来源：http://vey.fanxiaobao.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://oaz.pycfn.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vik.tian-w.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ddc.0kj1m.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wzc.gotoacloud.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rwo.fengsongda.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xcr.tarul.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bow.ydzc1.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gyx.gzhubu.top

[B04] for 计数循环
来源：http://slz.jlsjyb.cn

Py:   for i in range(10): print(i)
来源：http://nxu.gogol.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qqq.sysykeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wod.hfpthk.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://upz.uphjek.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dad.hongshengwenyu.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xcv.yvedp.cn

Ruby: 10.times { |i| puts i }
来源：http://lba.xingfuxueyuan.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://eea.52xcode.cn

[B05] 遍历数组 / 列表
来源：http://kuw.tian-w.cn

Py:   for item in arr: print(item)
来源：http://vem.chenzaomai.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ooh.hnxiangtu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://taw.ivvv.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hlo.sweek.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://srz.zhixingplan.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://orb.nanxinkj.top

Ruby: arr.each { |item| puts item }
来源：http://ovp.gogol.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ray.nwbrower.top

[B06] 遍历字典 / 对象
来源：http://vwn.jiagoushi.top

Py:   for k, v in d.items(): print(k, v)
来源：http://dwr.nanxuanxn.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vhu.xylfe.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rlo.vehdjk.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sbz.mhx1999.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://puv.vehdjk.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eqf.shanyushiyangkeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nyb.bbcook.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nlx.xylfe.cn

[B07] while 循环
来源：http://bkm.hywenlv.cn

Py:   while i < 10: i += 1
来源：http://xqv.iojbl.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jzf.yvedp.cn

JS:   while (i < 10) { i++; }
来源：http://wqa.dianchejie.cn

TS:   while (i < 10) { i++; }
来源：http://inn.bbcook.cn

Java: while (i < 10) { i++; }
来源：http://yqe.yfazqb.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xdr.zhiwuduotai.top

Ruby: while i < 10; i += 1; end
来源：http://xge.ydjk.org.cn

C#:   while (i < 10) { i++; }
来源：http://icn.gzhubu.top

[B08] do-while（至少执行一次）
来源：http://bna.meibo888.top

Py:   # 无 do-while：用 while True + break
来源：http://gar.fktsv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://fpi.316326.xyz

JS:   do { i++; } while (i < 10);
来源：http://jyx.dianchejie.cn

TS:   do { i++; } while (i < 10);
来源：http://wkd.aibaodan.cn

Java: do { i++; } while (i < 10);
来源：http://izg.jianghu66.top

Go:   for { i++; if i >= 10 { break } }
来源：http://dwz.feifeiyinyue.top

Ruby: begin; i += 1; end while i < 10
来源：http://uof.cashguo.top

C#:   do { i++; } while (i < 10);
来源：http://bmo.zhiwuduotai.top

[B09] break 与 continue
来源：http://lvi.fehbvm.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nsr.jinyuanbaomall.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fmc.sufxvd.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ztm.guannengcc.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gyj.yueranfly.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qbe.zdbjq.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://veg.gzhubu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vmw.xylfe.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gcs.zdbjq.cn

[B10] 遍历同时拿索引
来源：http://luc.hnqzz.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xxs.jqgufenzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bak.jlsjyb.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qqi.daria6918.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uhw.hysaishi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://imx.zdbjq.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://njk.shuidangran.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wiv.shuidangran.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ysv.zhengqikj.top

[B11] 生成数字序列 / 区间
来源：http://obj.aizwys.cn

Py:   list(range(0, 10, 2))
来源：http://nbd.andypj.xyz

PHP:  range(0, 10, 2);
来源：http://hre.mhx1999.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qrq.yanxiufei.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://omm.epnwcf.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hmm.xinyue.icu

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fvi.cdnleiting.top

Ruby: (0...10).step(2).to_a
来源：http://tsl.pengpengdd.cyou

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jsd.cqqwz.cn

[B12] 跳出多层循环
来源：http://jfc.bjfxy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kui.ivvv.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://uxq.sjlbkw.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://auf.pycfn.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nby.bbcook.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jvv.vqdsnc.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qoo.daxiang520.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bjz.316326.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://reo.chenlongwang.top

[B13] 判断是否为数字
来源：http://kpw.sjlbkw.cn

Py:   isinstance(x, (int, float))
来源：http://jxw.yangfankeji.com

PHP:  is_numeric($x)
来源：http://xiw.hnqzz.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vkx.yj20258.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kcg.hesvh.cn

Java: x instanceof Number
来源：http://jqn.zdqjudy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ndb.ydzc1.top

Ruby: x.is_a?(Numeric)
来源：http://csh.xingfuxueyuan.xyz


<!-- 参考信息 -->