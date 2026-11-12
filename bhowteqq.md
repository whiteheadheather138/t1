代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sgv.zdbjq.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qxv.fktsv.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://rxs.jyoumei.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://msi.dashuyun.cn

[A10] 生成随机数
来源：http://zff.ydzc1.top

Py:   import random; random.randint(1, 100)
来源：http://erh.gogol.net.cn

PHP:  random_int(1, 100);
来源：http://pgh.zdqjudy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://gfa.yangfankeji.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mmn.sufxvd.cn

Java: new Random().nextInt(100) + 1
来源：http://ewy.c1oappe.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pxa.yvedp.cn

Ruby: rand(1..100)
来源：http://ytc.cashguo.top

C#:   new Random().Next(1, 101)
来源：http://jqq.mhx1999.top

[A11] 条件表达式（三元）
来源：http://ojj.yj20258.top

Py:   "yes" if x > 0 else "no"
来源：http://vhf.chenzaomai.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://dde.hywenlv.cn

JS:   x > 0 ? "yes" : "no"
来源：http://dvn.mhx1999.top

TS:   x > 0 ? "yes" : "no"
来源：http://qju.jianghu66.top

Java: x > 0 ? "yes" : "no"
来源：http://vfi.gotoacloud.top

Go:   // 无三元运算符，需用 if 语句
来源：http://pmj.hammf.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://omu.zhengqikj.top

C#:   x > 0 ? "yes" : "no"
来源：http://nxq.dianchejie.cn

[A12] 字符串插值 / 格式化
来源：http://bcq.hywenlv.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://avy.hesvh.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fig.sufxvd.cn

JS:   `Hello, ${name}!`
来源：http://iyp.jinqigfzy.top

TS:   `Hello, ${name}!`
来源：http://cip.hnxiangtu.top

Java: "Hello, %s!".formatted(name)
来源：http://sxn.kuanghao11.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://uvd.shuidangran.top

Ruby: "Hello, #{name}!"
来源：http://pvq.hywenlv.cn

C#:   $"Hello, {name}!"
来源：http://cxj.fengsongda.top

[A13] 多行字符串（练习 \n 转义）
来源：http://lko.guowangkeji.top

Py:   "第一行\n第二行"
来源：http://mfo.xylfe.cn

PHP:  "第一行\n第二行"
来源：http://tod.9152youxi.cn

JS:   "第一行\n第二行"
来源：http://apn.tianlin.xyz

TS:   "第一行\n第二行"
来源：http://xry.tian-w.cn

Java: "第一行\n第二行"
来源：http://enf.iojbl.cn

Go:   "第一行\n第二行"
来源：http://gff.meibo888.top

Ruby: "第一行\n第二行"
来源：http://apn.chenzaomai.com

C#:   "第一行\n第二行"
来源：http://uvy.nanxinkj.top

[A14] 注释写法
来源：http://bdk.pengpengdd.cyou

Py:   # 单行；三引号字符串可作多行说明
来源：http://dom.smart0.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://syq.ppjwa.cn

JS:   // 单行；/* 多行 */
来源：http://ydz.bbcook.cn

TS:   // 单行；/* 多行 */
来源：http://mxn.52xcode.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ssu.svipenyu.cn

Go:   // 单行；/* 多行 */
来源：http://xoq.chenjidiqi.icu

Ruby: # 单行；=begin 多行 =end
来源：http://rwa.zhiwuduotai.top

C#:   // 单行；/* 多行 */
来源：http://uoy.zhiwuduotai.top

[A15] 空值判断与默认值
来源：http://ilc.fzhhl.top

Py:   value = data or "默认值"
来源：http://vqh.tarul.cn

PHP:  $value = $data ?? "默认值";
来源：http://kwt.tianlin.xyz

JS:   const value = data ?? "默认值";
来源：http://jzs.shuidangran.top

TS:   const value = data ?? "默认值";
来源：http://gsf.fengsongda.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://aou.cashguo.top

Go:   if data == "" { data = "默认值" }
来源：http://nmh.bjfxy.top

Ruby: value = data || "默认值"
来源：http://wqf.jlsjyb.cn

C#:   var value = data ?? "默认值";
来源：http://awg.hesvh.cn

[A16] 真假值判断规则
来源：http://ify.xingfuxueyuan.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xfq.zycfv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zin.jqgufenzy.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nih.zdqjudy.top

TS:   if (!x) {}
来源：http://hno.zhengqikj.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mad.ybcxt.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qkh.tanke756.top

Ruby: unless x            # nil 与 false 为假
来源：http://gjs.nanxuanxn.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jlk.quarkkingdee.top

[A17] 位运算
来源：http://bpa.quarkkingdee.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://axi.zhengqikj.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fks.cucudq.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cwy.epnwcf.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://urv.nanxuanxn.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nfb.jinghuilouyu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ewm.hammf.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dxn.dianchejie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ozz.yuanzhike.top

[A18] 字符与 ASCII 码互转
来源：http://ycw.pengpengdd.cyou

Py:   ord("A"); chr(65)
来源：http://exk.dianchejie.cn

PHP:  ord("A"); chr(65)
来源：http://ftx.meibo888.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lvf.quarkkingdee.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ewg.guowangkeji.top

Java: (int) 'A'; (char) 65
来源：http://aou.shanyushiyangtech.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ujw.cashguo.top

Ruby: "A".ord; 65.chr
来源：http://xjr.52xcode.cn

C#:   (int)'A'; (char)65
来源：http://oys.xingfuxueyuan.xyz

[A19] 交换两个变量
来源：http://unc.yuxming.cn

Py:   a, b = b, a
来源：http://uuu.wangshuangyany.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://lgc.kuanghao11.cn

JS:   [a, b] = [b, a];
来源：http://npl.xuanzx.com

TS:   [a, b] = [b, a];
来源：http://zcp.haohaochexian.top

Java: int t = a; a = b; b = t;
来源：http://qlm.gotoacloud.top

Go:   a, b = b, a
来源：http://zcv.haohaochexian.top

Ruby: a, b = b, a
来源：http://hrb.epnwcf.com

C#:   (a, b) = (b, a);
来源：http://ben.yongpay.top

[A20] 读取标准输入
来源：http://ews.ybcxt.top

Py:   name = input("请输入：")
来源：http://sxe.svipenyu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://nep.birdmap.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zbj.daria6918.cn

TS:   // Node.js：readline 模块
来源：http://ivg.dianchejie.cn

Java: new Scanner(System.in).nextLine()
来源：http://ktf.pengpengdd.cyou

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ugw.hnxiangtu.top

Ruby: gets.chomp
来源：http://clq.jinyuanbaomall.cn

C#:   Console.ReadLine();
来源：http://unk.sufxvd.cn

[A21] 保留指定小数位输出
来源：http://qkf.feifeiyinyue.top

Py:   f"{3.14159:.2f}"
来源：http://fig.pengpengdd.cyou

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://exl.zhongyouzk.top

JS:   (3.14159).toFixed(2)
来源：http://txs.bbcook.cn

TS:   (3.14159).toFixed(2)
来源：http://qvv.svipenyu.cn

Java: String.format("%.2f", 3.14159)
来源：http://kzb.svipenyu.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mph.shangyingyoupin.top

Ruby: format("%.2f", 3.14159)
来源：http://rjb.jlsjyb.cn

C#:   3.14159.ToString("F2")
来源：http://roj.yanxiufei.cn

[A22] 获取字符串长度
来源：http://giw.jiagoushi.top

Py:   len(s)
来源：http://xog.shuidangran.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hvj.zdqjudy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://enc.gaohongyu789.top

TS:   s.length
来源：http://uif.zhiwuduotai.top

Java: s.length()
来源：http://ezl.sjlbkw.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qga.tarul.cn

Ruby: s.length
来源：http://gqa.zhongyouzk.top

C#:   s.Length
来源：http://oqb.zdbjq.cn

[A23] 大小写转换
来源：http://aqo.0kj1m.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jes.chenlongwang.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xkm.daxiang520.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gsc.ydzc1.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.fzhhl.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bcw.zhiwuduotai.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mfs.cashguo.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://btu.zhoulong.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://wlx.ppjwa.cn

[A24] 去除首尾空白
来源：http://qdo.c1oappe.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hzp.guannengcc.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://aho.cqqwz.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lmq.9152youxi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qtw.cqqwz.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tql.gzhubu.top

Go:   strings.TrimSpace(s)
来源：http://heu.vqdsnc.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bto.yongpay.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://whb.ybcxt.top

[A25] 字符串比较
来源：http://lne.mhx1999.top

Py:   s1 == s2; s1 != s2
来源：http://mcc.jinqigufen.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uut.jinqigufen.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jhj.feifeiyinyue.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://smg.epnwcf.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mdi.zdqjudy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://chv.sxryk.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lnb.mhx1999.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rxi.hesvh.cn

[A26] 类型转换总览
来源：http://szp.zycfv.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kdw.fzhhl.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://umv.hfpthk.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gcw.jqgufenzy.top

TS:   Number() String() Boolean() x as number
来源：http://ygt.zhaomingkeji.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vgq.smart0.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://njq.yj20258.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://bxh.yangfankeji.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nhx.hysaishi.cn

================================================================================
来源：http://iws.sxryk.cn

B. 流程控制
来源：http://tkv.hcnkem.com

================================================================================
来源：http://udj.xuanzx.com

[B01] 条件判断 if / else
来源：http://uad.xziqi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mux.gaohongyu789.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://grh.bjfxy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://nyp.yuxming.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qum.ydzc1.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://bdr.nanxinkj.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kvo.hongshengwenyu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qtv.9152youxi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zjh.birdmap.top

[B02] 多分支 else if / elif
来源：http://yvh.sjlbkw.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uya.tianlin.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wtn.chenjidiqi.icu

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qnd.jqgufenzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sei.yj20258888.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ggk.svipenyu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ftp.tianlin.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://scg.cqqwz.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wph.havefunace.top

[B03] switch / match / case
来源：http://ssb.epnwcf.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ukp.xziqi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bww.ctjpmb.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wlg.ydjk.org.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pep.tarul.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xwf.gzhubu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uhv.ydzc1.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ssd.hongshengwenyu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ixv.hcnkem.com

[B04] for 计数循环
来源：http://wvd.ehwqpu.com

Py:   for i in range(10): print(i)
来源：http://qdt.zhaomingkeji.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gac.tanke756.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lwx.zhixingplan.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://enf.hysaishi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gnq.tianlin.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ewq.yuxming.cn

Ruby: 10.times { |i| puts i }
来源：http://xfj.snrcjt.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qng.nanxinkj.top

[B05] 遍历数组 / 列表
来源：http://eri.fzhhl.top

Py:   for item in arr: print(item)
来源：http://yyq.smart0.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cgp.daria6918.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://txk.hfpthk.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://epr.epnwcf.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://bcf.xziqi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lcy.xinyue.icu

Ruby: arr.each { |item| puts item }
来源：http://zmt.havefunace.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tgz.zhijiandao.cn

[B06] 遍历字典 / 对象
来源：http://baw.yj20258888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://azw.nanxinkj.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ybe.tian-w.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kyh.ehwqpu.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eem.yuanzhike.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lhg.fktsv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xgm.vehdjk.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vux.fzhhl.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://noo.hnxiangtu.top

[B07] while 循环
来源：http://eim.xylfe.cn

Py:   while i < 10: i += 1
来源：http://dzs.yonumen.top

PHP:  while ($i < 10) { $i++; }
来源：http://uvw.sysykeji.top

JS:   while (i < 10) { i++; }
来源：http://nvh.ivvv.top

TS:   while (i < 10) { i++; }
来源：http://dkp.yangfankeji.com

Java: while (i < 10) { i++; }
来源：http://tqo.hywenlv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bid.xingfuxueyuan.xyz

Ruby: while i < 10; i += 1; end
来源：http://eev.sjlbkw.cn

C#:   while (i < 10) { i++; }
来源：http://qtt.0kj1m.cn

[B08] do-while（至少执行一次）
来源：http://ogu.xziqi.cn

Py:   # 无 do-while：用 while True + break
来源：http://jnx.bbcook.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://iba.yj20258888.top

JS:   do { i++; } while (i < 10);
来源：http://crr.aizwys.cn

TS:   do { i++; } while (i < 10);
来源：http://lma.nwbrower.top

Java: do { i++; } while (i < 10);
来源：http://how.sjlbkw.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://sbb.sjlbkw.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hsa.dianchejie.cn

C#:   do { i++; } while (i < 10);
来源：http://mzn.gotoacloud.top

[B09] break 与 continue
来源：http://trq.tarul.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wll.52xcode.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hpk.birdmap.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dmw.yfazqb.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://boh.yfazqb.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rim.ppjwa.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wht.zhijiandao.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://itg.xuanzx.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jyg.zdqjudy.top

[B10] 遍历同时拿索引
来源：http://wiq.jinqigfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mec.shzxlz.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nnz.bjfxy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://iea.sysykeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oxn.haohaochexian.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jgr.iojbl.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://afc.jianghu66.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vzs.shangyingyoupin.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jeq.wangshuangyany.cn

[B11] 生成数字序列 / 区间
来源：http://abx.hnqzz.top

Py:   list(range(0, 10, 2))
来源：http://tqi.gogol.net.cn

PHP:  range(0, 10, 2);
来源：http://wzv.chenzaomai.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rrg.gaohongyu789.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hhu.hesvh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://iqm.aizwys.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ukw.yuxming.cn

Ruby: (0...10).step(2).to_a
来源：http://cpt.iojbl.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nql.mhx1999.top

[B12] 跳出多层循环
来源：http://qvc.fanxiaobao.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://baz.ywan-chungtsiang.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://lez.xuanzx.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pvp.zhoulong.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tvw.aibaodan.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ijg.dashuyun.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xtb.epnwcf.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://esc.hammf.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xba.sweek.top

[B13] 判断是否为数字
来源：http://cvw.meibo888.top

Py:   isinstance(x, (int, float))
来源：http://gqr.yueranfly.top

PHP:  is_numeric($x)
来源：http://kng.9152youxi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ttj.meibo888.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fnr.9152youxi.cn

Java: x instanceof Number
来源：http://hcv.bjfxy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ore.jinqigufen.top

Ruby: x.is_a?(Numeric)
来源：http://xcb.yj20258888.top

C#:   x is int or double or decimal
来源：http://ncn.chenlongwang.top

[B14] 判断值是否在集合内
来源：http://sjo.gogol.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zrk.yanxiufei.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xdh.dianchejie.cn

JS:   [1, 2, 3].includes(x)
来源：http://erm.zhijiandao.cn

TS:   [1, 2, 3].includes(x)
来源：http://vlk.ydjk.org.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hgn.yj20258888.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sgi.nwbrower.top

Ruby: [1, 2, 3].include?(x)
来源：http://wnk.vqdsnc.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://auh.cqqwz.cn

[B15] 布尔运算与取反
来源：http://qtm.xingfuxueyuan.xyz

Py:   a and b or not c
来源：http://bky.hfpthk.cn

PHP:  $a && $b || !$c
来源：http://lsj.fanxiaobao.xyz

JS:   a && b || !c
来源：http://fpp.xuanzx.com

TS:   a && b || !c
来源：http://wtw.zhoulong.xyz

Java: a && b || !c
来源：http://eit.zhiwuduotai.top

Go:   a && b || !c
来源：http://oil.jyoumei.cn

Ruby: a && b || !c
来源：http://pwn.chenlongwang.top

C#:   a && b || !c
来源：http://qzj.c1oappe.top

[B16] 卫语句：不满足条件提前返回
来源：http://vjh.xuanzx.com

Py:   if not data: return
来源：http://qak.hcnkem.com

PHP:  if (!$data) { return; }
来源：http://jvp.guowangkeji.top

JS:   if (!data) return;
来源：http://zaa.shanyushiyangkeji.top

TS:   if (!data) return;
来源：http://dlb.gzhubu.top


<!-- 参考信息 -->