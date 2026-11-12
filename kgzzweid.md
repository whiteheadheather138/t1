代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://jgy.dianchejie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://paw.xuetiantiany.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rjw.nanxinkj.top

[A25] 字符串比较
来源：http://xaj.xuetiantiany.cn

Py:   s1 == s2; s1 != s2
来源：http://dsj.fzhhl.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://waj.cashguo.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hzr.hysaishi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qsd.quarkkingdee.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hpe.kuanghao11.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dts.xylfe.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hkx.fengsongda.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hgq.ppjwa.cn

[A26] 类型转换总览
来源：http://dwn.9152youxi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wcq.zhiwuduotai.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mcc.ywan-chungtsiang.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dmu.daxiang520.top

TS:   Number() String() Boolean() x as number
来源：http://pna.316326.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ret.ppjwa.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oif.0kj1m.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zus.jyoumei.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nhn.jinyuanbaomall.cn

================================================================================
来源：http://fqq.zhiwuduotai.top

B. 流程控制
来源：http://vvj.hnqzz.top

================================================================================
来源：http://rls.ctjpmb.com

[B01] 条件判断 if / else
来源：http://nij.tian-w.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wbq.chenlongwang.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gdx.hywenlv.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://aoz.hfpthk.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://aat.yj202588.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://xjx.cashguo.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://akg.snrcjt.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nim.hesvh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nda.ctjpmb.com

[B02] 多分支 else if / elif
来源：http://bnm.epnwcf.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sho.hywenlv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zzp.yvedp.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aat.andypj.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mkm.xziqi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qtl.zhongyouzk.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rmk.tian-w.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hsr.xylfe.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zzl.epnwcf.com

[B03] switch / match / case
来源：http://pam.shangyingyoupin.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rgj.sxryk.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fbf.tianlin.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kwc.daxiang520.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jch.fengsongda.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zea.aizwys.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nkd.zdbjq.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fmr.52xcode.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vpa.yuanzhike.top

[B04] for 计数循环
来源：http://acq.hfpthk.cn

Py:   for i in range(10): print(i)
来源：http://amt.jlsjyb.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xzb.jlsjyb.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jwa.tianlin.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nxm.shangyingyoupin.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lha.hesvh.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nng.hongshengwenyu.top

Ruby: 10.times { |i| puts i }
来源：http://vcg.quarkkingdee.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mcs.chenzaomai.com

[B05] 遍历数组 / 列表
来源：http://qkj.yuanzhike.top

Py:   for item in arr: print(item)
来源：http://kvs.yj202588.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jgi.c1oappe.top

JS:   for (const item of arr) { console.log(item); }
来源：http://wym.svipenyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://atd.zhixingplan.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://txp.ehwqpu.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://isl.sysykeji.top

Ruby: arr.each { |item| puts item }
来源：http://hdv.tanke756.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oak.gaohongyu789.top

[B06] 遍历字典 / 对象
来源：http://xiv.hesvh.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://crl.birdmap.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uyt.jyoumei.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mhp.sjlbkw.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ite.ctjpmb.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gce.jlsjyb.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yan.ydjk.org.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://slr.jqgfzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wac.sufxvd.cn

[B07] while 循环
来源：http://xul.haohaochexian.top

Py:   while i < 10: i += 1
来源：http://rrk.daria6918.cn

PHP:  while ($i < 10) { $i++; }
来源：http://kme.ivvv.top

JS:   while (i < 10) { i++; }
来源：http://rij.52xcode.cn

TS:   while (i < 10) { i++; }
来源：http://pdg.uphjek.com

Java: while (i < 10) { i++; }
来源：http://cmp.shanyushiyangtech.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yag.uphjek.com

Ruby: while i < 10; i += 1; end
来源：http://gwd.wangdashe.top

C#:   while (i < 10) { i++; }
来源：http://fxv.xuanzx.com

[B08] do-while（至少执行一次）
来源：http://kzn.xylfe.cn

Py:   # 无 do-while：用 while True + break
来源：http://qgl.jyoumei.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jwi.52xcode.cn

JS:   do { i++; } while (i < 10);
来源：http://ksa.meibo888.top

TS:   do { i++; } while (i < 10);
来源：http://oeb.sufxvd.cn

Java: do { i++; } while (i < 10);
来源：http://oba.redwolf501.top

Go:   for { i++; if i >= 10 { break } }
来源：http://huv.birdmap.top

Ruby: begin; i += 1; end while i < 10
来源：http://tpw.hywenlv.cn

C#:   do { i++; } while (i < 10);
来源：http://nwk.hywenlv.cn

[B09] break 与 continue
来源：http://lco.sjlbkw.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wwh.xziqi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lcd.shangyingyoupin.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dkz.sxryk.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mwj.xuetiantiany.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lhc.zhaomingkeji.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qxs.yj20258.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jov.aibaodan.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mys.kuanghao11.cn

[B10] 遍历同时拿索引
来源：http://zyw.jqgfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://olu.cashguo.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://awc.tian-w.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cdj.hesvh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cyc.zhaomingkeji.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qvc.nanxinkj.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sau.tianlin.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kjt.zhongyouzk.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ssp.iojbl.cn

[B11] 生成数字序列 / 区间
来源：http://zda.cheryme.top

Py:   list(range(0, 10, 2))
来源：http://sgc.fanxiaobao.xyz

PHP:  range(0, 10, 2);
来源：http://ykk.sufxvd.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://imk.hesvh.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qzo.guowangkeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wpt.sjlbkw.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vnf.cheryme.top

Ruby: (0...10).step(2).to_a
来源：http://eqj.cqqwz.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ogl.zdbjq.cn

[B12] 跳出多层循环
来源：http://dlo.zdqjudy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://dyx.ctjpmb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://zep.epnwcf.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kcf.hcnkem.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://udj.havefunace.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ile.chenjidiqi.icu

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ing.yuanzhike.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dro.gogol.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lvs.jqgfzy.top

[B13] 判断是否为数字
来源：http://pvy.xuanzx.com

Py:   isinstance(x, (int, float))
来源：http://lgd.yj20258.top

PHP:  is_numeric($x)
来源：http://ant.cashguo.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ufw.c1oappe.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xnj.fanxiaobao.xyz

Java: x instanceof Number
来源：http://cab.hywenlv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jhz.ybcxt.top

Ruby: x.is_a?(Numeric)
来源：http://ykb.yangfankeji.com

C#:   x is int or double or decimal
来源：http://qcz.dianchejie.cn

[B14] 判断值是否在集合内
来源：http://pjn.cashguo.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qve.xinyue.icu

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eay.meibo888.top

JS:   [1, 2, 3].includes(x)
来源：http://gff.zhoulong.xyz

TS:   [1, 2, 3].includes(x)
来源：http://kzt.mhx1999.top

Java: List.of(1, 2, 3).contains(x)
来源：http://aue.ctjpmb.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cbz.xziqi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://uqs.9152youxi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rmn.jianghu66.top

[B15] 布尔运算与取反
来源：http://vcv.nwbrower.top

Py:   a and b or not c
来源：http://oip.iojbl.cn

PHP:  $a && $b || !$c
来源：http://kzj.tarul.cn

JS:   a && b || !c
来源：http://xkp.sjlbkw.cn

TS:   a && b || !c
来源：http://uql.sjlbkw.cn

Java: a && b || !c
来源：http://wlf.jinqigfzy.top

Go:   a && b || !c
来源：http://ria.fanxiaobao.xyz

Ruby: a && b || !c
来源：http://ulr.xingfuxueyuan.xyz

C#:   a && b || !c
来源：http://wzj.jqgufenzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://xqn.hammf.cn

Py:   if not data: return
来源：http://kxo.jlsjyb.cn

PHP:  if (!$data) { return; }
来源：http://qra.gzhubu.top

JS:   if (!data) return;
来源：http://bkk.guowangkeji.top

TS:   if (!data) return;
来源：http://yqd.feifeiyinyue.top

Java: if (data == null) return;
来源：http://kni.jinyuanbaomall.cn

Go:   if data == nil { return }
来源：http://ukc.ydzc1.top

Ruby: return if data.nil?
来源：http://hnp.guowangkeji.top

C#:   if (data == null) return;
来源：http://dzw.hesvh.cn

================================================================================
来源：http://wbq.cdnleiting.top

C. 函数与作用域
来源：http://jyo.sufxvd.cn

================================================================================
来源：http://coe.zhijiandao.cn

[C01] 定义函数
来源：http://grb.ivvv.top

Py:   def add(a, b): return a + b
来源：http://jyv.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ldz.yuxming.cn

JS:   function add(a, b) { return a + b; }
来源：http://qtn.zhoulong.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vxh.vqdsnc.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://gpi.jinyuanbaomall.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ikl.dashuyun.cn

Ruby: def add(a, b); a + b; end
来源：http://wyz.zhiwuduotai.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hxr.jlsjyb.cn

[C02] 默认参数
来源：http://beq.yangfankeji.com

Py:   def greet(name="World"): return name
来源：http://azr.nwbrower.top

PHP:  function greet($name = "World") { return $name; }
来源：http://mjo.uphjek.com

JS:   function greet(name = "World") { return name; }
来源：http://wjj.shuidangran.top

TS:   function greet(name: string = "World") { return name; }
来源：http://glf.uphjek.com

Java: // 无默认参数：方法重载或 Optional
来源：http://cnk.fehbvm.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tve.guannengcc.top

Ruby: def greet(name = "World") = name
来源：http://mwv.yj20258888.top

C#:   string Greet(string name = "World") => name;
来源：http://ify.fktsv.cn

[C03] 可变参数
来源：http://ito.ppjwa.cn

Py:   def total(*args): return sum(args)
来源：http://cug.yj20258.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://nmb.jiagoushi.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ctw.jinqigufen.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ylj.yongpay.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kri.fengsongda.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://adg.jianghu66.top

Ruby: def total(*nums); nums.sum; end
来源：http://xdq.hesvh.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dsd.sjlbkw.cn

[C04] 命名参数 / 关键字参数
来源：http://hzk.havefunace.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ztk.uphjek.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gfb.xuanzx.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pll.aizwys.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://icb.cqqwz.cn

Java: // 无：用 Builder 模式或 record
来源：http://kaw.nanxinkj.top

Go:   // 无：用配置结构体参数
来源：http://wfs.hysaishi.cn

Ruby: f(a: 1, b: 2)
来源：http://ssq.guannengcc.top

C#:   f(a: 1, b: 2)
来源：http://jzn.xuanzx.com

[C05] 返回多个值
来源：http://flm.andypj.xyz

Py:   return a, b
来源：http://rgy.daria6918.cn

PHP:  return [$a, $b];
来源：http://tdv.jqgufenzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qwb.jqgfzy.top

TS:   return { a, b };
来源：http://gxu.meibo888.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://enj.svipenyu.cn

Go:   return a, b
来源：http://jax.pengpengdd.cyou

Ruby: return a, b
来源：http://poc.hnqzz.top

C#:   return (a, b);              // ValueTuple
来源：http://gkr.dashuyun.cn

[C06] 匿名函数 / lambda
来源：http://hly.gzhubu.top

Py:   square = lambda x: x * x
来源：http://clg.hnxiangtu.top

PHP:  $square = fn($x) => $x * $x;
来源：http://dwd.epnwcf.com

JS:   const square = x => x * x;
来源：http://hod.yfazqb.com

TS:   const square = (x: number): number => x * x;
来源：http://msp.cucudq.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bwq.sufxvd.cn

Go:   sq := func(x int) int { return x * x }
来源：http://slq.jqgufenzy.top

Ruby: square = ->(x) { x * x }
来源：http://wae.birdmap.top

C#:   Func<int, int> square = x => x * x;
来源：http://cch.fktsv.cn

[C07] 把函数作为参数传入
来源：http://sgk.chenjidiqi.icu

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vit.tanke756.top

PHP:  array_map("strtoupper", $arr);
来源：http://wqo.jlsjyb.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gfn.jlsjyb.cn

TS:   arr.map(String)
来源：http://niz.ydzc1.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tqq.hfpthk.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pzc.cqqwz.cn

Ruby: arr.map(&:upcase)
来源：http://hjc.dashuyun.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://yzg.fengsongda.top

[C08] 闭包
来源：http://msq.haohaochexian.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xbz.havefunace.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://eid.gzhubu.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ars.xylfe.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rei.jinqigufen.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gmk.haohaochexian.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yde.sufxvd.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rdk.yonumen.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yed.hywenlv.cn

[C09] 递归
来源：http://hmk.0kj1m.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://rui.xziqi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://asn.fzhhl.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yce.hfpthk.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cdk.chenjidiqi.icu

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bea.fengsongda.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gty.ehwqpu.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jvd.cucudq.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lxn.kuanghao11.cn

[C10] 变量作用域
来源：http://ofv.gogol.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jqd.iojbl.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://utq.snrcjt.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cyk.cheryme.top

TS:   同 JS
来源：http://heu.xinyue.icu

Java: 方法内为块级作用域
来源：http://mqh.epnwcf.com

Go:   花括号块级作用域
来源：http://gvv.yangfankeji.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qzi.haohaochexian.top

C#:   块级作用域
来源：http://iji.jiagoushi.top

[C11] 模块导入与导出
来源：http://iym.pycfn.com

Py:   from module import func
来源：http://dpx.tanke756.top

PHP:  require "file.php";  或 use App\Service;
来源：http://shk.hysaishi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://dog.snrcjt.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mup.hywenlv.cn

Java: import java.util.List;
来源：http://geg.hnqzz.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wro.ivvv.top

Ruby: require "json"; require_relative "./util"
来源：http://tmo.zhiwuduotai.top

C#:   using System.Text;
来源：http://ota.0kj1m.cn

[C12] 立即执行函数 IIFE
来源：http://ckm.meibo888.top

Py:   (lambda: print("run"))()
来源：http://xmk.yvedp.cn

PHP:  (function () { echo "run"; })();
来源：http://uvf.cashguo.top

JS:   (() => { console.log("run"); })();
来源：http://seg.yueranfly.top

TS:   (() => { console.log("run"); })();
来源：http://iyw.chenzaomai.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://iyp.yongpay.top

Go:   func() { fmt.Println("run") }()
来源：http://yxv.tianlin.xyz

Ruby: -> { puts "run" }.call
来源：http://log.sjlbkw.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pon.aibaodan.cn

[C13] 类型声明 / 类型注解
来源：http://dnj.jinqigfzy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://alu.kuanghao11.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jhz.cashguo.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qlc.hnxiangtu.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tsy.cdnleiting.top

Java: int add(int a, int b) { return a + b; }
来源：http://pjy.xingfuxueyuan.xyz

Go:   func add(a, b int) int
来源：http://yhc.bbcook.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ina.shangyingyoupin.top

C#:   int Add(int a, int b) => a + b;
来源：http://ksl.xuetiantiany.cn

[C14] 泛型函数
来源：http://oql.zhixingplan.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rbg.shzxlz.cn

PHP:  // 无泛型
来源：http://joq.yangfankeji.com

JS:   // 无泛型
来源：http://biq.sweek.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nyt.shuidangran.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://uai.ctjpmb.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://efj.bbcook.cn

Ruby: # 无泛型
来源：http://xmu.jqgfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ifm.xuetiantiany.cn

[C15] 解构 / 展开参数
来源：http://qew.zhixingplan.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wrm.cashguo.top

PHP:  [$a, $b] = $pair;
来源：http://zbp.tanke756.top


<!-- 参考信息 -->