代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rbz.yuanzhike.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jps.yanxiufei.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vam.zdbjq.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://npu.jinghuilouyu.cn

Go:   strings.TrimSpace(s)
来源：http://ckf.uphjek.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ymi.shangyingyoupin.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fab.xinyue.icu

[A25] 字符串比较
来源：http://kxr.zhengqikj.top

Py:   s1 == s2; s1 != s2
来源：http://gbe.fanxiaobao.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://erk.chenzaomai.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tmr.chenzaomai.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lpd.cucudq.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://oro.yangfankeji.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sce.sweek.top

Ruby: s1 == s2; s1 <=> s2
来源：http://bva.fktsv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ari.yueranfly.top

[A26] 类型转换总览
来源：http://jvl.zhiwuduotai.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zkx.hywenlv.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fjj.cucudq.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oit.hywenlv.cn

TS:   Number() String() Boolean() x as number
来源：http://zbf.yj20258888.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://npl.vehdjk.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kwf.wangdashe.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://uad.sufxvd.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qrn.zhixingplan.top

================================================================================
来源：http://kzn.zdbjq.cn

B. 流程控制
来源：http://fxa.zhiwuduotai.top

================================================================================
来源：http://sky.tarul.cn

[B01] 条件判断 if / else
来源：http://gbx.zhoulong.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://chu.jinyuanbaomall.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kvg.jinqigufen.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://muu.shuidangran.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jpd.daria6918.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jmz.jqgufenzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ues.zhoulong.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xsq.bbcook.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ssl.yonumen.top

[B02] 多分支 else if / elif
来源：http://uzu.cheryme.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jzv.sxryk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dyz.ybcxt.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xbr.jlsjyb.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vry.zhaomingkeji.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jdn.dashuyun.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vuz.tian-w.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://crn.fehbvm.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qbb.epnwcf.com

[B03] switch / match / case
来源：http://nbs.epnwcf.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jbv.cdnleiting.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qhc.ydzc1.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sfm.quarkkingdee.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mjt.hongshengwenyu.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://odp.hnxiangtu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xco.svipenyu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ytp.cheryme.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sqn.9152youxi.cn

[B04] for 计数循环
来源：http://gxz.bjfxy.top

Py:   for i in range(10): print(i)
来源：http://wgn.cucudq.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zom.jlsjyb.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://upy.bbcook.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ssi.ybcxt.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vxb.jinghuilouyu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wbz.xingfuxueyuan.xyz

Ruby: 10.times { |i| puts i }
来源：http://nmz.pengpengdd.cyou

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vti.ybcxt.top

[B05] 遍历数组 / 列表
来源：http://bpf.yfazqb.com

Py:   for item in arr: print(item)
来源：http://fdt.jqgfzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ggk.0kj1m.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://urw.nwbrower.top

TS:   for (const item of arr) { console.log(item); }
来源：http://odl.mhx1999.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://kix.xinyue.icu

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bjz.hywenlv.cn

Ruby: arr.each { |item| puts item }
来源：http://yry.xingfuxueyuan.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ohk.yonumen.top

[B06] 遍历字典 / 对象
来源：http://epf.ybcxt.top

Py:   for k, v in d.items(): print(k, v)
来源：http://vdm.yj20258888.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bsr.c1oappe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zox.aizwys.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yqp.jinghuilouyu.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yer.daxiang520.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xkx.shzxlz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qfe.0kj1m.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nyn.vqdsnc.cn

[B07] while 循环
来源：http://gry.zdbjq.cn

Py:   while i < 10: i += 1
来源：http://vyo.nanxinkj.top

PHP:  while ($i < 10) { $i++; }
来源：http://ixs.hysaishi.cn

JS:   while (i < 10) { i++; }
来源：http://hyl.ctjpmb.com

TS:   while (i < 10) { i++; }
来源：http://oxz.vqdsnc.cn

Java: while (i < 10) { i++; }
来源：http://npt.hfpthk.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ema.ppjwa.cn

Ruby: while i < 10; i += 1; end
来源：http://vap.yonumen.top

C#:   while (i < 10) { i++; }
来源：http://qxz.zhijiandao.cn

[B08] do-while（至少执行一次）
来源：http://gln.yonumen.top

Py:   # 无 do-while：用 while True + break
来源：http://uct.zhengqikj.top

PHP:  do { $i++; } while ($i < 10);
来源：http://baj.ydzc1.top

JS:   do { i++; } while (i < 10);
来源：http://ebr.cdnleiting.top

TS:   do { i++; } while (i < 10);
来源：http://ikg.yuanzhike.top

Java: do { i++; } while (i < 10);
来源：http://ewo.jiagoushi.top

Go:   for { i++; if i >= 10 { break } }
来源：http://gon.316326.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://tci.ppjwa.cn

C#:   do { i++; } while (i < 10);
来源：http://mug.zdqjudy.top

[B09] break 与 continue
来源：http://bxa.zdbjq.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jtk.cucudq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://frl.xinyue.icu

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://woa.nwbrower.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://byc.chenzaomai.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jia.ctjpmb.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://piw.ydzc1.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pce.ctjpmb.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gkv.gotoacloud.top

[B10] 遍历同时拿索引
来源：http://wdw.cqqwz.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mfj.yanxiufei.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ypq.sufxvd.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zvw.yj20258888.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://azz.hnxiangtu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vmv.tianlin.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wnw.xylfe.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fvx.birdmap.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hph.xingfuxueyuan.xyz

[B11] 生成数字序列 / 区间
来源：http://fua.havefunace.top

Py:   list(range(0, 10, 2))
来源：http://ooy.cheryme.top

PHP:  range(0, 10, 2);
来源：http://ofa.yuxming.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://byo.havefunace.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cwu.xingfuxueyuan.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://cyn.svipenyu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uqx.vqdsnc.cn

Ruby: (0...10).step(2).to_a
来源：http://ygj.jqgufenzy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://koi.shzxlz.cn

[B12] 跳出多层循环
来源：http://uqk.nwbrower.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ndm.hongshengwenyu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://jiq.smart0.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gvh.jyoumei.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mnv.quarkkingdee.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://seu.ybcxt.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jwe.yangfankeji.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hii.c1oappe.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jvt.pengpengdd.cyou

[B13] 判断是否为数字
来源：http://skb.aizwys.cn

Py:   isinstance(x, (int, float))
来源：http://jha.sxryk.cn

PHP:  is_numeric($x)
来源：http://lke.zhengqikj.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dgs.yonumen.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uyu.epnwcf.com

Java: x instanceof Number
来源：http://jen.chenjidiqi.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cfh.aizwys.cn

Ruby: x.is_a?(Numeric)
来源：http://jkw.sweek.top

C#:   x is int or double or decimal
来源：http://evs.nanxinkj.top

[B14] 判断值是否在集合内
来源：http://rwl.jinyuanbaomall.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pvu.fzhhl.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nnf.xuanzx.com

JS:   [1, 2, 3].includes(x)
来源：http://uzx.gogol.net.cn

TS:   [1, 2, 3].includes(x)
来源：http://pli.mhx1999.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hth.cucudq.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jui.hnqzz.top

Ruby: [1, 2, 3].include?(x)
来源：http://kgc.yj202588.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kye.yangfankeji.com

[B15] 布尔运算与取反
来源：http://wdg.chenlongwang.top

Py:   a and b or not c
来源：http://cpf.feifeiyinyue.top

PHP:  $a && $b || !$c
来源：http://xdd.hnxiangtu.top

JS:   a && b || !c
来源：http://qfj.316326.xyz

TS:   a && b || !c
来源：http://zxp.cheryme.top

Java: a && b || !c
来源：http://kqp.zdbjq.cn

Go:   a && b || !c
来源：http://qcw.daria6918.cn

Ruby: a && b || !c
来源：http://owo.sysykeji.top

C#:   a && b || !c
来源：http://mdj.daria6918.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gov.xylfe.cn

Py:   if not data: return
来源：http://wpp.xuanzx.com

PHP:  if (!$data) { return; }
来源：http://jdw.shuidangran.top

JS:   if (!data) return;
来源：http://adi.jyoumei.cn

TS:   if (!data) return;
来源：http://qns.aibaodan.cn

Java: if (data == null) return;
来源：http://rsc.feifeiyinyue.top

Go:   if data == nil { return }
来源：http://gwu.jinghuilouyu.cn

Ruby: return if data.nil?
来源：http://qld.sysykeji.top

C#:   if (data == null) return;
来源：http://wzw.chenjidiqi.icu

================================================================================
来源：http://ywh.tianlin.xyz

C. 函数与作用域
来源：http://jyc.gzhubu.top

================================================================================
来源：http://bnx.dashuyun.cn

[C01] 定义函数
来源：http://ncn.fzhhl.top

Py:   def add(a, b): return a + b
来源：http://fpl.9152youxi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gdo.aizwys.cn

JS:   function add(a, b) { return a + b; }
来源：http://kjh.jinqigfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zav.zhaomingkeji.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://qeu.zdqjudy.top

Go:   func add(a, b int) int { return a + b }
来源：http://msk.ydzc1.top

Ruby: def add(a, b); a + b; end
来源：http://qtr.ydjk.org.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://aro.316326.xyz

[C02] 默认参数
来源：http://rud.jiagoushi.top

Py:   def greet(name="World"): return name
来源：http://jke.chenjidiqi.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://yzd.gaohongyu789.top

JS:   function greet(name = "World") { return name; }
来源：http://bsz.zhoulong.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://bst.yj20258888.top

Java: // 无默认参数：方法重载或 Optional
来源：http://vcv.zhaomingkeji.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ili.c1oappe.top

Ruby: def greet(name = "World") = name
来源：http://sja.yfazqb.com

C#:   string Greet(string name = "World") => name;
来源：http://eci.gaohongyu789.top

[C03] 可变参数
来源：http://blx.ybcxt.top

Py:   def total(*args): return sum(args)
来源：http://tma.zhoulong.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sgs.hywenlv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kty.nwbrower.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://oij.yuanzhike.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pqu.chenzaomai.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bch.gogol.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://dfc.feifeiyinyue.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rid.yangfankeji.com

[C04] 命名参数 / 关键字参数
来源：http://zdv.tianlin.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qpf.haohaochexian.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mlw.kuanghao11.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ngt.daxiang520.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zkk.havefunace.top

Java: // 无：用 Builder 模式或 record
来源：http://vll.nwbrower.top

Go:   // 无：用配置结构体参数
来源：http://sxy.gaohongyu789.top

Ruby: f(a: 1, b: 2)
来源：http://okn.sxryk.cn

C#:   f(a: 1, b: 2)
来源：http://kxp.yj20258888.top

[C05] 返回多个值
来源：http://fjn.yuanzhike.top

Py:   return a, b
来源：http://piq.xuetiantiany.cn

PHP:  return [$a, $b];
来源：http://lvd.wangshuangyany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://rcx.pengpengdd.cyou

TS:   return { a, b };
来源：http://rwb.yuxming.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tav.epnwcf.com

Go:   return a, b
来源：http://kqc.hnqzz.top

Ruby: return a, b
来源：http://eyi.epnwcf.com

C#:   return (a, b);              // ValueTuple
来源：http://pnp.zhengqikj.top

[C06] 匿名函数 / lambda
来源：http://tyn.tanke756.top

Py:   square = lambda x: x * x
来源：http://sol.aizwys.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fec.hysaishi.cn

JS:   const square = x => x * x;
来源：http://lyg.uphjek.com

TS:   const square = (x: number): number => x * x;
来源：http://svp.sxryk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uef.xinyue.icu

Go:   sq := func(x int) int { return x * x }
来源：http://rqc.guannengcc.top

Ruby: square = ->(x) { x * x }
来源：http://jzu.tanke756.top

C#:   Func<int, int> square = x => x * x;
来源：http://hra.ehwqpu.com

[C07] 把函数作为参数传入
来源：http://neu.jqgfzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://dxa.svipenyu.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hfl.smart0.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bfy.jqgfzy.top

TS:   arr.map(String)
来源：http://woa.pycfn.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hwf.jiagoushi.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://neb.yj202588.top

Ruby: arr.map(&:upcase)
来源：http://had.0kj1m.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jus.9152youxi.cn

[C08] 闭包
来源：http://jhe.sufxvd.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rjc.jianghu66.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jnr.shzxlz.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wup.yuanzhike.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xdr.xuetiantiany.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vah.svipenyu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://kbr.tarul.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gay.ybcxt.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ytw.dashuyun.cn

[C09] 递归
来源：http://hch.birdmap.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tzd.tian-w.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pwk.316326.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wob.cheryme.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dzr.cashguo.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://eos.cqqwz.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://crv.cheryme.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rmh.jiagoushi.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vhg.fehbvm.com

[C10] 变量作用域
来源：http://cpr.hammf.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dtt.9152youxi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vjo.jinqigfzy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bmn.zhengqikj.top

TS:   同 JS
来源：http://qhe.andypj.xyz

Java: 方法内为块级作用域
来源：http://swt.jqgufenzy.top

Go:   花括号块级作用域
来源：http://ldu.sufxvd.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rnu.zhixingplan.top

C#:   块级作用域
来源：http://jbq.sysykeji.top

[C11] 模块导入与导出
来源：http://tts.wangshuangyany.cn

Py:   from module import func
来源：http://zxa.sjlbkw.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hdn.pengpengdd.cyou

JS:   export default function f() {};  import f from "./m.js";
来源：http://fcr.daria6918.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ttf.aibaodan.cn

Java: import java.util.List;
来源：http://rdg.hcnkem.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mof.snrcjt.cn

Ruby: require "json"; require_relative "./util"
来源：http://lvx.aizwys.cn

C#:   using System.Text;
来源：http://rcd.gzhubu.top

[C12] 立即执行函数 IIFE
来源：http://uqf.yj20258888.top

Py:   (lambda: print("run"))()
来源：http://ior.hysaishi.cn

PHP:  (function () { echo "run"; })();
来源：http://gnk.yj202588.top

JS:   (() => { console.log("run"); })();
来源：http://xdk.jinyuanbaomall.cn

TS:   (() => { console.log("run"); })();
来源：http://ucc.dashuyun.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vfl.nanxuanxn.top

Go:   func() { fmt.Println("run") }()
来源：http://axa.daria6918.cn

Ruby: -> { puts "run" }.call
来源：http://sqt.dashuyun.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fcl.hcnkem.com

[C13] 类型声明 / 类型注解
来源：http://wxj.snrcjt.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xhv.52xcode.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bvp.ydzc1.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://bhq.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xqb.aizwys.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xnr.meibo888.top

Go:   func add(a, b int) int
来源：http://tcd.ctjpmb.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cdj.xziqi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hoq.sysykeji.top

[C14] 泛型函数
来源：http://nkl.jianghu66.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://erg.nanxinkj.top

PHP:  // 无泛型
来源：http://dgp.guannengcc.top

JS:   // 无泛型
来源：http://qyj.ehwqpu.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xrf.sysykeji.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pjj.hcnkem.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kjq.yonumen.top

Ruby: # 无泛型
来源：http://joj.xylfe.cn


<!-- 参考信息 -->