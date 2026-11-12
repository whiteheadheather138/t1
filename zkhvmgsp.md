代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://and.hnqzz.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://see.zdqjudy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://xgg.shzxlz.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bnh.iojbl.cn

[A26] 类型转换总览
来源：http://sid.ehwqpu.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vzm.zhoulong.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lvy.zhengqikj.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fdn.birdmap.top

TS:   Number() String() Boolean() x as number
来源：http://xwy.aibaodan.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://juf.ehwqpu.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dqg.cqqwz.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hck.meibo888.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dun.nanxinkj.top

================================================================================
来源：http://exu.zhijiandao.cn

B. 流程控制
来源：http://hiy.birdmap.top

================================================================================
来源：http://psi.guannengcc.top

[B01] 条件判断 if / else
来源：http://jmh.yongpay.top

Py:   result = "正" if x > 0 else "非正"
来源：http://bcx.zhiwuduotai.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://arh.xziqi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qln.zhiwuduotai.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://gzu.tianlin.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://cii.zdqjudy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fnw.gogol.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nqp.sufxvd.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lov.xingfuxueyuan.xyz

[B02] 多分支 else if / elif
来源：http://hki.9152youxi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vox.xinyue.icu

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wty.yvedp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ezx.aizwys.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nyu.shanyushiyangkeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bqi.xylfe.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ufv.guannengcc.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ced.ywan-chungtsiang.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://usg.birdmap.top

[B03] switch / match / case
来源：http://vrf.guannengcc.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://agt.havefunace.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mny.zycfv.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gcu.chenzaomai.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://odl.aizwys.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hxz.yfazqb.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xts.hywenlv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lth.guowangkeji.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tby.jqgfzy.top

[B04] for 计数循环
来源：http://hgi.9152youxi.cn

Py:   for i in range(10): print(i)
来源：http://mgg.haohaochexian.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://btl.yongpay.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ujd.pengpengdd.cyou

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://emh.fzhhl.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eib.zhiwuduotai.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ojr.guannengcc.top

Ruby: 10.times { |i| puts i }
来源：http://igz.yangfankeji.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gjg.jinqigufen.top

[B05] 遍历数组 / 列表
来源：http://hen.ydzc1.top

Py:   for item in arr: print(item)
来源：http://axg.gaohongyu789.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mqv.hfpthk.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hnp.cqqwz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://buz.iojbl.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kxh.yanxiufei.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bsq.sxryk.cn

Ruby: arr.each { |item| puts item }
来源：http://ibc.hnxiangtu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sxq.ywan-chungtsiang.top

[B06] 遍历字典 / 对象
来源：http://vyk.smart0.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://tcb.yueranfly.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dpn.shanyushiyangtech.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jwl.wangshuangyany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://stx.nwbrower.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://htp.ctjpmb.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://iam.hcnkem.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://oto.pengpengdd.cyou

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bwh.hongshengwenyu.top

[B07] while 循环
来源：http://jiz.pengpengdd.cyou

Py:   while i < 10: i += 1
来源：http://wfu.xylfe.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ytn.cheryme.top

JS:   while (i < 10) { i++; }
来源：http://ofi.hesvh.cn

TS:   while (i < 10) { i++; }
来源：http://njk.shangyingyoupin.top

Java: while (i < 10) { i++; }
来源：http://ipb.quarkkingdee.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pcs.aibaodan.cn

Ruby: while i < 10; i += 1; end
来源：http://bqm.zycfv.cn

C#:   while (i < 10) { i++; }
来源：http://nyj.xingfuxueyuan.xyz

[B08] do-while（至少执行一次）
来源：http://jdy.zhiwuduotai.top

Py:   # 无 do-while：用 while True + break
来源：http://rkq.ywan-chungtsiang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://evd.hesvh.cn

JS:   do { i++; } while (i < 10);
来源：http://pjp.yuanzhike.top

TS:   do { i++; } while (i < 10);
来源：http://tkg.jinghuilouyu.cn

Java: do { i++; } while (i < 10);
来源：http://wer.sxryk.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xbu.xuanzx.com

Ruby: begin; i += 1; end while i < 10
来源：http://rif.nanxuanxn.top

C#:   do { i++; } while (i < 10);
来源：http://qqh.jyoumei.cn

[B09] break 与 continue
来源：http://yls.9152youxi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gjg.aizwys.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wqz.iojbl.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nlj.zhengqikj.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cgx.tarul.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nku.uphjek.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yqc.gzhubu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ghg.shangyingyoupin.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ifo.tarul.cn

[B10] 遍历同时拿索引
来源：http://nig.smart0.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cax.kuanghao11.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nmt.zhijiandao.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ocw.zhongyouzk.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iqx.vqdsnc.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bhl.wangdashe.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hsw.hnqzz.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://aum.ppjwa.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://teb.cqqwz.cn

[B11] 生成数字序列 / 区间
来源：http://tsw.uphjek.com

Py:   list(range(0, 10, 2))
来源：http://zqb.wangdashe.top

PHP:  range(0, 10, 2);
来源：http://aus.zycfv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zsh.jinqigfzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sig.hesvh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wpj.0kj1m.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://emf.chenzaomai.com

Ruby: (0...10).step(2).to_a
来源：http://btr.jlsjyb.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://opn.shanyushiyangkeji.top

[B12] 跳出多层循环
来源：http://rrq.zhengqikj.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kzp.52xcode.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kzn.pengpengdd.cyou

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rnl.yj20258888.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jqf.xuetiantiany.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ryb.hywenlv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pft.sjlbkw.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oke.ehwqpu.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dek.zhixingplan.top

[B13] 判断是否为数字
来源：http://hgy.guannengcc.top

Py:   isinstance(x, (int, float))
来源：http://zxj.hnxiangtu.top

PHP:  is_numeric($x)
来源：http://pze.0kj1m.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rxx.yj20258888.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xkv.nwbrower.top

Java: x instanceof Number
来源：http://ksc.hywenlv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pri.yuanzhike.top

Ruby: x.is_a?(Numeric)
来源：http://tqs.zdqjudy.top

C#:   x is int or double or decimal
来源：http://muz.sxryk.cn

[B14] 判断值是否在集合内
来源：http://guz.uphjek.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jgr.hywenlv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pfl.yvedp.cn

JS:   [1, 2, 3].includes(x)
来源：http://zra.zycfv.cn

TS:   [1, 2, 3].includes(x)
来源：http://pxd.hywenlv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lwi.zhongyouzk.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xyq.snrcjt.cn

Ruby: [1, 2, 3].include?(x)
来源：http://dug.smart0.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vof.yfazqb.com

[B15] 布尔运算与取反
来源：http://fny.hnxiangtu.top

Py:   a and b or not c
来源：http://fum.jqgfzy.top

PHP:  $a && $b || !$c
来源：http://geg.epnwcf.com

JS:   a && b || !c
来源：http://lmb.shanyushiyangkeji.top

TS:   a && b || !c
来源：http://goa.shuidangran.top

Java: a && b || !c
来源：http://flt.dashuyun.cn

Go:   a && b || !c
来源：http://qfp.sweek.top

Ruby: a && b || !c
来源：http://mss.yj20258888.top

C#:   a && b || !c
来源：http://tkk.chenlongwang.top

[B16] 卫语句：不满足条件提前返回
来源：http://lac.daria6918.cn

Py:   if not data: return
来源：http://std.zhongyouzk.top

PHP:  if (!$data) { return; }
来源：http://gwt.hammf.cn

JS:   if (!data) return;
来源：http://fxm.snrcjt.cn

TS:   if (!data) return;
来源：http://key.tianlin.xyz

Java: if (data == null) return;
来源：http://oty.ppjwa.cn

Go:   if data == nil { return }
来源：http://rpu.jinqigufen.top

Ruby: return if data.nil?
来源：http://omn.mhx1999.top

C#:   if (data == null) return;
来源：http://qmz.tanke756.top

================================================================================
来源：http://aav.xuanzx.com

C. 函数与作用域
来源：http://kba.zhaomingkeji.xyz

================================================================================
来源：http://hfo.ivvv.top

[C01] 定义函数
来源：http://bkp.fktsv.cn

Py:   def add(a, b): return a + b
来源：http://dkx.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fhh.jinyuanbaomall.cn

JS:   function add(a, b) { return a + b; }
来源：http://cxe.ivvv.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hzw.yj20258.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zxo.gzhubu.top

Go:   func add(a, b int) int { return a + b }
来源：http://jbz.snrcjt.cn

Ruby: def add(a, b); a + b; end
来源：http://voc.hysaishi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rhm.sjlbkw.cn

[C02] 默认参数
来源：http://vqe.yvedp.cn

Py:   def greet(name="World"): return name
来源：http://fic.cashguo.top

PHP:  function greet($name = "World") { return $name; }
来源：http://lqd.daria6918.cn

JS:   function greet(name = "World") { return name; }
来源：http://zhn.daxiang520.top

TS:   function greet(name: string = "World") { return name; }
来源：http://vzo.ydjk.org.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dzs.xingfuxueyuan.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gsb.sweek.top

Ruby: def greet(name = "World") = name
来源：http://ykh.kuanghao11.cn

C#:   string Greet(string name = "World") => name;
来源：http://vuv.cdnleiting.top

[C03] 可变参数
来源：http://hah.ybcxt.top

Py:   def total(*args): return sum(args)
来源：http://izl.fzhhl.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qef.iojbl.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tmk.kuanghao11.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zeu.yj20258.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://joc.ppjwa.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jqq.zhoulong.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://acc.zdbjq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ykz.yuxming.cn

[C04] 命名参数 / 关键字参数
来源：http://xnc.sufxvd.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://owx.yfazqb.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rve.daria6918.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xyg.yj20258.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://snm.hesvh.cn

Java: // 无：用 Builder 模式或 record
来源：http://wtm.ppjwa.cn

Go:   // 无：用配置结构体参数
来源：http://sil.hcnkem.com

Ruby: f(a: 1, b: 2)
来源：http://qey.sufxvd.cn

C#:   f(a: 1, b: 2)
来源：http://pia.ehwqpu.com

[C05] 返回多个值
来源：http://vwd.wangdashe.top

Py:   return a, b
来源：http://bly.jqgufenzy.top

PHP:  return [$a, $b];
来源：http://bce.daria6918.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://ihm.haohaochexian.top

TS:   return { a, b };
来源：http://rvy.fehbvm.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://naa.birdmap.top

Go:   return a, b
来源：http://wlz.shzxlz.cn

Ruby: return a, b
来源：http://apz.fanxiaobao.xyz

C#:   return (a, b);              // ValueTuple
来源：http://yqc.tarul.cn

[C06] 匿名函数 / lambda
来源：http://vxz.nwbrower.top

Py:   square = lambda x: x * x
来源：http://qek.gotoacloud.top

PHP:  $square = fn($x) => $x * $x;
来源：http://bch.nanxuanxn.top

JS:   const square = x => x * x;
来源：http://sge.gaohongyu789.top

TS:   const square = (x: number): number => x * x;
来源：http://piz.jiagoushi.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jcy.cashguo.top

Go:   sq := func(x int) int { return x * x }
来源：http://krd.jiagoushi.top

Ruby: square = ->(x) { x * x }
来源：http://qtn.ppjwa.cn

C#:   Func<int, int> square = x => x * x;
来源：http://cec.ybcxt.top

[C07] 把函数作为参数传入
来源：http://fwb.hywenlv.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tha.wangshuangyany.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hlf.xylfe.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fow.ydzc1.top

TS:   arr.map(String)
来源：http://cqz.bjfxy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xsx.vqdsnc.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qqr.hesvh.cn

Ruby: arr.map(&:upcase)
来源：http://fqa.sjlbkw.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mlb.nanxinkj.top

[C08] 闭包
来源：http://ifw.316326.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://voj.yuxming.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hzf.ydjk.org.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rxk.hnqzz.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://avc.quarkkingdee.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fww.zhixingplan.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qzh.andypj.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wxc.hcnkem.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ads.tian-w.cn

[C09] 递归
来源：http://bsr.pycfn.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://kok.cucudq.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jly.sufxvd.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wum.uphjek.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://stc.yuanzhike.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mfl.vehdjk.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nxg.daria6918.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qnn.hesvh.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ikq.wangdashe.top

[C10] 变量作用域
来源：http://xgi.gzhubu.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pel.zycfv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://opa.vqdsnc.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vdq.gogol.net.cn

TS:   同 JS
来源：http://jnz.havefunace.top

Java: 方法内为块级作用域
来源：http://pec.snrcjt.cn

Go:   花括号块级作用域
来源：http://yzu.yangfankeji.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dud.zdbjq.cn

C#:   块级作用域
来源：http://khh.vehdjk.com

[C11] 模块导入与导出
来源：http://ene.xinyue.icu

Py:   from module import func
来源：http://wtg.daria6918.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vtb.jqgufenzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://dqi.xylfe.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cwp.hongshengwenyu.top

Java: import java.util.List;
来源：http://sgb.zdqjudy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ywc.sysykeji.top

Ruby: require "json"; require_relative "./util"
来源：http://pzi.xinyue.icu

C#:   using System.Text;
来源：http://rzo.ppjwa.cn

[C12] 立即执行函数 IIFE
来源：http://zeg.ctjpmb.com

Py:   (lambda: print("run"))()
来源：http://zab.feifeiyinyue.top

PHP:  (function () { echo "run"; })();
来源：http://yek.yj20258888.top

JS:   (() => { console.log("run"); })();
来源：http://luz.dianchejie.cn

TS:   (() => { console.log("run"); })();
来源：http://lig.jiagoushi.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://omt.snrcjt.cn

Go:   func() { fmt.Println("run") }()
来源：http://gld.hesvh.cn

Ruby: -> { puts "run" }.call
来源：http://giv.dashuyun.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://tnb.chenjidiqi.icu

[C13] 类型声明 / 类型注解
来源：http://omf.jinqigufen.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hpz.fktsv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sgv.jyoumei.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mht.pengpengdd.cyou

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mcb.jianghu66.top

Java: int add(int a, int b) { return a + b; }
来源：http://hqo.cheryme.top

Go:   func add(a, b int) int
来源：http://ruk.ydjk.org.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://liq.zhiwuduotai.top

C#:   int Add(int a, int b) => a + b;
来源：http://ywf.cdnleiting.top

[C14] 泛型函数
来源：http://psp.uphjek.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hoi.nwbrower.top

PHP:  // 无泛型
来源：http://jfm.ydzc1.top

JS:   // 无泛型
来源：http://xmg.jyoumei.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jne.ywan-chungtsiang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ivq.wangshuangyany.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://czw.zdqjudy.top

Ruby: # 无泛型
来源：http://xxe.chenlongwang.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pkd.yueranfly.top

[C15] 解构 / 展开参数
来源：http://ptn.fengsongda.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jzt.nanxinkj.top

PHP:  [$a, $b] = $pair;
来源：http://hzd.zhongyouzk.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://aab.ehwqpu.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lgp.jinqigufen.top

Java: // 无解构
来源：http://xxe.gzhubu.top

Go:   // 无解构
来源：http://kam.epnwcf.com

Ruby: a, b = pair
来源：http://suk.zhijiandao.cn

C#:   var (a, b) = pair;
来源：http://nkx.dianchejie.cn

[C16] 函数 / 方法重载
来源：http://mji.hcnkem.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gmi.nanxinkj.top


<!-- 参考信息 -->