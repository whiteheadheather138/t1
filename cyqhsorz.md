代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://pzp.tanke756.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qhy.zycfv.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vvs.aibaodan.cn

[A25] 字符串比较
来源：http://lwc.ehwqpu.com

Py:   s1 == s2; s1 != s2
来源：http://jdp.xziqi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dti.haohaochexian.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fal.zycfv.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ijm.yueranfly.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cdi.hammf.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pii.sysykeji.top

Ruby: s1 == s2; s1 <=> s2
来源：http://xic.cucudq.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xpj.yanxiufei.cn

[A26] 类型转换总览
来源：http://ias.hysaishi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mpu.zhiwuduotai.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lry.yongpay.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ekb.redwolf501.top

TS:   Number() String() Boolean() x as number
来源：http://nhx.chenlongwang.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ycu.jqgfzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hyw.vehdjk.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://aio.wangshuangyany.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fqo.zycfv.cn

================================================================================
来源：http://wjt.zhengqikj.top

B. 流程控制
来源：http://lnc.zdqjudy.top

================================================================================
来源：http://wfw.9152youxi.cn

[B01] 条件判断 if / else
来源：http://ysd.nwbrower.top

Py:   result = "正" if x > 0 else "非正"
来源：http://apf.sweek.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xwy.hnqzz.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jax.ivvv.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mod.birdmap.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://pxp.tarul.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nmm.dashuyun.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ypz.hysaishi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sib.sweek.top

[B02] 多分支 else if / elif
来源：http://aby.shanyushiyangtech.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ohw.gzhubu.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vea.tianlin.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dfw.yueranfly.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sju.52xcode.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://knw.xuetiantiany.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nip.tanke756.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://doi.tanke756.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cfy.yuanzhike.top

[B03] switch / match / case
来源：http://rvu.yj20258888.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://opk.pycfn.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jpn.xingfuxueyuan.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://boe.aibaodan.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nde.yongpay.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pcy.havefunace.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qeg.svipenyu.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sxw.haohaochexian.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xil.dianchejie.cn

[B04] for 计数循环
来源：http://edl.zhoulong.xyz

Py:   for i in range(10): print(i)
来源：http://zbr.yj202588.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ufo.yj20258888.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ujk.shzxlz.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nzz.wangshuangyany.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sff.shzxlz.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nep.cqqwz.cn

Ruby: 10.times { |i| puts i }
来源：http://wzx.fehbvm.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ldv.fzhhl.top

[B05] 遍历数组 / 列表
来源：http://aza.9152youxi.cn

Py:   for item in arr: print(item)
来源：http://pcz.zhiwuduotai.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lyn.yj202588.top

JS:   for (const item of arr) { console.log(item); }
来源：http://sap.jinghuilouyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://omq.andypj.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://krh.jinyuanbaomall.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ykm.gaohongyu789.top

Ruby: arr.each { |item| puts item }
来源：http://vlz.svipenyu.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vvh.316326.xyz

[B06] 遍历字典 / 对象
来源：http://oum.xziqi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gkh.pycfn.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fbi.nwbrower.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iec.xylfe.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fzh.redwolf501.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://afi.zhoulong.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sot.xuetiantiany.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://row.jinghuilouyu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://krp.xingfuxueyuan.xyz

[B07] while 循环
来源：http://djj.cdnleiting.top

Py:   while i < 10: i += 1
来源：http://ihy.hysaishi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vzn.daxiang520.top

JS:   while (i < 10) { i++; }
来源：http://jyd.ivvv.top

TS:   while (i < 10) { i++; }
来源：http://nvs.guannengcc.top

Java: while (i < 10) { i++; }
来源：http://cih.shanyushiyangtech.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dbb.316326.xyz

Ruby: while i < 10; i += 1; end
来源：http://sgu.yj202588.top

C#:   while (i < 10) { i++; }
来源：http://euw.shanyushiyangkeji.top

[B08] do-while（至少执行一次）
来源：http://kky.gotoacloud.top

Py:   # 无 do-while：用 while True + break
来源：http://fkb.daria6918.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gjv.hnxiangtu.top

JS:   do { i++; } while (i < 10);
来源：http://ipx.meibo888.top

TS:   do { i++; } while (i < 10);
来源：http://exe.9152youxi.cn

Java: do { i++; } while (i < 10);
来源：http://sjs.tarul.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ekj.dashuyun.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tlu.tarul.cn

C#:   do { i++; } while (i < 10);
来源：http://buc.dashuyun.cn

[B09] break 与 continue
来源：http://cac.xuanzx.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kdw.hnqzz.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://urh.meibo888.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zgm.ctjpmb.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vsz.redwolf501.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rpo.jyoumei.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ngm.chenlongwang.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ldc.0kj1m.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gnr.sufxvd.cn

[B10] 遍历同时拿索引
来源：http://hys.feifeiyinyue.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://icn.yj20258888.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://geq.shzxlz.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gyk.yangfankeji.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ajg.sweek.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qvf.shanyushiyangtech.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://duw.epnwcf.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://srp.yj202588.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bvp.9152youxi.cn

[B11] 生成数字序列 / 区间
来源：http://weu.ivvv.top

Py:   list(range(0, 10, 2))
来源：http://kiw.ydzc1.top

PHP:  range(0, 10, 2);
来源：http://rxm.hongshengwenyu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tnm.kuanghao11.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wmk.316326.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zvl.wangshuangyany.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rvm.yfazqb.com

Ruby: (0...10).step(2).to_a
来源：http://xrg.shanyushiyangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://evu.xingfuxueyuan.xyz

[B12] 跳出多层循环
来源：http://zbw.ctjpmb.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://wle.ydzc1.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://wzf.jlsjyb.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ivu.ehwqpu.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ygm.cashguo.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rag.yangfankeji.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wjt.wangshuangyany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ieq.zhengqikj.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dfm.ehwqpu.com

[B13] 判断是否为数字
来源：http://wym.aizwys.cn

Py:   isinstance(x, (int, float))
来源：http://wau.hfpthk.cn

PHP:  is_numeric($x)
来源：http://ctc.vehdjk.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tpy.hnqzz.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aae.yj20258888.top

Java: x instanceof Number
来源：http://fxr.ydjk.org.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wim.cdnleiting.top

Ruby: x.is_a?(Numeric)
来源：http://omz.hnqzz.top

C#:   x is int or double or decimal
来源：http://fxz.yueranfly.top

[B14] 判断值是否在集合内
来源：http://bbn.nanxinkj.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dqc.yvedp.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qsc.kuanghao11.cn

JS:   [1, 2, 3].includes(x)
来源：http://vkn.pengpengdd.cyou

TS:   [1, 2, 3].includes(x)
来源：http://lhf.xuanzx.com

Java: List.of(1, 2, 3).contains(x)
来源：http://fwf.sysykeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://cdb.gotoacloud.top

Ruby: [1, 2, 3].include?(x)
来源：http://hez.jianghu66.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://sct.gotoacloud.top

[B15] 布尔运算与取反
来源：http://rzv.jinqigfzy.top

Py:   a and b or not c
来源：http://zrt.daria6918.cn

PHP:  $a && $b || !$c
来源：http://ayo.ydzc1.top

JS:   a && b || !c
来源：http://bdl.chenlongwang.top

TS:   a && b || !c
来源：http://uvk.yj20258888.top

Java: a && b || !c
来源：http://xvf.xuetiantiany.cn

Go:   a && b || !c
来源：http://ojf.cheryme.top

Ruby: a && b || !c
来源：http://eex.ppjwa.cn

C#:   a && b || !c
来源：http://cks.quarkkingdee.top

[B16] 卫语句：不满足条件提前返回
来源：http://yan.dianchejie.cn

Py:   if not data: return
来源：http://xkj.ivvv.top

PHP:  if (!$data) { return; }
来源：http://bdb.shuidangran.top

JS:   if (!data) return;
来源：http://daz.yangfankeji.com

TS:   if (!data) return;
来源：http://fuh.zdqjudy.top

Java: if (data == null) return;
来源：http://dqx.ydjk.org.cn

Go:   if data == nil { return }
来源：http://nrr.yuanzhike.top

Ruby: return if data.nil?
来源：http://aal.c1oappe.top

C#:   if (data == null) return;
来源：http://ppd.ehwqpu.com

================================================================================
来源：http://ven.gotoacloud.top

C. 函数与作用域
来源：http://dux.hnxiangtu.top

================================================================================
来源：http://iqv.hnqzz.top

[C01] 定义函数
来源：http://fpr.vehdjk.com

Py:   def add(a, b): return a + b
来源：http://qut.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nty.chenjidiqi.icu

JS:   function add(a, b) { return a + b; }
来源：http://ndj.zhiwuduotai.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sln.guannengcc.top

Java: static int add(int a, int b) { return a + b; }
来源：http://pbc.xuetiantiany.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ayp.fktsv.cn

Ruby: def add(a, b); a + b; end
来源：http://bxd.kuanghao11.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nme.feifeiyinyue.top

[C02] 默认参数
来源：http://sxi.havefunace.top

Py:   def greet(name="World"): return name
来源：http://dzz.fzhhl.top

PHP:  function greet($name = "World") { return $name; }
来源：http://pyp.meibo888.top

JS:   function greet(name = "World") { return name; }
来源：http://hai.jyoumei.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://uhc.ivvv.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xsp.tarul.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qvb.yueranfly.top

Ruby: def greet(name = "World") = name
来源：http://xup.jqgfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://ixz.zhixingplan.top

[C03] 可变参数
来源：http://mqh.zhongyouzk.top

Py:   def total(*args): return sum(args)
来源：http://fxy.hesvh.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://duc.wangshuangyany.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://etx.yangfankeji.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ojb.jyoumei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jwn.fengsongda.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qwt.shangyingyoupin.top

Ruby: def total(*nums); nums.sum; end
来源：http://oyl.jqgfzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lcg.ybcxt.top

[C04] 命名参数 / 关键字参数
来源：http://alh.guannengcc.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ode.yj202588.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ckl.svipenyu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uge.epnwcf.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rhx.zhaomingkeji.xyz

Java: // 无：用 Builder 模式或 record
来源：http://kro.yueranfly.top

Go:   // 无：用配置结构体参数
来源：http://sub.uphjek.com

Ruby: f(a: 1, b: 2)
来源：http://tvf.hongshengwenyu.top

C#:   f(a: 1, b: 2)
来源：http://bfk.tarul.cn

[C05] 返回多个值
来源：http://wff.hywenlv.cn

Py:   return a, b
来源：http://gwc.nanxuanxn.top

PHP:  return [$a, $b];
来源：http://ske.jinqigufen.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://moi.havefunace.top

TS:   return { a, b };
来源：http://whe.sysykeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tnr.fzhhl.top

Go:   return a, b
来源：http://kle.xuetiantiany.cn

Ruby: return a, b
来源：http://moy.gaohongyu789.top

C#:   return (a, b);              // ValueTuple
来源：http://npy.sweek.top

[C06] 匿名函数 / lambda
来源：http://gqe.smart0.xyz

Py:   square = lambda x: x * x
来源：http://cof.jiagoushi.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ohw.quarkkingdee.top

JS:   const square = x => x * x;
来源：http://ktp.hammf.cn

TS:   const square = (x: number): number => x * x;
来源：http://qpo.jinqigfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://exo.yvedp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://rix.aizwys.cn

Ruby: square = ->(x) { x * x }
来源：http://nfj.chenzaomai.com

C#:   Func<int, int> square = x => x * x;
来源：http://ygg.bbcook.cn

[C07] 把函数作为参数传入
来源：http://azh.cqqwz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://job.snrcjt.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ivv.dianchejie.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xet.jqgufenzy.top

TS:   arr.map(String)
来源：http://qil.daxiang520.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zsi.epnwcf.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sxz.hysaishi.cn

Ruby: arr.map(&:upcase)
来源：http://rcb.xingfuxueyuan.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://kie.zhiwuduotai.top

[C08] 闭包
来源：http://uby.tian-w.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xsg.hcnkem.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kot.shanyushiyangkeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uwu.jinyuanbaomall.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://spz.yuxming.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://owu.tianlin.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vmd.sjlbkw.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://abc.yuanzhike.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gnt.ydzc1.top

[C09] 递归
来源：http://lqh.shuidangran.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tcu.ydzc1.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ehg.zhiwuduotai.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yex.jqgfzy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nqc.hcnkem.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://chp.uphjek.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yud.shuidangran.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bgx.cheryme.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nnb.xinyue.icu

[C10] 变量作用域
来源：http://tsg.aizwys.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ciw.shzxlz.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pnk.sweek.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fzn.tanke756.top

TS:   同 JS
来源：http://utg.nanxinkj.top

Java: 方法内为块级作用域
来源：http://ogw.zdbjq.cn

Go:   花括号块级作用域
来源：http://ojd.ydjk.org.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://muc.mhx1999.top

C#:   块级作用域
来源：http://cda.daxiang520.top

[C11] 模块导入与导出
来源：http://igf.xuetiantiany.cn

Py:   from module import func
来源：http://dni.chenzaomai.com

PHP:  require "file.php";  或 use App\Service;
来源：http://qbs.kuanghao11.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://odw.0kj1m.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://twq.yfazqb.com

Java: import java.util.List;
来源：http://pri.cashguo.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ytp.yuxming.cn

Ruby: require "json"; require_relative "./util"
来源：http://uft.zhijiandao.cn

C#:   using System.Text;
来源：http://ftk.pycfn.com

[C12] 立即执行函数 IIFE
来源：http://yak.jianghu66.top

Py:   (lambda: print("run"))()
来源：http://tch.epnwcf.com

PHP:  (function () { echo "run"; })();
来源：http://pzc.guannengcc.top

JS:   (() => { console.log("run"); })();
来源：http://mse.bbcook.cn

TS:   (() => { console.log("run"); })();
来源：http://vmn.ctjpmb.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xgt.gzhubu.top

Go:   func() { fmt.Println("run") }()
来源：http://ibw.shuidangran.top

Ruby: -> { puts "run" }.call
来源：http://afd.tianlin.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://bhg.jiagoushi.top

[C13] 类型声明 / 类型注解
来源：http://dte.bbcook.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wtl.aizwys.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dhr.yj202588.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://epy.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vxa.svipenyu.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qps.zhijiandao.cn

Go:   func add(a, b int) int
来源：http://ndh.wangshuangyany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://iye.meibo888.top

C#:   int Add(int a, int b) => a + b;
来源：http://tjy.jlsjyb.cn

[C14] 泛型函数
来源：http://zpf.redwolf501.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hos.c1oappe.top

PHP:  // 无泛型
来源：http://fci.yuanzhike.top

JS:   // 无泛型
来源：http://oxj.fehbvm.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bho.meibo888.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://izu.fehbvm.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://haz.shangyingyoupin.top

Ruby: # 无泛型
来源：http://pxa.hongshengwenyu.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qyq.bbcook.cn

[C15] 解构 / 展开参数
来源：http://kbo.ywan-chungtsiang.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lfm.jiagoushi.top

PHP:  [$a, $b] = $pair;
来源：http://ith.ybcxt.top


<!-- 参考信息 -->