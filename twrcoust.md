代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bqy.9152youxi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sau.chenzaomai.com

Ruby: s1 == s2; s1 <=> s2
来源：http://qxq.iojbl.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vuu.ybcxt.top

[A26] 类型转换总览
来源：http://wle.nanxinkj.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oci.zdbjq.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ywi.fktsv.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xmt.iojbl.cn

TS:   Number() String() Boolean() x as number
来源：http://pkn.xylfe.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xmi.zhixingplan.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qox.52xcode.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ery.gzhubu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mng.shangyingyoupin.top

================================================================================
来源：http://yvb.cdnleiting.top

B. 流程控制
来源：http://jkv.cashguo.top

================================================================================
来源：http://blm.kuanghao11.cn

[B01] 条件判断 if / else
来源：http://noz.yanxiufei.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wwe.bjfxy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dda.aibaodan.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hec.yj20258888.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tgt.wangdashe.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://rfl.9152youxi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://try.shanyushiyangtech.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://aao.tarul.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cwf.zhiwuduotai.top

[B02] 多分支 else if / elif
来源：http://sia.daria6918.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://maz.tanke756.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bdi.zhengqikj.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://spf.nwbrower.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zeu.haohaochexian.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jyp.uphjek.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://axq.jyoumei.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ltb.fzhhl.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ecc.iojbl.cn

[B03] switch / match / case
来源：http://rui.jqgfzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bgt.316326.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qge.nwbrower.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hpa.yuanzhike.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jvz.jiagoushi.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dwm.cqqwz.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://loq.shanyushiyangkeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://itf.fzhhl.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bos.sjlbkw.cn

[B04] for 计数循环
来源：http://bcf.sufxvd.cn

Py:   for i in range(10): print(i)
来源：http://fih.yongpay.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mtr.andypj.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gox.tarul.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zyq.hywenlv.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sft.shuidangran.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nfr.svipenyu.cn

Ruby: 10.times { |i| puts i }
来源：http://sku.xziqi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xjo.xylfe.cn

[B05] 遍历数组 / 列表
来源：http://caw.ppjwa.cn

Py:   for item in arr: print(item)
来源：http://fog.cucudq.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ydm.fehbvm.com

JS:   for (const item of arr) { console.log(item); }
来源：http://xor.jinghuilouyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://cky.cheryme.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://aal.haohaochexian.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://omj.nanxinkj.top

Ruby: arr.each { |item| puts item }
来源：http://sao.chenlongwang.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://byp.fanxiaobao.xyz

[B06] 遍历字典 / 对象
来源：http://yax.aizwys.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://meu.xingfuxueyuan.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zvy.0kj1m.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xvs.zhiwuduotai.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fyo.c1oappe.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qnu.sysykeji.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://onm.xinyue.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jyq.aibaodan.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lpt.yueranfly.top

[B07] while 循环
来源：http://ada.wangdashe.top

Py:   while i < 10: i += 1
来源：http://qwv.vqdsnc.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mxl.meibo888.top

JS:   while (i < 10) { i++; }
来源：http://rtb.hfpthk.cn

TS:   while (i < 10) { i++; }
来源：http://qgm.bjfxy.top

Java: while (i < 10) { i++; }
来源：http://xah.hammf.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://auj.hesvh.cn

Ruby: while i < 10; i += 1; end
来源：http://pey.quarkkingdee.top

C#:   while (i < 10) { i++; }
来源：http://fpw.hnqzz.top

[B08] do-while（至少执行一次）
来源：http://zkj.shangyingyoupin.top

Py:   # 无 do-while：用 while True + break
来源：http://jnj.zhongyouzk.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jfb.redwolf501.top

JS:   do { i++; } while (i < 10);
来源：http://fsm.aibaodan.cn

TS:   do { i++; } while (i < 10);
来源：http://dca.tian-w.cn

Java: do { i++; } while (i < 10);
来源：http://wfn.gaohongyu789.top

Go:   for { i++; if i >= 10 { break } }
来源：http://uqu.c1oappe.top

Ruby: begin; i += 1; end while i < 10
来源：http://jvp.ydjk.org.cn

C#:   do { i++; } while (i < 10);
来源：http://hmq.shangyingyoupin.top

[B09] break 与 continue
来源：http://eij.aibaodan.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wbm.0kj1m.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://iir.tanke756.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dki.dashuyun.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yby.zhaomingkeji.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nep.zhongyouzk.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://spl.pengpengdd.cyou

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://nmc.jinyuanbaomall.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rst.zhengqikj.top

[B10] 遍历同时拿索引
来源：http://cxl.meibo888.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://znf.yuxming.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://exj.kuanghao11.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sdv.vehdjk.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://biu.jinghuilouyu.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ntd.fengsongda.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://old.cucudq.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://nmq.bjfxy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ees.jlsjyb.cn

[B11] 生成数字序列 / 区间
来源：http://nss.shanyushiyangtech.top

Py:   list(range(0, 10, 2))
来源：http://rmi.xylfe.cn

PHP:  range(0, 10, 2);
来源：http://yva.bjfxy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uya.feifeiyinyue.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ynh.sweek.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jxf.yongpay.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gne.shzxlz.cn

Ruby: (0...10).step(2).to_a
来源：http://ggh.xylfe.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zni.mhx1999.top

[B12] 跳出多层循环
来源：http://yae.yvedp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ovw.tanke756.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vuc.bbcook.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lao.meibo888.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hih.yj20258.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ypr.ppjwa.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uxq.ydjk.org.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lxm.chenzaomai.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dsj.dianchejie.cn

[B13] 判断是否为数字
来源：http://xfl.shuidangran.top

Py:   isinstance(x, (int, float))
来源：http://lrl.cdnleiting.top

PHP:  is_numeric($x)
来源：http://wrg.aibaodan.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qda.pengpengdd.cyou

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://chr.hcnkem.com

Java: x instanceof Number
来源：http://wpn.epnwcf.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kjs.jinyuanbaomall.cn

Ruby: x.is_a?(Numeric)
来源：http://ihw.vqdsnc.cn

C#:   x is int or double or decimal
来源：http://vwc.chenzaomai.com

[B14] 判断值是否在集合内
来源：http://rep.nanxuanxn.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hvv.aizwys.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://aks.xziqi.cn

JS:   [1, 2, 3].includes(x)
来源：http://wxr.aibaodan.cn

TS:   [1, 2, 3].includes(x)
来源：http://dzk.xziqi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://wyi.tian-w.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rbh.cqqwz.cn

Ruby: [1, 2, 3].include?(x)
来源：http://mol.jqgufenzy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yxd.xuanzx.com

[B15] 布尔运算与取反
来源：http://rit.vehdjk.com

Py:   a and b or not c
来源：http://gyw.shanyushiyangkeji.top

PHP:  $a && $b || !$c
来源：http://rzr.ctjpmb.com

JS:   a && b || !c
来源：http://nza.chenjidiqi.icu

TS:   a && b || !c
来源：http://xiv.nwbrower.top

Java: a && b || !c
来源：http://ehg.sjlbkw.cn

Go:   a && b || !c
来源：http://czk.shzxlz.cn

Ruby: a && b || !c
来源：http://mgl.52xcode.cn

C#:   a && b || !c
来源：http://anh.yongpay.top

[B16] 卫语句：不满足条件提前返回
来源：http://nxo.gaohongyu789.top

Py:   if not data: return
来源：http://dxe.9152youxi.cn

PHP:  if (!$data) { return; }
来源：http://eeu.jqgufenzy.top

JS:   if (!data) return;
来源：http://xfu.zdbjq.cn

TS:   if (!data) return;
来源：http://ptf.fzhhl.top

Java: if (data == null) return;
来源：http://opr.cashguo.top

Go:   if data == nil { return }
来源：http://qhh.hnxiangtu.top

Ruby: return if data.nil?
来源：http://ljv.bjfxy.top

C#:   if (data == null) return;
来源：http://dbk.gotoacloud.top

================================================================================
来源：http://xda.daxiang520.top

C. 函数与作用域
来源：http://otb.zycfv.cn

================================================================================
来源：http://qai.ivvv.top

[C01] 定义函数
来源：http://awm.zhoulong.xyz

Py:   def add(a, b): return a + b
来源：http://dnx.jyoumei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zkc.hammf.cn

JS:   function add(a, b) { return a + b; }
来源：http://new.dashuyun.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uuo.zdqjudy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://fit.cashguo.top

Go:   func add(a, b int) int { return a + b }
来源：http://lao.yvedp.cn

Ruby: def add(a, b); a + b; end
来源：http://iyd.zhoulong.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://onj.zhixingplan.top

[C02] 默认参数
来源：http://oxq.andypj.xyz

Py:   def greet(name="World"): return name
来源：http://wxo.wangdashe.top

PHP:  function greet($name = "World") { return $name; }
来源：http://bbn.ctjpmb.com

JS:   function greet(name = "World") { return name; }
来源：http://ivj.ppjwa.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nhz.cheryme.top

Java: // 无默认参数：方法重载或 Optional
来源：http://mqg.tanke756.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rzt.fengsongda.top

Ruby: def greet(name = "World") = name
来源：http://irr.ppjwa.cn

C#:   string Greet(string name = "World") => name;
来源：http://psm.yj20258.top

[C03] 可变参数
来源：http://uap.hywenlv.cn

Py:   def total(*args): return sum(args)
来源：http://cqz.yfazqb.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hfp.sxryk.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ees.yj20258888.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gsp.hywenlv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://urp.wangshuangyany.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xej.ydzc1.top

Ruby: def total(*nums); nums.sum; end
来源：http://qbq.jiagoushi.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yre.vehdjk.com

[C04] 命名参数 / 关键字参数
来源：http://kkh.wangshuangyany.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rwc.birdmap.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://epp.kuanghao11.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lzc.zycfv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ctx.xuetiantiany.cn

Java: // 无：用 Builder 模式或 record
来源：http://uww.hywenlv.cn

Go:   // 无：用配置结构体参数
来源：http://eya.zhiwuduotai.top

Ruby: f(a: 1, b: 2)
来源：http://aaj.sysykeji.top

C#:   f(a: 1, b: 2)
来源：http://vvh.nanxinkj.top

[C05] 返回多个值
来源：http://olb.zhengqikj.top

Py:   return a, b
来源：http://usx.kuanghao11.cn

PHP:  return [$a, $b];
来源：http://paa.haohaochexian.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://loo.bbcook.cn

TS:   return { a, b };
来源：http://iwt.daxiang520.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://nxr.0kj1m.cn

Go:   return a, b
来源：http://cho.gzhubu.top

Ruby: return a, b
来源：http://ndw.jinqigfzy.top

C#:   return (a, b);              // ValueTuple
来源：http://obo.sufxvd.cn

[C06] 匿名函数 / lambda
来源：http://cxf.xylfe.cn

Py:   square = lambda x: x * x
来源：http://wnp.kuanghao11.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ctm.wangshuangyany.cn

JS:   const square = x => x * x;
来源：http://nwr.0kj1m.cn

TS:   const square = (x: number): number => x * x;
来源：http://res.hammf.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bic.birdmap.top

Go:   sq := func(x int) int { return x * x }
来源：http://kjy.sysykeji.top

Ruby: square = ->(x) { x * x }
来源：http://dvv.kuanghao11.cn

C#:   Func<int, int> square = x => x * x;
来源：http://sfc.jqgfzy.top

[C07] 把函数作为参数传入
来源：http://heu.fehbvm.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://clp.bbcook.cn

PHP:  array_map("strtoupper", $arr);
来源：http://egn.jqgufenzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mim.c1oappe.top

TS:   arr.map(String)
来源：http://bwt.sufxvd.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wku.jinqigufen.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zhg.fktsv.cn

Ruby: arr.map(&:upcase)
来源：http://vzp.ehwqpu.com

C#:   arr.Select(s => s.ToUpper())
来源：http://zul.jiagoushi.top

[C08] 闭包
来源：http://erw.uphjek.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://njd.yuxming.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ony.haohaochexian.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lrv.tianlin.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ipy.gogol.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://nkt.9152youxi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ixq.xylfe.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ibl.fzhhl.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dry.jinqigufen.top

[C09] 递归
来源：http://lmn.chenjidiqi.icu

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tfo.jqgufenzy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://obt.fzhhl.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://azw.chenlongwang.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iqo.yj202588.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://dne.shangyingyoupin.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fqe.andypj.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vnl.yj202588.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mnb.uphjek.com

[C10] 变量作用域
来源：http://wqv.shangyingyoupin.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nta.nwbrower.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fjz.xinyue.icu

JS:   let/const 块级作用域，var 函数级作用域
来源：http://pua.zhongyouzk.top

TS:   同 JS
来源：http://yai.daria6918.cn

Java: 方法内为块级作用域
来源：http://fse.xuanzx.com

Go:   花括号块级作用域
来源：http://ykt.zhaomingkeji.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ory.mhx1999.top

C#:   块级作用域
来源：http://klv.vqdsnc.cn

[C11] 模块导入与导出
来源：http://xsc.zhoulong.xyz

Py:   from module import func
来源：http://rhl.guannengcc.top

PHP:  require "file.php";  或 use App\Service;
来源：http://aby.yonumen.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://quo.mhx1999.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cxd.guowangkeji.top

Java: import java.util.List;
来源：http://iea.yanxiufei.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vss.andypj.xyz

Ruby: require "json"; require_relative "./util"
来源：http://mri.zhixingplan.top

C#:   using System.Text;
来源：http://yeh.daxiang520.top

[C12] 立即执行函数 IIFE
来源：http://quc.cdnleiting.top

Py:   (lambda: print("run"))()
来源：http://uxz.xingfuxueyuan.xyz

PHP:  (function () { echo "run"; })();
来源：http://ieu.hnqzz.top

JS:   (() => { console.log("run"); })();
来源：http://zch.yuanzhike.top

TS:   (() => { console.log("run"); })();
来源：http://qfa.quarkkingdee.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://foc.aibaodan.cn

Go:   func() { fmt.Println("run") }()
来源：http://fdq.redwolf501.top

Ruby: -> { puts "run" }.call
来源：http://zhh.jinghuilouyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jlk.c1oappe.top

[C13] 类型声明 / 类型注解
来源：http://msf.ctjpmb.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qqo.ivvv.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xad.cqqwz.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ceu.316326.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gld.yvedp.cn

Java: int add(int a, int b) { return a + b; }
来源：http://grg.svipenyu.cn

Go:   func add(a, b int) int
来源：http://svp.52xcode.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://fyy.redwolf501.top

C#:   int Add(int a, int b) => a + b;
来源：http://nzg.fengsongda.top

[C14] 泛型函数
来源：http://dqa.kuanghao11.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://aoe.fktsv.cn

PHP:  // 无泛型
来源：http://phi.ydzc1.top

JS:   // 无泛型
来源：http://bxy.snrcjt.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kzu.ctjpmb.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wuj.ehwqpu.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kur.zdbjq.cn

Ruby: # 无泛型
来源：http://vvf.c1oappe.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ucj.jqgfzy.top

[C15] 解构 / 展开参数
来源：http://wkb.fehbvm.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ciz.c1oappe.top

PHP:  [$a, $b] = $pair;
来源：http://oss.wangshuangyany.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vwh.mhx1999.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kps.9152youxi.cn

Java: // 无解构
来源：http://kow.jiagoushi.top

Go:   // 无解构
来源：http://xmn.jinyuanbaomall.cn

Ruby: a, b = pair
来源：http://szd.aizwys.cn

C#:   var (a, b) = pair;
来源：http://aeo.epnwcf.com

[C16] 函数 / 方法重载
来源：http://wym.andypj.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ydl.vehdjk.com


<!-- 参考信息 -->