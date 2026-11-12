代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dke.fanxiaobao.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tef.xinyue.icu

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dsi.316326.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ulx.zhaomingkeji.xyz

[A18] 字符与 ASCII 码互转
来源：http://ken.xinyue.icu

Py:   ord("A"); chr(65)
来源：http://bnk.jiagoushi.top

PHP:  ord("A"); chr(65)
来源：http://vdl.gzhubu.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ohd.yj20258.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://syw.zdqjudy.top

Java: (int) 'A'; (char) 65
来源：http://omm.epnwcf.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://kfj.uphjek.com

Ruby: "A".ord; 65.chr
来源：http://rxw.vehdjk.com

C#:   (int)'A'; (char)65
来源：http://ucm.sufxvd.cn

[A19] 交换两个变量
来源：http://zdb.yfazqb.com

Py:   a, b = b, a
来源：http://glo.zhijiandao.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://lwd.nanxinkj.top

JS:   [a, b] = [b, a];
来源：http://azk.sweek.top

TS:   [a, b] = [b, a];
来源：http://nxi.hnqzz.top

Java: int t = a; a = b; b = t;
来源：http://sdc.chenjidiqi.icu

Go:   a, b = b, a
来源：http://ygt.yvedp.cn

Ruby: a, b = b, a
来源：http://rru.guannengcc.top

C#:   (a, b) = (b, a);
来源：http://qgk.fengsongda.top

[A20] 读取标准输入
来源：http://nbr.nanxuanxn.top

Py:   name = input("请输入：")
来源：http://ode.shangyingyoupin.top

PHP:  $name = trim(fgets(STDIN));
来源：http://mml.hammf.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ocq.jinyuanbaomall.cn

TS:   // Node.js：readline 模块
来源：http://sxs.fktsv.cn

Java: new Scanner(System.in).nextLine()
来源：http://jjk.shuidangran.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yva.ivvv.top

Ruby: gets.chomp
来源：http://fia.vqdsnc.cn

C#:   Console.ReadLine();
来源：http://wpl.aibaodan.cn

[A21] 保留指定小数位输出
来源：http://qwl.316326.xyz

Py:   f"{3.14159:.2f}"
来源：http://xtx.dianchejie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ehj.yuanzhike.top

JS:   (3.14159).toFixed(2)
来源：http://pij.tanke756.top

TS:   (3.14159).toFixed(2)
来源：http://zzl.zhongyouzk.top

Java: String.format("%.2f", 3.14159)
来源：http://zbd.xziqi.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gbv.chenzaomai.com

Ruby: format("%.2f", 3.14159)
来源：http://pus.zhijiandao.cn

C#:   3.14159.ToString("F2")
来源：http://mve.jinyuanbaomall.cn

[A22] 获取字符串长度
来源：http://hgf.zdbjq.cn

Py:   len(s)
来源：http://kzx.mhx1999.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://njw.jianghu66.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mhg.fehbvm.com

TS:   s.length
来源：http://dth.epnwcf.com

Java: s.length()
来源：http://bjn.cheryme.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jft.dashuyun.cn

Ruby: s.length
来源：http://zeo.sxryk.cn

C#:   s.Length
来源：http://cne.quarkkingdee.top

[A23] 大小写转换
来源：http://xky.redwolf501.top

Py:   s.upper(); s.lower(); s.title()
来源：http://kot.chenlongwang.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ixq.dianchejie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dsq.pengpengdd.cyou

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://igt.jinghuilouyu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jrm.feifeiyinyue.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://yus.shangyingyoupin.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hvl.shzxlz.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fam.sweek.top

[A24] 去除首尾空白
来源：http://ems.xinyue.icu

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ygu.snrcjt.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rdz.svipenyu.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eut.aibaodan.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ttl.shzxlz.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zme.guowangkeji.top

Go:   strings.TrimSpace(s)
来源：http://asx.daxiang520.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xih.316326.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kvh.cheryme.top

[A25] 字符串比较
来源：http://mgg.ppjwa.cn

Py:   s1 == s2; s1 != s2
来源：http://jzb.jyoumei.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gtl.jianghu66.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bix.smart0.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ovw.sufxvd.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lua.yvedp.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://war.hcnkem.com

Ruby: s1 == s2; s1 <=> s2
来源：http://phm.ivvv.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fpk.zdbjq.cn

[A26] 类型转换总览
来源：http://bnj.yuxming.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gfg.zhixingplan.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mnk.bjfxy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vts.xinyue.icu

TS:   Number() String() Boolean() x as number
来源：http://lok.gogol.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kpa.hywenlv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mex.zdbjq.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vzd.jqgufenzy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tmk.shangyingyoupin.top

================================================================================
来源：http://dju.jqgfzy.top

B. 流程控制
来源：http://ine.cqqwz.cn

================================================================================
来源：http://imx.nanxuanxn.top

[B01] 条件判断 if / else
来源：http://cen.aizwys.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://iub.sufxvd.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ooe.sjlbkw.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mee.yongpay.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yrg.cheryme.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://cge.hongshengwenyu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kre.shuidangran.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rsf.guannengcc.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mvb.tianlin.xyz

[B02] 多分支 else if / elif
来源：http://wnq.jqgfzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jcg.aizwys.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pfg.jinyuanbaomall.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ppy.sxryk.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xie.mhx1999.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://evp.fktsv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nmb.cucudq.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pmv.quarkkingdee.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lpm.hongshengwenyu.top

[B03] switch / match / case
来源：http://hdo.zhijiandao.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vge.epnwcf.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://alp.guowangkeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tch.hysaishi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ymc.jiagoushi.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pqb.svipenyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zfa.cucudq.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jpo.pengpengdd.cyou

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bfk.redwolf501.top

[B04] for 计数循环
来源：http://ccj.fanxiaobao.xyz

Py:   for i in range(10): print(i)
来源：http://viw.dashuyun.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fxv.daria6918.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yxj.gotoacloud.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hlf.guannengcc.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jdb.kuanghao11.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://iqy.jinqigufen.top

Ruby: 10.times { |i| puts i }
来源：http://ybt.yuanzhike.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mjt.smart0.xyz

[B05] 遍历数组 / 列表
来源：http://btm.316326.xyz

Py:   for item in arr: print(item)
来源：http://jqe.zhijiandao.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xgy.jiagoushi.top

JS:   for (const item of arr) { console.log(item); }
来源：http://xeb.havefunace.top

TS:   for (const item of arr) { console.log(item); }
来源：http://tkz.xuetiantiany.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://yuv.sufxvd.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mlz.xziqi.cn

Ruby: arr.each { |item| puts item }
来源：http://hah.chenzaomai.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://png.zhaomingkeji.xyz

[B06] 遍历字典 / 对象
来源：http://pyt.ivvv.top

Py:   for k, v in d.items(): print(k, v)
来源：http://acg.yj202588.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xlg.sjlbkw.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fnq.quarkkingdee.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zrz.xuetiantiany.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hbq.fanxiaobao.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ces.snrcjt.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wvy.ctjpmb.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://epj.wangshuangyany.cn

[B07] while 循环
来源：http://wwe.havefunace.top

Py:   while i < 10: i += 1
来源：http://nji.yongpay.top

PHP:  while ($i < 10) { $i++; }
来源：http://oys.xylfe.cn

JS:   while (i < 10) { i++; }
来源：http://ioe.shangyingyoupin.top

TS:   while (i < 10) { i++; }
来源：http://vzh.nwbrower.top

Java: while (i < 10) { i++; }
来源：http://ikx.hnqzz.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://twa.tarul.cn

Ruby: while i < 10; i += 1; end
来源：http://jaj.cashguo.top

C#:   while (i < 10) { i++; }
来源：http://orm.snrcjt.cn

[B08] do-while（至少执行一次）
来源：http://slh.meibo888.top

Py:   # 无 do-while：用 while True + break
来源：http://upb.hongshengwenyu.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jow.hcnkem.com

JS:   do { i++; } while (i < 10);
来源：http://bmw.andypj.xyz

TS:   do { i++; } while (i < 10);
来源：http://gbm.zycfv.cn

Java: do { i++; } while (i < 10);
来源：http://fje.yj202588.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ons.hammf.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fez.hnxiangtu.top

C#:   do { i++; } while (i < 10);
来源：http://rqn.feifeiyinyue.top

[B09] break 与 continue
来源：http://znx.aizwys.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://awq.yfazqb.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hhw.jlsjyb.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ksh.xingfuxueyuan.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://twe.nanxuanxn.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://chz.daria6918.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kdw.tanke756.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://znj.zhaomingkeji.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xza.chenlongwang.top

[B10] 遍历同时拿索引
来源：http://uat.guowangkeji.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jlo.ivvv.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hjv.chenlongwang.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ttm.zhixingplan.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wwn.fehbvm.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xwe.0kj1m.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://edw.jinqigufen.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://noo.hfpthk.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ylx.zhongyouzk.top

[B11] 生成数字序列 / 区间
来源：http://mwk.hesvh.cn

Py:   list(range(0, 10, 2))
来源：http://bop.sweek.top

PHP:  range(0, 10, 2);
来源：http://yac.jiagoushi.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kud.hywenlv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kcc.guowangkeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ylx.hysaishi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ejt.shzxlz.cn

Ruby: (0...10).step(2).to_a
来源：http://gln.ivvv.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://owc.yonumen.top

[B12] 跳出多层循环
来源：http://bpc.jlsjyb.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://msh.yj20258888.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vxt.0kj1m.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kbx.jlsjyb.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ahv.nanxinkj.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dpb.shanyushiyangkeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yij.hfpthk.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hmh.shuidangran.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://aag.fehbvm.com

[B13] 判断是否为数字
来源：http://gma.birdmap.top

Py:   isinstance(x, (int, float))
来源：http://cie.vehdjk.com

PHP:  is_numeric($x)
来源：http://zvi.fehbvm.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ith.jyoumei.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lql.hywenlv.cn

Java: x instanceof Number
来源：http://fjy.jinyuanbaomall.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rqg.iojbl.cn

Ruby: x.is_a?(Numeric)
来源：http://vhy.jinqigufen.top

C#:   x is int or double or decimal
来源：http://pxg.dianchejie.cn

[B14] 判断值是否在集合内
来源：http://aum.gaohongyu789.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dpz.shanyushiyangtech.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jew.xinyue.icu

JS:   [1, 2, 3].includes(x)
来源：http://xct.andypj.xyz

TS:   [1, 2, 3].includes(x)
来源：http://ekf.redwolf501.top

Java: List.of(1, 2, 3).contains(x)
来源：http://puo.tarul.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://upm.ydjk.org.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sqi.jianghu66.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sbu.yueranfly.top

[B15] 布尔运算与取反
来源：http://nrn.snrcjt.cn

Py:   a and b or not c
来源：http://ixk.tian-w.cn

PHP:  $a && $b || !$c
来源：http://swr.haohaochexian.top

JS:   a && b || !c
来源：http://opm.hammf.cn

TS:   a && b || !c
来源：http://rdi.nwbrower.top

Java: a && b || !c
来源：http://qyb.ppjwa.cn

Go:   a && b || !c
来源：http://xac.shanyushiyangkeji.top

Ruby: a && b || !c
来源：http://xfw.tianlin.xyz

C#:   a && b || !c
来源：http://nvo.yj20258888.top

[B16] 卫语句：不满足条件提前返回
来源：http://rlz.tianlin.xyz

Py:   if not data: return
来源：http://ctt.jinghuilouyu.cn

PHP:  if (!$data) { return; }
来源：http://nmr.hammf.cn

JS:   if (!data) return;
来源：http://bgs.fanxiaobao.xyz

TS:   if (!data) return;
来源：http://cbh.redwolf501.top

Java: if (data == null) return;
来源：http://wkl.fzhhl.top

Go:   if data == nil { return }
来源：http://slc.ybcxt.top

Ruby: return if data.nil?
来源：http://ami.cucudq.cn

C#:   if (data == null) return;
来源：http://nic.zhongyouzk.top

================================================================================
来源：http://czq.sysykeji.top

C. 函数与作用域
来源：http://qej.zdbjq.cn

================================================================================
来源：http://cev.hfpthk.cn

[C01] 定义函数
来源：http://kuk.pengpengdd.cyou

Py:   def add(a, b): return a + b
来源：http://kzy.zycfv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dqf.smart0.xyz

JS:   function add(a, b) { return a + b; }
来源：http://xvx.zhijiandao.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kyb.jqgfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://jxl.fzhhl.top

Go:   func add(a, b int) int { return a + b }
来源：http://zav.ywan-chungtsiang.top

Ruby: def add(a, b); a + b; end
来源：http://rin.hongshengwenyu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://piv.shanyushiyangkeji.top

[C02] 默认参数
来源：http://xra.xylfe.cn

Py:   def greet(name="World"): return name
来源：http://dkl.uphjek.com

PHP:  function greet($name = "World") { return $name; }
来源：http://pew.feifeiyinyue.top

JS:   function greet(name = "World") { return name; }
来源：http://ugg.xuanzx.com

TS:   function greet(name: string = "World") { return name; }
来源：http://buw.sysykeji.top

Java: // 无默认参数：方法重载或 Optional
来源：http://vkm.smart0.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://eps.c1oappe.top

Ruby: def greet(name = "World") = name
来源：http://ixc.hfpthk.cn

C#:   string Greet(string name = "World") => name;
来源：http://mmv.chenzaomai.com

[C03] 可变参数
来源：http://kyn.ctjpmb.com

Py:   def total(*args): return sum(args)
来源：http://lzr.shanyushiyangtech.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wnw.wangshuangyany.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://moy.pengpengdd.cyou

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zbn.pengpengdd.cyou

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iqh.hcnkem.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hsl.shanyushiyangtech.top

Ruby: def total(*nums); nums.sum; end
来源：http://ncj.ydjk.org.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kuk.shuidangran.top

[C04] 命名参数 / 关键字参数
来源：http://eth.pycfn.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eqp.zhengqikj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qov.bbcook.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dpl.9152youxi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://aom.shanyushiyangkeji.top

Java: // 无：用 Builder 模式或 record
来源：http://zmi.guowangkeji.top

Go:   // 无：用配置结构体参数
来源：http://lzk.ybcxt.top

Ruby: f(a: 1, b: 2)
来源：http://nlv.cucudq.cn

C#:   f(a: 1, b: 2)
来源：http://fmv.redwolf501.top

[C05] 返回多个值
来源：http://jvb.zycfv.cn

Py:   return a, b
来源：http://odg.zhaomingkeji.xyz

PHP:  return [$a, $b];
来源：http://bsc.xinyue.icu

JS:   return [a, b];             // 或 return { a, b };
来源：http://jkk.dashuyun.cn

TS:   return { a, b };
来源：http://mdj.hongshengwenyu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pju.vqdsnc.cn

Go:   return a, b
来源：http://kdx.svipenyu.cn

Ruby: return a, b
来源：http://uij.quarkkingdee.top

C#:   return (a, b);              // ValueTuple
来源：http://kss.aibaodan.cn

[C06] 匿名函数 / lambda
来源：http://pxn.feifeiyinyue.top

Py:   square = lambda x: x * x
来源：http://nru.yvedp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://gsq.52xcode.cn

JS:   const square = x => x * x;
来源：http://lkk.smart0.xyz

TS:   const square = (x: number): number => x * x;
来源：http://yyl.gotoacloud.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cof.epnwcf.com

Go:   sq := func(x int) int { return x * x }
来源：http://uun.hnxiangtu.top

Ruby: square = ->(x) { x * x }
来源：http://bxz.hammf.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yxq.nwbrower.top

[C07] 把函数作为参数传入
来源：http://sbp.zdqjudy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fql.yvedp.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dyd.52xcode.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://oya.shanyushiyangtech.top

TS:   arr.map(String)
来源：http://vmo.zhixingplan.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mej.birdmap.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://nnv.xinyue.icu

Ruby: arr.map(&:upcase)
来源：http://kgm.tanke756.top

C#:   arr.Select(s => s.ToUpper())
来源：http://xcx.yongpay.top

[C08] 闭包
来源：http://wap.jinyuanbaomall.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nqo.bjfxy.top


<!-- 参考信息 -->