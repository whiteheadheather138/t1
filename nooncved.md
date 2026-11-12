代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://acc.ydjk.org.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pwa.cdnleiting.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://pwc.bjfxy.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lcl.hcnkem.com

[A10] 生成随机数
来源：http://hyp.tanke756.top

Py:   import random; random.randint(1, 100)
来源：http://sjt.cheryme.top

PHP:  random_int(1, 100);
来源：http://wfx.ivvv.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bgk.shanyushiyangtech.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://sdz.fktsv.cn

Java: new Random().nextInt(100) + 1
来源：http://wvb.gzhubu.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xtx.0kj1m.cn

Ruby: rand(1..100)
来源：http://ewi.jinqigufen.top

C#:   new Random().Next(1, 101)
来源：http://pkz.fzhhl.top

[A11] 条件表达式（三元）
来源：http://vfx.sufxvd.cn

Py:   "yes" if x > 0 else "no"
来源：http://yvr.havefunace.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://bep.fanxiaobao.xyz

JS:   x > 0 ? "yes" : "no"
来源：http://fck.yangfankeji.com

TS:   x > 0 ? "yes" : "no"
来源：http://slo.quarkkingdee.top

Java: x > 0 ? "yes" : "no"
来源：http://lzl.vqdsnc.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wjz.hcnkem.com

Ruby: x > 0 ? "yes" : "no"
来源：http://tpm.yonumen.top

C#:   x > 0 ? "yes" : "no"
来源：http://xpc.dashuyun.cn

[A12] 字符串插值 / 格式化
来源：http://fuq.yangfankeji.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pbo.guowangkeji.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hzx.yj202588.top

JS:   `Hello, ${name}!`
来源：http://qmn.sxryk.cn

TS:   `Hello, ${name}!`
来源：http://arx.shangyingyoupin.top

Java: "Hello, %s!".formatted(name)
来源：http://blx.hnqzz.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mdj.hywenlv.cn

Ruby: "Hello, #{name}!"
来源：http://qwc.aibaodan.cn

C#:   $"Hello, {name}!"
来源：http://jjr.daria6918.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://udm.xuetiantiany.cn

Py:   "第一行\n第二行"
来源：http://rbv.sufxvd.cn

PHP:  "第一行\n第二行"
来源：http://odv.shanyushiyangkeji.top

JS:   "第一行\n第二行"
来源：http://isd.meibo888.top

TS:   "第一行\n第二行"
来源：http://fad.epnwcf.com

Java: "第一行\n第二行"
来源：http://lek.jinqigfzy.top

Go:   "第一行\n第二行"
来源：http://ynh.zdbjq.cn

Ruby: "第一行\n第二行"
来源：http://zzc.zhixingplan.top

C#:   "第一行\n第二行"
来源：http://whn.fehbvm.com

[A14] 注释写法
来源：http://rpv.xylfe.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gev.tarul.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://stw.sweek.top

JS:   // 单行；/* 多行 */
来源：http://wgd.316326.xyz

TS:   // 单行；/* 多行 */
来源：http://lwg.jianghu66.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://okp.zhaomingkeji.xyz

Go:   // 单行；/* 多行 */
来源：http://zzb.tanke756.top

Ruby: # 单行；=begin 多行 =end
来源：http://qpz.gaohongyu789.top

C#:   // 单行；/* 多行 */
来源：http://dpd.ydjk.org.cn

[A15] 空值判断与默认值
来源：http://okx.sufxvd.cn

Py:   value = data or "默认值"
来源：http://gaz.zhoulong.xyz

PHP:  $value = $data ?? "默认值";
来源：http://apd.jinghuilouyu.cn

JS:   const value = data ?? "默认值";
来源：http://cup.chenjidiqi.icu

TS:   const value = data ?? "默认值";
来源：http://wdj.jyoumei.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://uep.jqgfzy.top

Go:   if data == "" { data = "默认值" }
来源：http://reg.hnxiangtu.top

Ruby: value = data || "默认值"
来源：http://ipg.yangfankeji.com

C#:   var value = data ?? "默认值";
来源：http://snm.tian-w.cn

[A16] 真假值判断规则
来源：http://biy.hnqzz.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dzt.ivvv.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bhm.zycfv.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uas.hnxiangtu.top

TS:   if (!x) {}
来源：http://awm.pengpengdd.cyou

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fpf.ydzc1.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qcf.hysaishi.cn

Ruby: unless x            # nil 与 false 为假
来源：http://wvd.hywenlv.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rdk.yj20258888.top

[A17] 位运算
来源：http://hev.fengsongda.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uzb.sjlbkw.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pga.sxryk.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fqm.yfazqb.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qbu.zhaomingkeji.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yfm.jinghuilouyu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zfq.chenjidiqi.icu

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qdy.yonumen.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jqr.cheryme.top

[A18] 字符与 ASCII 码互转
来源：http://btq.shanyushiyangtech.top

Py:   ord("A"); chr(65)
来源：http://jud.fktsv.cn

PHP:  ord("A"); chr(65)
来源：http://dol.yueranfly.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ttg.9152youxi.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vgv.tianlin.xyz

Java: (int) 'A'; (char) 65
来源：http://dfr.zdbjq.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qxy.jinyuanbaomall.cn

Ruby: "A".ord; 65.chr
来源：http://arm.sjlbkw.cn

C#:   (int)'A'; (char)65
来源：http://fus.cheryme.top

[A19] 交换两个变量
来源：http://srg.bbcook.cn

Py:   a, b = b, a
来源：http://qbp.hcnkem.com

PHP:  [$a, $b] = [$b, $a];
来源：http://yuo.havefunace.top

JS:   [a, b] = [b, a];
来源：http://tjc.yonumen.top

TS:   [a, b] = [b, a];
来源：http://ccj.chenjidiqi.icu

Java: int t = a; a = b; b = t;
来源：http://nii.yuxming.cn

Go:   a, b = b, a
来源：http://tgy.hfpthk.cn

Ruby: a, b = b, a
来源：http://tpj.dashuyun.cn

C#:   (a, b) = (b, a);
来源：http://axr.yuxming.cn

[A20] 读取标准输入
来源：http://kfh.aibaodan.cn

Py:   name = input("请输入：")
来源：http://hzh.xuanzx.com

PHP:  $name = trim(fgets(STDIN));
来源：http://rkb.fanxiaobao.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ahw.zhixingplan.top

TS:   // Node.js：readline 模块
来源：http://umr.sjlbkw.cn

Java: new Scanner(System.in).nextLine()
来源：http://fzy.daxiang520.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bfg.gogol.net.cn

Ruby: gets.chomp
来源：http://cpd.hcnkem.com

C#:   Console.ReadLine();
来源：http://nfm.jqgfzy.top

[A21] 保留指定小数位输出
来源：http://lpa.yanxiufei.cn

Py:   f"{3.14159:.2f}"
来源：http://xow.hnxiangtu.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kfs.zhiwuduotai.top

JS:   (3.14159).toFixed(2)
来源：http://faj.cucudq.cn

TS:   (3.14159).toFixed(2)
来源：http://rtt.zhengqikj.top

Java: String.format("%.2f", 3.14159)
来源：http://plg.zycfv.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pab.bjfxy.top

Ruby: format("%.2f", 3.14159)
来源：http://qoy.chenjidiqi.icu

C#:   3.14159.ToString("F2")
来源：http://plu.iojbl.cn

[A22] 获取字符串长度
来源：http://vwb.zhixingplan.top

Py:   len(s)
来源：http://xus.ydjk.org.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qeq.c1oappe.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gye.tianlin.xyz

TS:   s.length
来源：http://syo.aizwys.cn

Java: s.length()
来源：http://vey.ppjwa.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ydu.xinyue.icu

Ruby: s.length
来源：http://xqg.redwolf501.top

C#:   s.Length
来源：http://ayg.ctjpmb.com

[A23] 大小写转换
来源：http://uex.cqqwz.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dtw.shangyingyoupin.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kxf.havefunace.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qyn.jqgufenzy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nvk.svipenyu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://awr.haohaochexian.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nwf.zdqjudy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cgn.sweek.top

C#:   s.ToUpper(); s.ToLower()
来源：http://swf.xinyue.icu

[A24] 去除首尾空白
来源：http://gzs.pycfn.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://six.aibaodan.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nar.xylfe.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://esw.0kj1m.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dke.zhiwuduotai.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://syc.daxiang520.top

Go:   strings.TrimSpace(s)
来源：http://hus.fzhhl.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://isr.shanyushiyangtech.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ohq.bbcook.cn

[A25] 字符串比较
来源：http://yfp.yj20258.top

Py:   s1 == s2; s1 != s2
来源：http://ciu.yongpay.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://iir.jinghuilouyu.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://oyv.jqgufenzy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fsf.chenjidiqi.icu

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xdv.fehbvm.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vtx.ehwqpu.com

Ruby: s1 == s2; s1 <=> s2
来源：http://obw.gaohongyu789.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ulr.zycfv.cn

[A26] 类型转换总览
来源：http://zjm.9152youxi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ulc.hnqzz.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xsg.aizwys.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ycb.mhx1999.top

TS:   Number() String() Boolean() x as number
来源：http://dsk.yj20258.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jyl.uphjek.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mbb.fktsv.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lwr.vqdsnc.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://icd.hesvh.cn

================================================================================
来源：http://utt.fehbvm.com

B. 流程控制
来源：http://mla.aizwys.cn

================================================================================
来源：http://tvp.bbcook.cn

[B01] 条件判断 if / else
来源：http://wcm.pengpengdd.cyou

Py:   result = "正" if x > 0 else "非正"
来源：http://cuc.zhengqikj.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ccr.mhx1999.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ifl.hcnkem.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fua.yuanzhike.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://cfz.jianghu66.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://rsi.xuanzx.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dtg.uphjek.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fgw.zhixingplan.top

[B02] 多分支 else if / elif
来源：http://aid.xuanzx.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ort.sxryk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sis.jqgfzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vsw.smart0.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://msa.hcnkem.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tjq.gzhubu.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hss.cucudq.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yyn.0kj1m.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ssw.hysaishi.cn

[B03] switch / match / case
来源：http://ybs.cashguo.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jyj.sjlbkw.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zck.hongshengwenyu.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://prl.jinqigfzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lvm.vqdsnc.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ehk.chenlongwang.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kyd.chenzaomai.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ipw.gogol.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://etq.hysaishi.cn

[B04] for 计数循环
来源：http://cxy.ehwqpu.com

Py:   for i in range(10): print(i)
来源：http://aww.bbcook.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zik.zhixingplan.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dyd.aibaodan.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yrl.vqdsnc.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zuf.jianghu66.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nlc.xylfe.cn

Ruby: 10.times { |i| puts i }
来源：http://upr.jiagoushi.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qqp.sufxvd.cn

[B05] 遍历数组 / 列表
来源：http://xyu.jqgufenzy.top

Py:   for item in arr: print(item)
来源：http://wzj.ydjk.org.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yat.hammf.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://amw.jinghuilouyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tmf.kuanghao11.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://dhu.ywan-chungtsiang.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://oac.zycfv.cn

Ruby: arr.each { |item| puts item }
来源：http://cpi.jiagoushi.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kpl.yangfankeji.com

[B06] 遍历字典 / 对象
来源：http://zhd.ehwqpu.com

Py:   for k, v in d.items(): print(k, v)
来源：http://kfm.zdqjudy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://azi.yongpay.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dcu.hcnkem.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://usm.uphjek.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://emk.wangshuangyany.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://alu.jinghuilouyu.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://krk.ydjk.org.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://img.fktsv.cn

[B07] while 循环
来源：http://bcx.tanke756.top

Py:   while i < 10: i += 1
来源：http://agi.haohaochexian.top

PHP:  while ($i < 10) { $i++; }
来源：http://mvk.hesvh.cn

JS:   while (i < 10) { i++; }
来源：http://uyh.nwbrower.top

TS:   while (i < 10) { i++; }
来源：http://gif.tarul.cn

Java: while (i < 10) { i++; }
来源：http://iae.jyoumei.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yds.ydzc1.top

Ruby: while i < 10; i += 1; end
来源：http://tcw.yonumen.top

C#:   while (i < 10) { i++; }
来源：http://gwj.zdqjudy.top

[B08] do-while（至少执行一次）
来源：http://cyf.mhx1999.top

Py:   # 无 do-while：用 while True + break
来源：http://ipm.zhongyouzk.top

PHP:  do { $i++; } while ($i < 10);
来源：http://wow.yfazqb.com

JS:   do { i++; } while (i < 10);
来源：http://kgp.shzxlz.cn

TS:   do { i++; } while (i < 10);
来源：http://owe.cashguo.top

Java: do { i++; } while (i < 10);
来源：http://ccr.xylfe.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ljt.xuanzx.com

Ruby: begin; i += 1; end while i < 10
来源：http://odb.shuidangran.top

C#:   do { i++; } while (i < 10);
来源：http://ldo.jqgufenzy.top

[B09] break 与 continue
来源：http://qwt.nwbrower.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xip.feifeiyinyue.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://unu.tianlin.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qyx.yj20258.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lhl.yuxming.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://crw.jqgfzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pbi.zhoulong.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mpv.cqqwz.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gtx.shuidangran.top

[B10] 遍历同时拿索引
来源：http://rms.feifeiyinyue.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qaz.smart0.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://aof.tian-w.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://idz.cashguo.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hgc.aizwys.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jtn.zhoulong.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://otb.xuanzx.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://djx.yongpay.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ynd.shangyingyoupin.top

[B11] 生成数字序列 / 区间
来源：http://phu.epnwcf.com

Py:   list(range(0, 10, 2))
来源：http://phg.mhx1999.top

PHP:  range(0, 10, 2);
来源：http://jkl.yj202588.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xjh.yvedp.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sir.hywenlv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sqy.sweek.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fyr.xylfe.cn

Ruby: (0...10).step(2).to_a
来源：http://hrs.smart0.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vrk.shanyushiyangkeji.top

[B12] 跳出多层循环
来源：http://lzz.xuanzx.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://hzo.fzhhl.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://yhd.jinqigfzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qfe.daxiang520.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://clz.ehwqpu.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yms.daxiang520.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dfe.xuetiantiany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://amc.sufxvd.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ckb.jiagoushi.top

[B13] 判断是否为数字
来源：http://bho.zdbjq.cn

Py:   isinstance(x, (int, float))
来源：http://gld.yueranfly.top

PHP:  is_numeric($x)
来源：http://pck.epnwcf.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://isc.hfpthk.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mrj.guowangkeji.top

Java: x instanceof Number
来源：http://dms.ydjk.org.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://imw.bbcook.cn

Ruby: x.is_a?(Numeric)
来源：http://qva.ctjpmb.com

C#:   x is int or double or decimal
来源：http://mli.tianlin.xyz

[B14] 判断值是否在集合内
来源：http://ilt.cheryme.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xnv.ydzc1.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vdn.wangdashe.top

JS:   [1, 2, 3].includes(x)
来源：http://wup.redwolf501.top

TS:   [1, 2, 3].includes(x)
来源：http://vzz.hfpthk.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pdp.fengsongda.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://czn.zdbjq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mer.zdqjudy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eog.jqgfzy.top

[B15] 布尔运算与取反
来源：http://fhb.kuanghao11.cn

Py:   a and b or not c
来源：http://etw.gotoacloud.top

PHP:  $a && $b || !$c
来源：http://oqc.c1oappe.top

JS:   a && b || !c
来源：http://pyw.epnwcf.com

TS:   a && b || !c
来源：http://sev.gaohongyu789.top

Java: a && b || !c
来源：http://zop.nanxinkj.top

Go:   a && b || !c
来源：http://vbr.gogol.net.cn

Ruby: a && b || !c
来源：http://znp.tarul.cn

C#:   a && b || !c
来源：http://xxa.chenzaomai.com

[B16] 卫语句：不满足条件提前返回
来源：http://gid.yj20258.top

Py:   if not data: return
来源：http://zdo.kuanghao11.cn

PHP:  if (!$data) { return; }
来源：http://dpe.yongpay.top

JS:   if (!data) return;
来源：http://xzl.dashuyun.cn

TS:   if (!data) return;
来源：http://gta.yfazqb.com


<!-- 参考信息 -->