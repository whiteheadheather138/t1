代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ydc.shanyushiyangkeji.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rri.shanyushiyangkeji.top

Ruby: s1 == s2; s1 <=> s2
来源：http://nws.chenjidiqi.icu

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ukr.daria6918.cn

[A26] 类型转换总览
来源：http://bgp.zhoulong.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mmb.zycfv.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ron.redwolf501.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://awe.zhengqikj.top

TS:   Number() String() Boolean() x as number
来源：http://qlq.fanxiaobao.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://cbs.birdmap.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://tdj.gaohongyu789.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://dlx.fanxiaobao.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pch.xuanzx.com

================================================================================
来源：http://slf.ywan-chungtsiang.top

B. 流程控制
来源：http://kjc.wangdashe.top

================================================================================
来源：http://rzc.tanke756.top

[B01] 条件判断 if / else
来源：http://raz.nwbrower.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ped.kuanghao11.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dpr.svipenyu.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bss.havefunace.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sfs.ydjk.org.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://ywn.hongshengwenyu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xls.ybcxt.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://prb.kuanghao11.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mnb.ydzc1.top

[B02] 多分支 else if / elif
来源：http://dgb.yj202588.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gfh.jlsjyb.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tuk.wangdashe.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://byp.shanyushiyangtech.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://liw.yj20258.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bfe.zhoulong.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fff.hammf.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pzp.pycfn.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ppe.jqgufenzy.top

[B03] switch / match / case
来源：http://nrd.hysaishi.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://opk.yongpay.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ppc.nwbrower.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jtv.gotoacloud.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://smk.meibo888.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wfa.ppjwa.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bio.pengpengdd.cyou

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qwj.sysykeji.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sdc.jinghuilouyu.cn

[B04] for 计数循环
来源：http://eta.yj20258888.top

Py:   for i in range(10): print(i)
来源：http://pwk.aibaodan.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ybt.shangyingyoupin.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iiv.jinqigufen.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mtk.yuxming.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qeg.snrcjt.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://glq.52xcode.cn

Ruby: 10.times { |i| puts i }
来源：http://kcl.birdmap.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ciy.ywan-chungtsiang.top

[B05] 遍历数组 / 列表
来源：http://nfc.yj202588.top

Py:   for item in arr: print(item)
来源：http://eoc.zycfv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://abj.jianghu66.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hhh.hcnkem.com

TS:   for (const item of arr) { console.log(item); }
来源：http://lms.dianchejie.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mdk.c1oappe.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://nev.meibo888.top

Ruby: arr.each { |item| puts item }
来源：http://xyr.52xcode.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bqt.gaohongyu789.top

[B06] 遍历字典 / 对象
来源：http://nut.hongshengwenyu.top

Py:   for k, v in d.items(): print(k, v)
来源：http://goy.svipenyu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lbe.zhongyouzk.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vjx.yangfankeji.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hbs.smart0.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oge.hfpthk.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kcj.smart0.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wmg.zhengqikj.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wru.ybcxt.top

[B07] while 循环
来源：http://guo.aibaodan.cn

Py:   while i < 10: i += 1
来源：http://xkt.shzxlz.cn

PHP:  while ($i < 10) { $i++; }
来源：http://iav.yj20258888.top

JS:   while (i < 10) { i++; }
来源：http://wye.xylfe.cn

TS:   while (i < 10) { i++; }
来源：http://qsx.9152youxi.cn

Java: while (i < 10) { i++; }
来源：http://ufi.ydjk.org.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dft.c1oappe.top

Ruby: while i < 10; i += 1; end
来源：http://uer.hesvh.cn

C#:   while (i < 10) { i++; }
来源：http://cqy.hcnkem.com

[B08] do-while（至少执行一次）
来源：http://biw.zycfv.cn

Py:   # 无 do-while：用 while True + break
来源：http://ojx.zhongyouzk.top

PHP:  do { $i++; } while ($i < 10);
来源：http://gxx.shzxlz.cn

JS:   do { i++; } while (i < 10);
来源：http://ilr.fktsv.cn

TS:   do { i++; } while (i < 10);
来源：http://mgs.cucudq.cn

Java: do { i++; } while (i < 10);
来源：http://wiu.jiagoushi.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hgc.jqgfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://pwu.iojbl.cn

C#:   do { i++; } while (i < 10);
来源：http://lic.snrcjt.cn

[B09] break 与 continue
来源：http://sng.hnqzz.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lqj.bjfxy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jqf.aibaodan.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fwh.dianchejie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ehs.wangshuangyany.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kou.smart0.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://idu.nanxuanxn.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zlh.yuxming.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qaj.ppjwa.cn

[B10] 遍历同时拿索引
来源：http://ead.ybcxt.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://azg.yangfankeji.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jzg.cashguo.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lhi.sxryk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oic.guannengcc.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xjf.sufxvd.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hze.ydjk.org.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://obm.52xcode.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qbx.ybcxt.top

[B11] 生成数字序列 / 区间
来源：http://zmp.uphjek.com

Py:   list(range(0, 10, 2))
来源：http://eet.zhengqikj.top

PHP:  range(0, 10, 2);
来源：http://tyg.chenzaomai.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uhr.sysykeji.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mqt.yuanzhike.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uvv.jinghuilouyu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yap.wangshuangyany.cn

Ruby: (0...10).step(2).to_a
来源：http://mod.andypj.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jdp.yuxming.cn

[B12] 跳出多层循环
来源：http://xdi.tanke756.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://wlj.tarul.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nry.yanxiufei.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uel.zhiwuduotai.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hkm.quarkkingdee.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uip.yongpay.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tyx.shanyushiyangtech.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uib.guowangkeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mrk.shanyushiyangkeji.top

[B13] 判断是否为数字
来源：http://xqd.dianchejie.cn

Py:   isinstance(x, (int, float))
来源：http://zau.jinqigfzy.top

PHP:  is_numeric($x)
来源：http://avd.yj202588.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ykq.yj202588.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iyg.hfpthk.cn

Java: x instanceof Number
来源：http://bmx.hysaishi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fwg.tarul.cn

Ruby: x.is_a?(Numeric)
来源：http://rvg.mhx1999.top

C#:   x is int or double or decimal
来源：http://zhh.gaohongyu789.top

[B14] 判断值是否在集合内
来源：http://dko.shanyushiyangtech.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ytk.gotoacloud.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oyb.yanxiufei.cn

JS:   [1, 2, 3].includes(x)
来源：http://ecc.jqgufenzy.top

TS:   [1, 2, 3].includes(x)
来源：http://rvo.xziqi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://tmn.xuanzx.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kjo.chenlongwang.top

Ruby: [1, 2, 3].include?(x)
来源：http://foe.birdmap.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uyk.316326.xyz

[B15] 布尔运算与取反
来源：http://ipv.guowangkeji.top

Py:   a and b or not c
来源：http://tqf.ctjpmb.com

PHP:  $a && $b || !$c
来源：http://eov.fanxiaobao.xyz

JS:   a && b || !c
来源：http://ufq.cucudq.cn

TS:   a && b || !c
来源：http://kig.ybcxt.top

Java: a && b || !c
来源：http://roa.andypj.xyz

Go:   a && b || !c
来源：http://exw.feifeiyinyue.top

Ruby: a && b || !c
来源：http://puq.zycfv.cn

C#:   a && b || !c
来源：http://cvd.jianghu66.top

[B16] 卫语句：不满足条件提前返回
来源：http://wjc.yuxming.cn

Py:   if not data: return
来源：http://kbt.hammf.cn

PHP:  if (!$data) { return; }
来源：http://gts.316326.xyz

JS:   if (!data) return;
来源：http://rvr.hcnkem.com

TS:   if (!data) return;
来源：http://gir.aibaodan.cn

Java: if (data == null) return;
来源：http://vmg.dianchejie.cn

Go:   if data == nil { return }
来源：http://rke.cqqwz.cn

Ruby: return if data.nil?
来源：http://dir.sxryk.cn

C#:   if (data == null) return;
来源：http://fen.52xcode.cn

================================================================================
来源：http://sft.svipenyu.cn

C. 函数与作用域
来源：http://byf.xuanzx.com

================================================================================
来源：http://rwo.smart0.xyz

[C01] 定义函数
来源：http://rpa.nwbrower.top

Py:   def add(a, b): return a + b
来源：http://cgs.chenzaomai.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://awy.cashguo.top

JS:   function add(a, b) { return a + b; }
来源：http://bsc.cqqwz.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vad.cheryme.top

Java: static int add(int a, int b) { return a + b; }
来源：http://yyj.hfpthk.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yox.shangyingyoupin.top

Ruby: def add(a, b); a + b; end
来源：http://lkq.hysaishi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sav.epnwcf.com

[C02] 默认参数
来源：http://nqy.bbcook.cn

Py:   def greet(name="World"): return name
来源：http://spk.shangyingyoupin.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xvr.9152youxi.cn

JS:   function greet(name = "World") { return name; }
来源：http://ycd.ctjpmb.com

TS:   function greet(name: string = "World") { return name; }
来源：http://uap.gzhubu.top

Java: // 无默认参数：方法重载或 Optional
来源：http://dka.zhixingplan.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://czp.jinyuanbaomall.cn

Ruby: def greet(name = "World") = name
来源：http://ydm.andypj.xyz

C#:   string Greet(string name = "World") => name;
来源：http://dtd.dashuyun.cn

[C03] 可变参数
来源：http://uap.feifeiyinyue.top

Py:   def total(*args): return sum(args)
来源：http://qdt.epnwcf.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://itu.yonumen.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qrh.havefunace.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fbj.hesvh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gpv.shzxlz.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qqm.yuxming.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xqo.jqgfzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ich.vqdsnc.cn

[C04] 命名参数 / 关键字参数
来源：http://zoc.zhixingplan.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rrx.nwbrower.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zne.ctjpmb.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fkl.cqqwz.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yri.fengsongda.top

Java: // 无：用 Builder 模式或 record
来源：http://vjo.hesvh.cn

Go:   // 无：用配置结构体参数
来源：http://xaz.snrcjt.cn

Ruby: f(a: 1, b: 2)
来源：http://ciz.vehdjk.com

C#:   f(a: 1, b: 2)
来源：http://vgl.sjlbkw.cn

[C05] 返回多个值
来源：http://pxe.shangyingyoupin.top

Py:   return a, b
来源：http://fvw.c1oappe.top

PHP:  return [$a, $b];
来源：http://com.ehwqpu.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://tyn.fehbvm.com

TS:   return { a, b };
来源：http://gqq.sweek.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lkn.shuidangran.top

Go:   return a, b
来源：http://jrp.ehwqpu.com

Ruby: return a, b
来源：http://wim.haohaochexian.top

C#:   return (a, b);              // ValueTuple
来源：http://ntj.snrcjt.cn

[C06] 匿名函数 / lambda
来源：http://idu.quarkkingdee.top

Py:   square = lambda x: x * x
来源：http://mpe.guannengcc.top

PHP:  $square = fn($x) => $x * $x;
来源：http://zdz.yongpay.top

JS:   const square = x => x * x;
来源：http://adc.aizwys.cn

TS:   const square = (x: number): number => x * x;
来源：http://mad.zhoulong.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cco.yfazqb.com

Go:   sq := func(x int) int { return x * x }
来源：http://qpk.smart0.xyz

Ruby: square = ->(x) { x * x }
来源：http://rtr.yvedp.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hhi.sjlbkw.cn

[C07] 把函数作为参数传入
来源：http://lkb.ivvv.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hqy.sysykeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://cdt.zdqjudy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fvh.wangshuangyany.cn

TS:   arr.map(String)
来源：http://kiq.sweek.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qsh.nanxuanxn.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ysy.andypj.xyz

Ruby: arr.map(&:upcase)
来源：http://nmh.xziqi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mbe.bbcook.cn

[C08] 闭包
来源：http://kjx.zycfv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dnw.kuanghao11.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://anb.uphjek.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lsb.daxiang520.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ddh.haohaochexian.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ptj.yuxming.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sle.zdqjudy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xsr.yj20258.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://aqk.chenzaomai.com

[C09] 递归
来源：http://xrm.aibaodan.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hwe.0kj1m.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hgk.yj202588.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sbd.nwbrower.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rxk.quarkkingdee.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://isi.yj202588.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nrr.zdbjq.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vac.dianchejie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lvd.redwolf501.top

[C10] 变量作用域
来源：http://hoz.ybcxt.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://crm.yj20258.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fyg.zhixingplan.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qvl.zhoulong.xyz

TS:   同 JS
来源：http://rcp.fktsv.cn

Java: 方法内为块级作用域
来源：http://pvk.sweek.top

Go:   花括号块级作用域
来源：http://nlt.zhiwuduotai.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ykk.wangshuangyany.cn

C#:   块级作用域
来源：http://efu.fanxiaobao.xyz

[C11] 模块导入与导出
来源：http://idn.shanyushiyangtech.top

Py:   from module import func
来源：http://rie.andypj.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://eng.hywenlv.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://srk.tian-w.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://abt.yongpay.top

Java: import java.util.List;
来源：http://cql.redwolf501.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pqg.redwolf501.top

Ruby: require "json"; require_relative "./util"
来源：http://jcq.zdqjudy.top

C#:   using System.Text;
来源：http://kxp.nwbrower.top

[C12] 立即执行函数 IIFE
来源：http://bld.sysykeji.top

Py:   (lambda: print("run"))()
来源：http://jfr.ppjwa.cn

PHP:  (function () { echo "run"; })();
来源：http://rto.jinqigfzy.top

JS:   (() => { console.log("run"); })();
来源：http://lzl.hongshengwenyu.top

TS:   (() => { console.log("run"); })();
来源：http://cwg.yanxiufei.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://brv.sweek.top

Go:   func() { fmt.Println("run") }()
来源：http://lnx.havefunace.top

Ruby: -> { puts "run" }.call
来源：http://jcu.yuanzhike.top

C#:   // 无 IIFE：用静态构造函数
来源：http://eko.havefunace.top

[C13] 类型声明 / 类型注解
来源：http://ldq.bjfxy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ccq.wangdashe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xba.zhiwuduotai.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ruc.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://udb.hnxiangtu.top

Java: int add(int a, int b) { return a + b; }
来源：http://keb.quarkkingdee.top

Go:   func add(a, b int) int
来源：http://fvs.cdnleiting.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xot.ctjpmb.com

C#:   int Add(int a, int b) => a + b;
来源：http://izv.guannengcc.top

[C14] 泛型函数
来源：http://okp.jlsjyb.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gle.yanxiufei.cn

PHP:  // 无泛型
来源：http://spt.yuanzhike.top

JS:   // 无泛型
来源：http://wta.cucudq.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gem.nanxinkj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sds.yuxming.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://egm.hysaishi.cn

Ruby: # 无泛型
来源：http://yko.yvedp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cqw.zhaomingkeji.xyz

[C15] 解构 / 展开参数
来源：http://irf.meibo888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ojc.shanyushiyangtech.top

PHP:  [$a, $b] = $pair;
来源：http://whb.yueranfly.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zyi.wangdashe.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qyt.hywenlv.cn

Java: // 无解构
来源：http://wxk.sysykeji.top

Go:   // 无解构
来源：http://rco.gotoacloud.top

Ruby: a, b = pair
来源：http://wpv.zhongyouzk.top

C#:   var (a, b) = pair;
来源：http://qau.sysykeji.top

[C16] 函数 / 方法重载
来源：http://hle.zhengqikj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pci.yj20258.top


<!-- 参考信息 -->