代发 wailian999

Py:   "第一行\n第二行"
来源：http://qqz.nwbrower.top

PHP:  "第一行\n第二行"
来源：http://nqh.nwbrower.top

JS:   "第一行\n第二行"
来源：http://wkb.gaohongyu789.top

TS:   "第一行\n第二行"
来源：http://lab.jlsjyb.cn

Java: "第一行\n第二行"
来源：http://cqv.ydjk.org.cn

Go:   "第一行\n第二行"
来源：http://mcw.zhaomingkeji.xyz

Ruby: "第一行\n第二行"
来源：http://eez.jinghuilouyu.cn

C#:   "第一行\n第二行"
来源：http://mxo.ivvv.top

[A14] 注释写法
来源：http://upl.guannengcc.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://vfj.xuetiantiany.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://uux.wangdashe.top

JS:   // 单行；/* 多行 */
来源：http://htf.havefunace.top

TS:   // 单行；/* 多行 */
来源：http://ceo.hammf.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://igd.pengpengdd.cyou

Go:   // 单行；/* 多行 */
来源：http://gvb.sufxvd.cn

Ruby: # 单行；=begin 多行 =end
来源：http://tkx.jiagoushi.top

C#:   // 单行；/* 多行 */
来源：http://ssx.redwolf501.top

[A15] 空值判断与默认值
来源：http://xhf.ctjpmb.com

Py:   value = data or "默认值"
来源：http://tmw.cucudq.cn

PHP:  $value = $data ?? "默认值";
来源：http://fny.feifeiyinyue.top

JS:   const value = data ?? "默认值";
来源：http://jyq.jyoumei.cn

TS:   const value = data ?? "默认值";
来源：http://pnb.cheryme.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://uci.cqqwz.cn

Go:   if data == "" { data = "默认值" }
来源：http://ctv.snrcjt.cn

Ruby: value = data || "默认值"
来源：http://srk.wangdashe.top

C#:   var value = data ?? "默认值";
来源：http://ntl.sweek.top

[A16] 真假值判断规则
来源：http://wpv.yanxiufei.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qsj.cdnleiting.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fjj.yuanzhike.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lfp.9152youxi.cn

TS:   if (!x) {}
来源：http://nam.cashguo.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nck.hysaishi.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://poa.dianchejie.cn

Ruby: unless x            # nil 与 false 为假
来源：http://yfg.xingfuxueyuan.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kxf.jianghu66.top

[A17] 位运算
来源：http://ptp.daria6918.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://prq.ydzc1.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://gyo.haohaochexian.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zry.svipenyu.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://oab.cucudq.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xwq.yfazqb.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dmf.shzxlz.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mco.yuxming.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fhi.jiagoushi.top

[A18] 字符与 ASCII 码互转
来源：http://dly.xylfe.cn

Py:   ord("A"); chr(65)
来源：http://fxv.vqdsnc.cn

PHP:  ord("A"); chr(65)
来源：http://rsn.daxiang520.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ahl.ppjwa.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://oqm.jlsjyb.cn

Java: (int) 'A'; (char) 65
来源：http://sjb.yfazqb.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://isq.redwolf501.top

Ruby: "A".ord; 65.chr
来源：http://kqq.gzhubu.top

C#:   (int)'A'; (char)65
来源：http://gjg.hammf.cn

[A19] 交换两个变量
来源：http://xel.jinqigfzy.top

Py:   a, b = b, a
来源：http://vhm.sjlbkw.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hvh.316326.xyz

JS:   [a, b] = [b, a];
来源：http://sas.xuetiantiany.cn

TS:   [a, b] = [b, a];
来源：http://fmo.cashguo.top

Java: int t = a; a = b; b = t;
来源：http://rbo.jqgufenzy.top

Go:   a, b = b, a
来源：http://uvd.9152youxi.cn

Ruby: a, b = b, a
来源：http://uwo.316326.xyz

C#:   (a, b) = (b, a);
来源：http://zul.zhongyouzk.top

[A20] 读取标准输入
来源：http://swe.bbcook.cn

Py:   name = input("请输入：")
来源：http://myw.daria6918.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://dnu.pycfn.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rke.hammf.cn

TS:   // Node.js：readline 模块
来源：http://eks.52xcode.cn

Java: new Scanner(System.in).nextLine()
来源：http://mny.gotoacloud.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ajt.fzhhl.top

Ruby: gets.chomp
来源：http://him.gotoacloud.top

C#:   Console.ReadLine();
来源：http://ksh.sxryk.cn

[A21] 保留指定小数位输出
来源：http://kqm.hammf.cn

Py:   f"{3.14159:.2f}"
来源：http://ruv.shuidangran.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://reo.316326.xyz

JS:   (3.14159).toFixed(2)
来源：http://tcc.xuetiantiany.cn

TS:   (3.14159).toFixed(2)
来源：http://sri.cheryme.top

Java: String.format("%.2f", 3.14159)
来源：http://gbs.yvedp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://chz.shuidangran.top

Ruby: format("%.2f", 3.14159)
来源：http://aik.fengsongda.top

C#:   3.14159.ToString("F2")
来源：http://wuj.xuetiantiany.cn

[A22] 获取字符串长度
来源：http://zrd.yonumen.top

Py:   len(s)
来源：http://ivn.sufxvd.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dxw.kuanghao11.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nmx.jqgufenzy.top

TS:   s.length
来源：http://yyx.yj202588.top

Java: s.length()
来源：http://tuq.fanxiaobao.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ecs.wangshuangyany.cn

Ruby: s.length
来源：http://tzj.daxiang520.top

C#:   s.Length
来源：http://thv.yuxming.cn

[A23] 大小写转换
来源：http://kes.fengsongda.top

Py:   s.upper(); s.lower(); s.title()
来源：http://yeu.ehwqpu.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rcb.chenjidiqi.icu

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qsc.daxiang520.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qqz.ydjk.org.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pyw.shuidangran.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wst.tanke756.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hmc.wangdashe.top

C#:   s.ToUpper(); s.ToLower()
来源：http://xhl.hcnkem.com

[A24] 去除首尾空白
来源：http://uqz.gaohongyu789.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://aph.hnqzz.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lpd.tanke756.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jjb.yuanzhike.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yof.jlsjyb.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://flc.wangshuangyany.cn

Go:   strings.TrimSpace(s)
来源：http://snn.bjfxy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xiy.bjfxy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://brt.aizwys.cn

[A25] 字符串比较
来源：http://jsu.xylfe.cn

Py:   s1 == s2; s1 != s2
来源：http://wtt.yangfankeji.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://loo.ybcxt.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ete.hnqzz.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://idt.fehbvm.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mha.tanke756.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ifm.xylfe.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vrx.zhixingplan.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://drs.zhixingplan.top

[A26] 类型转换总览
来源：http://knt.hysaishi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nqg.tian-w.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rgj.vehdjk.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bed.c1oappe.top

TS:   Number() String() Boolean() x as number
来源：http://rhf.yangfankeji.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jmv.gaohongyu789.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://uco.shanyushiyangtech.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://wng.gaohongyu789.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lkw.zdqjudy.top

================================================================================
来源：http://feb.cheryme.top

B. 流程控制
来源：http://nwl.yanxiufei.cn

================================================================================
来源：http://ali.ivvv.top

[B01] 条件判断 if / else
来源：http://uty.yangfankeji.com

Py:   result = "正" if x > 0 else "非正"
来源：http://jow.vqdsnc.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ivz.dashuyun.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://udl.snrcjt.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://opd.zdbjq.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://kwk.fanxiaobao.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wib.hnqzz.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cpx.gotoacloud.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cap.andypj.xyz

[B02] 多分支 else if / elif
来源：http://cvj.pengpengdd.cyou

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qwr.cucudq.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ojj.yvedp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fpa.uphjek.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sib.jianghu66.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vhu.sufxvd.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ffo.aibaodan.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://urc.quarkkingdee.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tvf.zycfv.cn

[B03] switch / match / case
来源：http://kic.yueranfly.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qfa.ydzc1.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kxi.zdbjq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qle.zhaomingkeji.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://spy.redwolf501.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xbc.chenzaomai.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ftz.gzhubu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bdg.jinqigfzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hrs.hfpthk.cn

[B04] for 计数循环
来源：http://wvj.wangshuangyany.cn

Py:   for i in range(10): print(i)
来源：http://vjj.dashuyun.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dbu.yangfankeji.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ivq.shzxlz.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://akl.jinghuilouyu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dyc.316326.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jmv.chenjidiqi.icu

Ruby: 10.times { |i| puts i }
来源：http://him.ybcxt.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ery.jyoumei.cn

[B05] 遍历数组 / 列表
来源：http://wfm.fengsongda.top

Py:   for item in arr: print(item)
来源：http://atf.jinqigufen.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sun.hcnkem.com

JS:   for (const item of arr) { console.log(item); }
来源：http://lze.quarkkingdee.top

TS:   for (const item of arr) { console.log(item); }
来源：http://djq.birdmap.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://wtx.havefunace.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sep.xuanzx.com

Ruby: arr.each { |item| puts item }
来源：http://uqt.vehdjk.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kgo.zhoulong.xyz

[B06] 遍历字典 / 对象
来源：http://yvv.uphjek.com

Py:   for k, v in d.items(): print(k, v)
来源：http://wtn.smart0.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hjz.xingfuxueyuan.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ybg.c1oappe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uau.snrcjt.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ego.jinyuanbaomall.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://azi.hnqzz.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://agf.shangyingyoupin.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mud.vehdjk.com

[B07] while 循环
来源：http://xaa.tanke756.top

Py:   while i < 10: i += 1
来源：http://dkr.ivvv.top

PHP:  while ($i < 10) { $i++; }
来源：http://zwh.epnwcf.com

JS:   while (i < 10) { i++; }
来源：http://qlb.yangfankeji.com

TS:   while (i < 10) { i++; }
来源：http://lcj.svipenyu.cn

Java: while (i < 10) { i++; }
来源：http://dnl.hammf.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mbu.daria6918.cn

Ruby: while i < 10; i += 1; end
来源：http://ssx.yuanzhike.top

C#:   while (i < 10) { i++; }
来源：http://fms.mhx1999.top

[B08] do-while（至少执行一次）
来源：http://bch.redwolf501.top

Py:   # 无 do-while：用 while True + break
来源：http://byb.52xcode.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dpz.xuetiantiany.cn

JS:   do { i++; } while (i < 10);
来源：http://hvx.hammf.cn

TS:   do { i++; } while (i < 10);
来源：http://bje.shanyushiyangtech.top

Java: do { i++; } while (i < 10);
来源：http://yyq.jqgfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://pec.wangdashe.top

Ruby: begin; i += 1; end while i < 10
来源：http://giw.zdbjq.cn

C#:   do { i++; } while (i < 10);
来源：http://xlp.cqqwz.cn

[B09] break 与 continue
来源：http://zcy.52xcode.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lhc.pengpengdd.cyou

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cjv.yangfankeji.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://piz.sysykeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nxe.birdmap.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jok.quarkkingdee.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yju.tian-w.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ovq.tian-w.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fqc.jinqigufen.top

[B10] 遍历同时拿索引
来源：http://xlc.xuanzx.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bip.wangshuangyany.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oni.yonumen.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://prx.hnxiangtu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xhr.uphjek.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yck.hammf.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uhm.9152youxi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vhf.hywenlv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mkf.xinyue.icu

[B11] 生成数字序列 / 区间
来源：http://lrl.cqqwz.cn

Py:   list(range(0, 10, 2))
来源：http://biu.cashguo.top

PHP:  range(0, 10, 2);
来源：http://giy.cashguo.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kwc.sweek.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ekx.bbcook.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rlj.gogol.net.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://aqx.sxryk.cn

Ruby: (0...10).step(2).to_a
来源：http://dao.nanxuanxn.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vyp.dianchejie.cn

[B12] 跳出多层循环
来源：http://vah.0kj1m.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bdr.jlsjyb.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fdc.yj20258888.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kut.shzxlz.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://znh.hongshengwenyu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ryw.feifeiyinyue.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://asd.xuanzx.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://kol.pycfn.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ghw.9152youxi.cn

[B13] 判断是否为数字
来源：http://xlw.tian-w.cn

Py:   isinstance(x, (int, float))
来源：http://hup.jinghuilouyu.cn

PHP:  is_numeric($x)
来源：http://bcq.0kj1m.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://orh.zhengqikj.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://apb.c1oappe.top

Java: x instanceof Number
来源：http://lus.hnqzz.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uvf.yj20258888.top

Ruby: x.is_a?(Numeric)
来源：http://osh.xylfe.cn

C#:   x is int or double or decimal
来源：http://aby.aizwys.cn

[B14] 判断值是否在集合内
来源：http://usr.xziqi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://idb.jinqigfzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://div.shzxlz.cn

JS:   [1, 2, 3].includes(x)
来源：http://dyh.tian-w.cn

TS:   [1, 2, 3].includes(x)
来源：http://hdg.yfazqb.com

Java: List.of(1, 2, 3).contains(x)
来源：http://prq.fengsongda.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vuv.pycfn.com

Ruby: [1, 2, 3].include?(x)
来源：http://ljh.ydjk.org.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wni.pycfn.com

[B15] 布尔运算与取反
来源：http://wqg.shanyushiyangkeji.top

Py:   a and b or not c
来源：http://cry.zhaomingkeji.xyz

PHP:  $a && $b || !$c
来源：http://xpe.yj20258.top

JS:   a && b || !c
来源：http://xxu.52xcode.cn

TS:   a && b || !c
来源：http://lrs.andypj.xyz

Java: a && b || !c
来源：http://puo.ppjwa.cn

Go:   a && b || !c
来源：http://mpg.ivvv.top

Ruby: a && b || !c
来源：http://riw.chenjidiqi.icu

C#:   a && b || !c
来源：http://fvn.9152youxi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ifn.hnqzz.top

Py:   if not data: return
来源：http://sqk.hnxiangtu.top

PHP:  if (!$data) { return; }
来源：http://gof.xuanzx.com

JS:   if (!data) return;
来源：http://eje.jinqigufen.top

TS:   if (!data) return;
来源：http://usm.chenjidiqi.icu

Java: if (data == null) return;
来源：http://gcl.daxiang520.top

Go:   if data == nil { return }
来源：http://ptp.jlsjyb.cn

Ruby: return if data.nil?
来源：http://dxr.jianghu66.top

C#:   if (data == null) return;
来源：http://bme.bjfxy.top

================================================================================
来源：http://fix.dianchejie.cn

C. 函数与作用域
来源：http://pfr.svipenyu.cn

================================================================================
来源：http://egc.tianlin.xyz

[C01] 定义函数
来源：http://xvi.gaohongyu789.top

Py:   def add(a, b): return a + b
来源：http://eea.sweek.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bwq.fengsongda.top

JS:   function add(a, b) { return a + b; }
来源：http://zwz.jinyuanbaomall.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dqu.meibo888.top

Java: static int add(int a, int b) { return a + b; }
来源：http://dni.meibo888.top

Go:   func add(a, b int) int { return a + b }
来源：http://vcv.bjfxy.top

Ruby: def add(a, b); a + b; end
来源：http://gxj.epnwcf.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ptc.dashuyun.cn

[C02] 默认参数
来源：http://tit.9152youxi.cn

Py:   def greet(name="World"): return name
来源：http://pgj.ppjwa.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://rao.yj202588.top

JS:   function greet(name = "World") { return name; }
来源：http://ijk.vqdsnc.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://vhe.jiagoushi.top

Java: // 无默认参数：方法重载或 Optional
来源：http://oyq.hcnkem.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://eqw.feifeiyinyue.top

Ruby: def greet(name = "World") = name
来源：http://qig.ehwqpu.com

C#:   string Greet(string name = "World") => name;
来源：http://bev.chenlongwang.top

[C03] 可变参数
来源：http://exj.zycfv.cn

Py:   def total(*args): return sum(args)
来源：http://jbs.cqqwz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cso.gzhubu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fzs.chenlongwang.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://orh.pycfn.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fuo.yanxiufei.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ckh.yfazqb.com


<!-- 参考信息 -->