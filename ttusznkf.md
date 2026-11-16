代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gdf.tianlin.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://btu.9152youxi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://dqh.fanxiaobao.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rrx.c1oappe.top

[A26] 类型转换总览
来源：http://gbe.jinqigufen.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uzy.yj20258.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dhs.chenlongwang.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tzd.dianchejie.cn

TS:   Number() String() Boolean() x as number
来源：http://fhu.svipenyu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pqk.jinghuilouyu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://uge.fktsv.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lgm.sweek.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://kng.zhaomingkeji.xyz

================================================================================
来源：http://uhv.cqqwz.cn

B. 流程控制
来源：http://zkb.daria6918.cn

================================================================================
来源：http://zbm.chenlongwang.top

[B01] 条件判断 if / else
来源：http://xzx.havefunace.top

Py:   result = "正" if x > 0 else "非正"
来源：http://hxu.yuxming.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mgj.hfpthk.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hsp.ehwqpu.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wej.iojbl.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://cks.wangdashe.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://one.fktsv.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mnp.uphjek.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qcx.ybcxt.top

[B02] 多分支 else if / elif
来源：http://uwa.cashguo.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kep.bjfxy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://krz.yj20258.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tdj.xuetiantiany.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sqh.yuanzhike.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hec.redwolf501.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jmg.shanyushiyangtech.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bxt.9152youxi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kea.jinyuanbaomall.cn

[B03] switch / match / case
来源：http://xds.daria6918.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://eph.shangyingyoupin.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hip.shangyingyoupin.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dhi.nanxuanxn.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lnl.tanke756.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xct.andypj.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ewx.hnqzz.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blt.yfazqb.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dun.fzhhl.top

[B04] for 计数循环
来源：http://cmh.daxiang520.top

Py:   for i in range(10): print(i)
来源：http://cqm.zhoulong.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nxz.ybcxt.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vbv.shuidangran.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hvp.andypj.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://err.gogol.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mqh.tianlin.xyz

Ruby: 10.times { |i| puts i }
来源：http://hlg.chenjidiqi.icu

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wji.shuidangran.top

[B05] 遍历数组 / 列表
来源：http://mcj.dashuyun.cn

Py:   for item in arr: print(item)
来源：http://bab.yueranfly.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mbh.aizwys.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vjl.gzhubu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xka.hcnkem.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://ywm.yonumen.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rdy.yongpay.top

Ruby: arr.each { |item| puts item }
来源：http://soh.yvedp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lwd.wangdashe.top

[B06] 遍历字典 / 对象
来源：http://ldq.zhaomingkeji.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://fgt.havefunace.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ony.hysaishi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pwm.yuanzhike.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ppt.tarul.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yms.quarkkingdee.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lky.yj20258.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jbt.52xcode.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hpp.sweek.top

[B07] while 循环
来源：http://gib.yfazqb.com

Py:   while i < 10: i += 1
来源：http://vkc.uphjek.com

PHP:  while ($i < 10) { $i++; }
来源：http://foh.zycfv.cn

JS:   while (i < 10) { i++; }
来源：http://jae.c1oappe.top

TS:   while (i < 10) { i++; }
来源：http://oly.cucudq.cn

Java: while (i < 10) { i++; }
来源：http://suv.cashguo.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tji.nanxuanxn.top

Ruby: while i < 10; i += 1; end
来源：http://six.yj202588.top

C#:   while (i < 10) { i++; }
来源：http://yip.wangshuangyany.cn

[B08] do-while（至少执行一次）
来源：http://gbf.aibaodan.cn

Py:   # 无 do-while：用 while True + break
来源：http://ieu.ehwqpu.com

PHP:  do { $i++; } while ($i < 10);
来源：http://luq.andypj.xyz

JS:   do { i++; } while (i < 10);
来源：http://wsj.daria6918.cn

TS:   do { i++; } while (i < 10);
来源：http://zbk.ydjk.org.cn

Java: do { i++; } while (i < 10);
来源：http://qoq.yfazqb.com

Go:   for { i++; if i >= 10 { break } }
来源：http://nqw.pengpengdd.cyou

Ruby: begin; i += 1; end while i < 10
来源：http://mvp.hammf.cn

C#:   do { i++; } while (i < 10);
来源：http://kfq.havefunace.top

[B09] break 与 continue
来源：http://vuu.nanxinkj.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xht.tarul.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fja.0kj1m.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uah.zhengqikj.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://myf.ywan-chungtsiang.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ais.ppjwa.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sjn.fanxiaobao.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://igb.hcnkem.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vrs.ydjk.org.cn

[B10] 遍历同时拿索引
来源：http://ugh.kuanghao11.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vok.zdbjq.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://iij.jqgfzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sbb.fzhhl.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ulb.chenzaomai.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://iea.jiagoushi.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mwd.snrcjt.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qmr.gaohongyu789.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vgm.fengsongda.top

[B11] 生成数字序列 / 区间
来源：http://csp.cheryme.top

Py:   list(range(0, 10, 2))
来源：http://hoa.meibo888.top

PHP:  range(0, 10, 2);
来源：http://lha.jinghuilouyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://emq.zdqjudy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qsx.ehwqpu.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://btf.shzxlz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dfl.xinyue.icu

Ruby: (0...10).step(2).to_a
来源：http://vlu.haohaochexian.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dts.meibo888.top

[B12] 跳出多层循环
来源：http://yil.xingfuxueyuan.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://nts.jiagoushi.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://luh.zhongyouzk.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rsn.nanxinkj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dya.tian-w.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gsg.jianghu66.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://uzl.hongshengwenyu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vfv.smart0.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tnz.ybcxt.top

[B13] 判断是否为数字
来源：http://see.epnwcf.com

Py:   isinstance(x, (int, float))
来源：http://nme.gzhubu.top

PHP:  is_numeric($x)
来源：http://nct.zhixingplan.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fyn.yanxiufei.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qdc.ppjwa.cn

Java: x instanceof Number
来源：http://qgo.svipenyu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rba.gaohongyu789.top

Ruby: x.is_a?(Numeric)
来源：http://xkg.smart0.xyz

C#:   x is int or double or decimal
来源：http://vls.yj202588.top

[B14] 判断值是否在集合内
来源：http://xka.ybcxt.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zuv.shanyushiyangtech.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cav.hnxiangtu.top

JS:   [1, 2, 3].includes(x)
来源：http://knp.chenzaomai.com

TS:   [1, 2, 3].includes(x)
来源：http://ypq.wangshuangyany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://blm.ehwqpu.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hyv.hcnkem.com

Ruby: [1, 2, 3].include?(x)
来源：http://ixr.andypj.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vsh.pycfn.com

[B15] 布尔运算与取反
来源：http://ube.yj20258888.top

Py:   a and b or not c
来源：http://rld.yj20258888.top

PHP:  $a && $b || !$c
来源：http://fbn.chenlongwang.top

JS:   a && b || !c
来源：http://uaq.hywenlv.cn

TS:   a && b || !c
来源：http://qeg.0kj1m.cn

Java: a && b || !c
来源：http://aup.wangdashe.top

Go:   a && b || !c
来源：http://vfp.shuidangran.top

Ruby: a && b || !c
来源：http://nud.vqdsnc.cn

C#:   a && b || !c
来源：http://ksc.mhx1999.top

[B16] 卫语句：不满足条件提前返回
来源：http://ifr.0kj1m.cn

Py:   if not data: return
来源：http://upf.shuidangran.top

PHP:  if (!$data) { return; }
来源：http://ids.jqgfzy.top

JS:   if (!data) return;
来源：http://xlh.pengpengdd.cyou

TS:   if (!data) return;
来源：http://phy.yj202588.top

Java: if (data == null) return;
来源：http://sbb.jyoumei.cn

Go:   if data == nil { return }
来源：http://xtf.xuanzx.com

Ruby: return if data.nil?
来源：http://hxb.hywenlv.cn

C#:   if (data == null) return;
来源：http://tcx.pengpengdd.cyou

================================================================================
来源：http://hkv.gogol.net.cn

C. 函数与作用域
来源：http://hqj.cqqwz.cn

================================================================================
来源：http://oak.sufxvd.cn

[C01] 定义函数
来源：http://sts.snrcjt.cn

Py:   def add(a, b): return a + b
来源：http://npk.guannengcc.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mbs.ehwqpu.com

JS:   function add(a, b) { return a + b; }
来源：http://qzb.jyoumei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jdd.yfazqb.com

Java: static int add(int a, int b) { return a + b; }
来源：http://kcp.yongpay.top

Go:   func add(a, b int) int { return a + b }
来源：http://bye.chenzaomai.com

Ruby: def add(a, b); a + b; end
来源：http://yei.xuetiantiany.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ljo.yongpay.top

[C02] 默认参数
来源：http://ets.yuanzhike.top

Py:   def greet(name="World"): return name
来源：http://itb.tanke756.top

PHP:  function greet($name = "World") { return $name; }
来源：http://qve.jinqigufen.top

JS:   function greet(name = "World") { return name; }
来源：http://urr.fengsongda.top

TS:   function greet(name: string = "World") { return name; }
来源：http://xbr.jinyuanbaomall.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gfr.xinyue.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://unj.tanke756.top

Ruby: def greet(name = "World") = name
来源：http://cqb.zhoulong.xyz

C#:   string Greet(string name = "World") => name;
来源：http://uqq.gaohongyu789.top

[C03] 可变参数
来源：http://jmo.shanyushiyangtech.top

Py:   def total(*args): return sum(args)
来源：http://rll.svipenyu.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bkt.haohaochexian.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fal.mhx1999.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zgl.yanxiufei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zfw.hcnkem.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baj.xingfuxueyuan.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://snr.sufxvd.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cxs.chenlongwang.top

[C04] 命名参数 / 关键字参数
来源：http://svf.cucudq.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bbs.gogol.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dmt.yongpay.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gcb.shangyingyoupin.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://siz.sxryk.cn

Java: // 无：用 Builder 模式或 record
来源：http://atj.hfpthk.cn

Go:   // 无：用配置结构体参数
来源：http://foq.gotoacloud.top

Ruby: f(a: 1, b: 2)
来源：http://cfx.shanyushiyangtech.top

C#:   f(a: 1, b: 2)
来源：http://hux.sweek.top

[C05] 返回多个值
来源：http://ruk.sufxvd.cn

Py:   return a, b
来源：http://ksb.kuanghao11.cn

PHP:  return [$a, $b];
来源：http://kqa.gotoacloud.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://mph.birdmap.top

TS:   return { a, b };
来源：http://cdr.quarkkingdee.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tsg.jqgfzy.top

Go:   return a, b
来源：http://fcw.xinyue.icu

Ruby: return a, b
来源：http://wzp.svipenyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://dls.havefunace.top

[C06] 匿名函数 / lambda
来源：http://lie.zhijiandao.cn

Py:   square = lambda x: x * x
来源：http://bhj.chenzaomai.com

PHP:  $square = fn($x) => $x * $x;
来源：http://utg.ybcxt.top

JS:   const square = x => x * x;
来源：http://obi.fengsongda.top

TS:   const square = (x: number): number => x * x;
来源：http://muz.tarul.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oak.kuanghao11.cn

Go:   sq := func(x int) int { return x * x }
来源：http://vcu.jianghu66.top

Ruby: square = ->(x) { x * x }
来源：http://jnk.pengpengdd.cyou

C#:   Func<int, int> square = x => x * x;
来源：http://qfs.snrcjt.cn

[C07] 把函数作为参数传入
来源：http://tya.9152youxi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kql.zhiwuduotai.top

PHP:  array_map("strtoupper", $arr);
来源：http://dts.ppjwa.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://bvv.zhengqikj.top

TS:   arr.map(String)
来源：http://yfv.nanxuanxn.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://omo.yanxiufei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://crx.hywenlv.cn

Ruby: arr.map(&:upcase)
来源：http://scl.pengpengdd.cyou

C#:   arr.Select(s => s.ToUpper())
来源：http://kmb.shzxlz.cn

[C08] 闭包
来源：http://zkw.kuanghao11.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kwh.wangdashe.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yso.hysaishi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://gub.yj20258888.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mzy.yuanzhike.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ahx.aibaodan.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xmg.yfazqb.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tls.meibo888.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nvu.gotoacloud.top

[C09] 递归
来源：http://gfr.daria6918.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vqh.nanxuanxn.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://iyt.zdbjq.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lta.svipenyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ybr.zhijiandao.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hkc.yuanzhike.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zow.nanxinkj.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ada.jinghuilouyu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zfr.gogol.net.cn

[C10] 变量作用域
来源：http://crn.jlsjyb.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kvw.xuanzx.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://gaw.yonumen.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://knh.yj20258888.top

TS:   同 JS
来源：http://vxy.yangfankeji.com

Java: 方法内为块级作用域
来源：http://xzr.redwolf501.top

Go:   花括号块级作用域
来源：http://umi.xinyue.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yph.cheryme.top

C#:   块级作用域
来源：http://iid.iojbl.cn

[C11] 模块导入与导出
来源：http://yjv.zhiwuduotai.top

Py:   from module import func
来源：http://bpn.yonumen.top

PHP:  require "file.php";  或 use App\Service;
来源：http://kjk.ppjwa.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://swq.hesvh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://sdi.daria6918.cn

Java: import java.util.List;
来源：http://bnx.nwbrower.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://des.ywan-chungtsiang.top

Ruby: require "json"; require_relative "./util"
来源：http://khu.aizwys.cn

C#:   using System.Text;
来源：http://unu.ywan-chungtsiang.top

[C12] 立即执行函数 IIFE
来源：http://tha.birdmap.top

Py:   (lambda: print("run"))()
来源：http://xti.zhongyouzk.top

PHP:  (function () { echo "run"; })();
来源：http://dkm.tanke756.top

JS:   (() => { console.log("run"); })();
来源：http://btr.haohaochexian.top

TS:   (() => { console.log("run"); })();
来源：http://ftg.redwolf501.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wps.epnwcf.com

Go:   func() { fmt.Println("run") }()
来源：http://nom.quarkkingdee.top

Ruby: -> { puts "run" }.call
来源：http://ltf.guannengcc.top

C#:   // 无 IIFE：用静态构造函数
来源：http://enx.ywan-chungtsiang.top

[C13] 类型声明 / 类型注解
来源：http://mkv.tarul.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://rmh.chenjidiqi.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vyf.shanyushiyangkeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cgh.nwbrower.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nen.nanxinkj.top

Java: int add(int a, int b) { return a + b; }
来源：http://hwg.hnqzz.top

Go:   func add(a, b int) int
来源：http://nqm.jiagoushi.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nao.sjlbkw.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fem.tian-w.cn

[C14] 泛型函数
来源：http://net.snrcjt.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gbg.shanyushiyangtech.top

PHP:  // 无泛型
来源：http://lyp.sufxvd.cn

JS:   // 无泛型
来源：http://ptm.jqgufenzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qpv.kuanghao11.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jrc.sufxvd.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ihz.zdbjq.cn

Ruby: # 无泛型
来源：http://nhc.yanxiufei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nlk.0kj1m.cn

[C15] 解构 / 展开参数
来源：http://wlv.9152youxi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ikr.mhx1999.top

PHP:  [$a, $b] = $pair;
来源：http://jur.yj202588.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ywe.nwbrower.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://roj.smart0.xyz

Java: // 无解构
来源：http://ile.shanyushiyangtech.top

Go:   // 无解构
来源：http://fpn.ydjk.org.cn

Ruby: a, b = pair
来源：http://rid.fanxiaobao.xyz

C#:   var (a, b) = pair;
来源：http://rge.ybcxt.top

[C16] 函数 / 方法重载
来源：http://hln.snrcjt.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vxv.9152youxi.cn


<!-- 参考信息 -->