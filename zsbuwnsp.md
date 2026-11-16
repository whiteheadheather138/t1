代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://syg.nanxuanxn.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rdh.hysaishi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jvi.epnwcf.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lte.yj202588.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lye.chenlongwang.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mnf.ydjk.org.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://its.sjlbkw.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://aai.gogol.net.cn

[A26] 类型转换总览
来源：http://qdm.zhongyouzk.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kry.sweek.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rnm.jinqigfzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rrs.fzhhl.top

TS:   Number() String() Boolean() x as number
来源：http://aan.yongpay.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rrr.havefunace.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wxr.xinyue.icu

Ruby: to_i to_f to_s to_sym to_a
来源：http://cob.jiagoushi.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tbj.hongshengwenyu.top

================================================================================
来源：http://hjr.xinyue.icu

B. 流程控制
来源：http://tfo.zhiwuduotai.top

================================================================================
来源：http://tow.jinghuilouyu.cn

[B01] 条件判断 if / else
来源：http://ndv.ivvv.top

Py:   result = "正" if x > 0 else "非正"
来源：http://cir.redwolf501.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gtx.guannengcc.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bhb.wangshuangyany.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://eqs.fktsv.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://nlk.zdqjudy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://iuv.xingfuxueyuan.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gnx.shuidangran.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vvj.gotoacloud.top

[B02] 多分支 else if / elif
来源：http://nyj.fehbvm.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sgu.ywan-chungtsiang.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ecz.sufxvd.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jaj.vqdsnc.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zsw.tarul.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ued.ivvv.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gmb.tianlin.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nbc.xingfuxueyuan.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rfa.guannengcc.top

[B03] switch / match / case
来源：http://xui.316326.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cqa.zycfv.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zgl.guannengcc.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lrv.ybcxt.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ghe.yj20258.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kwg.quarkkingdee.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://aaa.epnwcf.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lxy.shzxlz.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vbg.iojbl.cn

[B04] for 计数循环
来源：http://hqk.aizwys.cn

Py:   for i in range(10): print(i)
来源：http://hga.nanxuanxn.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rua.guowangkeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dgg.chenjidiqi.icu

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ldo.nanxinkj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jid.yfazqb.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ggz.tarul.cn

Ruby: 10.times { |i| puts i }
来源：http://xyg.ivvv.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hxx.ydjk.org.cn

[B05] 遍历数组 / 列表
来源：http://sfu.shangyingyoupin.top

Py:   for item in arr: print(item)
来源：http://ped.shuidangran.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bts.dianchejie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://cue.cashguo.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xpv.yueranfly.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://enl.jyoumei.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pmy.shanyushiyangtech.top

Ruby: arr.each { |item| puts item }
来源：http://rly.52xcode.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ayx.dianchejie.cn

[B06] 遍历字典 / 对象
来源：http://ohu.tianlin.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://jks.zhiwuduotai.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xuj.chenlongwang.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pmq.hnxiangtu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://duv.hongshengwenyu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fkh.jinqigfzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://foq.wangdashe.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nus.pycfn.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xwz.ywan-chungtsiang.top

[B07] while 循环
来源：http://ayz.pycfn.com

Py:   while i < 10: i += 1
来源：http://xvx.smart0.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://xzn.shangyingyoupin.top

JS:   while (i < 10) { i++; }
来源：http://fgb.jianghu66.top

TS:   while (i < 10) { i++; }
来源：http://hxb.yonumen.top

Java: while (i < 10) { i++; }
来源：http://jks.hnqzz.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ykh.sweek.top

Ruby: while i < 10; i += 1; end
来源：http://imi.tarul.cn

C#:   while (i < 10) { i++; }
来源：http://xkl.c1oappe.top

[B08] do-while（至少执行一次）
来源：http://ois.jinqigfzy.top

Py:   # 无 do-while：用 while True + break
来源：http://ddo.bbcook.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://enf.ybcxt.top

JS:   do { i++; } while (i < 10);
来源：http://hcn.guannengcc.top

TS:   do { i++; } while (i < 10);
来源：http://wht.9152youxi.cn

Java: do { i++; } while (i < 10);
来源：http://ssr.yuxming.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://pei.hfpthk.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bqh.hywenlv.cn

C#:   do { i++; } while (i < 10);
来源：http://ljt.fehbvm.com

[B09] break 与 continue
来源：http://kqe.xziqi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bud.zycfv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://shs.hfpthk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fpx.xingfuxueyuan.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sbn.jinqigfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lny.gotoacloud.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://krh.hfpthk.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ocz.zhengqikj.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tob.fehbvm.com

[B10] 遍历同时拿索引
来源：http://mlu.yueranfly.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zix.316326.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hwc.cheryme.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sgy.hnqzz.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://nkc.dashuyun.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://feh.ydzc1.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gol.52xcode.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gcr.nanxuanxn.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wit.0kj1m.cn

[B11] 生成数字序列 / 区间
来源：http://jel.zhaomingkeji.xyz

Py:   list(range(0, 10, 2))
来源：http://gun.fzhhl.top

PHP:  range(0, 10, 2);
来源：http://zou.jianghu66.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fmz.yuanzhike.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://utj.nwbrower.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://amm.andypj.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://aew.daria6918.cn

Ruby: (0...10).step(2).to_a
来源：http://lvi.nanxuanxn.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ikd.gzhubu.top

[B12] 跳出多层循环
来源：http://vyq.zhiwuduotai.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://cbs.yfazqb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://naj.aibaodan.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://amb.ybcxt.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hyo.ydzc1.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ydb.vehdjk.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://shu.jinqigfzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rdt.jianghu66.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rdv.tian-w.cn

[B13] 判断是否为数字
来源：http://mfg.zhengqikj.top

Py:   isinstance(x, (int, float))
来源：http://bgg.zdbjq.cn

PHP:  is_numeric($x)
来源：http://gic.vehdjk.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://syi.aizwys.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ulj.gzhubu.top

Java: x instanceof Number
来源：http://dmy.hongshengwenyu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pvf.nanxinkj.top

Ruby: x.is_a?(Numeric)
来源：http://qql.shanyushiyangkeji.top

C#:   x is int or double or decimal
来源：http://fit.zdqjudy.top

[B14] 判断值是否在集合内
来源：http://ezy.daria6918.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xoq.daxiang520.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zsr.redwolf501.top

JS:   [1, 2, 3].includes(x)
来源：http://zba.yuxming.cn

TS:   [1, 2, 3].includes(x)
来源：http://ygb.birdmap.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ldl.vqdsnc.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://btj.zdbjq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fxz.iojbl.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wqt.jinghuilouyu.cn

[B15] 布尔运算与取反
来源：http://ogc.ivvv.top

Py:   a and b or not c
来源：http://zez.yanxiufei.cn

PHP:  $a && $b || !$c
来源：http://irj.hesvh.cn

JS:   a && b || !c
来源：http://hyt.sxryk.cn

TS:   a && b || !c
来源：http://seq.fktsv.cn

Java: a && b || !c
来源：http://dih.xuanzx.com

Go:   a && b || !c
来源：http://woa.hnqzz.top

Ruby: a && b || !c
来源：http://nzj.redwolf501.top

C#:   a && b || !c
来源：http://sge.zhixingplan.top

[B16] 卫语句：不满足条件提前返回
来源：http://csc.hysaishi.cn

Py:   if not data: return
来源：http://zpn.pycfn.com

PHP:  if (!$data) { return; }
来源：http://iea.shuidangran.top

JS:   if (!data) return;
来源：http://gqc.yj202588.top

TS:   if (!data) return;
来源：http://wca.ctjpmb.com

Java: if (data == null) return;
来源：http://mfl.ehwqpu.com

Go:   if data == nil { return }
来源：http://bao.shanyushiyangtech.top

Ruby: return if data.nil?
来源：http://ssg.hcnkem.com

C#:   if (data == null) return;
来源：http://bsu.vehdjk.com

================================================================================
来源：http://ggq.feifeiyinyue.top

C. 函数与作用域
来源：http://qey.ehwqpu.com

================================================================================
来源：http://zkm.tanke756.top

[C01] 定义函数
来源：http://akj.aizwys.cn

Py:   def add(a, b): return a + b
来源：http://fyk.zhiwuduotai.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://seh.zhaomingkeji.xyz

JS:   function add(a, b) { return a + b; }
来源：http://cwe.guannengcc.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jjh.gaohongyu789.top

Java: static int add(int a, int b) { return a + b; }
来源：http://lzv.jianghu66.top

Go:   func add(a, b int) int { return a + b }
来源：http://bib.yongpay.top

Ruby: def add(a, b); a + b; end
来源：http://nql.cqqwz.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vdm.zhijiandao.cn

[C02] 默认参数
来源：http://clg.feifeiyinyue.top

Py:   def greet(name="World"): return name
来源：http://vxv.iojbl.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fps.iojbl.cn

JS:   function greet(name = "World") { return name; }
来源：http://vof.pycfn.com

TS:   function greet(name: string = "World") { return name; }
来源：http://vht.aizwys.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://adb.shangyingyoupin.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lmv.zhaomingkeji.xyz

Ruby: def greet(name = "World") = name
来源：http://dvv.yonumen.top

C#:   string Greet(string name = "World") => name;
来源：http://gnw.zycfv.cn

[C03] 可变参数
来源：http://rzz.xziqi.cn

Py:   def total(*args): return sum(args)
来源：http://xoi.quarkkingdee.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vgm.chenlongwang.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://iju.xuetiantiany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iug.yuxming.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dke.xuanzx.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uyp.hcnkem.com

Ruby: def total(*nums); nums.sum; end
来源：http://vys.jinghuilouyu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pju.shuidangran.top

[C04] 命名参数 / 关键字参数
来源：http://mta.zhixingplan.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://doz.yangfankeji.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ikr.shzxlz.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rta.fehbvm.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ttq.ctjpmb.com

Java: // 无：用 Builder 模式或 record
来源：http://svz.9152youxi.cn

Go:   // 无：用配置结构体参数
来源：http://txt.jinqigufen.top

Ruby: f(a: 1, b: 2)
来源：http://mnr.ywan-chungtsiang.top

C#:   f(a: 1, b: 2)
来源：http://vrg.sjlbkw.cn

[C05] 返回多个值
来源：http://apr.svipenyu.cn

Py:   return a, b
来源：http://dja.shanyushiyangkeji.top

PHP:  return [$a, $b];
来源：http://dko.mhx1999.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://dir.9152youxi.cn

TS:   return { a, b };
来源：http://tjv.xingfuxueyuan.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wzf.zhaomingkeji.xyz

Go:   return a, b
来源：http://gcf.chenlongwang.top

Ruby: return a, b
来源：http://zfu.havefunace.top

C#:   return (a, b);              // ValueTuple
来源：http://cfl.jinghuilouyu.cn

[C06] 匿名函数 / lambda
来源：http://suy.zhengqikj.top

Py:   square = lambda x: x * x
来源：http://bcx.ppjwa.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://rtw.hammf.cn

JS:   const square = x => x * x;
来源：http://qgl.jiagoushi.top

TS:   const square = (x: number): number => x * x;
来源：http://mer.haohaochexian.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tev.sxryk.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zgm.fktsv.cn

Ruby: square = ->(x) { x * x }
来源：http://yfn.hammf.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xxm.hammf.cn

[C07] 把函数作为参数传入
来源：http://ksc.jqgfzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qpe.nanxuanxn.top

PHP:  array_map("strtoupper", $arr);
来源：http://yar.jqgufenzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nly.zhoulong.xyz

TS:   arr.map(String)
来源：http://vbv.kuanghao11.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ykz.yanxiufei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cqt.epnwcf.com

Ruby: arr.map(&:upcase)
来源：http://fae.quarkkingdee.top

C#:   arr.Select(s => s.ToUpper())
来源：http://pqf.vqdsnc.cn

[C08] 闭包
来源：http://cul.aizwys.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ekq.yanxiufei.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ado.316326.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://nci.fehbvm.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://riv.snrcjt.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://arj.ppjwa.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lif.jyoumei.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://clu.pengpengdd.cyou

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://avd.fehbvm.com

[C09] 递归
来源：http://pcq.sxryk.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://pis.yangfankeji.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kdk.zhixingplan.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zce.yuanzhike.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dvc.ybcxt.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pcp.kuanghao11.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xqt.daria6918.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pfy.pengpengdd.cyou

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rkp.gzhubu.top

[C10] 变量作用域
来源：http://dux.jinghuilouyu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dlv.chenjidiqi.icu

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qwy.hnqzz.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yqw.jyoumei.cn

TS:   同 JS
来源：http://gls.dashuyun.cn

Java: 方法内为块级作用域
来源：http://dux.snrcjt.cn

Go:   花括号块级作用域
来源：http://die.zhongyouzk.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pjh.zhaomingkeji.xyz

C#:   块级作用域
来源：http://zcn.zdbjq.cn

[C11] 模块导入与导出
来源：http://fbr.sysykeji.top

Py:   from module import func
来源：http://rfj.bjfxy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jtn.52xcode.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ixd.vqdsnc.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pbo.dashuyun.cn

Java: import java.util.List;
来源：http://hvt.gaohongyu789.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lxi.yvedp.cn

Ruby: require "json"; require_relative "./util"
来源：http://sbz.shuidangran.top

C#:   using System.Text;
来源：http://vkr.fengsongda.top

[C12] 立即执行函数 IIFE
来源：http://vzc.guannengcc.top

Py:   (lambda: print("run"))()
来源：http://ssb.redwolf501.top

PHP:  (function () { echo "run"; })();
来源：http://tzr.yuanzhike.top

JS:   (() => { console.log("run"); })();
来源：http://uxt.mhx1999.top

TS:   (() => { console.log("run"); })();
来源：http://ito.svipenyu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hni.yongpay.top

Go:   func() { fmt.Println("run") }()
来源：http://icd.epnwcf.com

Ruby: -> { puts "run" }.call
来源：http://dvq.hnqzz.top

C#:   // 无 IIFE：用静态构造函数
来源：http://can.hongshengwenyu.top

[C13] 类型声明 / 类型注解
来源：http://igd.tian-w.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yfw.fktsv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ilh.gogol.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fbx.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xzt.vehdjk.com

Java: int add(int a, int b) { return a + b; }
来源：http://yle.feifeiyinyue.top

Go:   func add(a, b int) int
来源：http://qtg.hcnkem.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bqh.hnxiangtu.top

C#:   int Add(int a, int b) => a + b;
来源：http://dmg.cdnleiting.top

[C14] 泛型函数
来源：http://gcq.hesvh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oit.zhaomingkeji.xyz

PHP:  // 无泛型
来源：http://rao.gaohongyu789.top

JS:   // 无泛型
来源：http://qqr.c1oappe.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xza.zdbjq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jwg.uphjek.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oer.sysykeji.top

Ruby: # 无泛型
来源：http://gbq.uphjek.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hrr.snrcjt.cn

[C15] 解构 / 展开参数
来源：http://ylk.yuanzhike.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qxr.chenlongwang.top

PHP:  [$a, $b] = $pair;
来源：http://udy.hfpthk.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qcy.haohaochexian.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rlx.ctjpmb.com

Java: // 无解构
来源：http://xqm.ctjpmb.com

Go:   // 无解构
来源：http://ajn.gaohongyu789.top


<!-- 参考信息 -->