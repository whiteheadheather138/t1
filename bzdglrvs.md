代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://lbm.yongpay.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dmi.vqdsnc.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hrh.hysaishi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kxm.hesvh.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rba.nwbrower.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://twe.yfazqb.com

Ruby: s1 == s2; s1 <=> s2
来源：http://nms.cucudq.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://lpa.jlsjyb.cn

[A26] 类型转换总览
来源：http://prz.nanxuanxn.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xgy.guowangkeji.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mhg.jiagoushi.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yao.zdbjq.cn

TS:   Number() String() Boolean() x as number
来源：http://kbf.bjfxy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wcv.chenzaomai.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xtt.ydzc1.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://vqh.kuanghao11.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xat.meibo888.top

================================================================================
来源：http://oum.yuxming.cn

B. 流程控制
来源：http://iah.zhengqikj.top

================================================================================
来源：http://dlp.pengpengdd.cyou

[B01] 条件判断 if / else
来源：http://qor.zhixingplan.top

Py:   result = "正" if x > 0 else "非正"
来源：http://dfa.redwolf501.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lip.jinqigfzy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://oqc.c1oappe.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://url.birdmap.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://elm.zycfv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://vnp.jlsjyb.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pjp.iojbl.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://eps.yfazqb.com

[B02] 多分支 else if / elif
来源：http://yrb.shanyushiyangkeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kix.jlsjyb.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pka.ywan-chungtsiang.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cag.jinqigfzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://skn.gotoacloud.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uvw.zhixingplan.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fsp.shuidangran.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fju.hfpthk.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nwu.meibo888.top

[B03] switch / match / case
来源：http://myt.yj202588.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://igh.xziqi.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bsr.smart0.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rwy.guannengcc.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qlv.ydjk.org.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qwl.fehbvm.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tbe.cucudq.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://loq.wangdashe.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nco.jqgfzy.top

[B04] for 计数循环
来源：http://osu.yj20258.top

Py:   for i in range(10): print(i)
来源：http://cbr.cashguo.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sdb.iojbl.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hxa.shanyushiyangkeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tnq.jinqigufen.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yyx.bbcook.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ryn.kuanghao11.cn

Ruby: 10.times { |i| puts i }
来源：http://vem.iojbl.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gwc.yj20258.top

[B05] 遍历数组 / 列表
来源：http://qax.xuanzx.com

Py:   for item in arr: print(item)
来源：http://dcf.uphjek.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uwy.zhiwuduotai.top

JS:   for (const item of arr) { console.log(item); }
来源：http://joc.fengsongda.top

TS:   for (const item of arr) { console.log(item); }
来源：http://foo.zhijiandao.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qtg.zdbjq.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zmi.ctjpmb.com

Ruby: arr.each { |item| puts item }
来源：http://tlk.fehbvm.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rhp.pengpengdd.cyou

[B06] 遍历字典 / 对象
来源：http://bpb.yongpay.top

Py:   for k, v in d.items(): print(k, v)
来源：http://uuh.yfazqb.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uoi.mhx1999.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pbw.hongshengwenyu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cdl.xinyue.icu

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jmr.daxiang520.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://keg.zhixingplan.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cwq.ywan-chungtsiang.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gnd.jlsjyb.cn

[B07] while 循环
来源：http://hmq.yangfankeji.com

Py:   while i < 10: i += 1
来源：http://lpc.kuanghao11.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bqa.jlsjyb.cn

JS:   while (i < 10) { i++; }
来源：http://ldz.yonumen.top

TS:   while (i < 10) { i++; }
来源：http://yzb.snrcjt.cn

Java: while (i < 10) { i++; }
来源：http://kai.ywan-chungtsiang.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://iuv.xinyue.icu

Ruby: while i < 10; i += 1; end
来源：http://bzd.daxiang520.top

C#:   while (i < 10) { i++; }
来源：http://jet.shangyingyoupin.top

[B08] do-while（至少执行一次）
来源：http://ylt.hongshengwenyu.top

Py:   # 无 do-while：用 while True + break
来源：http://aix.52xcode.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://eje.yuanzhike.top

JS:   do { i++; } while (i < 10);
来源：http://lih.xziqi.cn

TS:   do { i++; } while (i < 10);
来源：http://ykk.yueranfly.top

Java: do { i++; } while (i < 10);
来源：http://zvs.fengsongda.top

Go:   for { i++; if i >= 10 { break } }
来源：http://jfs.yueranfly.top

Ruby: begin; i += 1; end while i < 10
来源：http://ldv.jinyuanbaomall.cn

C#:   do { i++; } while (i < 10);
来源：http://irl.zdbjq.cn

[B09] break 与 continue
来源：http://lcy.sysykeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wri.jiagoushi.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://qzc.cashguo.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fik.yj20258.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wuo.bbcook.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nah.0kj1m.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dns.hesvh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://yzs.tianlin.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fvd.fehbvm.com

[B10] 遍历同时拿索引
来源：http://exq.zdqjudy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jwl.yangfankeji.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dio.fanxiaobao.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kdn.zdbjq.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yvw.kuanghao11.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dag.andypj.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wcd.sufxvd.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pie.yj20258.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xqm.tian-w.cn

[B11] 生成数字序列 / 区间
来源：http://jou.chenzaomai.com

Py:   list(range(0, 10, 2))
来源：http://hww.nanxinkj.top

PHP:  range(0, 10, 2);
来源：http://qnq.xingfuxueyuan.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pzn.hysaishi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ohz.zycfv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pwe.dashuyun.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gib.uphjek.com

Ruby: (0...10).step(2).to_a
来源：http://nph.ydjk.org.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gxw.zhoulong.xyz

[B12] 跳出多层循环
来源：http://auz.zhaomingkeji.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://eyn.yfazqb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://tqc.cucudq.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://phi.vehdjk.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hag.redwolf501.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kkz.wangshuangyany.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tsi.chenjidiqi.icu

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rji.xinyue.icu

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jjg.jiagoushi.top

[B13] 判断是否为数字
来源：http://sye.tarul.cn

Py:   isinstance(x, (int, float))
来源：http://ijg.pengpengdd.cyou

PHP:  is_numeric($x)
来源：http://sps.zhaomingkeji.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gqe.bbcook.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gzt.ywan-chungtsiang.top

Java: x instanceof Number
来源：http://ezz.yvedp.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kxx.cdnleiting.top

Ruby: x.is_a?(Numeric)
来源：http://gzo.andypj.xyz

C#:   x is int or double or decimal
来源：http://qys.sysykeji.top

[B14] 判断值是否在集合内
来源：http://ywx.gogol.net.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mlm.yongpay.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sxz.gotoacloud.top

JS:   [1, 2, 3].includes(x)
来源：http://oqj.feifeiyinyue.top

TS:   [1, 2, 3].includes(x)
来源：http://nep.shanyushiyangtech.top

Java: List.of(1, 2, 3).contains(x)
来源：http://xyz.bjfxy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oql.daxiang520.top

Ruby: [1, 2, 3].include?(x)
来源：http://elu.pengpengdd.cyou

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://grg.quarkkingdee.top

[B15] 布尔运算与取反
来源：http://ywo.guowangkeji.top

Py:   a and b or not c
来源：http://mpp.guowangkeji.top

PHP:  $a && $b || !$c
来源：http://vkh.chenzaomai.com

JS:   a && b || !c
来源：http://whg.yj202588.top

TS:   a && b || !c
来源：http://upd.uphjek.com

Java: a && b || !c
来源：http://kil.xylfe.cn

Go:   a && b || !c
来源：http://obf.ivvv.top

Ruby: a && b || !c
来源：http://uic.hysaishi.cn

C#:   a && b || !c
来源：http://yuo.haohaochexian.top

[B16] 卫语句：不满足条件提前返回
来源：http://mds.jinqigufen.top

Py:   if not data: return
来源：http://tsj.aizwys.cn

PHP:  if (!$data) { return; }
来源：http://ifr.ydzc1.top

JS:   if (!data) return;
来源：http://tjr.pengpengdd.cyou

TS:   if (!data) return;
来源：http://fch.hesvh.cn

Java: if (data == null) return;
来源：http://ula.xinyue.icu

Go:   if data == nil { return }
来源：http://mqh.fanxiaobao.xyz

Ruby: return if data.nil?
来源：http://fvs.zdbjq.cn

C#:   if (data == null) return;
来源：http://dco.cdnleiting.top

================================================================================
来源：http://clv.fanxiaobao.xyz

C. 函数与作用域
来源：http://wrx.hywenlv.cn

================================================================================
来源：http://zyc.chenlongwang.top

[C01] 定义函数
来源：http://ikr.jinghuilouyu.cn

Py:   def add(a, b): return a + b
来源：http://bra.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hgz.zhengqikj.top

JS:   function add(a, b) { return a + b; }
来源：http://ehi.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lkp.sweek.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gkg.zycfv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rix.jiagoushi.top

Ruby: def add(a, b); a + b; end
来源：http://rca.hnxiangtu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cae.zhongyouzk.top

[C02] 默认参数
来源：http://ssi.yangfankeji.com

Py:   def greet(name="World"): return name
来源：http://jxf.tanke756.top

PHP:  function greet($name = "World") { return $name; }
来源：http://whr.dashuyun.cn

JS:   function greet(name = "World") { return name; }
来源：http://qyk.guowangkeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://esk.kuanghao11.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vou.yuxming.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hcy.chenzaomai.com

Ruby: def greet(name = "World") = name
来源：http://qca.0kj1m.cn

C#:   string Greet(string name = "World") => name;
来源：http://ygx.zhengqikj.top

[C03] 可变参数
来源：http://qpt.tarul.cn

Py:   def total(*args): return sum(args)
来源：http://mjh.haohaochexian.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rfw.fehbvm.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://cjc.sxryk.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pne.quarkkingdee.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ajz.meibo888.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gfo.zhiwuduotai.top

Ruby: def total(*nums); nums.sum; end
来源：http://mmi.ydzc1.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hym.jiagoushi.top

[C04] 命名参数 / 关键字参数
来源：http://rpl.aibaodan.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qen.hammf.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ubf.aizwys.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xzu.gaohongyu789.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vcg.jinghuilouyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://nkk.zhixingplan.top

Go:   // 无：用配置结构体参数
来源：http://mji.yuxming.cn

Ruby: f(a: 1, b: 2)
来源：http://lzx.zhixingplan.top

C#:   f(a: 1, b: 2)
来源：http://fzy.hammf.cn

[C05] 返回多个值
来源：http://dew.sjlbkw.cn

Py:   return a, b
来源：http://ubf.zdqjudy.top

PHP:  return [$a, $b];
来源：http://mol.daria6918.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://nhs.kuanghao11.cn

TS:   return { a, b };
来源：http://axc.yfazqb.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ito.xuanzx.com

Go:   return a, b
来源：http://rip.ybcxt.top

Ruby: return a, b
来源：http://nmm.cheryme.top

C#:   return (a, b);              // ValueTuple
来源：http://yls.epnwcf.com

[C06] 匿名函数 / lambda
来源：http://ewy.uphjek.com

Py:   square = lambda x: x * x
来源：http://gcn.52xcode.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hem.daria6918.cn

JS:   const square = x => x * x;
来源：http://bqr.shanyushiyangtech.top

TS:   const square = (x: number): number => x * x;
来源：http://uao.zycfv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://vsm.yueranfly.top

Go:   sq := func(x int) int { return x * x }
来源：http://wcm.aizwys.cn

Ruby: square = ->(x) { x * x }
来源：http://hnc.nanxinkj.top

C#:   Func<int, int> square = x => x * x;
来源：http://vio.aizwys.cn

[C07] 把函数作为参数传入
来源：http://psz.xuetiantiany.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://zwb.yongpay.top

PHP:  array_map("strtoupper", $arr);
来源：http://hix.jyoumei.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://rrc.svipenyu.cn

TS:   arr.map(String)
来源：http://wcw.jyoumei.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kan.guannengcc.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ptb.c1oappe.top

Ruby: arr.map(&:upcase)
来源：http://ncc.fengsongda.top

C#:   arr.Select(s => s.ToUpper())
来源：http://wke.zhengqikj.top

[C08] 闭包
来源：http://avb.bjfxy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://efc.guowangkeji.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uge.jianghu66.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cfb.sjlbkw.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hes.zhixingplan.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rca.jlsjyb.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ies.svipenyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://usg.uphjek.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vrb.yanxiufei.cn

[C09] 递归
来源：http://cnk.cheryme.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sch.hnxiangtu.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ndi.ydjk.org.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sun.hongshengwenyu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sjs.ydzc1.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://niv.xziqi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://leq.snrcjt.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://svk.cqqwz.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hye.jinqigufen.top

[C10] 变量作用域
来源：http://ged.jlsjyb.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mjf.hywenlv.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xsx.yueranfly.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://oda.jianghu66.top

TS:   同 JS
来源：http://sja.zdqjudy.top

Java: 方法内为块级作用域
来源：http://psz.jqgufenzy.top

Go:   花括号块级作用域
来源：http://wdn.chenlongwang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fcw.fzhhl.top

C#:   块级作用域
来源：http://ikr.52xcode.cn

[C11] 模块导入与导出
来源：http://hrz.bbcook.cn

Py:   from module import func
来源：http://bxv.shangyingyoupin.top

PHP:  require "file.php";  或 use App\Service;
来源：http://awd.ivvv.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://zsg.zycfv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jmq.tarul.cn

Java: import java.util.List;
来源：http://gzn.yj20258888.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zym.shanyushiyangkeji.top

Ruby: require "json"; require_relative "./util"
来源：http://kyy.ywan-chungtsiang.top

C#:   using System.Text;
来源：http://ebi.nanxinkj.top

[C12] 立即执行函数 IIFE
来源：http://gpj.jinqigfzy.top

Py:   (lambda: print("run"))()
来源：http://dpu.zhijiandao.cn

PHP:  (function () { echo "run"; })();
来源：http://vip.jinghuilouyu.cn

JS:   (() => { console.log("run"); })();
来源：http://fom.fzhhl.top

TS:   (() => { console.log("run"); })();
来源：http://nnp.hywenlv.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://adi.gzhubu.top

Go:   func() { fmt.Println("run") }()
来源：http://get.hnqzz.top

Ruby: -> { puts "run" }.call
来源：http://ovy.fengsongda.top

C#:   // 无 IIFE：用静态构造函数
来源：http://gwu.ppjwa.cn

[C13] 类型声明 / 类型注解
来源：http://ipp.epnwcf.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cxh.0kj1m.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nha.guowangkeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ypx.meibo888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lvj.shangyingyoupin.top

Java: int add(int a, int b) { return a + b; }
来源：http://asp.zhixingplan.top

Go:   func add(a, b int) int
来源：http://rgf.tanke756.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ywn.hnqzz.top

C#:   int Add(int a, int b) => a + b;
来源：http://yep.zhixingplan.top

[C14] 泛型函数
来源：http://mlt.wangshuangyany.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vxa.316326.xyz

PHP:  // 无泛型
来源：http://ssy.cheryme.top

JS:   // 无泛型
来源：http://xlw.shanyushiyangkeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wdh.gzhubu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xgs.jinyuanbaomall.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ldh.uphjek.com

Ruby: # 无泛型
来源：http://bfz.52xcode.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ffb.jianghu66.top

[C15] 解构 / 展开参数
来源：http://dsh.havefunace.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://zab.andypj.xyz

PHP:  [$a, $b] = $pair;
来源：http://kqp.fzhhl.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lbk.ehwqpu.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://trv.xylfe.cn

Java: // 无解构
来源：http://ewh.hongshengwenyu.top

Go:   // 无解构
来源：http://osx.jinghuilouyu.cn


<!-- 参考信息 -->