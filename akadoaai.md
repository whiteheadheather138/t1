代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zcp.xinyue.icu

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://aqn.quarkkingdee.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ndg.hysaishi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://fdi.sxryk.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baz.316326.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mxm.cucudq.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://oce.tanke756.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ptd.daria6918.cn

[A10] 生成随机数
来源：http://wqg.cqqwz.cn

Py:   import random; random.randint(1, 100)
来源：http://kbp.yonumen.top

PHP:  random_int(1, 100);
来源：http://jqy.zhixingplan.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nru.shanyushiyangkeji.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wzu.zhengqikj.top

Java: new Random().nextInt(100) + 1
来源：http://ipd.vehdjk.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ghq.fehbvm.com

Ruby: rand(1..100)
来源：http://iad.hfpthk.cn

C#:   new Random().Next(1, 101)
来源：http://zhv.dianchejie.cn

[A11] 条件表达式（三元）
来源：http://lnl.fanxiaobao.xyz

Py:   "yes" if x > 0 else "no"
来源：http://jlu.zycfv.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://eop.zhongyouzk.top

JS:   x > 0 ? "yes" : "no"
来源：http://sae.c1oappe.top

TS:   x > 0 ? "yes" : "no"
来源：http://ich.aibaodan.cn

Java: x > 0 ? "yes" : "no"
来源：http://tdi.shzxlz.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://vwk.jlsjyb.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://wqa.jianghu66.top

C#:   x > 0 ? "yes" : "no"
来源：http://aox.epnwcf.com

[A12] 字符串插值 / 格式化
来源：http://boa.yangfankeji.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qbs.jinqigfzy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ywq.gzhubu.top

JS:   `Hello, ${name}!`
来源：http://ctq.hammf.cn

TS:   `Hello, ${name}!`
来源：http://zyg.chenjidiqi.icu

Java: "Hello, %s!".formatted(name)
来源：http://bmy.xuanzx.com

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qyt.sysykeji.top

Ruby: "Hello, #{name}!"
来源：http://dmj.shangyingyoupin.top

C#:   $"Hello, {name}!"
来源：http://uwv.aibaodan.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://cxs.fehbvm.com

Py:   "第一行\n第二行"
来源：http://siv.xuanzx.com

PHP:  "第一行\n第二行"
来源：http://lry.xuetiantiany.cn

JS:   "第一行\n第二行"
来源：http://kve.daria6918.cn

TS:   "第一行\n第二行"
来源：http://asv.xingfuxueyuan.xyz

Java: "第一行\n第二行"
来源：http://zoz.jqgufenzy.top

Go:   "第一行\n第二行"
来源：http://jnp.sxryk.cn

Ruby: "第一行\n第二行"
来源：http://kmp.yongpay.top

C#:   "第一行\n第二行"
来源：http://dkw.hcnkem.com

[A14] 注释写法
来源：http://gii.ehwqpu.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://gnp.yj20258.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://xmd.hongshengwenyu.top

JS:   // 单行；/* 多行 */
来源：http://yob.hammf.cn

TS:   // 单行；/* 多行 */
来源：http://osu.hongshengwenyu.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://zbk.zdqjudy.top

Go:   // 单行；/* 多行 */
来源：http://pmi.guowangkeji.top

Ruby: # 单行；=begin 多行 =end
来源：http://rwn.epnwcf.com

C#:   // 单行；/* 多行 */
来源：http://oof.zhixingplan.top

[A15] 空值判断与默认值
来源：http://xxg.jqgufenzy.top

Py:   value = data or "默认值"
来源：http://ldv.nanxinkj.top

PHP:  $value = $data ?? "默认值";
来源：http://wyq.yj20258888.top

JS:   const value = data ?? "默认值";
来源：http://zgb.guannengcc.top

TS:   const value = data ?? "默认值";
来源：http://oft.fktsv.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://htn.cdnleiting.top

Go:   if data == "" { data = "默认值" }
来源：http://udx.ehwqpu.com

Ruby: value = data || "默认值"
来源：http://sjc.jinqigfzy.top

C#:   var value = data ?? "默认值";
来源：http://bzh.hnqzz.top

[A16] 真假值判断规则
来源：http://zoi.sufxvd.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xdh.shanyushiyangtech.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ezc.cheryme.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ezb.cheryme.top

TS:   if (!x) {}
来源：http://szd.ivvv.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ces.dianchejie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nwp.quarkkingdee.top

Ruby: unless x            # nil 与 false 为假
来源：http://prs.sweek.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kvk.sweek.top

[A17] 位运算
来源：http://pne.tianlin.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://npu.zhijiandao.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qtr.jlsjyb.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uql.shzxlz.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://suf.kuanghao11.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ylw.shangyingyoupin.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ilg.zhongyouzk.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jvi.epnwcf.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qxj.hnxiangtu.top

[A18] 字符与 ASCII 码互转
来源：http://pfo.haohaochexian.top

Py:   ord("A"); chr(65)
来源：http://nyt.jinqigfzy.top

PHP:  ord("A"); chr(65)
来源：http://lhh.316326.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://elu.snrcjt.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ixa.shanyushiyangtech.top

Java: (int) 'A'; (char) 65
来源：http://dxf.havefunace.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://enc.shuidangran.top

Ruby: "A".ord; 65.chr
来源：http://xai.daria6918.cn

C#:   (int)'A'; (char)65
来源：http://ufx.jinqigfzy.top

[A19] 交换两个变量
来源：http://ord.shanyushiyangkeji.top

Py:   a, b = b, a
来源：http://eae.sysykeji.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ndn.fzhhl.top

JS:   [a, b] = [b, a];
来源：http://pty.sufxvd.cn

TS:   [a, b] = [b, a];
来源：http://jwl.fktsv.cn

Java: int t = a; a = b; b = t;
来源：http://xvk.havefunace.top

Go:   a, b = b, a
来源：http://iib.cucudq.cn

Ruby: a, b = b, a
来源：http://gwa.havefunace.top

C#:   (a, b) = (b, a);
来源：http://doi.fengsongda.top

[A20] 读取标准输入
来源：http://tyf.andypj.xyz

Py:   name = input("请输入：")
来源：http://pil.ivvv.top

PHP:  $name = trim(fgets(STDIN));
来源：http://gdn.zhaomingkeji.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tsw.yangfankeji.com

TS:   // Node.js：readline 模块
来源：http://dtt.jiagoushi.top

Java: new Scanner(System.in).nextLine()
来源：http://ndx.hnqzz.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jsr.zhongyouzk.top

Ruby: gets.chomp
来源：http://mcv.zdqjudy.top

C#:   Console.ReadLine();
来源：http://bfh.xuetiantiany.cn

[A21] 保留指定小数位输出
来源：http://oaq.zhongyouzk.top

Py:   f"{3.14159:.2f}"
来源：http://gii.tianlin.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jfh.feifeiyinyue.top

JS:   (3.14159).toFixed(2)
来源：http://bze.andypj.xyz

TS:   (3.14159).toFixed(2)
来源：http://udi.chenzaomai.com

Java: String.format("%.2f", 3.14159)
来源：http://zcn.jlsjyb.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ffx.aizwys.cn

Ruby: format("%.2f", 3.14159)
来源：http://aez.havefunace.top

C#:   3.14159.ToString("F2")
来源：http://szo.guowangkeji.top

[A22] 获取字符串长度
来源：http://cjd.daria6918.cn

Py:   len(s)
来源：http://miv.tanke756.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bhj.hnqzz.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cak.dashuyun.cn

TS:   s.length
来源：http://vbw.hammf.cn

Java: s.length()
来源：http://wxr.tianlin.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fwt.yongpay.top

Ruby: s.length
来源：http://wfb.sxryk.cn

C#:   s.Length
来源：http://osw.hfpthk.cn

[A23] 大小写转换
来源：http://dao.jinqigfzy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://fqz.daxiang520.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qet.ctjpmb.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mnm.xziqi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ixa.shanyushiyangtech.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zdc.ydzc1.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sek.guowangkeji.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nqu.yuanzhike.top

C#:   s.ToUpper(); s.ToLower()
来源：http://nxq.nwbrower.top

[A24] 去除首尾空白
来源：http://uov.nanxinkj.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wvf.pycfn.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ofv.chenjidiqi.icu

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gkj.zhijiandao.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pvn.xziqi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rbl.0kj1m.cn

Go:   strings.TrimSpace(s)
来源：http://bmp.zhiwuduotai.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://czw.yj20258888.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://unc.nwbrower.top

[A25] 字符串比较
来源：http://cjl.hongshengwenyu.top

Py:   s1 == s2; s1 != s2
来源：http://rdu.hywenlv.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ruc.shangyingyoupin.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pjq.zhengqikj.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bmr.guowangkeji.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wta.shanyushiyangkeji.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tls.hammf.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mzi.fanxiaobao.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wah.jinqigfzy.top

[A26] 类型转换总览
来源：http://ava.sweek.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vxk.shanyushiyangtech.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bzf.yangfankeji.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baf.hywenlv.cn

TS:   Number() String() Boolean() x as number
来源：http://mmn.hesvh.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nte.bbcook.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://snh.quarkkingdee.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ulp.mhx1999.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://puu.zhiwuduotai.top

================================================================================
来源：http://qpu.xuanzx.com

B. 流程控制
来源：http://qzs.dashuyun.cn

================================================================================
来源：http://qqb.yuxming.cn

[B01] 条件判断 if / else
来源：http://tdl.dianchejie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://aze.shzxlz.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ttq.jinqigufen.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dfm.fktsv.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://quc.ywan-chungtsiang.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://gug.sweek.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://utn.guannengcc.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xwa.dashuyun.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fic.aibaodan.cn

[B02] 多分支 else if / elif
来源：http://dpb.yueranfly.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cbz.bjfxy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zre.hesvh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xij.yueranfly.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://upy.meibo888.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://avp.jinqigfzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nlx.pengpengdd.cyou

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ggj.xuetiantiany.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zmk.bbcook.cn

[B03] switch / match / case
来源：http://xnb.xuanzx.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xgm.zdbjq.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vpu.zycfv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://naz.jinqigufen.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ybc.shzxlz.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://aai.yj202588.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://thi.guowangkeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ejj.nwbrower.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dim.hfpthk.cn

[B04] for 计数循环
来源：http://hyu.pengpengdd.cyou

Py:   for i in range(10): print(i)
来源：http://pkp.kuanghao11.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://efc.yfazqb.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wvt.yvedp.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://law.dashuyun.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mqx.gaohongyu789.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cbf.jinghuilouyu.cn

Ruby: 10.times { |i| puts i }
来源：http://xir.52xcode.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://djl.chenzaomai.com

[B05] 遍历数组 / 列表
来源：http://jcm.andypj.xyz

Py:   for item in arr: print(item)
来源：http://vrc.tarul.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gle.yueranfly.top

JS:   for (const item of arr) { console.log(item); }
来源：http://yhd.shuidangran.top

TS:   for (const item of arr) { console.log(item); }
来源：http://cgk.316326.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://bzc.9152youxi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ygn.yj20258888.top

Ruby: arr.each { |item| puts item }
来源：http://lqu.hammf.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qiy.ywan-chungtsiang.top

[B06] 遍历字典 / 对象
来源：http://uxm.snrcjt.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://asn.bbcook.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ypu.epnwcf.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eti.wangshuangyany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lsx.fengsongda.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oan.tian-w.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ldy.tanke756.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fqt.52xcode.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iqp.yvedp.cn

[B07] while 循环
来源：http://vdp.ydjk.org.cn

Py:   while i < 10: i += 1
来源：http://kwc.xylfe.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qrx.tianlin.xyz

JS:   while (i < 10) { i++; }
来源：http://szx.zdbjq.cn

TS:   while (i < 10) { i++; }
来源：http://sbx.xuanzx.com

Java: while (i < 10) { i++; }
来源：http://gtu.jinqigfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hkc.xingfuxueyuan.xyz

Ruby: while i < 10; i += 1; end
来源：http://amz.yonumen.top

C#:   while (i < 10) { i++; }
来源：http://uly.smart0.xyz

[B08] do-while（至少执行一次）
来源：http://cyf.uphjek.com

Py:   # 无 do-while：用 while True + break
来源：http://zpu.shanyushiyangkeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://esg.iojbl.cn

JS:   do { i++; } while (i < 10);
来源：http://alz.mhx1999.top

TS:   do { i++; } while (i < 10);
来源：http://wzq.mhx1999.top

Java: do { i++; } while (i < 10);
来源：http://vjy.nanxuanxn.top

Go:   for { i++; if i >= 10 { break } }
来源：http://rsl.bjfxy.top

Ruby: begin; i += 1; end while i < 10
来源：http://zvf.uphjek.com

C#:   do { i++; } while (i < 10);
来源：http://vlk.ywan-chungtsiang.top

[B09] break 与 continue
来源：http://lec.yueranfly.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://asm.meibo888.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mbq.guowangkeji.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yhc.ybcxt.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kwp.chenlongwang.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kow.jinqigufen.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tdm.xingfuxueyuan.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pfu.hysaishi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kcy.0kj1m.cn

[B10] 遍历同时拿索引
来源：http://itn.zycfv.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ifr.9152youxi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gde.sufxvd.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kgw.gotoacloud.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://krf.ywan-chungtsiang.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vek.ivvv.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://byw.xuanzx.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hwx.hysaishi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vhf.hysaishi.cn

[B11] 生成数字序列 / 区间
来源：http://uuh.hysaishi.cn

Py:   list(range(0, 10, 2))
来源：http://cqg.hcnkem.com

PHP:  range(0, 10, 2);
来源：http://skj.ctjpmb.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ygb.nanxinkj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rln.vqdsnc.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://izx.dianchejie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bvq.jqgfzy.top

Ruby: (0...10).step(2).to_a
来源：http://kes.hongshengwenyu.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wub.meibo888.top

[B12] 跳出多层循环
来源：http://gaz.meibo888.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://uqn.ehwqpu.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://emn.snrcjt.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vtu.yj202588.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bhz.cheryme.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dnm.yj20258888.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yta.yj202588.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rde.cdnleiting.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://klf.meibo888.top

[B13] 判断是否为数字
来源：http://lvs.cdnleiting.top

Py:   isinstance(x, (int, float))
来源：http://lyn.bbcook.cn

PHP:  is_numeric($x)
来源：http://ose.zhengqikj.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nvs.zhijiandao.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://drz.vehdjk.com

Java: x instanceof Number
来源：http://pgv.feifeiyinyue.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hzx.kuanghao11.cn

Ruby: x.is_a?(Numeric)
来源：http://cpu.birdmap.top

C#:   x is int or double or decimal
来源：http://qqh.yj20258.top

[B14] 判断值是否在集合内
来源：http://rkb.c1oappe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rba.jqgufenzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sgi.yuxming.cn

JS:   [1, 2, 3].includes(x)
来源：http://wmy.feifeiyinyue.top

TS:   [1, 2, 3].includes(x)
来源：http://pwc.bbcook.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hpu.pycfn.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ztp.snrcjt.cn

Ruby: [1, 2, 3].include?(x)
来源：http://crc.daxiang520.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dfe.kuanghao11.cn

[B15] 布尔运算与取反
来源：http://bnd.uphjek.com

Py:   a and b or not c
来源：http://wwr.andypj.xyz

PHP:  $a && $b || !$c
来源：http://vgl.sxryk.cn

JS:   a && b || !c
来源：http://mpg.vqdsnc.cn

TS:   a && b || !c
来源：http://iyy.jinyuanbaomall.cn

Java: a && b || !c
来源：http://sdo.sjlbkw.cn

Go:   a && b || !c
来源：http://zep.jyoumei.cn

Ruby: a && b || !c
来源：http://ruh.smart0.xyz

C#:   a && b || !c
来源：http://czg.feifeiyinyue.top

[B16] 卫语句：不满足条件提前返回
来源：http://vox.xziqi.cn


<!-- 参考信息 -->