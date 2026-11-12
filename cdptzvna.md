代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nat.fktsv.cn

Java: new Random().nextInt(100) + 1
来源：http://ook.aizwys.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xxs.iojbl.cn

Ruby: rand(1..100)
来源：http://qzp.yuanzhike.top

C#:   new Random().Next(1, 101)
来源：http://lxy.aibaodan.cn

[A11] 条件表达式（三元）
来源：http://cif.vehdjk.com

Py:   "yes" if x > 0 else "no"
来源：http://goj.meibo888.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://miw.hywenlv.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vhe.zycfv.cn

TS:   x > 0 ? "yes" : "no"
来源：http://rxm.andypj.xyz

Java: x > 0 ? "yes" : "no"
来源：http://hxp.sysykeji.top

Go:   // 无三元运算符，需用 if 语句
来源：http://fex.feifeiyinyue.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ggn.shanyushiyangkeji.top

C#:   x > 0 ? "yes" : "no"
来源：http://kvl.bjfxy.top

[A12] 字符串插值 / 格式化
来源：http://sqj.tianlin.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xfd.jqgfzy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rwe.gaohongyu789.top

JS:   `Hello, ${name}!`
来源：http://eak.sxryk.cn

TS:   `Hello, ${name}!`
来源：http://rnu.sjlbkw.cn

Java: "Hello, %s!".formatted(name)
来源：http://jps.andypj.xyz

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://jrb.quarkkingdee.top

Ruby: "Hello, #{name}!"
来源：http://fbc.zhongyouzk.top

C#:   $"Hello, {name}!"
来源：http://zom.vqdsnc.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://fqe.ydjk.org.cn

Py:   "第一行\n第二行"
来源：http://wed.zdbjq.cn

PHP:  "第一行\n第二行"
来源：http://eqk.fehbvm.com

JS:   "第一行\n第二行"
来源：http://svw.fktsv.cn

TS:   "第一行\n第二行"
来源：http://yjj.bbcook.cn

Java: "第一行\n第二行"
来源：http://xfb.fanxiaobao.xyz

Go:   "第一行\n第二行"
来源：http://gml.daria6918.cn

Ruby: "第一行\n第二行"
来源：http://guy.quarkkingdee.top

C#:   "第一行\n第二行"
来源：http://cco.zhijiandao.cn

[A14] 注释写法
来源：http://kgq.zycfv.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wpp.haohaochexian.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://frn.yuanzhike.top

JS:   // 单行；/* 多行 */
来源：http://rdg.gzhubu.top

TS:   // 单行；/* 多行 */
来源：http://fgn.fehbvm.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://iti.ctjpmb.com

Go:   // 单行；/* 多行 */
来源：http://ema.316326.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://qts.sxryk.cn

C#:   // 单行；/* 多行 */
来源：http://kpf.nwbrower.top

[A15] 空值判断与默认值
来源：http://ecv.ywan-chungtsiang.top

Py:   value = data or "默认值"
来源：http://quh.xingfuxueyuan.xyz

PHP:  $value = $data ?? "默认值";
来源：http://vfd.ehwqpu.com

JS:   const value = data ?? "默认值";
来源：http://nya.nanxinkj.top

TS:   const value = data ?? "默认值";
来源：http://shs.shuidangran.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mqa.hnqzz.top

Go:   if data == "" { data = "默认值" }
来源：http://erb.tanke756.top

Ruby: value = data || "默认值"
来源：http://mfj.daria6918.cn

C#:   var value = data ?? "默认值";
来源：http://lmz.jinghuilouyu.cn

[A16] 真假值判断规则
来源：http://for.sufxvd.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://izh.yj20258888.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zhw.316326.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pll.yongpay.top

TS:   if (!x) {}
来源：http://fax.nanxinkj.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gqw.mhx1999.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qei.zhengqikj.top

Ruby: unless x            # nil 与 false 为假
来源：http://rdd.jinqigfzy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jyf.gogol.net.cn

[A17] 位运算
来源：http://xzr.guowangkeji.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kna.ywan-chungtsiang.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://prz.sjlbkw.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mml.cdnleiting.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ioq.zhoulong.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lcj.zhoulong.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cmh.hfpthk.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hjq.ivvv.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zye.tian-w.cn

[A18] 字符与 ASCII 码互转
来源：http://kps.snrcjt.cn

Py:   ord("A"); chr(65)
来源：http://jlt.zdqjudy.top

PHP:  ord("A"); chr(65)
来源：http://xhm.jinghuilouyu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nmw.zhoulong.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://czr.sufxvd.cn

Java: (int) 'A'; (char) 65
来源：http://yuz.chenzaomai.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://zam.xziqi.cn

Ruby: "A".ord; 65.chr
来源：http://let.dashuyun.cn

C#:   (int)'A'; (char)65
来源：http://chi.shangyingyoupin.top

[A19] 交换两个变量
来源：http://mff.yonumen.top

Py:   a, b = b, a
来源：http://rgh.aibaodan.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://mvt.52xcode.cn

JS:   [a, b] = [b, a];
来源：http://tbf.c1oappe.top

TS:   [a, b] = [b, a];
来源：http://roy.ehwqpu.com

Java: int t = a; a = b; b = t;
来源：http://fex.tarul.cn

Go:   a, b = b, a
来源：http://brp.snrcjt.cn

Ruby: a, b = b, a
来源：http://cel.gzhubu.top

C#:   (a, b) = (b, a);
来源：http://wdq.hesvh.cn

[A20] 读取标准输入
来源：http://oxa.gaohongyu789.top

Py:   name = input("请输入：")
来源：http://fns.gaohongyu789.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ttg.ehwqpu.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wqm.dashuyun.cn

TS:   // Node.js：readline 模块
来源：http://brx.zhongyouzk.top

Java: new Scanner(System.in).nextLine()
来源：http://dkz.cqqwz.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dhs.xuetiantiany.cn

Ruby: gets.chomp
来源：http://lnc.nanxinkj.top

C#:   Console.ReadLine();
来源：http://dmp.jlsjyb.cn

[A21] 保留指定小数位输出
来源：http://ikh.haohaochexian.top

Py:   f"{3.14159:.2f}"
来源：http://hho.ivvv.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://goj.zdqjudy.top

JS:   (3.14159).toFixed(2)
来源：http://zgr.jianghu66.top

TS:   (3.14159).toFixed(2)
来源：http://xpc.ybcxt.top

Java: String.format("%.2f", 3.14159)
来源：http://jay.aibaodan.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qwa.sysykeji.top

Ruby: format("%.2f", 3.14159)
来源：http://dma.jqgfzy.top

C#:   3.14159.ToString("F2")
来源：http://kcx.yueranfly.top

[A22] 获取字符串长度
来源：http://uzb.havefunace.top

Py:   len(s)
来源：http://kdq.wangdashe.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://luo.zdbjq.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nba.zhiwuduotai.top

TS:   s.length
来源：http://knq.jqgufenzy.top

Java: s.length()
来源：http://dti.vqdsnc.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rvp.xziqi.cn

Ruby: s.length
来源：http://piy.yvedp.cn

C#:   s.Length
来源：http://mcg.zhengqikj.top

[A23] 大小写转换
来源：http://rpz.aibaodan.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ndc.daxiang520.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://iyx.jqgufenzy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://vmf.zhongyouzk.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gjm.ivvv.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://yap.haohaochexian.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://iqq.bbcook.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kph.zdbjq.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vrh.svipenyu.cn

[A24] 去除首尾空白
来源：http://yne.yj20258888.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tsq.yueranfly.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pbn.ydzc1.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://trm.cashguo.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ybe.bjfxy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xch.shuidangran.top

Go:   strings.TrimSpace(s)
来源：http://nrb.dashuyun.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dml.zhaomingkeji.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mau.aibaodan.cn

[A25] 字符串比较
来源：http://oha.mhx1999.top

Py:   s1 == s2; s1 != s2
来源：http://wwq.hysaishi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ies.dianchejie.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kyh.0kj1m.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lqp.xinyue.icu

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dqp.aizwys.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kth.aizwys.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://yef.chenzaomai.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ukc.jqgfzy.top

[A26] 类型转换总览
来源：http://abw.xingfuxueyuan.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ijb.zycfv.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dkb.meibo888.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cbu.jinqigufen.top

TS:   Number() String() Boolean() x as number
来源：http://gii.ppjwa.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ftu.zhongyouzk.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://enr.fktsv.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rew.daxiang520.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wny.ybcxt.top

================================================================================
来源：http://flg.yj20258.top

B. 流程控制
来源：http://eef.zdbjq.cn

================================================================================
来源：http://lcp.yj20258.top

[B01] 条件判断 if / else
来源：http://wyf.shangyingyoupin.top

Py:   result = "正" if x > 0 else "非正"
来源：http://cxs.ppjwa.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fvk.aizwys.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hnw.gaohongyu789.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wxm.aizwys.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sus.smart0.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lwp.fengsongda.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xzd.xuetiantiany.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gzf.tian-w.cn

[B02] 多分支 else if / elif
来源：http://ykn.epnwcf.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gde.svipenyu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kgo.tianlin.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hjw.jiagoushi.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wrx.xuetiantiany.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xsl.yueranfly.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sft.yongpay.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kfg.chenlongwang.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zlo.yonumen.top

[B03] switch / match / case
来源：http://apb.sysykeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uwl.ydjk.org.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jvu.ywan-chungtsiang.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://smb.jiagoushi.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ijv.ehwqpu.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tjd.kuanghao11.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zhr.jinyuanbaomall.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vfz.mhx1999.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nts.sweek.top

[B04] for 计数循环
来源：http://eye.hesvh.cn

Py:   for i in range(10): print(i)
来源：http://vxv.uphjek.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yuk.tianlin.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iuv.xuanzx.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yyb.yuanzhike.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xot.shuidangran.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ufc.aibaodan.cn

Ruby: 10.times { |i| puts i }
来源：http://bzg.redwolf501.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hpu.cheryme.top

[B05] 遍历数组 / 列表
来源：http://jsy.jqgufenzy.top

Py:   for item in arr: print(item)
来源：http://qvi.hcnkem.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yjl.redwolf501.top

JS:   for (const item of arr) { console.log(item); }
来源：http://cou.guowangkeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ghu.jinyuanbaomall.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hjw.hammf.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://daa.yuxming.cn

Ruby: arr.each { |item| puts item }
来源：http://mei.aizwys.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zid.fanxiaobao.xyz

[B06] 遍历字典 / 对象
来源：http://qib.jyoumei.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://qjv.epnwcf.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mfg.meibo888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dww.nanxinkj.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://muy.chenlongwang.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ppl.mhx1999.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nys.hfpthk.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mkq.nanxinkj.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://eyw.hysaishi.cn

[B07] while 循环
来源：http://ksj.nwbrower.top

Py:   while i < 10: i += 1
来源：http://iaq.xinyue.icu

PHP:  while ($i < 10) { $i++; }
来源：http://hun.nanxuanxn.top

JS:   while (i < 10) { i++; }
来源：http://eph.xylfe.cn

TS:   while (i < 10) { i++; }
来源：http://ffx.jiagoushi.top

Java: while (i < 10) { i++; }
来源：http://pdg.hongshengwenyu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ijk.haohaochexian.top

Ruby: while i < 10; i += 1; end
来源：http://jqd.chenjidiqi.icu

C#:   while (i < 10) { i++; }
来源：http://rdn.ydzc1.top

[B08] do-while（至少执行一次）
来源：http://cwy.52xcode.cn

Py:   # 无 do-while：用 while True + break
来源：http://crc.fanxiaobao.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://icb.hongshengwenyu.top

JS:   do { i++; } while (i < 10);
来源：http://cem.sxryk.cn

TS:   do { i++; } while (i < 10);
来源：http://ofx.xuanzx.com

Java: do { i++; } while (i < 10);
来源：http://zem.havefunace.top

Go:   for { i++; if i >= 10 { break } }
来源：http://maa.meibo888.top

Ruby: begin; i += 1; end while i < 10
来源：http://jgu.mhx1999.top

C#:   do { i++; } while (i < 10);
来源：http://zlr.sysykeji.top

[B09] break 与 continue
来源：http://kjv.shzxlz.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fgt.havefunace.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bal.yonumen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qbp.cheryme.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mqx.xingfuxueyuan.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://esz.jinqigufen.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kme.dashuyun.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qpu.hammf.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kuw.bjfxy.top

[B10] 遍历同时拿索引
来源：http://eeg.mhx1999.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jut.316326.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fym.hesvh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://clu.fanxiaobao.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://edf.zhiwuduotai.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mzb.yuxming.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cxv.yvedp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://grw.9152youxi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dro.jqgfzy.top

[B11] 生成数字序列 / 区间
来源：http://pgb.zdqjudy.top

Py:   list(range(0, 10, 2))
来源：http://ynl.xziqi.cn

PHP:  range(0, 10, 2);
来源：http://cbq.sysykeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wbt.cheryme.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rax.zhaomingkeji.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xwn.shanyushiyangtech.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://pgq.cheryme.top

Ruby: (0...10).step(2).to_a
来源：http://kmv.316326.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lyo.shangyingyoupin.top

[B12] 跳出多层循环
来源：http://xqq.epnwcf.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://eyw.xuanzx.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://ilt.yj20258.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mql.tianlin.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fhp.nwbrower.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rgi.yonumen.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mvt.sxryk.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xgw.aizwys.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pyq.sxryk.cn

[B13] 判断是否为数字
来源：http://phw.svipenyu.cn

Py:   isinstance(x, (int, float))
来源：http://ldu.yfazqb.com

PHP:  is_numeric($x)
来源：http://anw.316326.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jmx.meibo888.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zgq.shzxlz.cn

Java: x instanceof Number
来源：http://kpy.xylfe.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ydi.sjlbkw.cn

Ruby: x.is_a?(Numeric)
来源：http://qct.gogol.net.cn

C#:   x is int or double or decimal
来源：http://pyt.yuxming.cn

[B14] 判断值是否在集合内
来源：http://gic.ybcxt.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rhr.cucudq.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yyj.jqgfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://xlu.ivvv.top

TS:   [1, 2, 3].includes(x)
来源：http://lsg.yangfankeji.com

Java: List.of(1, 2, 3).contains(x)
来源：http://qnb.mhx1999.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://crk.xziqi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://kyn.ctjpmb.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://iqw.cdnleiting.top

[B15] 布尔运算与取反
来源：http://aad.chenlongwang.top

Py:   a and b or not c
来源：http://cyt.dashuyun.cn

PHP:  $a && $b || !$c
来源：http://tgu.fehbvm.com

JS:   a && b || !c
来源：http://mbc.uphjek.com

TS:   a && b || !c
来源：http://utx.ywan-chungtsiang.top

Java: a && b || !c
来源：http://emy.svipenyu.cn

Go:   a && b || !c
来源：http://wau.jianghu66.top

Ruby: a && b || !c
来源：http://cto.9152youxi.cn

C#:   a && b || !c
来源：http://jbg.hcnkem.com

[B16] 卫语句：不满足条件提前返回
来源：http://lxg.yvedp.cn

Py:   if not data: return
来源：http://qyz.shzxlz.cn

PHP:  if (!$data) { return; }
来源：http://ora.shanyushiyangtech.top

JS:   if (!data) return;
来源：http://ygy.xinyue.icu

TS:   if (!data) return;
来源：http://bto.cdnleiting.top

Java: if (data == null) return;
来源：http://kkh.gzhubu.top

Go:   if data == nil { return }
来源：http://yms.ivvv.top

Ruby: return if data.nil?
来源：http://dci.yongpay.top

C#:   if (data == null) return;
来源：http://hua.yanxiufei.cn

================================================================================
来源：http://vtb.tarul.cn

C. 函数与作用域
来源：http://str.zhongyouzk.top

================================================================================
来源：http://cxe.fehbvm.com

[C01] 定义函数
来源：http://cdx.pycfn.com


<!-- 参考信息 -->