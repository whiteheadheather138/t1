代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kks.ehwqpu.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cig.xuetiantiany.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wst.zhongyouzk.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ojx.jqgfzy.top

[A26] 类型转换总览
来源：http://ykt.feifeiyinyue.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kgg.jinqigufen.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ori.shanyushiyangkeji.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gsm.xingfuxueyuan.xyz

TS:   Number() String() Boolean() x as number
来源：http://hxa.sysykeji.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pyv.iojbl.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qrs.snrcjt.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cmq.chenjidiqi.icu

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fke.yj20258888.top

================================================================================
来源：http://pwv.yuanzhike.top

B. 流程控制
来源：http://vxo.jinyuanbaomall.cn

================================================================================
来源：http://soc.zycfv.cn

[B01] 条件判断 if / else
来源：http://ibz.zhixingplan.top

Py:   result = "正" if x > 0 else "非正"
来源：http://cgc.ydjk.org.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://igc.fanxiaobao.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ygq.shanyushiyangkeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yur.yangfankeji.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://nip.bbcook.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://veg.ppjwa.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://udd.hnqzz.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qay.52xcode.cn

[B02] 多分支 else if / elif
来源：http://jrt.pengpengdd.cyou

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xyc.xinyue.icu

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://omd.yuanzhike.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ujg.vqdsnc.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ecu.shanyushiyangkeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uod.jianghu66.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dpe.tianlin.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ina.jlsjyb.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kfz.cucudq.cn

[B03] switch / match / case
来源：http://eas.hammf.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ldq.nanxuanxn.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cqe.hfpthk.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://otc.shanyushiyangkeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ayj.fehbvm.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yvo.yangfankeji.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://voj.jlsjyb.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mhj.xuanzx.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hck.zdqjudy.top

[B04] for 计数循环
来源：http://msx.zhongyouzk.top

Py:   for i in range(10): print(i)
来源：http://ghx.sxryk.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bgj.jqgufenzy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://umt.yonumen.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sex.jlsjyb.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ncf.yonumen.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jrk.316326.xyz

Ruby: 10.times { |i| puts i }
来源：http://hlt.jqgufenzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qse.dashuyun.cn

[B05] 遍历数组 / 列表
来源：http://ius.shangyingyoupin.top

Py:   for item in arr: print(item)
来源：http://dnq.ydjk.org.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qqa.tian-w.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://epe.smart0.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://yve.mhx1999.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qna.redwolf501.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://skx.pengpengdd.cyou

Ruby: arr.each { |item| puts item }
来源：http://tfv.birdmap.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qut.pycfn.com

[B06] 遍历字典 / 对象
来源：http://nne.yj20258.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ias.gotoacloud.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uuj.hnxiangtu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ruf.zhaomingkeji.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ban.xingfuxueyuan.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://udm.dianchejie.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vvl.nwbrower.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vgt.nanxuanxn.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hbi.nanxuanxn.top

[B07] while 循环
来源：http://ttm.yuanzhike.top

Py:   while i < 10: i += 1
来源：http://pen.yuxming.cn

PHP:  while ($i < 10) { $i++; }
来源：http://has.pengpengdd.cyou

JS:   while (i < 10) { i++; }
来源：http://kcl.shanyushiyangtech.top

TS:   while (i < 10) { i++; }
来源：http://xeg.yongpay.top

Java: while (i < 10) { i++; }
来源：http://pvp.shuidangran.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rqf.jinqigufen.top

Ruby: while i < 10; i += 1; end
来源：http://otp.zhongyouzk.top

C#:   while (i < 10) { i++; }
来源：http://hou.zycfv.cn

[B08] do-while（至少执行一次）
来源：http://yuh.shanyushiyangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://jth.svipenyu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dse.cashguo.top

JS:   do { i++; } while (i < 10);
来源：http://tdo.fehbvm.com

TS:   do { i++; } while (i < 10);
来源：http://xve.52xcode.cn

Java: do { i++; } while (i < 10);
来源：http://urs.316326.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://ajx.snrcjt.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kpz.hnxiangtu.top

C#:   do { i++; } while (i < 10);
来源：http://mzs.sufxvd.cn

[B09] break 与 continue
来源：http://kss.dianchejie.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://khh.yongpay.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://voh.hnxiangtu.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iwq.0kj1m.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rto.ctjpmb.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eth.yj20258.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://drh.jqgufenzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kum.guannengcc.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eub.chenlongwang.top

[B10] 遍历同时拿索引
来源：http://hrw.gaohongyu789.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zil.fzhhl.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vnq.svipenyu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://etw.yueranfly.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hui.yuanzhike.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bot.vehdjk.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bql.xuetiantiany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://diw.mhx1999.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mem.fanxiaobao.xyz

[B11] 生成数字序列 / 区间
来源：http://yrz.tarul.cn

Py:   list(range(0, 10, 2))
来源：http://szd.tanke756.top

PHP:  range(0, 10, 2);
来源：http://vbw.chenlongwang.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zom.birdmap.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yaj.nanxuanxn.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ish.yvedp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nqu.jqgufenzy.top

Ruby: (0...10).step(2).to_a
来源：http://erh.tian-w.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fxn.andypj.xyz

[B12] 跳出多层循环
来源：http://epd.cheryme.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://zvx.jiagoushi.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://pir.shanyushiyangtech.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oym.jqgufenzy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rmx.hnxiangtu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fiy.tian-w.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jvk.yuxming.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gwo.hesvh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tot.fehbvm.com

[B13] 判断是否为数字
来源：http://llz.yanxiufei.cn

Py:   isinstance(x, (int, float))
来源：http://jjl.kuanghao11.cn

PHP:  is_numeric($x)
来源：http://tjn.dianchejie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://npu.fengsongda.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hoi.hcnkem.com

Java: x instanceof Number
来源：http://mzm.yfazqb.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://iyu.guannengcc.top

Ruby: x.is_a?(Numeric)
来源：http://gkk.feifeiyinyue.top

C#:   x is int or double or decimal
来源：http://eku.316326.xyz

[B14] 判断值是否在集合内
来源：http://rts.sjlbkw.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tsj.c1oappe.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xrp.ctjpmb.com

JS:   [1, 2, 3].includes(x)
来源：http://mus.redwolf501.top

TS:   [1, 2, 3].includes(x)
来源：http://kzs.epnwcf.com

Java: List.of(1, 2, 3).contains(x)
来源：http://pmd.zycfv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eit.zhoulong.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://atr.hcnkem.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://itn.zhaomingkeji.xyz

[B15] 布尔运算与取反
来源：http://skw.pycfn.com

Py:   a and b or not c
来源：http://knp.fehbvm.com

PHP:  $a && $b || !$c
来源：http://kob.xylfe.cn

JS:   a && b || !c
来源：http://ftc.chenzaomai.com

TS:   a && b || !c
来源：http://hzg.zhoulong.xyz

Java: a && b || !c
来源：http://mrs.hnqzz.top

Go:   a && b || !c
来源：http://zhf.yvedp.cn

Ruby: a && b || !c
来源：http://fja.316326.xyz

C#:   a && b || !c
来源：http://ubv.ctjpmb.com

[B16] 卫语句：不满足条件提前返回
来源：http://kdl.tian-w.cn

Py:   if not data: return
来源：http://zgc.xylfe.cn

PHP:  if (!$data) { return; }
来源：http://qpi.cheryme.top

JS:   if (!data) return;
来源：http://iqu.feifeiyinyue.top

TS:   if (!data) return;
来源：http://tff.yfazqb.com

Java: if (data == null) return;
来源：http://xye.zhengqikj.top

Go:   if data == nil { return }
来源：http://hqo.tian-w.cn

Ruby: return if data.nil?
来源：http://tjz.haohaochexian.top

C#:   if (data == null) return;
来源：http://vyt.zhixingplan.top

================================================================================
来源：http://xos.hammf.cn

C. 函数与作用域
来源：http://yjf.xingfuxueyuan.xyz

================================================================================
来源：http://mzc.zdbjq.cn

[C01] 定义函数
来源：http://cmn.jqgfzy.top

Py:   def add(a, b): return a + b
来源：http://cuk.wangdashe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hey.yvedp.cn

JS:   function add(a, b) { return a + b; }
来源：http://vpc.yangfankeji.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zfu.yvedp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://fik.yuanzhike.top

Go:   func add(a, b int) int { return a + b }
来源：http://qqz.ydjk.org.cn

Ruby: def add(a, b); a + b; end
来源：http://rov.yongpay.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qbe.xingfuxueyuan.xyz

[C02] 默认参数
来源：http://mpl.aibaodan.cn

Py:   def greet(name="World"): return name
来源：http://dxl.vqdsnc.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://fvl.ehwqpu.com

JS:   function greet(name = "World") { return name; }
来源：http://qet.sjlbkw.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://voa.aibaodan.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rge.tian-w.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://suv.sxryk.cn

Ruby: def greet(name = "World") = name
来源：http://ykw.redwolf501.top

C#:   string Greet(string name = "World") => name;
来源：http://ffv.nwbrower.top

[C03] 可变参数
来源：http://tml.zhiwuduotai.top

Py:   def total(*args): return sum(args)
来源：http://psj.zycfv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lty.yuxming.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kpd.hcnkem.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bow.yj20258.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rqe.mhx1999.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kho.ydzc1.top

Ruby: def total(*nums); nums.sum; end
来源：http://oak.yuxming.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vyq.uphjek.com

[C04] 命名参数 / 关键字参数
来源：http://nwd.yuanzhike.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://irj.hywenlv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jif.ivvv.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kpz.yj20258888.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dmy.quarkkingdee.top

Java: // 无：用 Builder 模式或 record
来源：http://sao.yanxiufei.cn

Go:   // 无：用配置结构体参数
来源：http://mzk.cqqwz.cn

Ruby: f(a: 1, b: 2)
来源：http://ruv.daria6918.cn

C#:   f(a: 1, b: 2)
来源：http://uls.jqgufenzy.top

[C05] 返回多个值
来源：http://apg.guannengcc.top

Py:   return a, b
来源：http://vtf.andypj.xyz

PHP:  return [$a, $b];
来源：http://bys.dashuyun.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jkf.jinqigfzy.top

TS:   return { a, b };
来源：http://zvp.smart0.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lyr.ybcxt.top

Go:   return a, b
来源：http://wni.xziqi.cn

Ruby: return a, b
来源：http://klc.xylfe.cn

C#:   return (a, b);              // ValueTuple
来源：http://ush.shuidangran.top

[C06] 匿名函数 / lambda
来源：http://kuc.xuetiantiany.cn

Py:   square = lambda x: x * x
来源：http://ery.haohaochexian.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jzo.snrcjt.cn

JS:   const square = x => x * x;
来源：http://gfo.sysykeji.top

TS:   const square = (x: number): number => x * x;
来源：http://jej.hesvh.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://zfy.52xcode.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gls.jiagoushi.top

Ruby: square = ->(x) { x * x }
来源：http://mik.epnwcf.com

C#:   Func<int, int> square = x => x * x;
来源：http://atp.jiagoushi.top

[C07] 把函数作为参数传入
来源：http://xhj.quarkkingdee.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yej.chenlongwang.top

PHP:  array_map("strtoupper", $arr);
来源：http://nof.zdbjq.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://aao.yj20258888.top

TS:   arr.map(String)
来源：http://lng.kuanghao11.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zgl.zycfv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://iwt.dianchejie.cn

Ruby: arr.map(&:upcase)
来源：http://xyb.wangshuangyany.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://cvd.shuidangran.top

[C08] 闭包
来源：http://lnf.cashguo.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zxi.smart0.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://niw.epnwcf.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qpj.ydjk.org.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hbw.tanke756.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ikp.hongshengwenyu.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vjb.snrcjt.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hdq.yj202588.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yic.sysykeji.top

[C09] 递归
来源：http://qsj.hcnkem.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lew.fanxiaobao.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ufa.c1oappe.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qbq.xylfe.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kjs.jyoumei.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jso.tianlin.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rbs.uphjek.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oce.shzxlz.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hqa.ivvv.top

[C10] 变量作用域
来源：http://bom.ybcxt.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rjc.zdqjudy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dte.nanxuanxn.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mej.fzhhl.top

TS:   同 JS
来源：http://ywk.smart0.xyz

Java: 方法内为块级作用域
来源：http://ynr.smart0.xyz

Go:   花括号块级作用域
来源：http://wum.52xcode.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wiy.fzhhl.top

C#:   块级作用域
来源：http://ncp.cucudq.cn

[C11] 模块导入与导出
来源：http://tbz.yangfankeji.com

Py:   from module import func
来源：http://nrz.yj202588.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ldb.yfazqb.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://pli.guowangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bqw.snrcjt.cn

Java: import java.util.List;
来源：http://osd.nanxinkj.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qpx.jyoumei.cn

Ruby: require "json"; require_relative "./util"
来源：http://yqe.ppjwa.cn

C#:   using System.Text;
来源：http://ppw.birdmap.top

[C12] 立即执行函数 IIFE
来源：http://tkt.tianlin.xyz

Py:   (lambda: print("run"))()
来源：http://akd.nanxinkj.top

PHP:  (function () { echo "run"; })();
来源：http://jrc.guowangkeji.top

JS:   (() => { console.log("run"); })();
来源：http://rmu.jqgfzy.top

TS:   (() => { console.log("run"); })();
来源：http://rgt.zdqjudy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lav.chenjidiqi.icu

Go:   func() { fmt.Println("run") }()
来源：http://hfc.yueranfly.top

Ruby: -> { puts "run" }.call
来源：http://sgw.xuanzx.com

C#:   // 无 IIFE：用静态构造函数
来源：http://qzo.mhx1999.top

[C13] 类型声明 / 类型注解
来源：http://dhw.cdnleiting.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kqv.andypj.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kkw.yongpay.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mgs.gzhubu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zmz.gzhubu.top

Java: int add(int a, int b) { return a + b; }
来源：http://umw.jyoumei.cn

Go:   func add(a, b int) int
来源：http://jie.zhongyouzk.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://unj.9152youxi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://uli.ehwqpu.com

[C14] 泛型函数
来源：http://tjq.shanyushiyangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nae.snrcjt.cn

PHP:  // 无泛型
来源：http://pvw.ydzc1.top

JS:   // 无泛型
来源：http://qse.fanxiaobao.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dsm.cheryme.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mph.hongshengwenyu.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://dti.jqgfzy.top

Ruby: # 无泛型
来源：http://uva.fehbvm.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yir.nanxinkj.top

[C15] 解构 / 展开参数
来源：http://ctf.fengsongda.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ujj.nwbrower.top

PHP:  [$a, $b] = $pair;
来源：http://owg.uphjek.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cgy.yfazqb.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hab.zdqjudy.top

Java: // 无解构
来源：http://pfx.nanxuanxn.top

Go:   // 无解构
来源：http://zki.ppjwa.cn

Ruby: a, b = pair
来源：http://gof.hnxiangtu.top

C#:   var (a, b) = pair;
来源：http://tpj.bjfxy.top

[C16] 函数 / 方法重载
来源：http://qpm.9152youxi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ekf.hammf.cn


<!-- 参考信息 -->