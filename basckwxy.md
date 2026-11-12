代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://eja.gotoacloud.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rrs.ydjk.org.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://opa.pengpengdd.cyou

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pow.xingfuxueyuan.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fjv.yj20258.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yin.yonumen.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ekf.svipenyu.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://odx.pengpengdd.cyou

[A26] 类型转换总览
来源：http://bwv.svipenyu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://adm.hywenlv.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qav.zhoulong.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ptq.epnwcf.com

TS:   Number() String() Boolean() x as number
来源：http://bjm.xziqi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xqt.svipenyu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://aer.ybcxt.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ngy.cucudq.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ooj.ywan-chungtsiang.top

================================================================================
来源：http://zqz.fanxiaobao.xyz

B. 流程控制
来源：http://zta.epnwcf.com

================================================================================
来源：http://iko.andypj.xyz

[B01] 条件判断 if / else
来源：http://anm.0kj1m.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://skh.wangshuangyany.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://djr.nwbrower.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zqw.zdbjq.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ocw.9152youxi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qvu.pengpengdd.cyou

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://asg.svipenyu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uan.0kj1m.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xks.yueranfly.top

[B02] 多分支 else if / elif
来源：http://btv.hywenlv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ran.yangfankeji.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bfm.shanyushiyangtech.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iek.shuidangran.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qdq.wangshuangyany.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://frx.vqdsnc.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ezg.cucudq.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://and.yj20258.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ofu.ywan-chungtsiang.top

[B03] switch / match / case
来源：http://gqg.xingfuxueyuan.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://egn.aizwys.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nbv.gotoacloud.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vbj.yangfankeji.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zqo.xinyue.icu

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zkd.xuetiantiany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ell.sysykeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rqk.wangdashe.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iem.sysykeji.top

[B04] for 计数循环
来源：http://oss.xinyue.icu

Py:   for i in range(10): print(i)
来源：http://bkg.hesvh.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vdx.dianchejie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ghl.jqgufenzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vyc.bjfxy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xno.feifeiyinyue.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yrk.yfazqb.com

Ruby: 10.times { |i| puts i }
来源：http://azd.yfazqb.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kwv.ctjpmb.com

[B05] 遍历数组 / 列表
来源：http://uuf.jianghu66.top

Py:   for item in arr: print(item)
来源：http://uka.guannengcc.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yrw.kuanghao11.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://snr.yj20258888.top

TS:   for (const item of arr) { console.log(item); }
来源：http://smf.xylfe.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://cwq.yvedp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://iea.hywenlv.cn

Ruby: arr.each { |item| puts item }
来源：http://flx.cashguo.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wop.dashuyun.cn

[B06] 遍历字典 / 对象
来源：http://afu.nanxinkj.top

Py:   for k, v in d.items(): print(k, v)
来源：http://nmu.mhx1999.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pzx.xuanzx.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ood.jianghu66.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bdx.havefunace.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tfj.zhongyouzk.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://guz.redwolf501.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jik.yj202588.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sbu.zdbjq.cn

[B07] while 循环
来源：http://mpz.jinyuanbaomall.cn

Py:   while i < 10: i += 1
来源：http://jyd.quarkkingdee.top

PHP:  while ($i < 10) { $i++; }
来源：http://fja.316326.xyz

JS:   while (i < 10) { i++; }
来源：http://yym.chenlongwang.top

TS:   while (i < 10) { i++; }
来源：http://uxb.iojbl.cn

Java: while (i < 10) { i++; }
来源：http://xgs.chenzaomai.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ekw.yanxiufei.cn

Ruby: while i < 10; i += 1; end
来源：http://era.epnwcf.com

C#:   while (i < 10) { i++; }
来源：http://mcu.9152youxi.cn

[B08] do-while（至少执行一次）
来源：http://rbm.jyoumei.cn

Py:   # 无 do-while：用 while True + break
来源：http://gpp.ydjk.org.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://aoy.yanxiufei.cn

JS:   do { i++; } while (i < 10);
来源：http://saj.redwolf501.top

TS:   do { i++; } while (i < 10);
来源：http://rqe.sweek.top

Java: do { i++; } while (i < 10);
来源：http://edl.jqgufenzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://nhx.cashguo.top

Ruby: begin; i += 1; end while i < 10
来源：http://xqx.tian-w.cn

C#:   do { i++; } while (i < 10);
来源：http://akb.xuanzx.com

[B09] break 与 continue
来源：http://ivp.zycfv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rky.sxryk.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tbl.zhixingplan.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tbl.shanyushiyangtech.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cwx.hesvh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gva.shangyingyoupin.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hal.yfazqb.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://epu.aibaodan.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qcl.zhengqikj.top

[B10] 遍历同时拿索引
来源：http://esi.gogol.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jlp.cqqwz.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ebu.sweek.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://krd.ydjk.org.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lum.yvedp.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xmt.jinqigfzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kvb.zhoulong.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jlt.yueranfly.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xnw.fehbvm.com

[B11] 生成数字序列 / 区间
来源：http://xfm.ctjpmb.com

Py:   list(range(0, 10, 2))
来源：http://dxe.haohaochexian.top

PHP:  range(0, 10, 2);
来源：http://igp.tanke756.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dqf.bjfxy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gwb.yj202588.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ehb.jianghu66.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://psd.hnqzz.top

Ruby: (0...10).step(2).to_a
来源：http://yom.jinghuilouyu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oog.bjfxy.top

[B12] 跳出多层循环
来源：http://wdq.316326.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://cdb.zycfv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://msj.chenzaomai.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mpo.jianghu66.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://kha.daxiang520.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hyo.ydjk.org.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pra.bbcook.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rbw.gzhubu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://iwc.cucudq.cn

[B13] 判断是否为数字
来源：http://ves.quarkkingdee.top

Py:   isinstance(x, (int, float))
来源：http://zta.tarul.cn

PHP:  is_numeric($x)
来源：http://bol.yj202588.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dff.316326.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kee.jinghuilouyu.cn

Java: x instanceof Number
来源：http://tbd.jinqigfzy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cfb.ppjwa.cn

Ruby: x.is_a?(Numeric)
来源：http://ivr.shanyushiyangtech.top

C#:   x is int or double or decimal
来源：http://jyu.andypj.xyz

[B14] 判断值是否在集合内
来源：http://qmg.aizwys.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vbx.aibaodan.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kaa.zdqjudy.top

JS:   [1, 2, 3].includes(x)
来源：http://bal.xuanzx.com

TS:   [1, 2, 3].includes(x)
来源：http://mpr.chenzaomai.com

Java: List.of(1, 2, 3).contains(x)
来源：http://txo.guannengcc.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rlv.sxryk.cn

Ruby: [1, 2, 3].include?(x)
来源：http://lzf.redwolf501.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cwl.hongshengwenyu.top

[B15] 布尔运算与取反
来源：http://aeg.shzxlz.cn

Py:   a and b or not c
来源：http://nfn.quarkkingdee.top

PHP:  $a && $b || !$c
来源：http://fvu.zhijiandao.cn

JS:   a && b || !c
来源：http://ugk.zhixingplan.top

TS:   a && b || !c
来源：http://slx.fehbvm.com

Java: a && b || !c
来源：http://dyh.sufxvd.cn

Go:   a && b || !c
来源：http://obf.mhx1999.top

Ruby: a && b || !c
来源：http://xli.haohaochexian.top

C#:   a && b || !c
来源：http://bef.tanke756.top

[B16] 卫语句：不满足条件提前返回
来源：http://wim.xziqi.cn

Py:   if not data: return
来源：http://xki.quarkkingdee.top

PHP:  if (!$data) { return; }
来源：http://bpg.yonumen.top

JS:   if (!data) return;
来源：http://xtb.dianchejie.cn

TS:   if (!data) return;
来源：http://yhk.zhoulong.xyz

Java: if (data == null) return;
来源：http://lju.ppjwa.cn

Go:   if data == nil { return }
来源：http://vjf.xuetiantiany.cn

Ruby: return if data.nil?
来源：http://lio.jqgfzy.top

C#:   if (data == null) return;
来源：http://dit.vqdsnc.cn

================================================================================
来源：http://vfk.yj202588.top

C. 函数与作用域
来源：http://reh.zhoulong.xyz

================================================================================
来源：http://pdy.feifeiyinyue.top

[C01] 定义函数
来源：http://sfr.jiagoushi.top

Py:   def add(a, b): return a + b
来源：http://myb.bbcook.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nxw.hesvh.cn

JS:   function add(a, b) { return a + b; }
来源：http://hap.zhixingplan.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tmu.zycfv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mbb.gzhubu.top

Go:   func add(a, b int) int { return a + b }
来源：http://ilx.chenlongwang.top

Ruby: def add(a, b); a + b; end
来源：http://cme.tian-w.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jhb.zhengqikj.top

[C02] 默认参数
来源：http://cpd.hesvh.cn

Py:   def greet(name="World"): return name
来源：http://rfv.jyoumei.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qmp.quarkkingdee.top

JS:   function greet(name = "World") { return name; }
来源：http://mnd.cdnleiting.top

TS:   function greet(name: string = "World") { return name; }
来源：http://kgh.vehdjk.com

Java: // 无默认参数：方法重载或 Optional
来源：http://zku.yuanzhike.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fea.feifeiyinyue.top

Ruby: def greet(name = "World") = name
来源：http://gmc.zdqjudy.top

C#:   string Greet(string name = "World") => name;
来源：http://bxt.sjlbkw.cn

[C03] 可变参数
来源：http://tbh.aibaodan.cn

Py:   def total(*args): return sum(args)
来源：http://gyt.c1oappe.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kmb.jinyuanbaomall.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bgd.quarkkingdee.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iof.sufxvd.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://swl.haohaochexian.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://axb.vqdsnc.cn

Ruby: def total(*nums); nums.sum; end
来源：http://uti.zhengqikj.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kxu.gotoacloud.top

[C04] 命名参数 / 关键字参数
来源：http://sro.nwbrower.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://oha.gaohongyu789.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kbc.yuanzhike.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kpl.tanke756.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nfe.c1oappe.top

Java: // 无：用 Builder 模式或 record
来源：http://zxa.xuanzx.com

Go:   // 无：用配置结构体参数
来源：http://hcf.jqgufenzy.top

Ruby: f(a: 1, b: 2)
来源：http://mcc.hysaishi.cn

C#:   f(a: 1, b: 2)
来源：http://ovc.gogol.net.cn

[C05] 返回多个值
来源：http://zpv.hesvh.cn

Py:   return a, b
来源：http://pjc.epnwcf.com

PHP:  return [$a, $b];
来源：http://ukv.nwbrower.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://gzj.ppjwa.cn

TS:   return { a, b };
来源：http://dhy.smart0.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cue.yvedp.cn

Go:   return a, b
来源：http://atw.cdnleiting.top

Ruby: return a, b
来源：http://wzi.ywan-chungtsiang.top

C#:   return (a, b);              // ValueTuple
来源：http://krz.xuanzx.com

[C06] 匿名函数 / lambda
来源：http://xsr.yuxming.cn

Py:   square = lambda x: x * x
来源：http://rse.birdmap.top

PHP:  $square = fn($x) => $x * $x;
来源：http://sec.shuidangran.top

JS:   const square = x => x * x;
来源：http://exs.mhx1999.top

TS:   const square = (x: number): number => x * x;
来源：http://zcn.dashuyun.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hzu.52xcode.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dtp.gogol.net.cn

Ruby: square = ->(x) { x * x }
来源：http://rlo.jinyuanbaomall.cn

C#:   Func<int, int> square = x => x * x;
来源：http://eaj.wangshuangyany.cn

[C07] 把函数作为参数传入
来源：http://zsm.chenzaomai.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bxz.sufxvd.cn

PHP:  array_map("strtoupper", $arr);
来源：http://diy.zhiwuduotai.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://aqa.yuxming.cn

TS:   arr.map(String)
来源：http://eee.jlsjyb.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vwn.sysykeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://isr.cqqwz.cn

Ruby: arr.map(&:upcase)
来源：http://emw.redwolf501.top

C#:   arr.Select(s => s.ToUpper())
来源：http://kms.ctjpmb.com

[C08] 闭包
来源：http://ckk.jyoumei.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ugl.52xcode.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dkl.zycfv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wnu.vehdjk.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://udw.chenlongwang.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uib.pycfn.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xho.fzhhl.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qkn.wangdashe.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mnj.9152youxi.cn

[C09] 递归
来源：http://xkq.hywenlv.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bfo.ehwqpu.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dpy.yj20258888.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xwu.wangshuangyany.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fcf.xinyue.icu

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://guo.jqgfzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wst.jinyuanbaomall.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://azy.ybcxt.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lbq.ydzc1.top

[C10] 变量作用域
来源：http://tag.jqgufenzy.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qis.guannengcc.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://cpx.zdbjq.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dne.sufxvd.cn

TS:   同 JS
来源：http://pmj.smart0.xyz

Java: 方法内为块级作用域
来源：http://fct.0kj1m.cn

Go:   花括号块级作用域
来源：http://oos.uphjek.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pzh.tianlin.xyz

C#:   块级作用域
来源：http://jjn.epnwcf.com

[C11] 模块导入与导出
来源：http://tag.yuanzhike.top

Py:   from module import func
来源：http://stk.ydjk.org.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uhe.xuanzx.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://igx.cqqwz.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hin.snrcjt.cn

Java: import java.util.List;
来源：http://aze.ywan-chungtsiang.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iru.quarkkingdee.top

Ruby: require "json"; require_relative "./util"
来源：http://mek.shzxlz.cn

C#:   using System.Text;
来源：http://okz.jinqigfzy.top

[C12] 立即执行函数 IIFE
来源：http://hja.snrcjt.cn

Py:   (lambda: print("run"))()
来源：http://xfi.gzhubu.top

PHP:  (function () { echo "run"; })();
来源：http://wmi.zdqjudy.top

JS:   (() => { console.log("run"); })();
来源：http://kgs.sufxvd.cn

TS:   (() => { console.log("run"); })();
来源：http://ihj.nanxinkj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gjh.jinqigufen.top

Go:   func() { fmt.Println("run") }()
来源：http://qxm.jinyuanbaomall.cn

Ruby: -> { puts "run" }.call
来源：http://nuu.316326.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://fyd.52xcode.cn

[C13] 类型声明 / 类型注解
来源：http://xpc.sjlbkw.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://odc.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vll.mhx1999.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rtx.hammf.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zxk.xziqi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://sqs.yj20258.top

Go:   func add(a, b int) int
来源：http://kab.xuetiantiany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kcq.hesvh.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qsg.yueranfly.top

[C14] 泛型函数
来源：http://rmn.yuanzhike.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xxs.hcnkem.com

PHP:  // 无泛型
来源：http://uva.shuidangran.top

JS:   // 无泛型
来源：http://orc.aizwys.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kbr.epnwcf.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ihx.wangshuangyany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ujv.zhengqikj.top

Ruby: # 无泛型
来源：http://fky.xinyue.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hci.zycfv.cn

[C15] 解构 / 展开参数
来源：http://fmc.bbcook.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gtp.havefunace.top

PHP:  [$a, $b] = $pair;
来源：http://kgx.tianlin.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wyt.cdnleiting.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bze.sysykeji.top

Java: // 无解构
来源：http://qel.gogol.net.cn

Go:   // 无解构
来源：http://hml.fzhhl.top


<!-- 参考信息 -->