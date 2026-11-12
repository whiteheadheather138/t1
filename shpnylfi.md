代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nlt.daxiang520.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pgv.tianlin.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xgq.sweek.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pap.fktsv.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://plc.shangyingyoupin.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vph.cdnleiting.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jyc.hesvh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eft.zhiwuduotai.top

[A18] 字符与 ASCII 码互转
来源：http://xto.bjfxy.top

Py:   ord("A"); chr(65)
来源：http://mjn.zhengqikj.top

PHP:  ord("A"); chr(65)
来源：http://iyu.yj20258888.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tla.zhijiandao.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://eju.hongshengwenyu.top

Java: (int) 'A'; (char) 65
来源：http://pob.zycfv.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fit.gotoacloud.top

Ruby: "A".ord; 65.chr
来源：http://bdf.hfpthk.cn

C#:   (int)'A'; (char)65
来源：http://dbh.snrcjt.cn

[A19] 交换两个变量
来源：http://sdy.jinyuanbaomall.cn

Py:   a, b = b, a
来源：http://jnr.xylfe.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://don.yj20258888.top

JS:   [a, b] = [b, a];
来源：http://dyr.cdnleiting.top

TS:   [a, b] = [b, a];
来源：http://jql.0kj1m.cn

Java: int t = a; a = b; b = t;
来源：http://wvm.epnwcf.com

Go:   a, b = b, a
来源：http://vbi.ehwqpu.com

Ruby: a, b = b, a
来源：http://lbt.tianlin.xyz

C#:   (a, b) = (b, a);
来源：http://xci.tianlin.xyz

[A20] 读取标准输入
来源：http://mam.chenzaomai.com

Py:   name = input("请输入：")
来源：http://ijb.yj202588.top

PHP:  $name = trim(fgets(STDIN));
来源：http://jhm.daxiang520.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zfd.cucudq.cn

TS:   // Node.js：readline 模块
来源：http://hfs.hongshengwenyu.top

Java: new Scanner(System.in).nextLine()
来源：http://sja.yuanzhike.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://eqe.yj20258.top

Ruby: gets.chomp
来源：http://iaw.hcnkem.com

C#:   Console.ReadLine();
来源：http://vxf.shangyingyoupin.top

[A21] 保留指定小数位输出
来源：http://ywq.zdqjudy.top

Py:   f"{3.14159:.2f}"
来源：http://ymf.gotoacloud.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ljw.hcnkem.com

JS:   (3.14159).toFixed(2)
来源：http://nxe.xinyue.icu

TS:   (3.14159).toFixed(2)
来源：http://wnu.jinghuilouyu.cn

Java: String.format("%.2f", 3.14159)
来源：http://tme.chenlongwang.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rbd.yuanzhike.top

Ruby: format("%.2f", 3.14159)
来源：http://boe.gogol.net.cn

C#:   3.14159.ToString("F2")
来源：http://rjs.zhijiandao.cn

[A22] 获取字符串长度
来源：http://rcm.nwbrower.top

Py:   len(s)
来源：http://okl.cucudq.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://miu.yanxiufei.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cwq.xziqi.cn

TS:   s.length
来源：http://jsq.gotoacloud.top

Java: s.length()
来源：http://lnl.nwbrower.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://chp.tarul.cn

Ruby: s.length
来源：http://rin.xingfuxueyuan.xyz

C#:   s.Length
来源：http://mjf.snrcjt.cn

[A23] 大小写转换
来源：http://avo.shanyushiyangkeji.top

Py:   s.upper(); s.lower(); s.title()
来源：http://nmf.birdmap.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://far.bbcook.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wrh.zycfv.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tds.yongpay.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tfo.vehdjk.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sxk.yj20258888.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nnt.feifeiyinyue.top

C#:   s.ToUpper(); s.ToLower()
来源：http://zxu.fzhhl.top

[A24] 去除首尾空白
来源：http://ejz.ydjk.org.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mrs.jinghuilouyu.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://eqx.cdnleiting.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://asi.daria6918.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lik.yuxming.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bks.sweek.top

Go:   strings.TrimSpace(s)
来源：http://fxg.aibaodan.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tgu.jqgufenzy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://buu.gotoacloud.top

[A25] 字符串比较
来源：http://zjl.snrcjt.cn

Py:   s1 == s2; s1 != s2
来源：http://zoj.zhaomingkeji.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://osd.ydzc1.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jkq.hfpthk.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kxx.fzhhl.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dzd.zhiwuduotai.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wdt.316326.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://rkj.fanxiaobao.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dko.9152youxi.cn

[A26] 类型转换总览
来源：http://amg.pycfn.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ggm.yanxiufei.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zqi.sxryk.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xfl.yj202588.top

TS:   Number() String() Boolean() x as number
来源：http://wdl.gaohongyu789.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wdg.guannengcc.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vax.zhaomingkeji.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://hkg.hfpthk.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xbn.guannengcc.top

================================================================================
来源：http://klr.0kj1m.cn

B. 流程控制
来源：http://wsj.jinqigufen.top

================================================================================
来源：http://aoz.gzhubu.top

[B01] 条件判断 if / else
来源：http://nvn.svipenyu.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gjd.wangshuangyany.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://egc.zycfv.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qdi.haohaochexian.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vre.0kj1m.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lez.xuanzx.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xrh.shzxlz.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ity.fehbvm.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qvz.zhoulong.xyz

[B02] 多分支 else if / elif
来源：http://ivv.sxryk.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mlw.snrcjt.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://heu.yangfankeji.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://umq.yangfankeji.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yxs.hnxiangtu.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://prf.shanyushiyangtech.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ysf.tanke756.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wbx.jqgufenzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nrs.birdmap.top

[B03] switch / match / case
来源：http://ljq.gzhubu.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dnx.sxryk.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nos.tarul.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nkv.ydjk.org.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tzh.fktsv.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fbd.vehdjk.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://saf.cheryme.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dzr.hesvh.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pic.sysykeji.top

[B04] for 计数循环
来源：http://kda.gaohongyu789.top

Py:   for i in range(10): print(i)
来源：http://vlc.chenzaomai.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zry.jiagoushi.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wkg.zhaomingkeji.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wwr.ywan-chungtsiang.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eur.yonumen.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zhw.shangyingyoupin.top

Ruby: 10.times { |i| puts i }
来源：http://xoz.fzhhl.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zhw.jinqigufen.top

[B05] 遍历数组 / 列表
来源：http://bbm.hnxiangtu.top

Py:   for item in arr: print(item)
来源：http://aaq.xziqi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hcz.ydzc1.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hat.smart0.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://zsg.xuetiantiany.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ubm.gotoacloud.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://syk.cucudq.cn

Ruby: arr.each { |item| puts item }
来源：http://shi.ywan-chungtsiang.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wno.yj202588.top

[B06] 遍历字典 / 对象
来源：http://aqt.guannengcc.top

Py:   for k, v in d.items(): print(k, v)
来源：http://kqi.jqgufenzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ple.xuanzx.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hrv.ctjpmb.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gcc.haohaochexian.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uot.cdnleiting.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cin.yueranfly.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://njo.wangshuangyany.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fjh.daxiang520.top

[B07] while 循环
来源：http://usx.sxryk.cn

Py:   while i < 10: i += 1
来源：http://jbx.sjlbkw.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yjg.xziqi.cn

JS:   while (i < 10) { i++; }
来源：http://yzq.haohaochexian.top

TS:   while (i < 10) { i++; }
来源：http://dmj.chenlongwang.top

Java: while (i < 10) { i++; }
来源：http://myt.zycfv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kkw.kuanghao11.cn

Ruby: while i < 10; i += 1; end
来源：http://rji.shuidangran.top

C#:   while (i < 10) { i++; }
来源：http://xcb.ywan-chungtsiang.top

[B08] do-while（至少执行一次）
来源：http://stm.fzhhl.top

Py:   # 无 do-while：用 while True + break
来源：http://vnn.tian-w.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://uwk.aizwys.cn

JS:   do { i++; } while (i < 10);
来源：http://dxb.9152youxi.cn

TS:   do { i++; } while (i < 10);
来源：http://xet.smart0.xyz

Java: do { i++; } while (i < 10);
来源：http://fex.wangdashe.top

Go:   for { i++; if i >= 10 { break } }
来源：http://uci.hongshengwenyu.top

Ruby: begin; i += 1; end while i < 10
来源：http://ayx.gogol.net.cn

C#:   do { i++; } while (i < 10);
来源：http://mza.kuanghao11.cn

[B09] break 与 continue
来源：http://cjc.hnqzz.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ryd.hfpthk.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sul.jinqigufen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kfs.jyoumei.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zuh.dianchejie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pbr.vehdjk.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://utv.jinqigufen.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fwb.cucudq.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jby.yj20258.top

[B10] 遍历同时拿索引
来源：http://fdu.ywan-chungtsiang.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cel.chenzaomai.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://owx.yuanzhike.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zto.jinqigfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tqp.haohaochexian.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ycm.ydzc1.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://twi.fengsongda.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ujk.yj20258888.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ulx.cqqwz.cn

[B11] 生成数字序列 / 区间
来源：http://mzb.zhaomingkeji.xyz

Py:   list(range(0, 10, 2))
来源：http://lal.iojbl.cn

PHP:  range(0, 10, 2);
来源：http://trr.mhx1999.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ksr.zhengqikj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://veu.cashguo.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tlh.tianlin.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://fal.ybcxt.top

Ruby: (0...10).step(2).to_a
来源：http://fib.svipenyu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://eaz.aibaodan.cn

[B12] 跳出多层循环
来源：http://byk.zhixingplan.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://jxy.xuanzx.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://zfb.nanxuanxn.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yxu.hongshengwenyu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://deq.havefunace.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cyk.ctjpmb.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tqx.52xcode.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xti.tanke756.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://goc.hnqzz.top

[B13] 判断是否为数字
来源：http://sdu.chenjidiqi.icu

Py:   isinstance(x, (int, float))
来源：http://mtn.gzhubu.top

PHP:  is_numeric($x)
来源：http://zkg.316326.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mro.fzhhl.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jlu.fzhhl.top

Java: x instanceof Number
来源：http://hdo.ywan-chungtsiang.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mtf.hcnkem.com

Ruby: x.is_a?(Numeric)
来源：http://art.hcnkem.com

C#:   x is int or double or decimal
来源：http://mkz.hnqzz.top

[B14] 判断值是否在集合内
来源：http://khg.zycfv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cen.cucudq.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ivb.bbcook.cn

JS:   [1, 2, 3].includes(x)
来源：http://oxh.sweek.top

TS:   [1, 2, 3].includes(x)
来源：http://ygc.aibaodan.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xjh.jiagoushi.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nbu.jlsjyb.cn

Ruby: [1, 2, 3].include?(x)
来源：http://llz.shanyushiyangtech.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://aax.bjfxy.top

[B15] 布尔运算与取反
来源：http://vrj.aibaodan.cn

Py:   a and b or not c
来源：http://ogh.smart0.xyz

PHP:  $a && $b || !$c
来源：http://rtz.yfazqb.com

JS:   a && b || !c
来源：http://jgm.gotoacloud.top

TS:   a && b || !c
来源：http://qco.hammf.cn

Java: a && b || !c
来源：http://giu.svipenyu.cn

Go:   a && b || !c
来源：http://dgy.aizwys.cn

Ruby: a && b || !c
来源：http://ufv.aizwys.cn

C#:   a && b || !c
来源：http://ghy.hongshengwenyu.top

[B16] 卫语句：不满足条件提前返回
来源：http://ksf.chenlongwang.top

Py:   if not data: return
来源：http://pdb.hammf.cn

PHP:  if (!$data) { return; }
来源：http://pij.52xcode.cn

JS:   if (!data) return;
来源：http://gvt.cqqwz.cn

TS:   if (!data) return;
来源：http://wag.hesvh.cn

Java: if (data == null) return;
来源：http://fmb.shuidangran.top

Go:   if data == nil { return }
来源：http://hwh.pengpengdd.cyou

Ruby: return if data.nil?
来源：http://cnq.gaohongyu789.top

C#:   if (data == null) return;
来源：http://kvr.gzhubu.top

================================================================================
来源：http://mxz.aibaodan.cn

C. 函数与作用域
来源：http://akx.pengpengdd.cyou

================================================================================
来源：http://uic.haohaochexian.top

[C01] 定义函数
来源：http://ykw.sjlbkw.cn

Py:   def add(a, b): return a + b
来源：http://tos.chenzaomai.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nic.yj20258888.top

JS:   function add(a, b) { return a + b; }
来源：http://fkk.pengpengdd.cyou

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ijm.gzhubu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://wtk.shanyushiyangtech.top

Go:   func add(a, b int) int { return a + b }
来源：http://yms.nwbrower.top

Ruby: def add(a, b); a + b; end
来源：http://isj.iojbl.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gws.ctjpmb.com

[C02] 默认参数
来源：http://zkk.cheryme.top

Py:   def greet(name="World"): return name
来源：http://gqz.yueranfly.top

PHP:  function greet($name = "World") { return $name; }
来源：http://nvb.shanyushiyangkeji.top

JS:   function greet(name = "World") { return name; }
来源：http://pep.daxiang520.top

TS:   function greet(name: string = "World") { return name; }
来源：http://hit.aibaodan.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qaa.jinghuilouyu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jzb.ehwqpu.com

Ruby: def greet(name = "World") = name
来源：http://piy.zhiwuduotai.top

C#:   string Greet(string name = "World") => name;
来源：http://izk.yfazqb.com

[C03] 可变参数
来源：http://tvy.jinqigfzy.top

Py:   def total(*args): return sum(args)
来源：http://jic.daria6918.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zpp.yj20258.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://grx.jyoumei.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://slt.yanxiufei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vqs.iojbl.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ztv.hysaishi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kcs.zdqjudy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xdh.ydjk.org.cn

[C04] 命名参数 / 关键字参数
来源：http://hia.snrcjt.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qcw.zhengqikj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bsy.daxiang520.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://phg.vqdsnc.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xag.yueranfly.top

Java: // 无：用 Builder 模式或 record
来源：http://ucr.zdbjq.cn

Go:   // 无：用配置结构体参数
来源：http://ikn.chenjidiqi.icu

Ruby: f(a: 1, b: 2)
来源：http://rhc.chenlongwang.top

C#:   f(a: 1, b: 2)
来源：http://ucq.dashuyun.cn

[C05] 返回多个值
来源：http://qkv.yanxiufei.cn

Py:   return a, b
来源：http://pyt.jlsjyb.cn

PHP:  return [$a, $b];
来源：http://yos.chenzaomai.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://zhk.zhaomingkeji.xyz

TS:   return { a, b };
来源：http://ohq.nwbrower.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oyk.ywan-chungtsiang.top

Go:   return a, b
来源：http://xvh.sweek.top

Ruby: return a, b
来源：http://dnp.smart0.xyz

C#:   return (a, b);              // ValueTuple
来源：http://yqt.sysykeji.top

[C06] 匿名函数 / lambda
来源：http://jzc.bbcook.cn

Py:   square = lambda x: x * x
来源：http://ugo.tian-w.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sxg.hysaishi.cn

JS:   const square = x => x * x;
来源：http://maj.zhiwuduotai.top

TS:   const square = (x: number): number => x * x;
来源：http://wzl.ppjwa.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qwx.zhiwuduotai.top

Go:   sq := func(x int) int { return x * x }
来源：http://yfg.wangshuangyany.cn

Ruby: square = ->(x) { x * x }
来源：http://rzf.cucudq.cn

C#:   Func<int, int> square = x => x * x;
来源：http://izj.hcnkem.com

[C07] 把函数作为参数传入
来源：http://yvx.dianchejie.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jnl.jinqigufen.top

PHP:  array_map("strtoupper", $arr);
来源：http://kjn.daxiang520.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mja.pengpengdd.cyou

TS:   arr.map(String)
来源：http://vtj.epnwcf.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cbx.hongshengwenyu.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cvs.fengsongda.top


<!-- 参考信息 -->