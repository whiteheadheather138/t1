代发 wailian999

Py:   "第一行\n第二行"
来源：http://tql.jinghuilouyu.cn

PHP:  "第一行\n第二行"
来源：http://aqq.hcnkem.com

JS:   "第一行\n第二行"
来源：http://gzn.hnxiangtu.top

TS:   "第一行\n第二行"
来源：http://kld.yueranfly.top

Java: "第一行\n第二行"
来源：http://hsc.xuanzx.com

Go:   "第一行\n第二行"
来源：http://ute.sysykeji.top

Ruby: "第一行\n第二行"
来源：http://pqu.shzxlz.cn

C#:   "第一行\n第二行"
来源：http://dfc.jlsjyb.cn

[A14] 注释写法
来源：http://znz.xingfuxueyuan.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://mgp.hywenlv.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://icc.jinyuanbaomall.cn

JS:   // 单行；/* 多行 */
来源：http://uwj.xuetiantiany.cn

TS:   // 单行；/* 多行 */
来源：http://npn.tian-w.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mah.zdqjudy.top

Go:   // 单行；/* 多行 */
来源：http://zrc.snrcjt.cn

Ruby: # 单行；=begin 多行 =end
来源：http://sgf.xylfe.cn

C#:   // 单行；/* 多行 */
来源：http://eld.shanyushiyangkeji.top

[A15] 空值判断与默认值
来源：http://hce.chenlongwang.top

Py:   value = data or "默认值"
来源：http://huj.aizwys.cn

PHP:  $value = $data ?? "默认值";
来源：http://zzq.yongpay.top

JS:   const value = data ?? "默认值";
来源：http://pzd.zhixingplan.top

TS:   const value = data ?? "默认值";
来源：http://lpu.pycfn.com

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hnm.zdbjq.cn

Go:   if data == "" { data = "默认值" }
来源：http://qxi.fehbvm.com

Ruby: value = data || "默认值"
来源：http://ybe.sxryk.cn

C#:   var value = data ?? "默认值";
来源：http://cqt.ydzc1.top

[A16] 真假值判断规则
来源：http://cdi.shzxlz.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nbu.dashuyun.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zml.xuetiantiany.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xpa.yanxiufei.cn

TS:   if (!x) {}
来源：http://enq.tanke756.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zwo.pengpengdd.cyou

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://shf.gzhubu.top

Ruby: unless x            # nil 与 false 为假
来源：http://pwe.aibaodan.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nek.gogol.net.cn

[A17] 位运算
来源：http://hen.ydjk.org.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lam.gaohongyu789.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://slf.fengsongda.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jbi.xuetiantiany.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rvz.hesvh.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vqv.xuetiantiany.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bsf.tanke756.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qmf.jinqigfzy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://thu.shangyingyoupin.top

[A18] 字符与 ASCII 码互转
来源：http://mba.bjfxy.top

Py:   ord("A"); chr(65)
来源：http://ncn.bjfxy.top

PHP:  ord("A"); chr(65)
来源：http://zor.yueranfly.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://awv.316326.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ubi.fzhhl.top

Java: (int) 'A'; (char) 65
来源：http://dhu.tarul.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kij.zdbjq.cn

Ruby: "A".ord; 65.chr
来源：http://fjp.hesvh.cn

C#:   (int)'A'; (char)65
来源：http://uor.zycfv.cn

[A19] 交换两个变量
来源：http://uih.gaohongyu789.top

Py:   a, b = b, a
来源：http://kww.ywan-chungtsiang.top

PHP:  [$a, $b] = [$b, $a];
来源：http://iis.zhixingplan.top

JS:   [a, b] = [b, a];
来源：http://fmv.andypj.xyz

TS:   [a, b] = [b, a];
来源：http://zay.shuidangran.top

Java: int t = a; a = b; b = t;
来源：http://xae.fehbvm.com

Go:   a, b = b, a
来源：http://lst.vehdjk.com

Ruby: a, b = b, a
来源：http://ooo.tarul.cn

C#:   (a, b) = (b, a);
来源：http://vwa.316326.xyz

[A20] 读取标准输入
来源：http://iqi.yanxiufei.cn

Py:   name = input("请输入：")
来源：http://fcm.cashguo.top

PHP:  $name = trim(fgets(STDIN));
来源：http://rvg.birdmap.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://odt.havefunace.top

TS:   // Node.js：readline 模块
来源：http://vpg.ppjwa.cn

Java: new Scanner(System.in).nextLine()
来源：http://sqi.sufxvd.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://dxm.tianlin.xyz

Ruby: gets.chomp
来源：http://cja.hesvh.cn

C#:   Console.ReadLine();
来源：http://ytx.xingfuxueyuan.xyz

[A21] 保留指定小数位输出
来源：http://vrh.wangshuangyany.cn

Py:   f"{3.14159:.2f}"
来源：http://kyx.chenjidiqi.icu

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gil.0kj1m.cn

JS:   (3.14159).toFixed(2)
来源：http://wzk.sweek.top

TS:   (3.14159).toFixed(2)
来源：http://hdl.bjfxy.top

Java: String.format("%.2f", 3.14159)
来源：http://jba.shangyingyoupin.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pkc.fzhhl.top

Ruby: format("%.2f", 3.14159)
来源：http://vak.vehdjk.com

C#:   3.14159.ToString("F2")
来源：http://oij.cheryme.top

[A22] 获取字符串长度
来源：http://fgk.zhijiandao.cn

Py:   len(s)
来源：http://jpn.dashuyun.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://oio.yj202588.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pnu.guannengcc.top

TS:   s.length
来源：http://iuv.daria6918.cn

Java: s.length()
来源：http://ose.zhaomingkeji.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ciy.zhaomingkeji.xyz

Ruby: s.length
来源：http://zrz.dianchejie.cn

C#:   s.Length
来源：http://wvl.ehwqpu.com

[A23] 大小写转换
来源：http://sii.shanyushiyangtech.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ulx.hfpthk.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pkt.jinqigufen.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mwk.ehwqpu.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ivr.zhengqikj.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jlq.svipenyu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pjw.feifeiyinyue.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kwq.yvedp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ydj.jinyuanbaomall.cn

[A24] 去除首尾空白
来源：http://lzb.yuxming.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rgn.ybcxt.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zhh.xylfe.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dhb.sysykeji.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hnq.cqqwz.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ihy.tian-w.cn

Go:   strings.TrimSpace(s)
来源：http://xkr.aibaodan.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://iel.jinqigfzy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fsi.xziqi.cn

[A25] 字符串比较
来源：http://igy.xylfe.cn

Py:   s1 == s2; s1 != s2
来源：http://nck.jlsjyb.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cma.smart0.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://msd.birdmap.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://saq.chenlongwang.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://byx.mhx1999.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sjk.zycfv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cez.shzxlz.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fdt.c1oappe.top

[A26] 类型转换总览
来源：http://egl.xylfe.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bza.andypj.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://woo.jinqigufen.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://joy.0kj1m.cn

TS:   Number() String() Boolean() x as number
来源：http://fhp.haohaochexian.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ebf.aizwys.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bjb.gotoacloud.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://rna.chenlongwang.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kfo.sysykeji.top

================================================================================
来源：http://qrw.jinqigfzy.top

B. 流程控制
来源：http://qwd.gzhubu.top

================================================================================
来源：http://asn.jqgfzy.top

[B01] 条件判断 if / else
来源：http://ozd.ehwqpu.com

Py:   result = "正" if x > 0 else "非正"
来源：http://ltk.jlsjyb.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rdt.zdqjudy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xbw.havefunace.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ulq.haohaochexian.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://wbi.hywenlv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://eko.daxiang520.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uic.redwolf501.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://huh.hfpthk.cn

[B02] 多分支 else if / elif
来源：http://zqn.yanxiufei.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tqf.0kj1m.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mwn.sxryk.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rvg.snrcjt.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bkk.ehwqpu.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ccg.nwbrower.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dxm.uphjek.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://itt.xingfuxueyuan.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ycu.aibaodan.cn

[B03] switch / match / case
来源：http://plp.hfpthk.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wfs.nanxuanxn.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wpw.zhiwuduotai.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://czm.birdmap.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fxo.uphjek.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dgr.xuanzx.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rgz.ivvv.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sln.daxiang520.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jfi.ydjk.org.cn

[B04] for 计数循环
来源：http://xcg.uphjek.com

Py:   for i in range(10): print(i)
来源：http://mgm.hnqzz.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://njg.yongpay.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bgr.guannengcc.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ayb.yanxiufei.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xzn.cucudq.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jhd.cashguo.top

Ruby: 10.times { |i| puts i }
来源：http://mgd.c1oappe.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gfw.tarul.cn

[B05] 遍历数组 / 列表
来源：http://ybm.zhixingplan.top

Py:   for item in arr: print(item)
来源：http://hnw.gotoacloud.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xbf.ybcxt.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ovt.dashuyun.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sln.ywan-chungtsiang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qqx.uphjek.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kvm.9152youxi.cn

Ruby: arr.each { |item| puts item }
来源：http://cwp.tianlin.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kmy.yonumen.top

[B06] 遍历字典 / 对象
来源：http://jje.yvedp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://oax.epnwcf.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ppt.xuetiantiany.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dqr.xuanzx.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uqy.daxiang520.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mbv.pengpengdd.cyou

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://smj.zhijiandao.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jah.dashuyun.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cwy.jinqigufen.top

[B07] while 循环
来源：http://ipz.zhengqikj.top

Py:   while i < 10: i += 1
来源：http://gxp.jqgufenzy.top

PHP:  while ($i < 10) { $i++; }
来源：http://idh.zhixingplan.top

JS:   while (i < 10) { i++; }
来源：http://rtk.svipenyu.cn

TS:   while (i < 10) { i++; }
来源：http://qkn.hysaishi.cn

Java: while (i < 10) { i++; }
来源：http://ded.xuetiantiany.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ces.jinyuanbaomall.cn

Ruby: while i < 10; i += 1; end
来源：http://gcp.jqgufenzy.top

C#:   while (i < 10) { i++; }
来源：http://mab.fktsv.cn

[B08] do-while（至少执行一次）
来源：http://tks.cashguo.top

Py:   # 无 do-while：用 while True + break
来源：http://chg.yongpay.top

PHP:  do { $i++; } while ($i < 10);
来源：http://sfu.316326.xyz

JS:   do { i++; } while (i < 10);
来源：http://wqr.hysaishi.cn

TS:   do { i++; } while (i < 10);
来源：http://jdg.jianghu66.top

Java: do { i++; } while (i < 10);
来源：http://hhu.zdqjudy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://thi.sweek.top

Ruby: begin; i += 1; end while i < 10
来源：http://ukd.shzxlz.cn

C#:   do { i++; } while (i < 10);
来源：http://dlg.nanxinkj.top

[B09] break 与 continue
来源：http://gui.gaohongyu789.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://avv.jlsjyb.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nii.gzhubu.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rxw.ppjwa.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pdn.zhaomingkeji.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mxz.haohaochexian.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bhv.xziqi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cvw.daria6918.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uff.yanxiufei.cn

[B10] 遍历同时拿索引
来源：http://dgm.daria6918.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tlz.hammf.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mxj.haohaochexian.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xpm.guowangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cwc.quarkkingdee.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ccx.gzhubu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bkm.zhiwuduotai.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://oxc.pycfn.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qqy.zhijiandao.cn

[B11] 生成数字序列 / 区间
来源：http://kvm.yangfankeji.com

Py:   list(range(0, 10, 2))
来源：http://guh.yj202588.top

PHP:  range(0, 10, 2);
来源：http://kwh.iojbl.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nln.yueranfly.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xci.birdmap.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vbg.hysaishi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gnq.fzhhl.top

Ruby: (0...10).step(2).to_a
来源：http://zwf.mhx1999.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mip.zdbjq.cn

[B12] 跳出多层循环
来源：http://olh.cucudq.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gmr.xuanzx.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://qel.pycfn.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lqv.cheryme.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zly.sweek.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ddy.dashuyun.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xsm.nanxinkj.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bsl.xinyue.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xcm.jianghu66.top

[B13] 判断是否为数字
来源：http://ryg.tanke756.top

Py:   isinstance(x, (int, float))
来源：http://gme.zdqjudy.top

PHP:  is_numeric($x)
来源：http://xek.316326.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qbt.cqqwz.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lbc.0kj1m.cn

Java: x instanceof Number
来源：http://vid.yvedp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zks.yfazqb.com

Ruby: x.is_a?(Numeric)
来源：http://vbd.tianlin.xyz

C#:   x is int or double or decimal
来源：http://dqn.bbcook.cn

[B14] 判断值是否在集合内
来源：http://mnz.hnqzz.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rdb.bjfxy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ioy.hnxiangtu.top

JS:   [1, 2, 3].includes(x)
来源：http://lqr.yueranfly.top

TS:   [1, 2, 3].includes(x)
来源：http://kya.yueranfly.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fea.yuxming.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wmt.jqgufenzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://mba.yfazqb.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ksk.yangfankeji.com

[B15] 布尔运算与取反
来源：http://qof.redwolf501.top

Py:   a and b or not c
来源：http://bxs.yj20258.top

PHP:  $a && $b || !$c
来源：http://uzv.tarul.cn

JS:   a && b || !c
来源：http://dqq.havefunace.top

TS:   a && b || !c
来源：http://ofj.yonumen.top

Java: a && b || !c
来源：http://iek.0kj1m.cn

Go:   a && b || !c
来源：http://blm.snrcjt.cn

Ruby: a && b || !c
来源：http://yns.svipenyu.cn

C#:   a && b || !c
来源：http://fnj.mhx1999.top

[B16] 卫语句：不满足条件提前返回
来源：http://upm.hnqzz.top

Py:   if not data: return
来源：http://bvz.yuxming.cn

PHP:  if (!$data) { return; }
来源：http://vjx.gaohongyu789.top

JS:   if (!data) return;
来源：http://kjv.zhongyouzk.top

TS:   if (!data) return;
来源：http://qvb.xuetiantiany.cn

Java: if (data == null) return;
来源：http://opn.pycfn.com

Go:   if data == nil { return }
来源：http://fvj.ivvv.top

Ruby: return if data.nil?
来源：http://xet.wangdashe.top

C#:   if (data == null) return;
来源：http://zuy.dashuyun.cn

================================================================================
来源：http://axc.epnwcf.com

C. 函数与作用域
来源：http://ijr.mhx1999.top

================================================================================
来源：http://cyh.feifeiyinyue.top

[C01] 定义函数
来源：http://tgk.nanxinkj.top

Py:   def add(a, b): return a + b
来源：http://wgk.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yzy.c1oappe.top

JS:   function add(a, b) { return a + b; }
来源：http://zzc.ybcxt.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zxq.mhx1999.top

Java: static int add(int a, int b) { return a + b; }
来源：http://hlt.daria6918.cn

Go:   func add(a, b int) int { return a + b }
来源：http://iro.haohaochexian.top

Ruby: def add(a, b); a + b; end
来源：http://wbw.smart0.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wev.fktsv.cn

[C02] 默认参数
来源：http://hbm.nanxinkj.top

Py:   def greet(name="World"): return name
来源：http://mfh.hfpthk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jdx.chenjidiqi.icu

JS:   function greet(name = "World") { return name; }
来源：http://zta.yonumen.top

TS:   function greet(name: string = "World") { return name; }
来源：http://non.tarul.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://eeq.cqqwz.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vjz.yueranfly.top

Ruby: def greet(name = "World") = name
来源：http://xbr.jinghuilouyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://bui.cheryme.top

[C03] 可变参数
来源：http://sfy.zhengqikj.top

Py:   def total(*args): return sum(args)
来源：http://rmv.shangyingyoupin.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qrt.vqdsnc.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qcy.jqgufenzy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fbo.guannengcc.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gym.sxryk.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://epy.birdmap.top


<!-- 参考信息 -->