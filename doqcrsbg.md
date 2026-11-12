代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ezi.tarul.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://cdy.kuanghao11.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://how.zhaomingkeji.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yqu.dashuyun.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://zuz.ehwqpu.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ely.andypj.xyz

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cxm.epnwcf.com

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wiw.snrcjt.cn

[A10] 生成随机数
来源：http://ynv.jqgfzy.top

Py:   import random; random.randint(1, 100)
来源：http://ypm.gzhubu.top

PHP:  random_int(1, 100);
来源：http://ycd.hammf.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://krz.yj20258.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://boy.gotoacloud.top

Java: new Random().nextInt(100) + 1
来源：http://vge.dianchejie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://rll.gotoacloud.top

Ruby: rand(1..100)
来源：http://rdn.quarkkingdee.top

C#:   new Random().Next(1, 101)
来源：http://jpl.guannengcc.top

[A11] 条件表达式（三元）
来源：http://ibd.jinqigfzy.top

Py:   "yes" if x > 0 else "no"
来源：http://pzz.iojbl.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fkh.vehdjk.com

JS:   x > 0 ? "yes" : "no"
来源：http://mjz.cucudq.cn

TS:   x > 0 ? "yes" : "no"
来源：http://gef.chenzaomai.com

Java: x > 0 ? "yes" : "no"
来源：http://nsf.sweek.top

Go:   // 无三元运算符，需用 if 语句
来源：http://gig.jinyuanbaomall.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jlp.kuanghao11.cn

C#:   x > 0 ? "yes" : "no"
来源：http://guh.sxryk.cn

[A12] 字符串插值 / 格式化
来源：http://sva.wangdashe.top

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rnh.xziqi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://xkf.yangfankeji.com

JS:   `Hello, ${name}!`
来源：http://ocy.dianchejie.cn

TS:   `Hello, ${name}!`
来源：http://aty.jianghu66.top

Java: "Hello, %s!".formatted(name)
来源：http://gbb.meibo888.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rvg.epnwcf.com

Ruby: "Hello, #{name}!"
来源：http://wmc.snrcjt.cn

C#:   $"Hello, {name}!"
来源：http://wwd.snrcjt.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://tkf.hywenlv.cn

Py:   "第一行\n第二行"
来源：http://fxd.hysaishi.cn

PHP:  "第一行\n第二行"
来源：http://jky.fehbvm.com

JS:   "第一行\n第二行"
来源：http://bgh.mhx1999.top

TS:   "第一行\n第二行"
来源：http://isy.yj20258888.top

Java: "第一行\n第二行"
来源：http://hrx.zdqjudy.top

Go:   "第一行\n第二行"
来源：http://rdp.nanxinkj.top

Ruby: "第一行\n第二行"
来源：http://cal.birdmap.top

C#:   "第一行\n第二行"
来源：http://veh.chenzaomai.com

[A14] 注释写法
来源：http://zer.jinghuilouyu.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://zog.xuetiantiany.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://van.ctjpmb.com

JS:   // 单行；/* 多行 */
来源：http://mdx.guannengcc.top

TS:   // 单行；/* 多行 */
来源：http://smf.tian-w.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://uoo.shangyingyoupin.top

Go:   // 单行；/* 多行 */
来源：http://xan.ydzc1.top

Ruby: # 单行；=begin 多行 =end
来源：http://vnl.sxryk.cn

C#:   // 单行；/* 多行 */
来源：http://glt.guannengcc.top

[A15] 空值判断与默认值
来源：http://lvm.shzxlz.cn

Py:   value = data or "默认值"
来源：http://ltz.jyoumei.cn

PHP:  $value = $data ?? "默认值";
来源：http://dnc.daxiang520.top

JS:   const value = data ?? "默认值";
来源：http://cgu.zhongyouzk.top

TS:   const value = data ?? "默认值";
来源：http://pmr.guannengcc.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://den.bbcook.cn

Go:   if data == "" { data = "默认值" }
来源：http://hct.xziqi.cn

Ruby: value = data || "默认值"
来源：http://vya.vehdjk.com

C#:   var value = data ?? "默认值";
来源：http://zcu.yvedp.cn

[A16] 真假值判断规则
来源：http://nda.aizwys.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mex.hfpthk.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wzf.yfazqb.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ymy.hnxiangtu.top

TS:   if (!x) {}
来源：http://wal.guowangkeji.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://syy.yvedp.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qbr.nwbrower.top

Ruby: unless x            # nil 与 false 为假
来源：http://ctu.haohaochexian.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jet.yueranfly.top

[A17] 位运算
来源：http://gce.sxryk.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jzy.yj20258.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hxd.iojbl.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vxa.zycfv.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lap.jyoumei.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xbs.dianchejie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jdk.tanke756.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lgi.kuanghao11.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ehe.hesvh.cn

[A18] 字符与 ASCII 码互转
来源：http://hay.52xcode.cn

Py:   ord("A"); chr(65)
来源：http://hrz.wangdashe.top

PHP:  ord("A"); chr(65)
来源：http://ikq.yuxming.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fxl.sjlbkw.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rbf.xziqi.cn

Java: (int) 'A'; (char) 65
来源：http://xbc.gaohongyu789.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ugq.fktsv.cn

Ruby: "A".ord; 65.chr
来源：http://ert.bjfxy.top

C#:   (int)'A'; (char)65
来源：http://aqo.nanxinkj.top

[A19] 交换两个变量
来源：http://nhe.hnqzz.top

Py:   a, b = b, a
来源：http://soi.mhx1999.top

PHP:  [$a, $b] = [$b, $a];
来源：http://csu.bjfxy.top

JS:   [a, b] = [b, a];
来源：http://yal.gogol.net.cn

TS:   [a, b] = [b, a];
来源：http://xmg.jqgufenzy.top

Java: int t = a; a = b; b = t;
来源：http://dzv.cqqwz.cn

Go:   a, b = b, a
来源：http://wmh.shuidangran.top

Ruby: a, b = b, a
来源：http://pfb.hnxiangtu.top

C#:   (a, b) = (b, a);
来源：http://qva.yuanzhike.top

[A20] 读取标准输入
来源：http://sjl.tianlin.xyz

Py:   name = input("请输入：")
来源：http://pda.jinyuanbaomall.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://pwu.yuxming.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nth.gotoacloud.top

TS:   // Node.js：readline 模块
来源：http://zck.gaohongyu789.top

Java: new Scanner(System.in).nextLine()
来源：http://zph.zycfv.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lmu.uphjek.com

Ruby: gets.chomp
来源：http://ylo.cdnleiting.top

C#:   Console.ReadLine();
来源：http://uqw.yfazqb.com

[A21] 保留指定小数位输出
来源：http://kfa.iojbl.cn

Py:   f"{3.14159:.2f}"
来源：http://zaf.yj202588.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cnt.daxiang520.top

JS:   (3.14159).toFixed(2)
来源：http://qmr.guannengcc.top

TS:   (3.14159).toFixed(2)
来源：http://kxv.daxiang520.top

Java: String.format("%.2f", 3.14159)
来源：http://ixg.fktsv.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://azv.pengpengdd.cyou

Ruby: format("%.2f", 3.14159)
来源：http://fzq.pycfn.com

C#:   3.14159.ToString("F2")
来源：http://qfi.guowangkeji.top

[A22] 获取字符串长度
来源：http://mec.gogol.net.cn

Py:   len(s)
来源：http://uyh.chenjidiqi.icu

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zed.zhiwuduotai.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zch.cqqwz.cn

TS:   s.length
来源：http://rzq.yonumen.top

Java: s.length()
来源：http://zxh.andypj.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nwo.ehwqpu.com

Ruby: s.length
来源：http://dpt.feifeiyinyue.top

C#:   s.Length
来源：http://hlq.feifeiyinyue.top

[A23] 大小写转换
来源：http://qqh.tianlin.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://oxs.smart0.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mxz.gotoacloud.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://suz.zhixingplan.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xst.svipenyu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qxj.hysaishi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ohs.yonumen.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://azw.fzhhl.top

C#:   s.ToUpper(); s.ToLower()
来源：http://bnk.daxiang520.top

[A24] 去除首尾空白
来源：http://fsl.cdnleiting.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://oee.yonumen.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lzx.cheryme.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yqz.ydzc1.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qet.shangyingyoupin.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rly.ivvv.top

Go:   strings.TrimSpace(s)
来源：http://yzf.yongpay.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lyn.haohaochexian.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gkf.yueranfly.top

[A25] 字符串比较
来源：http://taf.nwbrower.top

Py:   s1 == s2; s1 != s2
来源：http://gju.meibo888.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kwz.316326.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dcn.sweek.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vob.xziqi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://znf.cheryme.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://osn.jinqigufen.top

Ruby: s1 == s2; s1 <=> s2
来源：http://shd.bbcook.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dmb.52xcode.cn

[A26] 类型转换总览
来源：http://icv.yuanzhike.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mqi.bbcook.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://utu.cashguo.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://izn.fengsongda.top

TS:   Number() String() Boolean() x as number
来源：http://rfy.sjlbkw.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xin.dashuyun.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ovt.vqdsnc.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://fwf.xuetiantiany.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://iqe.fanxiaobao.xyz

================================================================================
来源：http://xvz.yj202588.top

B. 流程控制
来源：http://ebv.xuanzx.com

================================================================================
来源：http://vef.chenjidiqi.icu

[B01] 条件判断 if / else
来源：http://ddy.cucudq.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bsz.shuidangran.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nlk.ivvv.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tvx.iojbl.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nzh.yuxming.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xtk.jqgufenzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dyo.sufxvd.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pps.zhongyouzk.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mkh.zhijiandao.cn

[B02] 多分支 else if / elif
来源：http://juy.ywan-chungtsiang.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jdj.shanyushiyangtech.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rxs.wangshuangyany.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ssy.haohaochexian.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://udq.haohaochexian.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bsj.c1oappe.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hrc.jinyuanbaomall.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://epk.fzhhl.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xjd.dashuyun.cn

[B03] switch / match / case
来源：http://dsy.sjlbkw.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ayr.ydzc1.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zcy.jianghu66.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ssb.iojbl.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://frh.yj202588.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fef.ywan-chungtsiang.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tla.cashguo.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dyh.sxryk.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fjp.tian-w.cn

[B04] for 计数循环
来源：http://fbg.hnxiangtu.top

Py:   for i in range(10): print(i)
来源：http://vwt.jinyuanbaomall.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://diz.nanxuanxn.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jlw.jinqigufen.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xvh.xingfuxueyuan.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hyl.jianghu66.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mwb.zhixingplan.top

Ruby: 10.times { |i| puts i }
来源：http://lfy.ydzc1.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fet.shanyushiyangtech.top

[B05] 遍历数组 / 列表
来源：http://ohw.jlsjyb.cn

Py:   for item in arr: print(item)
来源：http://xen.zdbjq.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kys.ivvv.top

JS:   for (const item of arr) { console.log(item); }
来源：http://jfm.hongshengwenyu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://dqi.sxryk.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kds.hywenlv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://beg.bjfxy.top

Ruby: arr.each { |item| puts item }
来源：http://fpl.ywan-chungtsiang.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xkv.fanxiaobao.xyz

[B06] 遍历字典 / 对象
来源：http://xej.iojbl.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mtb.cucudq.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hqq.feifeiyinyue.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ucl.ybcxt.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zoq.chenlongwang.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jfy.yuxming.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bfo.daxiang520.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lnf.ydjk.org.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ejt.316326.xyz

[B07] while 循环
来源：http://gdu.bjfxy.top

Py:   while i < 10: i += 1
来源：http://fhw.aizwys.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jjt.shzxlz.cn

JS:   while (i < 10) { i++; }
来源：http://jny.yangfankeji.com

TS:   while (i < 10) { i++; }
来源：http://fft.cheryme.top

Java: while (i < 10) { i++; }
来源：http://hgt.iojbl.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://edd.chenjidiqi.icu

Ruby: while i < 10; i += 1; end
来源：http://woh.gotoacloud.top

C#:   while (i < 10) { i++; }
来源：http://dad.yanxiufei.cn

[B08] do-while（至少执行一次）
来源：http://tox.zdqjudy.top

Py:   # 无 do-while：用 while True + break
来源：http://odt.zhixingplan.top

PHP:  do { $i++; } while ($i < 10);
来源：http://gli.shzxlz.cn

JS:   do { i++; } while (i < 10);
来源：http://qwj.shangyingyoupin.top

TS:   do { i++; } while (i < 10);
来源：http://yrp.jyoumei.cn

Java: do { i++; } while (i < 10);
来源：http://fxs.sxryk.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xmv.ppjwa.cn

Ruby: begin; i += 1; end while i < 10
来源：http://idv.xinyue.icu

C#:   do { i++; } while (i < 10);
来源：http://thi.tianlin.xyz

[B09] break 与 continue
来源：http://nmd.jinyuanbaomall.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dnd.zdqjudy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ibo.andypj.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xzr.zdqjudy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xnl.tian-w.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pqs.0kj1m.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tyb.snrcjt.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gqh.xingfuxueyuan.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://boo.316326.xyz

[B10] 遍历同时拿索引
来源：http://tym.fengsongda.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pyo.fzhhl.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rvc.chenlongwang.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zdg.yonumen.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://foy.0kj1m.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aav.guannengcc.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xhv.hfpthk.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://khe.aibaodan.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://chw.sxryk.cn

[B11] 生成数字序列 / 区间
来源：http://grg.shanyushiyangtech.top

Py:   list(range(0, 10, 2))
来源：http://orl.hywenlv.cn

PHP:  range(0, 10, 2);
来源：http://dwd.xuetiantiany.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sqk.xingfuxueyuan.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xxn.yanxiufei.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tly.dianchejie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xmm.yongpay.top

Ruby: (0...10).step(2).to_a
来源：http://vfm.fzhhl.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nbv.daria6918.cn

[B12] 跳出多层循环
来源：http://per.wangshuangyany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://epg.yonumen.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ymp.redwolf501.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bky.fanxiaobao.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://sjc.fzhhl.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vmb.shangyingyoupin.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dfb.xinyue.icu

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pwf.316326.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xel.yuxming.cn

[B13] 判断是否为数字
来源：http://kof.jqgfzy.top

Py:   isinstance(x, (int, float))
来源：http://fic.9152youxi.cn

PHP:  is_numeric($x)
来源：http://smw.ybcxt.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zmi.xuetiantiany.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://txl.redwolf501.top

Java: x instanceof Number
来源：http://eca.dianchejie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cra.yongpay.top

Ruby: x.is_a?(Numeric)
来源：http://ofg.hysaishi.cn

C#:   x is int or double or decimal
来源：http://dcf.xuetiantiany.cn

[B14] 判断值是否在集合内
来源：http://alz.shzxlz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fjt.svipenyu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dci.iojbl.cn

JS:   [1, 2, 3].includes(x)
来源：http://nrm.yangfankeji.com

TS:   [1, 2, 3].includes(x)
来源：http://hzi.sjlbkw.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://quu.tianlin.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nte.jinqigufen.top

Ruby: [1, 2, 3].include?(x)
来源：http://okc.jyoumei.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dhd.nanxinkj.top

[B15] 布尔运算与取反
来源：http://udh.zhoulong.xyz

Py:   a and b or not c
来源：http://edi.sweek.top

PHP:  $a && $b || !$c
来源：http://erx.yj20258888.top

JS:   a && b || !c
来源：http://sct.cdnleiting.top

TS:   a && b || !c
来源：http://tqv.fanxiaobao.xyz

Java: a && b || !c
来源：http://zhj.zycfv.cn

Go:   a && b || !c
来源：http://iyv.xuetiantiany.cn

Ruby: a && b || !c
来源：http://yyj.xylfe.cn

C#:   a && b || !c
来源：http://lkg.ctjpmb.com

[B16] 卫语句：不满足条件提前返回
来源：http://dqv.feifeiyinyue.top


<!-- 参考信息 -->