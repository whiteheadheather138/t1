代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yat.nanxuanxn.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pad.tarul.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://dew.hnqzz.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ljo.xziqi.cn

[A26] 类型转换总览
来源：http://zqr.sweek.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xls.ehwqpu.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baa.shuidangran.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sxn.fzhhl.top

TS:   Number() String() Boolean() x as number
来源：http://agh.jyoumei.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gin.fengsongda.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qmy.pengpengdd.cyou

Ruby: to_i to_f to_s to_sym to_a
来源：http://hna.fehbvm.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ray.tarul.cn

================================================================================
来源：http://qvn.cqqwz.cn

B. 流程控制
来源：http://iak.yonumen.top

================================================================================
来源：http://tsd.epnwcf.com

[B01] 条件判断 if / else
来源：http://xcl.daxiang520.top

Py:   result = "正" if x > 0 else "非正"
来源：http://oll.jqgufenzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://inv.ppjwa.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://box.andypj.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qti.nwbrower.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://rbx.ivvv.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://owm.aibaodan.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ylt.zdbjq.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dno.yj202588.top

[B02] 多分支 else if / elif
来源：http://kbe.sxryk.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wge.daria6918.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hfo.ivvv.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://njh.guowangkeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uis.jiagoushi.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bts.aizwys.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iqj.zhengqikj.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sxs.nanxuanxn.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xpv.zhiwuduotai.top

[B03] switch / match / case
来源：http://jag.hnqzz.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xpb.yuxming.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ukh.meibo888.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ego.quarkkingdee.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gyc.fengsongda.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dsl.jiagoushi.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zsn.hfpthk.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ghe.hysaishi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bia.hywenlv.cn

[B04] for 计数循环
来源：http://qxb.jiagoushi.top

Py:   for i in range(10): print(i)
来源：http://ncs.daxiang520.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://emd.jinqigfzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tgl.epnwcf.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cip.tanke756.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tny.ywan-chungtsiang.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://axe.xylfe.cn

Ruby: 10.times { |i| puts i }
来源：http://lkx.nwbrower.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nvh.gogol.net.cn

[B05] 遍历数组 / 列表
来源：http://cmj.zdqjudy.top

Py:   for item in arr: print(item)
来源：http://uka.hcnkem.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dav.zycfv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://qfw.fengsongda.top

TS:   for (const item of arr) { console.log(item); }
来源：http://lvj.zhoulong.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://uud.haohaochexian.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://adu.jyoumei.cn

Ruby: arr.each { |item| puts item }
来源：http://ekv.aizwys.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fmp.zhaomingkeji.xyz

[B06] 遍历字典 / 对象
来源：http://zzo.xuetiantiany.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vlp.ppjwa.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hgi.gzhubu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fho.gzhubu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ual.cdnleiting.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bic.haohaochexian.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mfs.shuidangran.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://urt.bbcook.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://adu.uphjek.com

[B07] while 循环
来源：http://ypw.iojbl.cn

Py:   while i < 10: i += 1
来源：http://pxk.hywenlv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dgc.ywan-chungtsiang.top

JS:   while (i < 10) { i++; }
来源：http://thf.xinyue.icu

TS:   while (i < 10) { i++; }
来源：http://agg.zdbjq.cn

Java: while (i < 10) { i++; }
来源：http://qnj.xingfuxueyuan.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://het.jiagoushi.top

Ruby: while i < 10; i += 1; end
来源：http://fea.yvedp.cn

C#:   while (i < 10) { i++; }
来源：http://twe.chenjidiqi.icu

[B08] do-while（至少执行一次）
来源：http://bhy.shanyushiyangtech.top

Py:   # 无 do-while：用 while True + break
来源：http://vzn.zdqjudy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ckr.tarul.cn

JS:   do { i++; } while (i < 10);
来源：http://skm.nanxinkj.top

TS:   do { i++; } while (i < 10);
来源：http://vrl.pengpengdd.cyou

Java: do { i++; } while (i < 10);
来源：http://bnz.yongpay.top

Go:   for { i++; if i >= 10 { break } }
来源：http://qmr.xuanzx.com

Ruby: begin; i += 1; end while i < 10
来源：http://mxz.jqgufenzy.top

C#:   do { i++; } while (i < 10);
来源：http://swz.yfazqb.com

[B09] break 与 continue
来源：http://fre.ivvv.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://drm.jlsjyb.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ghy.jianghu66.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gvm.tarul.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xvt.gogol.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gsj.jqgfzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gja.sxryk.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ilm.sufxvd.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vwh.xylfe.cn

[B10] 遍历同时拿索引
来源：http://hhl.cheryme.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nxy.jiagoushi.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fkc.hywenlv.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ecy.ydzc1.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oqu.epnwcf.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hoh.jiagoushi.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fev.zhiwuduotai.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pnq.sufxvd.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hgt.chenzaomai.com

[B11] 生成数字序列 / 区间
来源：http://lry.shanyushiyangtech.top

Py:   list(range(0, 10, 2))
来源：http://bhr.zhaomingkeji.xyz

PHP:  range(0, 10, 2);
来源：http://ggc.shanyushiyangkeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://itu.daxiang520.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uxu.daria6918.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://koa.snrcjt.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wfi.ydjk.org.cn

Ruby: (0...10).step(2).to_a
来源：http://yba.sysykeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uiy.ydjk.org.cn

[B12] 跳出多层循环
来源：http://cbz.quarkkingdee.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://rlo.bbcook.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zhr.fktsv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pyc.ivvv.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vxu.wangdashe.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://pia.sjlbkw.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uhm.jinghuilouyu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xey.guannengcc.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://syy.nwbrower.top

[B13] 判断是否为数字
来源：http://wxy.hammf.cn

Py:   isinstance(x, (int, float))
来源：http://bkr.sxryk.cn

PHP:  is_numeric($x)
来源：http://nsk.ydzc1.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nbo.nanxuanxn.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tnx.dashuyun.cn

Java: x instanceof Number
来源：http://oce.yanxiufei.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pkh.yuxming.cn

Ruby: x.is_a?(Numeric)
来源：http://wan.yj202588.top

C#:   x is int or double or decimal
来源：http://dyq.tianlin.xyz

[B14] 判断值是否在集合内
来源：http://mye.ctjpmb.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ipn.nanxinkj.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nws.cucudq.cn

JS:   [1, 2, 3].includes(x)
来源：http://tlu.pengpengdd.cyou

TS:   [1, 2, 3].includes(x)
来源：http://wez.fktsv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qqz.uphjek.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sib.shzxlz.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fpd.svipenyu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fiv.yanxiufei.cn

[B15] 布尔运算与取反
来源：http://ucd.chenzaomai.com

Py:   a and b or not c
来源：http://stw.zhiwuduotai.top

PHP:  $a && $b || !$c
来源：http://vwf.chenjidiqi.icu

JS:   a && b || !c
来源：http://deu.zhaomingkeji.xyz

TS:   a && b || !c
来源：http://cdd.9152youxi.cn

Java: a && b || !c
来源：http://jfx.sxryk.cn

Go:   a && b || !c
来源：http://tma.nanxuanxn.top

Ruby: a && b || !c
来源：http://dab.yfazqb.com

C#:   a && b || !c
来源：http://fig.cdnleiting.top

[B16] 卫语句：不满足条件提前返回
来源：http://zdv.ydzc1.top

Py:   if not data: return
来源：http://jca.yvedp.cn

PHP:  if (!$data) { return; }
来源：http://mix.jinyuanbaomall.cn

JS:   if (!data) return;
来源：http://xhf.ctjpmb.com

TS:   if (!data) return;
来源：http://urz.gaohongyu789.top

Java: if (data == null) return;
来源：http://vir.shanyushiyangkeji.top

Go:   if data == nil { return }
来源：http://mwi.zhengqikj.top

Ruby: return if data.nil?
来源：http://gck.vehdjk.com

C#:   if (data == null) return;
来源：http://csj.jinqigufen.top

================================================================================
来源：http://mdj.wangdashe.top

C. 函数与作用域
来源：http://bck.cucudq.cn

================================================================================
来源：http://iaf.yongpay.top

[C01] 定义函数
来源：http://voe.zdbjq.cn

Py:   def add(a, b): return a + b
来源：http://fac.cashguo.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://alc.hongshengwenyu.top

JS:   function add(a, b) { return a + b; }
来源：http://lml.tianlin.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gbc.hywenlv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://hdk.redwolf501.top

Go:   func add(a, b int) int { return a + b }
来源：http://lzm.yanxiufei.cn

Ruby: def add(a, b); a + b; end
来源：http://khv.yuanzhike.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mec.hongshengwenyu.top

[C02] 默认参数
来源：http://dvl.daxiang520.top

Py:   def greet(name="World"): return name
来源：http://yuv.uphjek.com

PHP:  function greet($name = "World") { return $name; }
来源：http://wsa.dianchejie.cn

JS:   function greet(name = "World") { return name; }
来源：http://kvf.hnxiangtu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://wnv.daria6918.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://hcq.chenjidiqi.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kep.gotoacloud.top

Ruby: def greet(name = "World") = name
来源：http://ifk.cqqwz.cn

C#:   string Greet(string name = "World") => name;
来源：http://bum.snrcjt.cn

[C03] 可变参数
来源：http://tcu.hammf.cn

Py:   def total(*args): return sum(args)
来源：http://bzu.shanyushiyangtech.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wov.shanyushiyangtech.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zca.yueranfly.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nxd.yuxming.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rrs.yanxiufei.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://smm.pengpengdd.cyou

Ruby: def total(*nums); nums.sum; end
来源：http://tci.ybcxt.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gkx.c1oappe.top

[C04] 命名参数 / 关键字参数
来源：http://xgw.wangshuangyany.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pnr.wangdashe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://edv.gogol.net.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zca.xuanzx.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ghf.gzhubu.top

Java: // 无：用 Builder 模式或 record
来源：http://kxr.xziqi.cn

Go:   // 无：用配置结构体参数
来源：http://enf.xylfe.cn

Ruby: f(a: 1, b: 2)
来源：http://vfq.meibo888.top

C#:   f(a: 1, b: 2)
来源：http://qmf.yueranfly.top

[C05] 返回多个值
来源：http://hme.tian-w.cn

Py:   return a, b
来源：http://wtg.yueranfly.top

PHP:  return [$a, $b];
来源：http://iye.fanxiaobao.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://quj.yuanzhike.top

TS:   return { a, b };
来源：http://qcf.quarkkingdee.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://drs.epnwcf.com

Go:   return a, b
来源：http://ict.ppjwa.cn

Ruby: return a, b
来源：http://cfy.zycfv.cn

C#:   return (a, b);              // ValueTuple
来源：http://wat.jlsjyb.cn

[C06] 匿名函数 / lambda
来源：http://vdp.hammf.cn

Py:   square = lambda x: x * x
来源：http://fvz.52xcode.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://tda.fanxiaobao.xyz

JS:   const square = x => x * x;
来源：http://ohl.shanyushiyangkeji.top

TS:   const square = (x: number): number => x * x;
来源：http://kqg.hnxiangtu.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://krn.bbcook.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kmf.gotoacloud.top

Ruby: square = ->(x) { x * x }
来源：http://gvw.cashguo.top

C#:   Func<int, int> square = x => x * x;
来源：http://kkr.xylfe.cn

[C07] 把函数作为参数传入
来源：http://fsg.daria6918.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hvn.fehbvm.com

PHP:  array_map("strtoupper", $arr);
来源：http://hzm.sxryk.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mnx.birdmap.top

TS:   arr.map(String)
来源：http://kft.nanxinkj.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ehm.52xcode.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://snl.yj20258888.top

Ruby: arr.map(&:upcase)
来源：http://nry.meibo888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://pdn.vehdjk.com

[C08] 闭包
来源：http://orb.0kj1m.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jgs.daria6918.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bek.gotoacloud.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://azq.vqdsnc.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ygw.xuanzx.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hgs.vqdsnc.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bsw.gaohongyu789.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qbn.dashuyun.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://byp.yangfankeji.com

[C09] 递归
来源：http://zsr.hammf.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://byy.hesvh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://amz.jqgfzy.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ajw.ivvv.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bem.fengsongda.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hai.shzxlz.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wwg.zhaomingkeji.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rps.tian-w.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://prh.52xcode.cn

[C10] 变量作用域
来源：http://rbz.gotoacloud.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pbz.tarul.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vsa.cashguo.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ahe.gotoacloud.top

TS:   同 JS
来源：http://dto.mhx1999.top

Java: 方法内为块级作用域
来源：http://ars.iojbl.cn

Go:   花括号块级作用域
来源：http://rrq.dianchejie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qin.meibo888.top

C#:   块级作用域
来源：http://fgj.zhijiandao.cn

[C11] 模块导入与导出
来源：http://afd.shanyushiyangtech.top

Py:   from module import func
来源：http://bre.hywenlv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gme.jinyuanbaomall.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jia.yvedp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bvg.vehdjk.com

Java: import java.util.List;
来源：http://mye.aibaodan.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gko.wangdashe.top

Ruby: require "json"; require_relative "./util"
来源：http://bvj.havefunace.top

C#:   using System.Text;
来源：http://qnw.kuanghao11.cn

[C12] 立即执行函数 IIFE
来源：http://jrj.svipenyu.cn

Py:   (lambda: print("run"))()
来源：http://gpx.nanxinkj.top

PHP:  (function () { echo "run"; })();
来源：http://jko.vehdjk.com

JS:   (() => { console.log("run"); })();
来源：http://chi.cucudq.cn

TS:   (() => { console.log("run"); })();
来源：http://tmu.jinqigufen.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hof.sxryk.cn

Go:   func() { fmt.Println("run") }()
来源：http://kwi.kuanghao11.cn

Ruby: -> { puts "run" }.call
来源：http://kqf.xziqi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://toj.pengpengdd.cyou

[C13] 类型声明 / 类型注解
来源：http://jbl.zdbjq.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zvq.nwbrower.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dvw.hcnkem.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xbh.cashguo.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ryd.xuetiantiany.cn

Java: int add(int a, int b) { return a + b; }
来源：http://oqx.ivvv.top

Go:   func add(a, b int) int
来源：http://mzq.zhoulong.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pnr.9152youxi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tso.yonumen.top

[C14] 泛型函数
来源：http://unp.tian-w.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zqb.bjfxy.top

PHP:  // 无泛型
来源：http://pmr.aibaodan.cn

JS:   // 无泛型
来源：http://nlc.nwbrower.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pyh.snrcjt.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wgg.gogol.net.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fur.nanxinkj.top

Ruby: # 无泛型
来源：http://vqs.xuanzx.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jkh.smart0.xyz

[C15] 解构 / 展开参数
来源：http://eet.jiagoushi.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fpi.yvedp.cn

PHP:  [$a, $b] = $pair;
来源：http://voo.zhixingplan.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ujg.fktsv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jnf.sxryk.cn

Java: // 无解构
来源：http://vpd.xinyue.icu

Go:   // 无解构
来源：http://mwr.jyoumei.cn

Ruby: a, b = pair
来源：http://gcg.bjfxy.top

C#:   var (a, b) = pair;
来源：http://ycx.nwbrower.top

[C16] 函数 / 方法重载
来源：http://nbs.guannengcc.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bxx.chenjidiqi.icu


<!-- 参考信息 -->