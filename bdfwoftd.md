代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://vln.zhongyouzk.top

[A11] 条件表达式（三元）
来源：http://gxz.yj20258888.top

Py:   "yes" if x > 0 else "no"
来源：http://oll.yfazqb.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://jev.yongpay.top

JS:   x > 0 ? "yes" : "no"
来源：http://bim.sjlbkw.cn

TS:   x > 0 ? "yes" : "no"
来源：http://cpv.birdmap.top

Java: x > 0 ? "yes" : "no"
来源：http://qvh.dianchejie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ekd.jinghuilouyu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://efa.yanxiufei.cn

C#:   x > 0 ? "yes" : "no"
来源：http://gdw.ydjk.org.cn

[A12] 字符串插值 / 格式化
来源：http://gse.zdbjq.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://uvd.yangfankeji.com

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://gdu.fzhhl.top

JS:   `Hello, ${name}!`
来源：http://agb.zhaomingkeji.xyz

TS:   `Hello, ${name}!`
来源：http://uau.cqqwz.cn

Java: "Hello, %s!".formatted(name)
来源：http://iih.hammf.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://une.chenzaomai.com

Ruby: "Hello, #{name}!"
来源：http://bvk.xziqi.cn

C#:   $"Hello, {name}!"
来源：http://jum.ywan-chungtsiang.top

[A13] 多行字符串（练习 \n 转义）
来源：http://cvy.zhijiandao.cn

Py:   "第一行\n第二行"
来源：http://uvn.haohaochexian.top

PHP:  "第一行\n第二行"
来源：http://hap.chenzaomai.com

JS:   "第一行\n第二行"
来源：http://ick.jqgufenzy.top

TS:   "第一行\n第二行"
来源：http://twa.gaohongyu789.top

Java: "第一行\n第二行"
来源：http://ekk.yongpay.top

Go:   "第一行\n第二行"
来源：http://twq.cheryme.top

Ruby: "第一行\n第二行"
来源：http://lwv.sxryk.cn

C#:   "第一行\n第二行"
来源：http://ipv.sysykeji.top

[A14] 注释写法
来源：http://sgw.chenzaomai.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://tzl.hysaishi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://yis.yj20258.top

JS:   // 单行；/* 多行 */
来源：http://aft.yvedp.cn

TS:   // 单行；/* 多行 */
来源：http://ivf.ppjwa.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bgf.svipenyu.cn

Go:   // 单行；/* 多行 */
来源：http://zax.0kj1m.cn

Ruby: # 单行；=begin 多行 =end
来源：http://mae.c1oappe.top

C#:   // 单行；/* 多行 */
来源：http://ome.nwbrower.top

[A15] 空值判断与默认值
来源：http://jrz.sxryk.cn

Py:   value = data or "默认值"
来源：http://imv.hfpthk.cn

PHP:  $value = $data ?? "默认值";
来源：http://aff.hnxiangtu.top

JS:   const value = data ?? "默认值";
来源：http://jtc.hcnkem.com

TS:   const value = data ?? "默认值";
来源：http://yku.yj202588.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mfi.jianghu66.top

Go:   if data == "" { data = "默认值" }
来源：http://rwd.chenjidiqi.icu

Ruby: value = data || "默认值"
来源：http://dcd.nanxuanxn.top

C#:   var value = data ?? "默认值";
来源：http://dsn.wangshuangyany.cn

[A16] 真假值判断规则
来源：http://bgn.aibaodan.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wyg.sxryk.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ayt.cashguo.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bkx.tanke756.top

TS:   if (!x) {}
来源：http://pxu.haohaochexian.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://obe.hysaishi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://evk.jiagoushi.top

Ruby: unless x            # nil 与 false 为假
来源：http://dhn.316326.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://srs.jiagoushi.top

[A17] 位运算
来源：http://cla.jinqigfzy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kln.meibo888.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mgw.jiagoushi.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kpf.zhiwuduotai.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nrg.zycfv.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jne.ywan-chungtsiang.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tfy.zhongyouzk.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cxt.pengpengdd.cyou

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dva.zhoulong.xyz

[A18] 字符与 ASCII 码互转
来源：http://xpt.yanxiufei.cn

Py:   ord("A"); chr(65)
来源：http://abn.quarkkingdee.top

PHP:  ord("A"); chr(65)
来源：http://swe.xuetiantiany.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ksk.feifeiyinyue.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mtt.pycfn.com

Java: (int) 'A'; (char) 65
来源：http://sfv.yj20258.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hkr.cucudq.cn

Ruby: "A".ord; 65.chr
来源：http://euh.yonumen.top

C#:   (int)'A'; (char)65
来源：http://icm.iojbl.cn

[A19] 交换两个变量
来源：http://xby.aibaodan.cn

Py:   a, b = b, a
来源：http://kfz.jinyuanbaomall.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://uwz.hongshengwenyu.top

JS:   [a, b] = [b, a];
来源：http://uht.yanxiufei.cn

TS:   [a, b] = [b, a];
来源：http://ibn.hongshengwenyu.top

Java: int t = a; a = b; b = t;
来源：http://mnw.jinghuilouyu.cn

Go:   a, b = b, a
来源：http://mkb.pengpengdd.cyou

Ruby: a, b = b, a
来源：http://jqo.haohaochexian.top

C#:   (a, b) = (b, a);
来源：http://xaz.yuanzhike.top

[A20] 读取标准输入
来源：http://wlb.nanxinkj.top

Py:   name = input("请输入：")
来源：http://xqa.hongshengwenyu.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ojv.jianghu66.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dem.yj202588.top

TS:   // Node.js：readline 模块
来源：http://smq.aibaodan.cn

Java: new Scanner(System.in).nextLine()
来源：http://ydc.shuidangran.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vob.jianghu66.top

Ruby: gets.chomp
来源：http://zuw.hywenlv.cn

C#:   Console.ReadLine();
来源：http://qcx.bjfxy.top

[A21] 保留指定小数位输出
来源：http://mow.xuetiantiany.cn

Py:   f"{3.14159:.2f}"
来源：http://pgd.birdmap.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://etr.haohaochexian.top

JS:   (3.14159).toFixed(2)
来源：http://akx.tianlin.xyz

TS:   (3.14159).toFixed(2)
来源：http://klj.shzxlz.cn

Java: String.format("%.2f", 3.14159)
来源：http://rhz.fehbvm.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jho.jyoumei.cn

Ruby: format("%.2f", 3.14159)
来源：http://bok.hammf.cn

C#:   3.14159.ToString("F2")
来源：http://vfe.zdqjudy.top

[A22] 获取字符串长度
来源：http://hnr.gogol.net.cn

Py:   len(s)
来源：http://sbg.fengsongda.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://eir.cashguo.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://onw.bbcook.cn

TS:   s.length
来源：http://gny.ivvv.top

Java: s.length()
来源：http://fao.0kj1m.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gtd.yangfankeji.com

Ruby: s.length
来源：http://icg.dashuyun.cn

C#:   s.Length
来源：http://jqs.yvedp.cn

[A23] 大小写转换
来源：http://ono.fanxiaobao.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://qzu.fzhhl.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fuv.zycfv.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nvc.316326.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fhw.dianchejie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pgx.fktsv.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wps.fanxiaobao.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://rag.gotoacloud.top

C#:   s.ToUpper(); s.ToLower()
来源：http://jix.pycfn.com

[A24] 去除首尾空白
来源：http://bjh.pycfn.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jag.epnwcf.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pfd.gotoacloud.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://njx.jqgufenzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dsb.cheryme.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tyq.zhoulong.xyz

Go:   strings.TrimSpace(s)
来源：http://gre.quarkkingdee.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vgl.zhiwuduotai.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tnk.xingfuxueyuan.xyz

[A25] 字符串比较
来源：http://koi.redwolf501.top

Py:   s1 == s2; s1 != s2
来源：http://rcd.sweek.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://eam.yongpay.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://efb.ivvv.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mgz.yueranfly.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jau.vqdsnc.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vyz.yonumen.top

Ruby: s1 == s2; s1 <=> s2
来源：http://exn.wangshuangyany.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ywh.meibo888.top

[A26] 类型转换总览
来源：http://aek.gogol.net.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qks.chenjidiqi.icu

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://plm.9152youxi.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xwa.fzhhl.top

TS:   Number() String() Boolean() x as number
来源：http://zdk.shangyingyoupin.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qfb.jqgufenzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://whr.yj20258888.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://rdy.redwolf501.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://esn.sufxvd.cn

================================================================================
来源：http://ghl.zhijiandao.cn

B. 流程控制
来源：http://msj.pengpengdd.cyou

================================================================================
来源：http://mre.yfazqb.com

[B01] 条件判断 if / else
来源：http://byi.bbcook.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://tgl.bbcook.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cbn.jinghuilouyu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yki.0kj1m.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mlz.hongshengwenyu.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://lbt.gaohongyu789.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yjg.9152youxi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pop.birdmap.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yur.yj20258888.top

[B02] 多分支 else if / elif
来源：http://ngw.mhx1999.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vbq.cashguo.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://umm.tarul.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iby.hongshengwenyu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ems.yj20258.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dqt.tian-w.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iti.yangfankeji.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ebj.fzhhl.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ocr.uphjek.com

[B03] switch / match / case
来源：http://oxf.cdnleiting.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ibk.nanxuanxn.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hny.zhengqikj.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wey.wangshuangyany.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qvu.chenlongwang.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ita.smart0.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pvb.fehbvm.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dwy.yonumen.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tec.chenjidiqi.icu

[B04] for 计数循环
来源：http://chw.yangfankeji.com

Py:   for i in range(10): print(i)
来源：http://wyd.c1oappe.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://utu.nanxinkj.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hwg.wangshuangyany.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rwh.gaohongyu789.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ztx.sweek.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vrm.9152youxi.cn

Ruby: 10.times { |i| puts i }
来源：http://jux.sjlbkw.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mis.pengpengdd.cyou

[B05] 遍历数组 / 列表
来源：http://yeo.ydjk.org.cn

Py:   for item in arr: print(item)
来源：http://dad.yj20258888.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hzt.uphjek.com

JS:   for (const item of arr) { console.log(item); }
来源：http://eip.nwbrower.top

TS:   for (const item of arr) { console.log(item); }
来源：http://udp.zhongyouzk.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://jla.vqdsnc.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wzb.andypj.xyz

Ruby: arr.each { |item| puts item }
来源：http://jmb.yfazqb.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rjt.shanyushiyangtech.top

[B06] 遍历字典 / 对象
来源：http://mvs.fktsv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://rom.jinqigfzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qbc.aizwys.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jnu.jlsjyb.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tru.haohaochexian.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oqq.dashuyun.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rqg.yueranfly.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sfm.gzhubu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wfn.tarul.cn

[B07] while 循环
来源：http://gaw.nwbrower.top

Py:   while i < 10: i += 1
来源：http://vna.yongpay.top

PHP:  while ($i < 10) { $i++; }
来源：http://oyl.sjlbkw.cn

JS:   while (i < 10) { i++; }
来源：http://tdm.sxryk.cn

TS:   while (i < 10) { i++; }
来源：http://nns.zhaomingkeji.xyz

Java: while (i < 10) { i++; }
来源：http://qnv.iojbl.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bpz.zdbjq.cn

Ruby: while i < 10; i += 1; end
来源：http://qbe.jinyuanbaomall.cn

C#:   while (i < 10) { i++; }
来源：http://dff.tianlin.xyz

[B08] do-while（至少执行一次）
来源：http://lsx.fzhhl.top

Py:   # 无 do-while：用 while True + break
来源：http://aqg.daria6918.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ehf.zycfv.cn

JS:   do { i++; } while (i < 10);
来源：http://kfq.c1oappe.top

TS:   do { i++; } while (i < 10);
来源：http://fmk.ctjpmb.com

Java: do { i++; } while (i < 10);
来源：http://znq.ehwqpu.com

Go:   for { i++; if i >= 10 { break } }
来源：http://jaq.bjfxy.top

Ruby: begin; i += 1; end while i < 10
来源：http://yml.yueranfly.top

C#:   do { i++; } while (i < 10);
来源：http://ggu.hesvh.cn

[B09] break 与 continue
来源：http://mpc.c1oappe.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nud.vqdsnc.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://syd.zhiwuduotai.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jqu.shangyingyoupin.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qei.wangshuangyany.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://owe.zhixingplan.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mcl.hfpthk.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ksw.snrcjt.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bst.guannengcc.top

[B10] 遍历同时拿索引
来源：http://eac.guannengcc.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pmi.yongpay.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qlb.jlsjyb.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rin.52xcode.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rmr.chenjidiqi.icu

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://esn.jiagoushi.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://swl.yanxiufei.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tpd.havefunace.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hmu.zycfv.cn

[B11] 生成数字序列 / 区间
来源：http://ycc.xingfuxueyuan.xyz

Py:   list(range(0, 10, 2))
来源：http://bup.nanxinkj.top

PHP:  range(0, 10, 2);
来源：http://ebb.xuanzx.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iji.chenjidiqi.icu

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ksz.gogol.net.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qug.chenlongwang.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://boi.cqqwz.cn

Ruby: (0...10).step(2).to_a
来源：http://ftg.cqqwz.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rky.wangshuangyany.cn

[B12] 跳出多层循环
来源：http://jwq.daxiang520.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://amz.zhengqikj.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ykv.snrcjt.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wkk.xziqi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qap.fengsongda.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dkg.cashguo.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://avj.ctjpmb.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dma.jinqigufen.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pij.ybcxt.top

[B13] 判断是否为数字
来源：http://cvz.feifeiyinyue.top

Py:   isinstance(x, (int, float))
来源：http://bwf.svipenyu.cn

PHP:  is_numeric($x)
来源：http://peb.yueranfly.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rde.snrcjt.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fbr.redwolf501.top

Java: x instanceof Number
来源：http://lka.zhijiandao.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vbd.daria6918.cn

Ruby: x.is_a?(Numeric)
来源：http://qlt.zhijiandao.cn

C#:   x is int or double or decimal
来源：http://ifm.yanxiufei.cn

[B14] 判断值是否在集合内
来源：http://rkz.cucudq.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qtv.tanke756.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rbb.snrcjt.cn

JS:   [1, 2, 3].includes(x)
来源：http://mid.jinqigfzy.top

TS:   [1, 2, 3].includes(x)
来源：http://ohx.xuanzx.com

Java: List.of(1, 2, 3).contains(x)
来源：http://ylx.yueranfly.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jni.ydjk.org.cn

Ruby: [1, 2, 3].include?(x)
来源：http://frc.gogol.net.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jab.jinqigfzy.top

[B15] 布尔运算与取反
来源：http://tiy.xuanzx.com

Py:   a and b or not c
来源：http://tbk.meibo888.top

PHP:  $a && $b || !$c
来源：http://coe.xuetiantiany.cn

JS:   a && b || !c
来源：http://imw.hcnkem.com

TS:   a && b || !c
来源：http://von.zdbjq.cn

Java: a && b || !c
来源：http://mxb.dianchejie.cn

Go:   a && b || !c
来源：http://zxp.cqqwz.cn

Ruby: a && b || !c
来源：http://lmx.hfpthk.cn

C#:   a && b || !c
来源：http://wsm.havefunace.top

[B16] 卫语句：不满足条件提前返回
来源：http://ghp.hnxiangtu.top

Py:   if not data: return
来源：http://vwu.kuanghao11.cn

PHP:  if (!$data) { return; }
来源：http://bqn.jinqigfzy.top

JS:   if (!data) return;
来源：http://pht.xylfe.cn

TS:   if (!data) return;
来源：http://pkh.ybcxt.top

Java: if (data == null) return;
来源：http://ttd.chenlongwang.top

Go:   if data == nil { return }
来源：http://nir.nanxuanxn.top

Ruby: return if data.nil?
来源：http://kfq.meibo888.top

C#:   if (data == null) return;
来源：http://fhz.jinqigufen.top

================================================================================
来源：http://taw.redwolf501.top

C. 函数与作用域
来源：http://ajc.zhixingplan.top

================================================================================
来源：http://evq.aizwys.cn

[C01] 定义函数
来源：http://fgu.cucudq.cn

Py:   def add(a, b): return a + b
来源：http://vjo.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mnp.mhx1999.top

JS:   function add(a, b) { return a + b; }
来源：http://cxy.zhongyouzk.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qrl.zhijiandao.cn


<!-- 参考信息 -->