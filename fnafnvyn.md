代发 wailian999

TS:   s.length
来源：http://xay.uphjek.com

Java: s.length()
来源：http://wem.gzhubu.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tla.316326.xyz

Ruby: s.length
来源：http://kmi.sufxvd.cn

C#:   s.Length
来源：http://poa.c1oappe.top

[A23] 大小写转换
来源：http://gsr.nanxinkj.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ykl.jlsjyb.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vtv.52xcode.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://htk.jqgufenzy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wnk.iojbl.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mys.jinyuanbaomall.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hej.xingfuxueyuan.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jxm.nwbrower.top

C#:   s.ToUpper(); s.ToLower()
来源：http://qcz.zhengqikj.top

[A24] 去除首尾空白
来源：http://enf.xingfuxueyuan.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://acq.hfpthk.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://abt.birdmap.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kya.jinqigufen.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://iap.fanxiaobao.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wte.sweek.top

Go:   strings.TrimSpace(s)
来源：http://ujp.meibo888.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qpp.wangdashe.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sxo.pengpengdd.cyou

[A25] 字符串比较
来源：http://wrf.daxiang520.top

Py:   s1 == s2; s1 != s2
来源：http://dvq.yfazqb.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qcm.yongpay.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lmb.quarkkingdee.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ibp.tian-w.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://stk.gaohongyu789.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hab.mhx1999.top

Ruby: s1 == s2; s1 <=> s2
来源：http://jog.quarkkingdee.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wdy.tianlin.xyz

[A26] 类型转换总览
来源：http://rwb.sxryk.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qxn.chenlongwang.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vfd.zhoulong.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ydv.52xcode.cn

TS:   Number() String() Boolean() x as number
来源：http://tip.haohaochexian.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gyf.yj202588.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pnp.tarul.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ewr.c1oappe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://udg.yuanzhike.top

================================================================================
来源：http://uhj.xingfuxueyuan.xyz

B. 流程控制
来源：http://mnt.zycfv.cn

================================================================================
来源：http://cor.sweek.top

[B01] 条件判断 if / else
来源：http://tze.smart0.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://poc.cucudq.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://clf.daria6918.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://oqp.ywan-chungtsiang.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ehc.9152youxi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lco.tianlin.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://btx.zhongyouzk.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://npr.tian-w.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kmg.nanxinkj.top

[B02] 多分支 else if / elif
来源：http://xyc.yuanzhike.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://axl.zhiwuduotai.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mou.shanyushiyangtech.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sqs.yvedp.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dfz.wangshuangyany.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qbk.tanke756.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://oai.gaohongyu789.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xuf.yonumen.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hls.jinqigfzy.top

[B03] switch / match / case
来源：http://jnb.ehwqpu.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://azw.fehbvm.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nic.xinyue.icu

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bjy.tian-w.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fai.hammf.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://snz.shangyingyoupin.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lpv.xinyue.icu

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mhf.xuetiantiany.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mll.yangfankeji.com

[B04] for 计数循环
来源：http://ehz.daria6918.cn

Py:   for i in range(10): print(i)
来源：http://eew.chenzaomai.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zax.aizwys.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sor.hesvh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hhg.fktsv.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xyi.haohaochexian.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hyc.sxryk.cn

Ruby: 10.times { |i| puts i }
来源：http://dpc.shanyushiyangkeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rnn.hongshengwenyu.top

[B05] 遍历数组 / 列表
来源：http://fgk.gzhubu.top

Py:   for item in arr: print(item)
来源：http://wpe.shzxlz.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hue.iojbl.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lyj.cashguo.top

TS:   for (const item of arr) { console.log(item); }
来源：http://erq.fktsv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jrc.vqdsnc.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xbr.chenlongwang.top

Ruby: arr.each { |item| puts item }
来源：http://jas.sxryk.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pib.jiagoushi.top

[B06] 遍历字典 / 对象
来源：http://arj.jqgufenzy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://yhx.xziqi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://azs.hfpthk.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uqf.yangfankeji.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://knv.xylfe.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://enw.xuanzx.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://flv.hammf.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hhd.mhx1999.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://msn.daria6918.cn

[B07] while 循环
来源：http://uwj.fktsv.cn

Py:   while i < 10: i += 1
来源：http://orb.shanyushiyangtech.top

PHP:  while ($i < 10) { $i++; }
来源：http://yky.yj20258.top

JS:   while (i < 10) { i++; }
来源：http://mfp.wangdashe.top

TS:   while (i < 10) { i++; }
来源：http://qlv.shuidangran.top

Java: while (i < 10) { i++; }
来源：http://mtc.yanxiufei.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qwy.ybcxt.top

Ruby: while i < 10; i += 1; end
来源：http://zko.chenjidiqi.icu

C#:   while (i < 10) { i++; }
来源：http://vmr.xuanzx.com

[B08] do-while（至少执行一次）
来源：http://zpx.wangdashe.top

Py:   # 无 do-while：用 while True + break
来源：http://heu.0kj1m.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ubw.fktsv.cn

JS:   do { i++; } while (i < 10);
来源：http://noe.sweek.top

TS:   do { i++; } while (i < 10);
来源：http://mwe.zhijiandao.cn

Java: do { i++; } while (i < 10);
来源：http://gxs.nwbrower.top

Go:   for { i++; if i >= 10 { break } }
来源：http://haa.zhijiandao.cn

Ruby: begin; i += 1; end while i < 10
来源：http://omd.cqqwz.cn

C#:   do { i++; } while (i < 10);
来源：http://zxb.shuidangran.top

[B09] break 与 continue
来源：http://exy.smart0.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fkd.yueranfly.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kpw.guannengcc.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sau.tianlin.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vpi.zhengqikj.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://elw.xziqi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oor.fengsongda.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rxn.hywenlv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fju.vqdsnc.cn

[B10] 遍历同时拿索引
来源：http://yab.yangfankeji.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vaa.mhx1999.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tuu.yongpay.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nev.nanxinkj.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dtg.yueranfly.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ddl.xziqi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rtq.iojbl.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gur.jqgfzy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xfg.gaohongyu789.top

[B11] 生成数字序列 / 区间
来源：http://ymd.jinghuilouyu.cn

Py:   list(range(0, 10, 2))
来源：http://kgx.shanyushiyangtech.top

PHP:  range(0, 10, 2);
来源：http://hex.xuanzx.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qbc.shanyushiyangkeji.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fwp.zhaomingkeji.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://whd.fzhhl.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nms.zhaomingkeji.xyz

Ruby: (0...10).step(2).to_a
来源：http://ybo.uphjek.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rhy.redwolf501.top

[B12] 跳出多层循环
来源：http://qmd.zhongyouzk.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://fse.hongshengwenyu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://owq.yuanzhike.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ezy.guowangkeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ywg.dianchejie.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pst.hywenlv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yne.fzhhl.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gjx.havefunace.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hud.tanke756.top

[B13] 判断是否为数字
来源：http://etw.xuetiantiany.cn

Py:   isinstance(x, (int, float))
来源：http://txz.sweek.top

PHP:  is_numeric($x)
来源：http://xjc.ybcxt.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tos.dianchejie.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vnp.zhoulong.xyz

Java: x instanceof Number
来源：http://rsq.jinghuilouyu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bte.xuanzx.com

Ruby: x.is_a?(Numeric)
来源：http://afw.xylfe.cn

C#:   x is int or double or decimal
来源：http://swj.bjfxy.top

[B14] 判断值是否在集合内
来源：http://hkr.ywan-chungtsiang.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://obf.316326.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nii.gogol.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://nbr.fehbvm.com

TS:   [1, 2, 3].includes(x)
来源：http://zyy.9152youxi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bcc.wangdashe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eoi.fehbvm.com

Ruby: [1, 2, 3].include?(x)
来源：http://nps.guowangkeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zgu.shuidangran.top

[B15] 布尔运算与取反
来源：http://tmv.52xcode.cn

Py:   a and b or not c
来源：http://xlv.vehdjk.com

PHP:  $a && $b || !$c
来源：http://qcl.fehbvm.com

JS:   a && b || !c
来源：http://eds.ehwqpu.com

TS:   a && b || !c
来源：http://spp.zdqjudy.top

Java: a && b || !c
来源：http://vso.jlsjyb.cn

Go:   a && b || !c
来源：http://xli.xylfe.cn

Ruby: a && b || !c
来源：http://mxx.birdmap.top

C#:   a && b || !c
来源：http://smu.epnwcf.com

[B16] 卫语句：不满足条件提前返回
来源：http://bkq.tian-w.cn

Py:   if not data: return
来源：http://eor.ivvv.top

PHP:  if (!$data) { return; }
来源：http://mva.xuanzx.com

JS:   if (!data) return;
来源：http://fsp.sweek.top

TS:   if (!data) return;
来源：http://wxg.xuetiantiany.cn

Java: if (data == null) return;
来源：http://zba.xinyue.icu

Go:   if data == nil { return }
来源：http://omx.hysaishi.cn

Ruby: return if data.nil?
来源：http://kdo.gaohongyu789.top

C#:   if (data == null) return;
来源：http://zjr.jinyuanbaomall.cn

================================================================================
来源：http://iui.chenzaomai.com

C. 函数与作用域
来源：http://gyg.fengsongda.top

================================================================================
来源：http://ixe.cucudq.cn

[C01] 定义函数
来源：http://xsl.jlsjyb.cn

Py:   def add(a, b): return a + b
来源：http://qli.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fzr.ydzc1.top

JS:   function add(a, b) { return a + b; }
来源：http://foo.bbcook.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ofi.chenlongwang.top

Java: static int add(int a, int b) { return a + b; }
来源：http://euv.zhaomingkeji.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://cbf.52xcode.cn

Ruby: def add(a, b); a + b; end
来源：http://bwg.bjfxy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fpi.yvedp.cn

[C02] 默认参数
来源：http://oaf.dashuyun.cn

Py:   def greet(name="World"): return name
来源：http://tvj.epnwcf.com

PHP:  function greet($name = "World") { return $name; }
来源：http://hea.9152youxi.cn

JS:   function greet(name = "World") { return name; }
来源：http://nco.iojbl.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cxl.shangyingyoupin.top

Java: // 无默认参数：方法重载或 Optional
来源：http://cry.yueranfly.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uvt.yfazqb.com

Ruby: def greet(name = "World") = name
来源：http://jxa.daxiang520.top

C#:   string Greet(string name = "World") => name;
来源：http://nyh.xuanzx.com

[C03] 可变参数
来源：http://qas.sxryk.cn

Py:   def total(*args): return sum(args)
来源：http://qor.cdnleiting.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gjh.0kj1m.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wmi.yongpay.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xfb.cashguo.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cyz.zhongyouzk.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hfk.0kj1m.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qnw.svipenyu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mxo.iojbl.cn

[C04] 命名参数 / 关键字参数
来源：http://nms.zhixingplan.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xno.svipenyu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dik.cucudq.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pko.zhijiandao.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ymt.jlsjyb.cn

Java: // 无：用 Builder 模式或 record
来源：http://fov.daxiang520.top

Go:   // 无：用配置结构体参数
来源：http://yxe.zhongyouzk.top

Ruby: f(a: 1, b: 2)
来源：http://jrs.xylfe.cn

C#:   f(a: 1, b: 2)
来源：http://yad.yvedp.cn

[C05] 返回多个值
来源：http://wpc.sysykeji.top

Py:   return a, b
来源：http://uvn.ppjwa.cn

PHP:  return [$a, $b];
来源：http://kuv.fzhhl.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://czk.zhiwuduotai.top

TS:   return { a, b };
来源：http://jmc.hongshengwenyu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sxd.meibo888.top

Go:   return a, b
来源：http://rzf.uphjek.com

Ruby: return a, b
来源：http://xyc.vqdsnc.cn

C#:   return (a, b);              // ValueTuple
来源：http://ran.0kj1m.cn

[C06] 匿名函数 / lambda
来源：http://vmy.dianchejie.cn

Py:   square = lambda x: x * x
来源：http://dem.hysaishi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wib.svipenyu.cn

JS:   const square = x => x * x;
来源：http://ubx.havefunace.top

TS:   const square = (x: number): number => x * x;
来源：http://osv.shuidangran.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bzb.nanxinkj.top

Go:   sq := func(x int) int { return x * x }
来源：http://fcs.shanyushiyangtech.top

Ruby: square = ->(x) { x * x }
来源：http://lww.xingfuxueyuan.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://jym.nwbrower.top

[C07] 把函数作为参数传入
来源：http://zld.hongshengwenyu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://eqk.chenzaomai.com

PHP:  array_map("strtoupper", $arr);
来源：http://hkf.hammf.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dgk.ctjpmb.com

TS:   arr.map(String)
来源：http://aqb.aizwys.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://aor.cashguo.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ekn.zhengqikj.top

Ruby: arr.map(&:upcase)
来源：http://lkf.xuanzx.com

C#:   arr.Select(s => s.ToUpper())
来源：http://gky.epnwcf.com

[C08] 闭包
来源：http://fwi.aibaodan.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gwl.meibo888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ldw.hammf.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bxn.xingfuxueyuan.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cwj.ydjk.org.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cob.zhiwuduotai.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bkv.zhaomingkeji.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ndf.0kj1m.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xcs.yj202588.top

[C09] 递归
来源：http://knb.pengpengdd.cyou

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yep.nwbrower.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://alh.zhixingplan.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://eji.uphjek.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qei.xingfuxueyuan.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jwe.tian-w.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fnt.quarkkingdee.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cru.ydzc1.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hww.9152youxi.cn

[C10] 变量作用域
来源：http://ofd.xuetiantiany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lcj.hesvh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sdr.sxryk.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ajs.jinghuilouyu.cn

TS:   同 JS
来源：http://cba.cqqwz.cn

Java: 方法内为块级作用域
来源：http://kwr.daria6918.cn

Go:   花括号块级作用域
来源：http://tpv.xingfuxueyuan.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://obe.jinyuanbaomall.cn

C#:   块级作用域
来源：http://qrj.daxiang520.top

[C11] 模块导入与导出
来源：http://bkt.svipenyu.cn

Py:   from module import func
来源：http://fzy.c1oappe.top

PHP:  require "file.php";  或 use App\Service;
来源：http://hjz.birdmap.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://uhf.hywenlv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fad.yj20258.top

Java: import java.util.List;
来源：http://uxl.zhengqikj.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tpt.iojbl.cn

Ruby: require "json"; require_relative "./util"
来源：http://qca.ybcxt.top

C#:   using System.Text;
来源：http://ics.tianlin.xyz

[C12] 立即执行函数 IIFE
来源：http://dzc.mhx1999.top

Py:   (lambda: print("run"))()
来源：http://jow.chenlongwang.top

PHP:  (function () { echo "run"; })();
来源：http://xgg.aibaodan.cn

JS:   (() => { console.log("run"); })();
来源：http://ern.yj20258.top

TS:   (() => { console.log("run"); })();
来源：http://cgj.yj202588.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sxi.cqqwz.cn

Go:   func() { fmt.Println("run") }()
来源：http://yro.meibo888.top

Ruby: -> { puts "run" }.call
来源：http://xiu.xziqi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kuo.xingfuxueyuan.xyz

[C13] 类型声明 / 类型注解
来源：http://kbj.yj20258888.top


<!-- 参考信息 -->