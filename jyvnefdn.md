代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://aks.hnxiangtu.top

[A11] 条件表达式（三元）
来源：http://hwg.yuxming.cn

Py:   "yes" if x > 0 else "no"
来源：http://amm.nanxinkj.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://iix.shangyingyoupin.top

JS:   x > 0 ? "yes" : "no"
来源：http://bld.yonumen.top

TS:   x > 0 ? "yes" : "no"
来源：http://bhz.hesvh.cn

Java: x > 0 ? "yes" : "no"
来源：http://sji.svipenyu.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://bvg.dianchejie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://eac.pengpengdd.cyou

C#:   x > 0 ? "yes" : "no"
来源：http://iqt.fehbvm.com

[A12] 字符串插值 / 格式化
来源：http://syu.yanxiufei.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://lli.zdbjq.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zsw.hysaishi.cn

JS:   `Hello, ${name}!`
来源：http://lkr.quarkkingdee.top

TS:   `Hello, ${name}!`
来源：http://cnz.nwbrower.top

Java: "Hello, %s!".formatted(name)
来源：http://bnr.yuanzhike.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://aeo.cqqwz.cn

Ruby: "Hello, #{name}!"
来源：http://lki.cashguo.top

C#:   $"Hello, {name}!"
来源：http://nea.ybcxt.top

[A13] 多行字符串（练习 \n 转义）
来源：http://vsi.fengsongda.top

Py:   "第一行\n第二行"
来源：http://pwz.tanke756.top

PHP:  "第一行\n第二行"
来源：http://xgn.shuidangran.top

JS:   "第一行\n第二行"
来源：http://fyn.aizwys.cn

TS:   "第一行\n第二行"
来源：http://qxe.chenjidiqi.icu

Java: "第一行\n第二行"
来源：http://zra.gogol.net.cn

Go:   "第一行\n第二行"
来源：http://bjc.svipenyu.cn

Ruby: "第一行\n第二行"
来源：http://phv.9152youxi.cn

C#:   "第一行\n第二行"
来源：http://arh.pengpengdd.cyou

[A14] 注释写法
来源：http://tck.aibaodan.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://bys.ydzc1.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://gwo.yongpay.top

JS:   // 单行；/* 多行 */
来源：http://pgs.kuanghao11.cn

TS:   // 单行；/* 多行 */
来源：http://uzd.dashuyun.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kql.yueranfly.top

Go:   // 单行；/* 多行 */
来源：http://cwv.iojbl.cn

Ruby: # 单行；=begin 多行 =end
来源：http://llu.zdqjudy.top

C#:   // 单行；/* 多行 */
来源：http://dpd.316326.xyz

[A15] 空值判断与默认值
来源：http://znw.jinqigufen.top

Py:   value = data or "默认值"
来源：http://pkv.hnxiangtu.top

PHP:  $value = $data ?? "默认值";
来源：http://ctl.zhiwuduotai.top

JS:   const value = data ?? "默认值";
来源：http://scq.zhengqikj.top

TS:   const value = data ?? "默认值";
来源：http://ooy.cashguo.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://fge.aizwys.cn

Go:   if data == "" { data = "默认值" }
来源：http://sze.yj20258888.top

Ruby: value = data || "默认值"
来源：http://htx.zhoulong.xyz

C#:   var value = data ?? "默认值";
来源：http://oav.xziqi.cn

[A16] 真假值判断规则
来源：http://ild.chenjidiqi.icu

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://egh.bbcook.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://clv.ydzc1.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gnz.zdbjq.cn

TS:   if (!x) {}
来源：http://mfv.shzxlz.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dmg.haohaochexian.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xvb.yj202588.top

Ruby: unless x            # nil 与 false 为假
来源：http://iix.jqgfzy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vqz.tianlin.xyz

[A17] 位运算
来源：http://jog.zhaomingkeji.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bez.smart0.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xgy.ywan-chungtsiang.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wpg.aizwys.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nrd.52xcode.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ngj.cucudq.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kis.tian-w.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vut.bbcook.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mbd.daxiang520.top

[A18] 字符与 ASCII 码互转
来源：http://njv.shangyingyoupin.top

Py:   ord("A"); chr(65)
来源：http://xnh.hnqzz.top

PHP:  ord("A"); chr(65)
来源：http://evn.haohaochexian.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ina.cheryme.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nuv.ehwqpu.com

Java: (int) 'A'; (char) 65
来源：http://fqv.bbcook.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qlb.zdqjudy.top

Ruby: "A".ord; 65.chr
来源：http://xmc.pengpengdd.cyou

C#:   (int)'A'; (char)65
来源：http://rjn.52xcode.cn

[A19] 交换两个变量
来源：http://ghh.guannengcc.top

Py:   a, b = b, a
来源：http://qmz.fktsv.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://emo.gzhubu.top

JS:   [a, b] = [b, a];
来源：http://jyk.yj20258888.top

TS:   [a, b] = [b, a];
来源：http://yrw.shangyingyoupin.top

Java: int t = a; a = b; b = t;
来源：http://kcz.zhengqikj.top

Go:   a, b = b, a
来源：http://lbx.zdbjq.cn

Ruby: a, b = b, a
来源：http://idm.nanxuanxn.top

C#:   (a, b) = (b, a);
来源：http://owy.yvedp.cn

[A20] 读取标准输入
来源：http://ksd.yangfankeji.com

Py:   name = input("请输入：")
来源：http://ibt.ivvv.top

PHP:  $name = trim(fgets(STDIN));
来源：http://lxi.xinyue.icu

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fck.shangyingyoupin.top

TS:   // Node.js：readline 模块
来源：http://jgz.pycfn.com

Java: new Scanner(System.in).nextLine()
来源：http://tmf.bjfxy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jav.yonumen.top

Ruby: gets.chomp
来源：http://igg.haohaochexian.top

C#:   Console.ReadLine();
来源：http://tqn.gogol.net.cn

[A21] 保留指定小数位输出
来源：http://txv.chenzaomai.com

Py:   f"{3.14159:.2f}"
来源：http://yrz.yj20258.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://obh.xinyue.icu

JS:   (3.14159).toFixed(2)
来源：http://dhv.316326.xyz

TS:   (3.14159).toFixed(2)
来源：http://alk.hnxiangtu.top

Java: String.format("%.2f", 3.14159)
来源：http://hwj.epnwcf.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zai.hesvh.cn

Ruby: format("%.2f", 3.14159)
来源：http://jdp.jinyuanbaomall.cn

C#:   3.14159.ToString("F2")
来源：http://eqn.feifeiyinyue.top

[A22] 获取字符串长度
来源：http://aaw.tarul.cn

Py:   len(s)
来源：http://mpz.jiagoushi.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ggc.iojbl.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rzo.feifeiyinyue.top

TS:   s.length
来源：http://eqq.jinqigfzy.top

Java: s.length()
来源：http://ydp.zhiwuduotai.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://puc.cashguo.top

Ruby: s.length
来源：http://ycu.yvedp.cn

C#:   s.Length
来源：http://ati.svipenyu.cn

[A23] 大小写转换
来源：http://agp.jinghuilouyu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://qep.redwolf501.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zmb.dashuyun.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tot.pycfn.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fqu.zhijiandao.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jwu.yongpay.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tsa.feifeiyinyue.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wcj.jqgfzy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://pof.xingfuxueyuan.xyz

[A24] 去除首尾空白
来源：http://fmr.xziqi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kbw.daxiang520.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://svv.yvedp.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lcl.jinqigfzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fzg.snrcjt.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bli.jlsjyb.cn

Go:   strings.TrimSpace(s)
来源：http://mvy.mhx1999.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://scf.zdbjq.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://trn.yfazqb.com

[A25] 字符串比较
来源：http://ofq.dianchejie.cn

Py:   s1 == s2; s1 != s2
来源：http://kfk.guannengcc.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://khs.gzhubu.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://efr.chenlongwang.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://aoc.xziqi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uby.guowangkeji.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://srx.zdqjudy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ujd.zhijiandao.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://eoq.shangyingyoupin.top

[A26] 类型转换总览
来源：http://nfb.jyoumei.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://orf.shzxlz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://yxw.jlsjyb.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oua.guowangkeji.top

TS:   Number() String() Boolean() x as number
来源：http://zld.ivvv.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wum.shangyingyoupin.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kgf.ywan-chungtsiang.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://wpi.jinqigfzy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wjr.dianchejie.cn

================================================================================
来源：http://abj.zdqjudy.top

B. 流程控制
来源：http://yfm.epnwcf.com

================================================================================
来源：http://jim.dashuyun.cn

[B01] 条件判断 if / else
来源：http://fmy.fengsongda.top

Py:   result = "正" if x > 0 else "非正"
来源：http://cqm.meibo888.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yur.nwbrower.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://spc.wangdashe.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bhk.gotoacloud.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://wwf.jinqigufen.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vvn.shzxlz.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ixq.birdmap.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mls.fzhhl.top

[B02] 多分支 else if / elif
来源：http://toq.nwbrower.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fvr.zhiwuduotai.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yqg.jinqigufen.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oyx.vehdjk.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pse.jinghuilouyu.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aoz.birdmap.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ipm.cucudq.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://khk.ydjk.org.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bxq.shangyingyoupin.top

[B03] switch / match / case
来源：http://hqf.hongshengwenyu.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yri.yj20258.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://olv.xylfe.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nht.zhongyouzk.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cti.shzxlz.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pgf.jlsjyb.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nzw.wangshuangyany.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sph.fzhhl.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vtr.jinghuilouyu.cn

[B04] for 计数循环
来源：http://lnh.hysaishi.cn

Py:   for i in range(10): print(i)
来源：http://ysz.andypj.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tsq.chenjidiqi.icu

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ekz.chenjidiqi.icu

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hes.xuetiantiany.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mah.ehwqpu.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yrg.xingfuxueyuan.xyz

Ruby: 10.times { |i| puts i }
来源：http://qcq.pengpengdd.cyou

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://htb.zhengqikj.top

[B05] 遍历数组 / 列表
来源：http://kpi.ywan-chungtsiang.top

Py:   for item in arr: print(item)
来源：http://ekk.xuetiantiany.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ehu.yuxming.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qyr.xuetiantiany.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fpy.xziqi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hzl.316326.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://elr.ctjpmb.com

Ruby: arr.each { |item| puts item }
来源：http://dbn.zdbjq.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uge.snrcjt.cn

[B06] 遍历字典 / 对象
来源：http://ldd.fehbvm.com

Py:   for k, v in d.items(): print(k, v)
来源：http://imb.fengsongda.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dsq.zhijiandao.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sgb.yj20258.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://glw.xziqi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fhj.xinyue.icu

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hmm.tanke756.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hfv.meibo888.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://eof.quarkkingdee.top

[B07] while 循环
来源：http://ltf.ppjwa.cn

Py:   while i < 10: i += 1
来源：http://zhr.fengsongda.top

PHP:  while ($i < 10) { $i++; }
来源：http://ero.quarkkingdee.top

JS:   while (i < 10) { i++; }
来源：http://ypk.shangyingyoupin.top

TS:   while (i < 10) { i++; }
来源：http://nrh.ydzc1.top

Java: while (i < 10) { i++; }
来源：http://ncr.gogol.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wyb.zhixingplan.top

Ruby: while i < 10; i += 1; end
来源：http://orw.tanke756.top

C#:   while (i < 10) { i++; }
来源：http://sfd.ppjwa.cn

[B08] do-while（至少执行一次）
来源：http://onv.zhiwuduotai.top

Py:   # 无 do-while：用 while True + break
来源：http://wsn.yongpay.top

PHP:  do { $i++; } while ($i < 10);
来源：http://kip.hnqzz.top

JS:   do { i++; } while (i < 10);
来源：http://vxc.zhixingplan.top

TS:   do { i++; } while (i < 10);
来源：http://bpt.guowangkeji.top

Java: do { i++; } while (i < 10);
来源：http://qle.ydzc1.top

Go:   for { i++; if i >= 10 { break } }
来源：http://tsy.jlsjyb.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tfu.cucudq.cn

C#:   do { i++; } while (i < 10);
来源：http://jrg.sjlbkw.cn

[B09] break 与 continue
来源：http://ywy.smart0.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://eqo.zhaomingkeji.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nfm.cqqwz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zpj.sufxvd.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qdk.xinyue.icu

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xqe.jianghu66.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gmd.shzxlz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hyl.hongshengwenyu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pzp.xuanzx.com

[B10] 遍历同时拿索引
来源：http://vzq.xuanzx.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kss.hywenlv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ese.sjlbkw.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://okz.yuanzhike.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kby.52xcode.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rmz.smart0.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bel.yongpay.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vxv.dianchejie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ckn.0kj1m.cn

[B11] 生成数字序列 / 区间
来源：http://wqi.wangdashe.top

Py:   list(range(0, 10, 2))
来源：http://cev.bbcook.cn

PHP:  range(0, 10, 2);
来源：http://myh.yongpay.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cqw.guannengcc.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kvx.daria6918.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eto.jinqigfzy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hpr.shanyushiyangkeji.top

Ruby: (0...10).step(2).to_a
来源：http://ssd.hesvh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uqj.shanyushiyangtech.top

[B12] 跳出多层循环
来源：http://ovp.zdbjq.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://pja.snrcjt.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hft.jinghuilouyu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tam.birdmap.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://eyx.gogol.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vfl.pengpengdd.cyou

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hmg.zdbjq.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ekl.jinghuilouyu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uxf.yuxming.cn

[B13] 判断是否为数字
来源：http://ffb.guowangkeji.top

Py:   isinstance(x, (int, float))
来源：http://blh.mhx1999.top

PHP:  is_numeric($x)
来源：http://efg.kuanghao11.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://frc.cqqwz.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jed.birdmap.top

Java: x instanceof Number
来源：http://per.aibaodan.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://thv.ywan-chungtsiang.top

Ruby: x.is_a?(Numeric)
来源：http://rob.sysykeji.top

C#:   x is int or double or decimal
来源：http://gbu.dashuyun.cn

[B14] 判断值是否在集合内
来源：http://zlt.bbcook.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://usb.zhaomingkeji.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bhp.yuxming.cn

JS:   [1, 2, 3].includes(x)
来源：http://ahj.tian-w.cn

TS:   [1, 2, 3].includes(x)
来源：http://zpz.hnqzz.top

Java: List.of(1, 2, 3).contains(x)
来源：http://sbb.tianlin.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pby.cucudq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lhj.gogol.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gpb.bjfxy.top

[B15] 布尔运算与取反
来源：http://tlu.shanyushiyangkeji.top

Py:   a and b or not c
来源：http://kmn.ivvv.top

PHP:  $a && $b || !$c
来源：http://zqj.zdqjudy.top

JS:   a && b || !c
来源：http://kkl.quarkkingdee.top

TS:   a && b || !c
来源：http://vww.quarkkingdee.top

Java: a && b || !c
来源：http://vcs.ydjk.org.cn

Go:   a && b || !c
来源：http://yuk.xziqi.cn

Ruby: a && b || !c
来源：http://sav.xylfe.cn

C#:   a && b || !c
来源：http://afz.hysaishi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://drc.yj20258.top

Py:   if not data: return
来源：http://ftw.svipenyu.cn

PHP:  if (!$data) { return; }
来源：http://oja.snrcjt.cn

JS:   if (!data) return;
来源：http://qqv.shuidangran.top

TS:   if (!data) return;
来源：http://hhx.xziqi.cn

Java: if (data == null) return;
来源：http://ofk.vehdjk.com

Go:   if data == nil { return }
来源：http://hiy.quarkkingdee.top

Ruby: return if data.nil?
来源：http://qqo.ivvv.top

C#:   if (data == null) return;
来源：http://asd.hammf.cn

================================================================================
来源：http://lts.nanxuanxn.top

C. 函数与作用域
来源：http://frl.zhaomingkeji.xyz

================================================================================
来源：http://rhz.cdnleiting.top

[C01] 定义函数
来源：http://hgu.guowangkeji.top

Py:   def add(a, b): return a + b
来源：http://urk.cheryme.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fzf.hcnkem.com

JS:   function add(a, b) { return a + b; }
来源：http://ocv.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eig.pengpengdd.cyou


<!-- 参考信息 -->