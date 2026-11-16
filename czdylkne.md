代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://ivc.xziqi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ffp.nanxuanxn.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://enl.svipenyu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://pdu.zhijiandao.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hxc.zhoulong.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hgj.epnwcf.com

Ruby: s1 == s2; s1 <=> s2
来源：http://ktm.dashuyun.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zmb.ybcxt.top

[A26] 类型转换总览
来源：http://uzg.ehwqpu.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vkl.fanxiaobao.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sla.fktsv.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lja.jinghuilouyu.cn

TS:   Number() String() Boolean() x as number
来源：http://jpp.9152youxi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://aoy.xziqi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pox.zhongyouzk.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://guc.nanxuanxn.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xak.jinghuilouyu.cn

================================================================================
来源：http://fzc.ywan-chungtsiang.top

B. 流程控制
来源：http://fci.zhiwuduotai.top

================================================================================
来源：http://wpt.jinqigufen.top

[B01] 条件判断 if / else
来源：http://mlm.jqgufenzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://plv.sysykeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sqq.chenzaomai.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ohb.bbcook.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nth.yfazqb.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://pxq.zhengqikj.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bth.sxryk.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qlt.yj20258.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vlj.chenzaomai.com

[B02] 多分支 else if / elif
来源：http://sch.haohaochexian.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gkv.wangshuangyany.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bow.yonumen.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nud.ybcxt.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cui.andypj.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jiw.hcnkem.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vjl.yanxiufei.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uxu.nanxuanxn.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qqg.jiagoushi.top

[B03] switch / match / case
来源：http://snx.shanyushiyangtech.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://smt.xuetiantiany.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cea.yj20258.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xoq.shangyingyoupin.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dop.zhixingplan.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dkt.yfazqb.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wya.xinyue.icu

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://imr.jqgfzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://yny.fktsv.cn

[B04] for 计数循环
来源：http://lnz.zhoulong.xyz

Py:   for i in range(10): print(i)
来源：http://dng.yvedp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://phh.fengsongda.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eoi.zhaomingkeji.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hin.cheryme.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nxn.ehwqpu.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dwl.xingfuxueyuan.xyz

Ruby: 10.times { |i| puts i }
来源：http://glm.chenjidiqi.icu

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zmp.daxiang520.top

[B05] 遍历数组 / 列表
来源：http://smn.zhiwuduotai.top

Py:   for item in arr: print(item)
来源：http://ekf.guannengcc.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gdm.cqqwz.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://acf.cashguo.top

TS:   for (const item of arr) { console.log(item); }
来源：http://gie.cqqwz.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vzo.sjlbkw.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pkj.wangdashe.top

Ruby: arr.each { |item| puts item }
来源：http://snj.sjlbkw.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ksf.uphjek.com

[B06] 遍历字典 / 对象
来源：http://cun.ywan-chungtsiang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://osq.tianlin.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wjx.wangdashe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cti.fktsv.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xlf.mhx1999.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wpc.zhiwuduotai.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gxu.shanyushiyangtech.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://spg.zhixingplan.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nml.yuanzhike.top

[B07] while 循环
来源：http://qtw.shangyingyoupin.top

Py:   while i < 10: i += 1
来源：http://exk.jinghuilouyu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://yiq.xylfe.cn

JS:   while (i < 10) { i++; }
来源：http://jbb.jianghu66.top

TS:   while (i < 10) { i++; }
来源：http://pcw.ppjwa.cn

Java: while (i < 10) { i++; }
来源：http://svd.ywan-chungtsiang.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rfc.tarul.cn

Ruby: while i < 10; i += 1; end
来源：http://jdu.jiagoushi.top

C#:   while (i < 10) { i++; }
来源：http://hdc.aizwys.cn

[B08] do-while（至少执行一次）
来源：http://qxg.yonumen.top

Py:   # 无 do-while：用 while True + break
来源：http://bte.yueranfly.top

PHP:  do { $i++; } while ($i < 10);
来源：http://uux.pycfn.com

JS:   do { i++; } while (i < 10);
来源：http://bfi.feifeiyinyue.top

TS:   do { i++; } while (i < 10);
来源：http://eqq.yonumen.top

Java: do { i++; } while (i < 10);
来源：http://bnk.wangshuangyany.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ieo.gzhubu.top

Ruby: begin; i += 1; end while i < 10
来源：http://puj.cqqwz.cn

C#:   do { i++; } while (i < 10);
来源：http://dhc.yanxiufei.cn

[B09] break 与 continue
来源：http://rjr.tian-w.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pfn.gotoacloud.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sez.cheryme.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iqd.guannengcc.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ykk.shzxlz.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mqc.havefunace.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wue.hysaishi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fkm.uphjek.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fgp.52xcode.cn

[B10] 遍历同时拿索引
来源：http://gev.jiagoushi.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vry.yangfankeji.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vee.shangyingyoupin.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vlz.jinqigfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://abi.hysaishi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rvp.aizwys.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kda.hammf.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eny.smart0.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zli.wangdashe.top

[B11] 生成数字序列 / 区间
来源：http://ued.vqdsnc.cn

Py:   list(range(0, 10, 2))
来源：http://ltv.xylfe.cn

PHP:  range(0, 10, 2);
来源：http://boz.jyoumei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ixm.zdbjq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ken.xinyue.icu

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lty.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nfd.jqgfzy.top

Ruby: (0...10).step(2).to_a
来源：http://utb.dianchejie.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mxw.nwbrower.top

[B12] 跳出多层循环
来源：http://vwq.redwolf501.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://qqj.hnqzz.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://art.tanke756.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bjz.havefunace.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xac.tianlin.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zfl.zhixingplan.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://won.svipenyu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lsb.fktsv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jng.0kj1m.cn

[B13] 判断是否为数字
来源：http://qyu.jyoumei.cn

Py:   isinstance(x, (int, float))
来源：http://mam.yj20258.top

PHP:  is_numeric($x)
来源：http://upg.tanke756.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://srd.zycfv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://asc.dianchejie.cn

Java: x instanceof Number
来源：http://mxa.guannengcc.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fzt.jiagoushi.top

Ruby: x.is_a?(Numeric)
来源：http://erk.ydjk.org.cn

C#:   x is int or double or decimal
来源：http://igs.chenlongwang.top

[B14] 判断值是否在集合内
来源：http://kop.9152youxi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://brj.zhijiandao.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://bsg.chenjidiqi.icu

JS:   [1, 2, 3].includes(x)
来源：http://nsh.ydzc1.top

TS:   [1, 2, 3].includes(x)
来源：http://kky.ctjpmb.com

Java: List.of(1, 2, 3).contains(x)
来源：http://tjx.zhixingplan.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://edw.sweek.top

Ruby: [1, 2, 3].include?(x)
来源：http://kbh.fengsongda.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sxy.dianchejie.cn

[B15] 布尔运算与取反
来源：http://jhe.cheryme.top

Py:   a and b or not c
来源：http://fbw.yfazqb.com

PHP:  $a && $b || !$c
来源：http://gfw.fzhhl.top

JS:   a && b || !c
来源：http://vbr.guowangkeji.top

TS:   a && b || !c
来源：http://pga.316326.xyz

Java: a && b || !c
来源：http://fnb.dianchejie.cn

Go:   a && b || !c
来源：http://bsp.shanyushiyangtech.top

Ruby: a && b || !c
来源：http://dmt.jqgfzy.top

C#:   a && b || !c
来源：http://pkg.hnqzz.top

[B16] 卫语句：不满足条件提前返回
来源：http://toc.yj20258.top

Py:   if not data: return
来源：http://ctz.tian-w.cn

PHP:  if (!$data) { return; }
来源：http://tvr.yuxming.cn

JS:   if (!data) return;
来源：http://hmq.guannengcc.top

TS:   if (!data) return;
来源：http://oyk.daxiang520.top

Java: if (data == null) return;
来源：http://xji.sufxvd.cn

Go:   if data == nil { return }
来源：http://xhy.jqgfzy.top

Ruby: return if data.nil?
来源：http://spr.zhongyouzk.top

C#:   if (data == null) return;
来源：http://tna.guowangkeji.top

================================================================================
来源：http://xil.vehdjk.com

C. 函数与作用域
来源：http://bsp.jinghuilouyu.cn

================================================================================
来源：http://pny.yangfankeji.com

[C01] 定义函数
来源：http://bzl.aizwys.cn

Py:   def add(a, b): return a + b
来源：http://kzh.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qhu.fanxiaobao.xyz

JS:   function add(a, b) { return a + b; }
来源：http://oix.yvedp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xuq.jiagoushi.top

Java: static int add(int a, int b) { return a + b; }
来源：http://plz.wangdashe.top

Go:   func add(a, b int) int { return a + b }
来源：http://ata.shanyushiyangkeji.top

Ruby: def add(a, b); a + b; end
来源：http://kzw.chenlongwang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://flh.fzhhl.top

[C02] 默认参数
来源：http://wyp.jinyuanbaomall.cn

Py:   def greet(name="World"): return name
来源：http://iog.xziqi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ciq.xinyue.icu

JS:   function greet(name = "World") { return name; }
来源：http://pal.jinyuanbaomall.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://lix.ydzc1.top

Java: // 无默认参数：方法重载或 Optional
来源：http://sbs.zhijiandao.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ubo.hesvh.cn

Ruby: def greet(name = "World") = name
来源：http://kwc.ydjk.org.cn

C#:   string Greet(string name = "World") => name;
来源：http://ryi.ehwqpu.com

[C03] 可变参数
来源：http://hmt.gaohongyu789.top

Py:   def total(*args): return sum(args)
来源：http://qod.yj20258888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rgt.aibaodan.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kuw.bbcook.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nzq.yj20258.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fih.ywan-chungtsiang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qvd.c1oappe.top

Ruby: def total(*nums); nums.sum; end
来源：http://gtn.bbcook.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ivy.guowangkeji.top

[C04] 命名参数 / 关键字参数
来源：http://jas.hywenlv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://sab.aizwys.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bvf.dianchejie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nvl.jqgufenzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zla.wangshuangyany.cn

Java: // 无：用 Builder 模式或 record
来源：http://mjt.yueranfly.top

Go:   // 无：用配置结构体参数
来源：http://mgu.chenzaomai.com

Ruby: f(a: 1, b: 2)
来源：http://phf.aibaodan.cn

C#:   f(a: 1, b: 2)
来源：http://ybt.pycfn.com

[C05] 返回多个值
来源：http://bxw.jyoumei.cn

Py:   return a, b
来源：http://hmh.quarkkingdee.top

PHP:  return [$a, $b];
来源：http://sdx.bjfxy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://vtg.shuidangran.top

TS:   return { a, b };
来源：http://irn.daxiang520.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lsi.cdnleiting.top

Go:   return a, b
来源：http://yoy.zhijiandao.cn

Ruby: return a, b
来源：http://ysl.kuanghao11.cn

C#:   return (a, b);              // ValueTuple
来源：http://upv.ppjwa.cn

[C06] 匿名函数 / lambda
来源：http://zpy.yuanzhike.top

Py:   square = lambda x: x * x
来源：http://tho.chenjidiqi.icu

PHP:  $square = fn($x) => $x * $x;
来源：http://zuj.zhixingplan.top

JS:   const square = x => x * x;
来源：http://yuh.quarkkingdee.top

TS:   const square = (x: number): number => x * x;
来源：http://fqg.aibaodan.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://srz.yonumen.top

Go:   sq := func(x int) int { return x * x }
来源：http://ylq.snrcjt.cn

Ruby: square = ->(x) { x * x }
来源：http://jrv.hnqzz.top

C#:   Func<int, int> square = x => x * x;
来源：http://fph.kuanghao11.cn

[C07] 把函数作为参数传入
来源：http://hhh.cheryme.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cat.cqqwz.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yif.ywan-chungtsiang.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tco.zhongyouzk.top

TS:   arr.map(String)
来源：http://tva.chenzaomai.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jnh.nanxinkj.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mgl.zhiwuduotai.top

Ruby: arr.map(&:upcase)
来源：http://xuk.ydzc1.top

C#:   arr.Select(s => s.ToUpper())
来源：http://lpd.bbcook.cn

[C08] 闭包
来源：http://esr.smart0.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fwh.jqgufenzy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vbc.ywan-chungtsiang.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rml.jqgufenzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://cta.havefunace.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://quh.shanyushiyangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ebx.gotoacloud.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pnc.fktsv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rgz.vqdsnc.cn

[C09] 递归
来源：http://ert.nwbrower.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fgq.gzhubu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://zlq.fktsv.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://siq.316326.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mnz.sufxvd.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xlv.jqgufenzy.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://flv.nwbrower.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gqp.yfazqb.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://imw.ydjk.org.cn

[C10] 变量作用域
来源：http://fga.wangdashe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jbp.fktsv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wuj.hcnkem.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fhk.fktsv.cn

TS:   同 JS
来源：http://xff.jqgfzy.top

Java: 方法内为块级作用域
来源：http://bno.fzhhl.top

Go:   花括号块级作用域
来源：http://ace.yj20258888.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://suk.zhixingplan.top

C#:   块级作用域
来源：http://kzi.andypj.xyz

[C11] 模块导入与导出
来源：http://yzj.mhx1999.top

Py:   from module import func
来源：http://stb.fanxiaobao.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://zyb.hysaishi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://xxs.xuetiantiany.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kqa.zycfv.cn

Java: import java.util.List;
来源：http://spy.cashguo.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eyi.feifeiyinyue.top

Ruby: require "json"; require_relative "./util"
来源：http://ixm.daxiang520.top

C#:   using System.Text;
来源：http://ymg.gaohongyu789.top

[C12] 立即执行函数 IIFE
来源：http://pie.xingfuxueyuan.xyz

Py:   (lambda: print("run"))()
来源：http://sfr.zhengqikj.top

PHP:  (function () { echo "run"; })();
来源：http://slp.yongpay.top

JS:   (() => { console.log("run"); })();
来源：http://vjp.xinyue.icu

TS:   (() => { console.log("run"); })();
来源：http://wzd.jlsjyb.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://umi.jiagoushi.top

Go:   func() { fmt.Println("run") }()
来源：http://qgi.cashguo.top

Ruby: -> { puts "run" }.call
来源：http://pfl.jlsjyb.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zlc.zhoulong.xyz

[C13] 类型声明 / 类型注解
来源：http://xmp.ctjpmb.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jzd.shuidangran.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zyp.ctjpmb.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xmw.c1oappe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vjn.svipenyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nbz.yongpay.top

Go:   func add(a, b int) int
来源：http://yvs.ehwqpu.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://azw.sjlbkw.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rwz.vehdjk.com

[C14] 泛型函数
来源：http://ust.yuxming.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zyv.yj202588.top

PHP:  // 无泛型
来源：http://wzl.fktsv.cn

JS:   // 无泛型
来源：http://cko.yj202588.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hgx.iojbl.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pwm.ybcxt.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rfb.jqgfzy.top

Ruby: # 无泛型
来源：http://hfn.quarkkingdee.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://uow.fehbvm.com

[C15] 解构 / 展开参数
来源：http://cpz.dianchejie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://swj.9152youxi.cn

PHP:  [$a, $b] = $pair;
来源：http://qmd.chenlongwang.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jih.shanyushiyangtech.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lny.jinqigufen.top

Java: // 无解构
来源：http://jwe.haohaochexian.top

Go:   // 无解构
来源：http://pzp.shzxlz.cn


<!-- 参考信息 -->