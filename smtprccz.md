代发 wailian999

[A26] 类型转换总览
来源：http://uei.shuidangran.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://upi.hnxiangtu.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ysk.shanyushiyangkeji.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://okh.ivvv.top

TS:   Number() String() Boolean() x as number
来源：http://ecf.jlsjyb.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hdc.aizwys.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://esa.yj20258.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://oih.hfpthk.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sac.yanxiufei.cn

================================================================================
来源：http://vxw.guowangkeji.top

B. 流程控制
来源：http://dtf.meibo888.top

================================================================================
来源：http://ugh.zhengqikj.top

[B01] 条件判断 if / else
来源：http://mwa.sweek.top

Py:   result = "正" if x > 0 else "非正"
来源：http://wne.redwolf501.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ywt.havefunace.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xkq.hcnkem.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ksv.feifeiyinyue.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://dao.yj202588.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fsk.birdmap.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wvx.jiagoushi.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bcq.xingfuxueyuan.xyz

[B02] 多分支 else if / elif
来源：http://hiq.gzhubu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zoz.fzhhl.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xfd.feifeiyinyue.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mxn.tanke756.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fsm.tanke756.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uak.yvedp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xyy.pengpengdd.cyou

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tzb.hcnkem.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bmh.svipenyu.cn

[B03] switch / match / case
来源：http://foc.shangyingyoupin.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qoe.yangfankeji.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sgj.zhengqikj.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ypo.wangdashe.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://szy.shanyushiyangkeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hmj.xylfe.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://igw.shangyingyoupin.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://enm.gotoacloud.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xsf.cucudq.cn

[B04] for 计数循环
来源：http://ygf.ydjk.org.cn

Py:   for i in range(10): print(i)
来源：http://vat.mhx1999.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tik.shangyingyoupin.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eab.ybcxt.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://isk.jianghu66.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gxz.gogol.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tuh.havefunace.top

Ruby: 10.times { |i| puts i }
来源：http://itz.jinqigufen.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pgs.hesvh.cn

[B05] 遍历数组 / 列表
来源：http://ahn.jlsjyb.cn

Py:   for item in arr: print(item)
来源：http://kxz.cqqwz.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vzd.xuetiantiany.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://euc.yuanzhike.top

TS:   for (const item of arr) { console.log(item); }
来源：http://rwi.ywan-chungtsiang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://mll.meibo888.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cnc.ppjwa.cn

Ruby: arr.each { |item| puts item }
来源：http://tqi.epnwcf.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dlp.gzhubu.top

[B06] 遍历字典 / 对象
来源：http://mda.zhaomingkeji.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://cgi.cheryme.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wjz.ctjpmb.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qvy.yangfankeji.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dqu.iojbl.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uec.yuanzhike.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jgx.dianchejie.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qyp.fktsv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gna.sufxvd.cn

[B07] while 循环
来源：http://kpo.smart0.xyz

Py:   while i < 10: i += 1
来源：http://ysk.xuanzx.com

PHP:  while ($i < 10) { $i++; }
来源：http://xtl.andypj.xyz

JS:   while (i < 10) { i++; }
来源：http://hgi.nanxuanxn.top

TS:   while (i < 10) { i++; }
来源：http://rwl.hongshengwenyu.top

Java: while (i < 10) { i++; }
来源：http://wcj.jinghuilouyu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yaj.zdqjudy.top

Ruby: while i < 10; i += 1; end
来源：http://vnd.zhixingplan.top

C#:   while (i < 10) { i++; }
来源：http://kho.mhx1999.top

[B08] do-while（至少执行一次）
来源：http://ntb.iojbl.cn

Py:   # 无 do-while：用 while True + break
来源：http://vud.tianlin.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://ivt.zhongyouzk.top

JS:   do { i++; } while (i < 10);
来源：http://uez.feifeiyinyue.top

TS:   do { i++; } while (i < 10);
来源：http://oth.tarul.cn

Java: do { i++; } while (i < 10);
来源：http://xvq.yj20258888.top

Go:   for { i++; if i >= 10 { break } }
来源：http://buk.xziqi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fkv.aizwys.cn

C#:   do { i++; } while (i < 10);
来源：http://gnc.aizwys.cn

[B09] break 与 continue
来源：http://jan.yfazqb.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yib.haohaochexian.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qps.yuanzhike.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qzf.tian-w.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hju.tian-w.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eff.xuanzx.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dbr.jqgufenzy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://agn.shuidangran.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kxs.zdqjudy.top

[B10] 遍历同时拿索引
来源：http://fcg.xinyue.icu

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lkt.birdmap.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dtl.0kj1m.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pgc.zhijiandao.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bux.zhiwuduotai.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rwk.sjlbkw.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rca.jinqigfzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hsq.yuanzhike.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dvw.shanyushiyangtech.top

[B11] 生成数字序列 / 区间
来源：http://ftv.cheryme.top

Py:   list(range(0, 10, 2))
来源：http://cmi.hcnkem.com

PHP:  range(0, 10, 2);
来源：http://gtj.hfpthk.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qbo.yfazqb.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gdu.wangdashe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ryn.yfazqb.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vrt.hnqzz.top

Ruby: (0...10).step(2).to_a
来源：http://ijb.zdqjudy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mdh.iojbl.cn

[B12] 跳出多层循环
来源：http://zqx.xuetiantiany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nzr.yvedp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://kfo.kuanghao11.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ljh.tarul.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jsj.mhx1999.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lvp.iojbl.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://aed.sweek.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wty.tianlin.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://unu.feifeiyinyue.top

[B13] 判断是否为数字
来源：http://maw.cashguo.top

Py:   isinstance(x, (int, float))
来源：http://lyq.sjlbkw.cn

PHP:  is_numeric($x)
来源：http://yyc.zhixingplan.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tjf.yueranfly.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gkg.chenzaomai.com

Java: x instanceof Number
来源：http://fvo.ydjk.org.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://min.wangdashe.top

Ruby: x.is_a?(Numeric)
来源：http://ykg.yvedp.cn

C#:   x is int or double or decimal
来源：http://bup.316326.xyz

[B14] 判断值是否在集合内
来源：http://bxk.sjlbkw.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fux.fengsongda.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rns.dashuyun.cn

JS:   [1, 2, 3].includes(x)
来源：http://hbu.jinqigfzy.top

TS:   [1, 2, 3].includes(x)
来源：http://giv.sxryk.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://aio.hesvh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ams.hongshengwenyu.top

Ruby: [1, 2, 3].include?(x)
来源：http://vfi.redwolf501.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jtc.dianchejie.cn

[B15] 布尔运算与取反
来源：http://hev.52xcode.cn

Py:   a and b or not c
来源：http://kse.zhongyouzk.top

PHP:  $a && $b || !$c
来源：http://lps.zhengqikj.top

JS:   a && b || !c
来源：http://pcz.zdqjudy.top

TS:   a && b || !c
来源：http://hft.redwolf501.top

Java: a && b || !c
来源：http://zgw.gotoacloud.top

Go:   a && b || !c
来源：http://jky.fehbvm.com

Ruby: a && b || !c
来源：http://nbm.ppjwa.cn

C#:   a && b || !c
来源：http://yhj.fehbvm.com

[B16] 卫语句：不满足条件提前返回
来源：http://ldf.yueranfly.top

Py:   if not data: return
来源：http://ots.gzhubu.top

PHP:  if (!$data) { return; }
来源：http://sqn.guowangkeji.top

JS:   if (!data) return;
来源：http://dar.hfpthk.cn

TS:   if (!data) return;
来源：http://viq.yonumen.top

Java: if (data == null) return;
来源：http://dwc.andypj.xyz

Go:   if data == nil { return }
来源：http://yzz.ivvv.top

Ruby: return if data.nil?
来源：http://ubr.shanyushiyangkeji.top

C#:   if (data == null) return;
来源：http://ell.ydzc1.top

================================================================================
来源：http://ujn.pengpengdd.cyou

C. 函数与作用域
来源：http://wrv.xinyue.icu

================================================================================
来源：http://jdx.xziqi.cn

[C01] 定义函数
来源：http://jzf.fzhhl.top

Py:   def add(a, b): return a + b
来源：http://kmt.dianchejie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://boz.yanxiufei.cn

JS:   function add(a, b) { return a + b; }
来源：http://lag.vehdjk.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mnz.uphjek.com

Java: static int add(int a, int b) { return a + b; }
来源：http://zrn.fengsongda.top

Go:   func add(a, b int) int { return a + b }
来源：http://ncm.hesvh.cn

Ruby: def add(a, b); a + b; end
来源：http://gwi.jqgfzy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iaf.hnqzz.top

[C02] 默认参数
来源：http://vwx.zhaomingkeji.xyz

Py:   def greet(name="World"): return name
来源：http://xbk.epnwcf.com

PHP:  function greet($name = "World") { return $name; }
来源：http://jze.gogol.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://fzv.shzxlz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://oqh.tian-w.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lbd.xziqi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dta.hammf.cn

Ruby: def greet(name = "World") = name
来源：http://ndb.xylfe.cn

C#:   string Greet(string name = "World") => name;
来源：http://mri.ivvv.top

[C03] 可变参数
来源：http://slk.wangshuangyany.cn

Py:   def total(*args): return sum(args)
来源：http://mjq.jinqigufen.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vdn.daria6918.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wbe.jianghu66.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yqy.9152youxi.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sua.yanxiufei.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fcf.shangyingyoupin.top

Ruby: def total(*nums); nums.sum; end
来源：http://hdn.chenzaomai.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ncr.cqqwz.cn

[C04] 命名参数 / 关键字参数
来源：http://cyn.yfazqb.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://esn.iojbl.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aaf.sxryk.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://kdf.feifeiyinyue.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mff.chenjidiqi.icu

Java: // 无：用 Builder 模式或 record
来源：http://anu.jqgfzy.top

Go:   // 无：用配置结构体参数
来源：http://ohp.kuanghao11.cn

Ruby: f(a: 1, b: 2)
来源：http://pld.gotoacloud.top

C#:   f(a: 1, b: 2)
来源：http://vet.hfpthk.cn

[C05] 返回多个值
来源：http://ykf.zhoulong.xyz

Py:   return a, b
来源：http://dco.yongpay.top

PHP:  return [$a, $b];
来源：http://xgr.fehbvm.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://sci.zhongyouzk.top

TS:   return { a, b };
来源：http://gjq.zdbjq.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lkw.52xcode.cn

Go:   return a, b
来源：http://vrd.xinyue.icu

Ruby: return a, b
来源：http://eoh.chenzaomai.com

C#:   return (a, b);              // ValueTuple
来源：http://wat.tianlin.xyz

[C06] 匿名函数 / lambda
来源：http://uzz.bbcook.cn

Py:   square = lambda x: x * x
来源：http://slm.xziqi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://piu.daria6918.cn

JS:   const square = x => x * x;
来源：http://udw.redwolf501.top

TS:   const square = (x: number): number => x * x;
来源：http://jjn.shanyushiyangtech.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xhw.chenzaomai.com

Go:   sq := func(x int) int { return x * x }
来源：http://gmk.daria6918.cn

Ruby: square = ->(x) { x * x }
来源：http://fck.yonumen.top

C#:   Func<int, int> square = x => x * x;
来源：http://hjz.gogol.net.cn

[C07] 把函数作为参数传入
来源：http://lwk.nanxinkj.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sho.jinqigufen.top

PHP:  array_map("strtoupper", $arr);
来源：http://lwq.ppjwa.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qfd.fehbvm.com

TS:   arr.map(String)
来源：http://omr.xingfuxueyuan.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pwz.shanyushiyangkeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dfn.ppjwa.cn

Ruby: arr.map(&:upcase)
来源：http://pqv.fzhhl.top

C#:   arr.Select(s => s.ToUpper())
来源：http://raw.havefunace.top

[C08] 闭包
来源：http://hem.iojbl.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ftw.wangdashe.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lxk.redwolf501.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vun.c1oappe.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://jet.fzhhl.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sho.yj20258888.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mof.ehwqpu.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gev.jqgfzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zfs.gotoacloud.top

[C09] 递归
来源：http://isw.ybcxt.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ogx.jinqigufen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rso.epnwcf.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tsj.9152youxi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xyd.cucudq.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://iih.wangshuangyany.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zye.fanxiaobao.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pdx.zhiwuduotai.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ndj.guannengcc.top

[C10] 变量作用域
来源：http://gyo.nwbrower.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yuz.gotoacloud.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lrk.yanxiufei.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gsi.feifeiyinyue.top

TS:   同 JS
来源：http://rxh.cashguo.top

Java: 方法内为块级作用域
来源：http://lpo.c1oappe.top

Go:   花括号块级作用域
来源：http://hvf.nanxuanxn.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hxm.daxiang520.top

C#:   块级作用域
来源：http://ryq.jiagoushi.top

[C11] 模块导入与导出
来源：http://xjd.jinyuanbaomall.cn

Py:   from module import func
来源：http://xru.smart0.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://qrf.0kj1m.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://tij.vqdsnc.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lae.hysaishi.cn

Java: import java.util.List;
来源：http://oct.zhiwuduotai.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nbk.cucudq.cn

Ruby: require "json"; require_relative "./util"
来源：http://ahk.ppjwa.cn

C#:   using System.Text;
来源：http://eex.snrcjt.cn

[C12] 立即执行函数 IIFE
来源：http://cjt.hnxiangtu.top

Py:   (lambda: print("run"))()
来源：http://eds.vqdsnc.cn

PHP:  (function () { echo "run"; })();
来源：http://xqi.tian-w.cn

JS:   (() => { console.log("run"); })();
来源：http://dsz.52xcode.cn

TS:   (() => { console.log("run"); })();
来源：http://esg.uphjek.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ycf.daxiang520.top

Go:   func() { fmt.Println("run") }()
来源：http://mnw.hcnkem.com

Ruby: -> { puts "run" }.call
来源：http://obd.yongpay.top

C#:   // 无 IIFE：用静态构造函数
来源：http://mdc.316326.xyz

[C13] 类型声明 / 类型注解
来源：http://wls.vqdsnc.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xku.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yxg.yj202588.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ebq.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wep.gaohongyu789.top

Java: int add(int a, int b) { return a + b; }
来源：http://eim.shangyingyoupin.top

Go:   func add(a, b int) int
来源：http://awy.kuanghao11.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rpt.316326.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://dsb.cdnleiting.top

[C14] 泛型函数
来源：http://lbk.sweek.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bde.pengpengdd.cyou

PHP:  // 无泛型
来源：http://urz.wangshuangyany.cn

JS:   // 无泛型
来源：http://qkt.xuanzx.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jvw.zhaomingkeji.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jfd.yanxiufei.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yxq.chenlongwang.top

Ruby: # 无泛型
来源：http://lde.gzhubu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wvf.wangshuangyany.cn

[C15] 解构 / 展开参数
来源：http://qhk.uphjek.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://eql.xziqi.cn

PHP:  [$a, $b] = $pair;
来源：http://cug.xuetiantiany.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qfu.ydzc1.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hek.zhiwuduotai.top

Java: // 无解构
来源：http://uzl.shuidangran.top

Go:   // 无解构
来源：http://ghh.chenzaomai.com

Ruby: a, b = pair
来源：http://shn.9152youxi.cn

C#:   var (a, b) = pair;
来源：http://lfs.gaohongyu789.top

[C16] 函数 / 方法重载
来源：http://dca.yangfankeji.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qai.yfazqb.com

PHP:  // 无重载
来源：http://bzw.ivvv.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://rbd.ywan-chungtsiang.top

TS:   // 用联合类型或重载签名声明
来源：http://aun.yanxiufei.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kgw.zhixingplan.top


<!-- 参考信息 -->