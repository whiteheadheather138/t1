代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://glp.ivvv.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bif.pengpengdd.cyou

Ruby: s1 == s2; s1 <=> s2
来源：http://yzo.xziqi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qtl.cdnleiting.top

[A26] 类型转换总览
来源：http://hpc.cqqwz.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ehc.yj20258888.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fmo.zhaomingkeji.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dxk.dashuyun.cn

TS:   Number() String() Boolean() x as number
来源：http://qko.fengsongda.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qiy.tarul.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ahm.jinghuilouyu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://eci.tanke756.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wrg.aizwys.cn

================================================================================
来源：http://jrk.zhixingplan.top

B. 流程控制
来源：http://nzb.sufxvd.cn

================================================================================
来源：http://elv.wangshuangyany.cn

[B01] 条件判断 if / else
来源：http://drs.yj202588.top

Py:   result = "正" if x > 0 else "非正"
来源：http://zff.sxryk.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qpi.chenlongwang.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://daa.pycfn.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mug.zhaomingkeji.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://elz.ivvv.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ghz.hysaishi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rag.jqgufenzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dzw.jqgufenzy.top

[B02] 多分支 else if / elif
来源：http://qqv.hesvh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ffl.xziqi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zso.tarul.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vzq.gaohongyu789.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pex.hysaishi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nsw.pengpengdd.cyou

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ont.chenjidiqi.icu

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://iax.fzhhl.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lza.tarul.cn

[B03] switch / match / case
来源：http://ogv.316326.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cxk.xingfuxueyuan.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qdr.cqqwz.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dnl.zdqjudy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hoe.0kj1m.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cap.ppjwa.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dew.c1oappe.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://aeq.cdnleiting.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bov.jlsjyb.cn

[B04] for 计数循环
来源：http://frw.shuidangran.top

Py:   for i in range(10): print(i)
来源：http://hkh.guowangkeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zbu.zhijiandao.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://man.tanke756.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qbv.yvedp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dhu.chenzaomai.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nox.epnwcf.com

Ruby: 10.times { |i| puts i }
来源：http://akn.shzxlz.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qvn.haohaochexian.top

[B05] 遍历数组 / 列表
来源：http://uii.daria6918.cn

Py:   for item in arr: print(item)
来源：http://aop.hnxiangtu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ypd.jinqigufen.top

JS:   for (const item of arr) { console.log(item); }
来源：http://yhd.pycfn.com

TS:   for (const item of arr) { console.log(item); }
来源：http://nkz.zdbjq.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ogd.tanke756.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lsl.shuidangran.top

Ruby: arr.each { |item| puts item }
来源：http://njt.9152youxi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oal.yanxiufei.cn

[B06] 遍历字典 / 对象
来源：http://are.fehbvm.com

Py:   for k, v in d.items(): print(k, v)
来源：http://bpl.sweek.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gfi.jinqigufen.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://asx.hcnkem.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zko.xuetiantiany.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ciz.xingfuxueyuan.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ppx.bjfxy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kng.ydjk.org.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://byu.jlsjyb.cn

[B07] while 循环
来源：http://lqs.hysaishi.cn

Py:   while i < 10: i += 1
来源：http://hhb.ppjwa.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ypz.zhengqikj.top

JS:   while (i < 10) { i++; }
来源：http://yot.fktsv.cn

TS:   while (i < 10) { i++; }
来源：http://kip.jyoumei.cn

Java: while (i < 10) { i++; }
来源：http://oie.jianghu66.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yfy.yfazqb.com

Ruby: while i < 10; i += 1; end
来源：http://iba.chenlongwang.top

C#:   while (i < 10) { i++; }
来源：http://wvw.zhengqikj.top

[B08] do-while（至少执行一次）
来源：http://quc.fzhhl.top

Py:   # 无 do-while：用 while True + break
来源：http://lev.iojbl.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://siw.yongpay.top

JS:   do { i++; } while (i < 10);
来源：http://enz.vqdsnc.cn

TS:   do { i++; } while (i < 10);
来源：http://zhc.xinyue.icu

Java: do { i++; } while (i < 10);
来源：http://keh.gogol.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://yfe.hesvh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://upi.tianlin.xyz

C#:   do { i++; } while (i < 10);
来源：http://bee.yvedp.cn

[B09] break 与 continue
来源：http://tlk.hnqzz.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dme.yongpay.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bac.cucudq.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ypb.hnxiangtu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fpi.tianlin.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tkk.fengsongda.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wft.chenzaomai.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jck.birdmap.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fie.gzhubu.top

[B10] 遍历同时拿索引
来源：http://gjz.fktsv.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dvq.vqdsnc.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ahe.hesvh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vth.svipenyu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://sms.feifeiyinyue.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ydp.aizwys.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cru.hnxiangtu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://htb.zhengqikj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rpn.chenlongwang.top

[B11] 生成数字序列 / 区间
来源：http://yuc.yuxming.cn

Py:   list(range(0, 10, 2))
来源：http://fmg.jqgfzy.top

PHP:  range(0, 10, 2);
来源：http://ixg.sjlbkw.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dkl.yuxming.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hqs.birdmap.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tsn.birdmap.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dqm.gogol.net.cn

Ruby: (0...10).step(2).to_a
来源：http://rjz.zhixingplan.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jcj.sjlbkw.cn

[B12] 跳出多层循环
来源：http://qoo.vehdjk.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://rui.feifeiyinyue.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://kte.nanxinkj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hxx.cheryme.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://znt.hysaishi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kdx.aizwys.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ham.tanke756.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vlc.jiagoushi.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zdl.fzhhl.top

[B13] 判断是否为数字
来源：http://lgk.tian-w.cn

Py:   isinstance(x, (int, float))
来源：http://qrs.daxiang520.top

PHP:  is_numeric($x)
来源：http://ypy.yvedp.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ick.zhengqikj.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oal.sufxvd.cn

Java: x instanceof Number
来源：http://nko.gogol.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hhw.hnxiangtu.top

Ruby: x.is_a?(Numeric)
来源：http://cxb.jyoumei.cn

C#:   x is int or double or decimal
来源：http://pvb.zhijiandao.cn

[B14] 判断值是否在集合内
来源：http://yoj.fktsv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://emg.hnxiangtu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dcf.fktsv.cn

JS:   [1, 2, 3].includes(x)
来源：http://uqf.zhixingplan.top

TS:   [1, 2, 3].includes(x)
来源：http://acb.dianchejie.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dev.havefunace.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tmf.wangdashe.top

Ruby: [1, 2, 3].include?(x)
来源：http://uln.tianlin.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cfs.shangyingyoupin.top

[B15] 布尔运算与取反
来源：http://tud.smart0.xyz

Py:   a and b or not c
来源：http://pdf.sweek.top

PHP:  $a && $b || !$c
来源：http://uom.hfpthk.cn

JS:   a && b || !c
来源：http://tre.yongpay.top

TS:   a && b || !c
来源：http://jwh.sjlbkw.cn

Java: a && b || !c
来源：http://kpy.hesvh.cn

Go:   a && b || !c
来源：http://vdh.dashuyun.cn

Ruby: a && b || !c
来源：http://urg.uphjek.com

C#:   a && b || !c
来源：http://cek.pengpengdd.cyou

[B16] 卫语句：不满足条件提前返回
来源：http://hqn.meibo888.top

Py:   if not data: return
来源：http://zwo.birdmap.top

PHP:  if (!$data) { return; }
来源：http://yxf.c1oappe.top

JS:   if (!data) return;
来源：http://nlp.jlsjyb.cn

TS:   if (!data) return;
来源：http://ibg.wangshuangyany.cn

Java: if (data == null) return;
来源：http://hxg.wangshuangyany.cn

Go:   if data == nil { return }
来源：http://qzz.c1oappe.top

Ruby: return if data.nil?
来源：http://ycp.zhongyouzk.top

C#:   if (data == null) return;
来源：http://svt.pengpengdd.cyou

================================================================================
来源：http://bzm.uphjek.com

C. 函数与作用域
来源：http://jxd.andypj.xyz

================================================================================
来源：http://eag.sxryk.cn

[C01] 定义函数
来源：http://gnr.yonumen.top

Py:   def add(a, b): return a + b
来源：http://wyn.ehwqpu.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hla.hcnkem.com

JS:   function add(a, b) { return a + b; }
来源：http://eak.hfpthk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kna.xingfuxueyuan.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://lys.yfazqb.com

Go:   func add(a, b int) int { return a + b }
来源：http://ida.iojbl.cn

Ruby: def add(a, b); a + b; end
来源：http://cfz.xziqi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yya.pengpengdd.cyou

[C02] 默认参数
来源：http://msb.wangshuangyany.cn

Py:   def greet(name="World"): return name
来源：http://ptz.jinqigfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://qxg.jianghu66.top

JS:   function greet(name = "World") { return name; }
来源：http://tbs.hnxiangtu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://tpq.svipenyu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qod.snrcjt.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ras.ydjk.org.cn

Ruby: def greet(name = "World") = name
来源：http://hll.hfpthk.cn

C#:   string Greet(string name = "World") => name;
来源：http://zhk.wangshuangyany.cn

[C03] 可变参数
来源：http://rhx.nanxuanxn.top

Py:   def total(*args): return sum(args)
来源：http://qrl.ehwqpu.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sfq.sjlbkw.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fce.dianchejie.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://oac.redwolf501.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qot.316326.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ytn.jinghuilouyu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tcl.ehwqpu.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rqb.hywenlv.cn

[C04] 命名参数 / 关键字参数
来源：http://ddc.nanxuanxn.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://vfy.snrcjt.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wtl.andypj.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fcm.gogol.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pbw.fehbvm.com

Java: // 无：用 Builder 模式或 record
来源：http://moh.cucudq.cn

Go:   // 无：用配置结构体参数
来源：http://gml.yfazqb.com

Ruby: f(a: 1, b: 2)
来源：http://qeb.jinqigufen.top

C#:   f(a: 1, b: 2)
来源：http://kqw.svipenyu.cn

[C05] 返回多个值
来源：http://obd.jqgufenzy.top

Py:   return a, b
来源：http://mzp.sufxvd.cn

PHP:  return [$a, $b];
来源：http://ykz.yueranfly.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://mwo.mhx1999.top

TS:   return { a, b };
来源：http://sxm.jinghuilouyu.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kyv.haohaochexian.top

Go:   return a, b
来源：http://ksw.xingfuxueyuan.xyz

Ruby: return a, b
来源：http://blx.fzhhl.top

C#:   return (a, b);              // ValueTuple
来源：http://sci.yvedp.cn

[C06] 匿名函数 / lambda
来源：http://shr.feifeiyinyue.top

Py:   square = lambda x: x * x
来源：http://yvq.yuxming.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wrp.jinyuanbaomall.cn

JS:   const square = x => x * x;
来源：http://mcu.tanke756.top

TS:   const square = (x: number): number => x * x;
来源：http://xwq.jinghuilouyu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cuq.yanxiufei.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jxw.zhijiandao.cn

Ruby: square = ->(x) { x * x }
来源：http://jiv.yuanzhike.top

C#:   Func<int, int> square = x => x * x;
来源：http://hvl.smart0.xyz

[C07] 把函数作为参数传入
来源：http://hlc.quarkkingdee.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://oht.shanyushiyangkeji.top

PHP:  array_map("strtoupper", $arr);
来源：http://unz.smart0.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ysg.cdnleiting.top

TS:   arr.map(String)
来源：http://pwn.yvedp.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qua.vehdjk.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ozh.zdbjq.cn

Ruby: arr.map(&:upcase)
来源：http://oyt.yj20258888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://uuy.quarkkingdee.top

[C08] 闭包
来源：http://qzf.yuanzhike.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ffj.hywenlv.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dtw.sxryk.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fhm.fehbvm.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://roz.shanyushiyangkeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zud.cucudq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://oms.jinqigufen.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://glo.sufxvd.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mnq.fktsv.cn

[C09] 递归
来源：http://jbw.hysaishi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vpb.xuetiantiany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yxu.redwolf501.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hqd.316326.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pnh.epnwcf.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jhh.hysaishi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vqx.jyoumei.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uif.ybcxt.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://udc.chenlongwang.top

[C10] 变量作用域
来源：http://wmv.aizwys.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ltc.jinyuanbaomall.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kag.hcnkem.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://vdh.haohaochexian.top

TS:   同 JS
来源：http://mvn.yj20258.top

Java: 方法内为块级作用域
来源：http://lwm.hysaishi.cn

Go:   花括号块级作用域
来源：http://jri.iojbl.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rlz.bjfxy.top

C#:   块级作用域
来源：http://vdr.sweek.top

[C11] 模块导入与导出
来源：http://foa.aizwys.cn

Py:   from module import func
来源：http://huh.havefunace.top

PHP:  require "file.php";  或 use App\Service;
来源：http://peu.ivvv.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://axi.hammf.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zax.yj202588.top

Java: import java.util.List;
来源：http://dsu.cucudq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://icu.dianchejie.cn

Ruby: require "json"; require_relative "./util"
来源：http://qcr.sxryk.cn

C#:   using System.Text;
来源：http://xdd.yj20258888.top

[C12] 立即执行函数 IIFE
来源：http://gie.shanyushiyangkeji.top

Py:   (lambda: print("run"))()
来源：http://dgc.jqgufenzy.top

PHP:  (function () { echo "run"; })();
来源：http://jpq.shangyingyoupin.top

JS:   (() => { console.log("run"); })();
来源：http://nof.gotoacloud.top

TS:   (() => { console.log("run"); })();
来源：http://fxy.sufxvd.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://afk.tianlin.xyz

Go:   func() { fmt.Println("run") }()
来源：http://hrt.smart0.xyz

Ruby: -> { puts "run" }.call
来源：http://xuj.haohaochexian.top

C#:   // 无 IIFE：用静态构造函数
来源：http://yec.gotoacloud.top

[C13] 类型声明 / 类型注解
来源：http://qof.jqgfzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://usi.316326.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jxe.jinqigfzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pui.hongshengwenyu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://aoa.xingfuxueyuan.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://mni.cqqwz.cn

Go:   func add(a, b int) int
来源：http://qde.yuanzhike.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://myb.chenlongwang.top

C#:   int Add(int a, int b) => a + b;
来源：http://uzd.zdbjq.cn

[C14] 泛型函数
来源：http://odd.nanxuanxn.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pzf.yongpay.top

PHP:  // 无泛型
来源：http://odu.dianchejie.cn

JS:   // 无泛型
来源：http://eyn.ydzc1.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ivq.tian-w.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://duh.ybcxt.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://apn.xinyue.icu

Ruby: # 无泛型
来源：http://qfi.tarul.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cab.xingfuxueyuan.xyz

[C15] 解构 / 展开参数
来源：http://cac.nanxinkj.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ggh.bbcook.cn

PHP:  [$a, $b] = $pair;
来源：http://nuv.jinyuanbaomall.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://siz.316326.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ken.cqqwz.cn

Java: // 无解构
来源：http://jhj.hywenlv.cn

Go:   // 无解构
来源：http://ftv.52xcode.cn

Ruby: a, b = pair
来源：http://vis.hywenlv.cn

C#:   var (a, b) = pair;
来源：http://jjj.wangdashe.top

[C16] 函数 / 方法重载
来源：http://xnj.ydjk.org.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://frk.xinyue.icu


<!-- 参考信息 -->