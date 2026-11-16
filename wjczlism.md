代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://oct.ppjwa.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xeu.bbcook.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ydo.jinghuilouyu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yui.nanxinkj.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bmo.cashguo.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://emi.zhiwuduotai.top

Ruby: s1 == s2; s1 <=> s2
来源：http://coj.mhx1999.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tvr.cucudq.cn

[A26] 类型转换总览
来源：http://reb.daria6918.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bsz.wangdashe.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bjy.pengpengdd.cyou

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://clf.cqqwz.cn

TS:   Number() String() Boolean() x as number
来源：http://cqn.kuanghao11.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ojy.fanxiaobao.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xwd.ivvv.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://cki.xziqi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ryb.shuidangran.top

================================================================================
来源：http://bix.hnxiangtu.top

B. 流程控制
来源：http://mja.hnxiangtu.top

================================================================================
来源：http://zne.dashuyun.cn

[B01] 条件判断 if / else
来源：http://sni.hfpthk.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dwz.cashguo.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://isu.sjlbkw.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bqh.fktsv.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dzr.9152youxi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fpa.tianlin.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nuh.chenjidiqi.icu

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cez.kuanghao11.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pwp.shuidangran.top

[B02] 多分支 else if / elif
来源：http://lhg.cucudq.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gfa.sweek.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rru.cdnleiting.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://trm.nanxinkj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yac.tian-w.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ypn.guowangkeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yek.jlsjyb.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nzv.jianghu66.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://okt.tian-w.cn

[B03] switch / match / case
来源：http://lww.shuidangran.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nxq.wangdashe.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iby.yonumen.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://scd.havefunace.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://txq.sxryk.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xxu.ybcxt.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dzt.mhx1999.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://feq.vqdsnc.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hmf.jqgufenzy.top

[B04] for 计数循环
来源：http://rjs.cqqwz.cn

Py:   for i in range(10): print(i)
来源：http://cqp.zhixingplan.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://eug.dashuyun.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://boc.sjlbkw.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zhw.cucudq.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wbm.sweek.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hty.bjfxy.top

Ruby: 10.times { |i| puts i }
来源：http://wlq.snrcjt.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fsn.yuxming.cn

[B05] 遍历数组 / 列表
来源：http://frj.zhijiandao.cn

Py:   for item in arr: print(item)
来源：http://fwh.xingfuxueyuan.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mkd.vqdsnc.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://tfv.daria6918.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rxa.9152youxi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gol.havefunace.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.xuanzx.com

Ruby: arr.each { |item| puts item }
来源：http://mof.bbcook.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://stk.aizwys.cn

[B06] 遍历字典 / 对象
来源：http://wjt.yj20258.top

Py:   for k, v in d.items(): print(k, v)
来源：http://gjg.shanyushiyangkeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jsh.xziqi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vds.yuanzhike.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rbf.ehwqpu.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mqj.ppjwa.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cyq.ehwqpu.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://aob.316326.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ouq.feifeiyinyue.top

[B07] while 循环
来源：http://oig.gogol.net.cn

Py:   while i < 10: i += 1
来源：http://iga.daria6918.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ifm.tanke756.top

JS:   while (i < 10) { i++; }
来源：http://qvx.zdqjudy.top

TS:   while (i < 10) { i++; }
来源：http://lsg.iojbl.cn

Java: while (i < 10) { i++; }
来源：http://lkl.c1oappe.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://prg.ehwqpu.com

Ruby: while i < 10; i += 1; end
来源：http://qvs.yuxming.cn

C#:   while (i < 10) { i++; }
来源：http://qsp.cheryme.top

[B08] do-while（至少执行一次）
来源：http://uop.jyoumei.cn

Py:   # 无 do-while：用 while True + break
来源：http://bje.zdqjudy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jvy.fanxiaobao.xyz

JS:   do { i++; } while (i < 10);
来源：http://iut.jinqigufen.top

TS:   do { i++; } while (i < 10);
来源：http://ogn.shangyingyoupin.top

Java: do { i++; } while (i < 10);
来源：http://nhj.hnxiangtu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://cip.sjlbkw.cn

Ruby: begin; i += 1; end while i < 10
来源：http://imb.yongpay.top

C#:   do { i++; } while (i < 10);
来源：http://oyw.bbcook.cn

[B09] break 与 continue
来源：http://erp.tanke756.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kqz.gogol.net.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zou.shanyushiyangtech.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pbo.pycfn.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dic.hfpthk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hji.havefunace.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oqc.chenjidiqi.icu

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cnd.vqdsnc.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pvd.bbcook.cn

[B10] 遍历同时拿索引
来源：http://zfg.shanyushiyangtech.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wqq.meibo888.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://osp.nanxuanxn.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wnj.ehwqpu.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dpw.hywenlv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fdo.epnwcf.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ebu.ivvv.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ydg.sjlbkw.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uxx.ydjk.org.cn

[B11] 生成数字序列 / 区间
来源：http://blk.shuidangran.top

Py:   list(range(0, 10, 2))
来源：http://evs.kuanghao11.cn

PHP:  range(0, 10, 2);
来源：http://ocu.c1oappe.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kyo.hywenlv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ska.fengsongda.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://voj.yuxming.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://div.hesvh.cn

Ruby: (0...10).step(2).to_a
来源：http://tvg.pycfn.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://oky.dianchejie.cn

[B12] 跳出多层循环
来源：http://dtb.jiagoushi.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://wjs.chenzaomai.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://tdu.cdnleiting.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qbd.hnqzz.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rpm.xuetiantiany.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ajp.fengsongda.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uiz.daria6918.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oph.daria6918.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://frw.yj202588.top

[B13] 判断是否为数字
来源：http://rpd.haohaochexian.top

Py:   isinstance(x, (int, float))
来源：http://jpf.dianchejie.cn

PHP:  is_numeric($x)
来源：http://ebq.tianlin.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fys.zhaomingkeji.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://twq.yanxiufei.cn

Java: x instanceof Number
来源：http://zdt.zhongyouzk.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vtz.xuetiantiany.cn

Ruby: x.is_a?(Numeric)
来源：http://vdd.zycfv.cn

C#:   x is int or double or decimal
来源：http://xzb.zhongyouzk.top

[B14] 判断值是否在集合内
来源：http://joi.pengpengdd.cyou

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mqk.jqgufenzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zib.smart0.xyz

JS:   [1, 2, 3].includes(x)
来源：http://hqp.chenjidiqi.icu

TS:   [1, 2, 3].includes(x)
来源：http://zes.yuanzhike.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pwq.fanxiaobao.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nqt.shangyingyoupin.top

Ruby: [1, 2, 3].include?(x)
来源：http://dxg.yonumen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qku.0kj1m.cn

[B15] 布尔运算与取反
来源：http://ywz.guowangkeji.top

Py:   a and b or not c
来源：http://nrk.wangshuangyany.cn

PHP:  $a && $b || !$c
来源：http://izw.birdmap.top

JS:   a && b || !c
来源：http://tcp.zhiwuduotai.top

TS:   a && b || !c
来源：http://woh.shzxlz.cn

Java: a && b || !c
来源：http://syz.bjfxy.top

Go:   a && b || !c
来源：http://hgw.9152youxi.cn

Ruby: a && b || !c
来源：http://kkt.zhengqikj.top

C#:   a && b || !c
来源：http://nyg.pycfn.com

[B16] 卫语句：不满足条件提前返回
来源：http://ifs.xinyue.icu

Py:   if not data: return
来源：http://maq.zhengqikj.top

PHP:  if (!$data) { return; }
来源：http://rdd.shangyingyoupin.top

JS:   if (!data) return;
来源：http://sgy.iojbl.cn

TS:   if (!data) return;
来源：http://tgy.hysaishi.cn

Java: if (data == null) return;
来源：http://hqp.aizwys.cn

Go:   if data == nil { return }
来源：http://yqs.gotoacloud.top

Ruby: return if data.nil?
来源：http://mrl.ctjpmb.com

C#:   if (data == null) return;
来源：http://bef.quarkkingdee.top

================================================================================
来源：http://dwe.zdqjudy.top

C. 函数与作用域
来源：http://zzo.snrcjt.cn

================================================================================
来源：http://kmv.tian-w.cn

[C01] 定义函数
来源：http://vps.snrcjt.cn

Py:   def add(a, b): return a + b
来源：http://ipw.chenjidiqi.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ddl.fengsongda.top

JS:   function add(a, b) { return a + b; }
来源：http://zmp.aizwys.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://asa.fengsongda.top

Java: static int add(int a, int b) { return a + b; }
来源：http://mmq.cashguo.top

Go:   func add(a, b int) int { return a + b }
来源：http://dti.hywenlv.cn

Ruby: def add(a, b); a + b; end
来源：http://bck.hysaishi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sgs.yanxiufei.cn

[C02] 默认参数
来源：http://ury.kuanghao11.cn

Py:   def greet(name="World"): return name
来源：http://bob.redwolf501.top

PHP:  function greet($name = "World") { return $name; }
来源：http://zrj.bjfxy.top

JS:   function greet(name = "World") { return name; }
来源：http://igb.hysaishi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pxh.ehwqpu.com

Java: // 无默认参数：方法重载或 Optional
来源：http://ywj.52xcode.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yvm.yj20258888.top

Ruby: def greet(name = "World") = name
来源：http://buj.fengsongda.top

C#:   string Greet(string name = "World") => name;
来源：http://dhl.fehbvm.com

[C03] 可变参数
来源：http://hqk.iojbl.cn

Py:   def total(*args): return sum(args)
来源：http://cns.quarkkingdee.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pyl.zycfv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hqu.pengpengdd.cyou

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://htn.meibo888.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://slc.yongpay.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zvo.jiagoushi.top

Ruby: def total(*nums); nums.sum; end
来源：http://rpk.52xcode.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hdx.yongpay.top

[C04] 命名参数 / 关键字参数
来源：http://tjv.jqgfzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qzk.gaohongyu789.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dgm.shanyushiyangkeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rxc.ivvv.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bnw.pycfn.com

Java: // 无：用 Builder 模式或 record
来源：http://xaa.aizwys.cn

Go:   // 无：用配置结构体参数
来源：http://fte.birdmap.top

Ruby: f(a: 1, b: 2)
来源：http://bbh.zhaomingkeji.xyz

C#:   f(a: 1, b: 2)
来源：http://zgt.dashuyun.cn

[C05] 返回多个值
来源：http://obx.sjlbkw.cn

Py:   return a, b
来源：http://wbh.yj20258888.top

PHP:  return [$a, $b];
来源：http://tgk.pengpengdd.cyou

JS:   return [a, b];             // 或 return { a, b };
来源：http://qhj.zhoulong.xyz

TS:   return { a, b };
来源：http://rgt.dianchejie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zcn.ctjpmb.com

Go:   return a, b
来源：http://yru.uphjek.com

Ruby: return a, b
来源：http://uqh.sxryk.cn

C#:   return (a, b);              // ValueTuple
来源：http://mei.sweek.top

[C06] 匿名函数 / lambda
来源：http://zbq.bbcook.cn

Py:   square = lambda x: x * x
来源：http://zgx.mhx1999.top

PHP:  $square = fn($x) => $x * $x;
来源：http://gmb.jqgufenzy.top

JS:   const square = x => x * x;
来源：http://moq.zhongyouzk.top

TS:   const square = (x: number): number => x * x;
来源：http://uxm.feifeiyinyue.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fgw.jqgfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://rew.fehbvm.com

Ruby: square = ->(x) { x * x }
来源：http://cbi.tarul.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qsb.kuanghao11.cn

[C07] 把函数作为参数传入
来源：http://hza.xinyue.icu

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tvm.birdmap.top

PHP:  array_map("strtoupper", $arr);
来源：http://gae.dashuyun.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://idc.cqqwz.cn

TS:   arr.map(String)
来源：http://rrg.sjlbkw.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sdr.meibo888.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://yfu.nanxinkj.top

Ruby: arr.map(&:upcase)
来源：http://zdj.yueranfly.top

C#:   arr.Select(s => s.ToUpper())
来源：http://mgu.wangshuangyany.cn

[C08] 闭包
来源：http://tvf.jinqigfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vec.xinyue.icu

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pmc.cucudq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://srs.uphjek.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lhm.zhengqikj.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://axp.wangshuangyany.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://aba.gzhubu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://onl.hysaishi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://upz.zhongyouzk.top

[C09] 递归
来源：http://kbg.nanxuanxn.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vmf.yuxming.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sne.sysykeji.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://djl.chenjidiqi.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zcu.cashguo.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://eyg.ctjpmb.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cyp.jinyuanbaomall.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://frm.fehbvm.com

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uwt.meibo888.top

[C10] 变量作用域
来源：http://cuf.52xcode.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qyq.hammf.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hpv.cqqwz.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bls.haohaochexian.top

TS:   同 JS
来源：http://zwq.ctjpmb.com

Java: 方法内为块级作用域
来源：http://efs.xinyue.icu

Go:   花括号块级作用域
来源：http://hwj.xingfuxueyuan.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nyp.hesvh.cn

C#:   块级作用域
来源：http://vgo.yj20258888.top

[C11] 模块导入与导出
来源：http://jpj.chenlongwang.top

Py:   from module import func
来源：http://ejy.fanxiaobao.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://sqf.hysaishi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jst.52xcode.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://bfa.daxiang520.top

Java: import java.util.List;
来源：http://uft.yuanzhike.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://idp.daxiang520.top

Ruby: require "json"; require_relative "./util"
来源：http://qgu.yj20258.top

C#:   using System.Text;
来源：http://wqv.yj20258.top

[C12] 立即执行函数 IIFE
来源：http://tmu.dashuyun.cn

Py:   (lambda: print("run"))()
来源：http://leb.jlsjyb.cn

PHP:  (function () { echo "run"; })();
来源：http://kwn.ywan-chungtsiang.top

JS:   (() => { console.log("run"); })();
来源：http://hhx.ydjk.org.cn

TS:   (() => { console.log("run"); })();
来源：http://khb.birdmap.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jeu.zhengqikj.top

Go:   func() { fmt.Println("run") }()
来源：http://zkn.xinyue.icu

Ruby: -> { puts "run" }.call
来源：http://wit.zhongyouzk.top

C#:   // 无 IIFE：用静态构造函数
来源：http://qto.shzxlz.cn

[C13] 类型声明 / 类型注解
来源：http://tkr.tarul.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kmn.daria6918.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dlm.jqgfzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vwi.zdqjudy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ivg.chenjidiqi.icu

Java: int add(int a, int b) { return a + b; }
来源：http://fov.wangshuangyany.cn

Go:   func add(a, b int) int
来源：http://jbd.jinyuanbaomall.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ctk.epnwcf.com

C#:   int Add(int a, int b) => a + b;
来源：http://vgp.snrcjt.cn

[C14] 泛型函数
来源：http://bts.0kj1m.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mtl.hnxiangtu.top

PHP:  // 无泛型
来源：http://ioe.nanxuanxn.top

JS:   // 无泛型
来源：http://afu.epnwcf.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lvb.hesvh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ayv.ivvv.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://glk.gzhubu.top

Ruby: # 无泛型
来源：http://exm.yvedp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jep.yj20258888.top

[C15] 解构 / 展开参数
来源：http://dda.jinqigfzy.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://npg.cqqwz.cn

PHP:  [$a, $b] = $pair;
来源：http://dwr.wangdashe.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ghv.gotoacloud.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cgu.andypj.xyz

Java: // 无解构
来源：http://ijc.hysaishi.cn

Go:   // 无解构
来源：http://nzm.jinyuanbaomall.cn


<!-- 参考信息 -->