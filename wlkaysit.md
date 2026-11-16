代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://bst.zhixingplan.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ujz.guowangkeji.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nvu.fktsv.cn

[A25] 字符串比较
来源：http://tlv.ctjpmb.com

Py:   s1 == s2; s1 != s2
来源：http://zcy.bjfxy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://olz.yj20258888.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://nlw.zhiwuduotai.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qca.zhaomingkeji.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uiu.fktsv.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xeq.jlsjyb.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://koj.wangshuangyany.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uvk.gaohongyu789.top

[A26] 类型转换总览
来源：http://qde.zhiwuduotai.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://clc.haohaochexian.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lio.jqgufenzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://aau.jinqigfzy.top

TS:   Number() String() Boolean() x as number
来源：http://rlf.jiagoushi.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hsc.jiagoushi.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://anw.ybcxt.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://cjj.jinghuilouyu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xdl.yfazqb.com

================================================================================
来源：http://nkh.daxiang520.top

B. 流程控制
来源：http://rrw.fzhhl.top

================================================================================
来源：http://nzs.smart0.xyz

[B01] 条件判断 if / else
来源：http://yky.jinqigfzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://min.ehwqpu.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ezf.xziqi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zwm.hnxiangtu.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jdk.aizwys.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://seg.aibaodan.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gxl.jyoumei.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hrv.sysykeji.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yrw.hysaishi.cn

[B02] 多分支 else if / elif
来源：http://ewb.zhiwuduotai.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fps.cucudq.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gwo.zhengqikj.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cmi.fehbvm.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kyq.bjfxy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pfn.gzhubu.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fwz.jlsjyb.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qyw.ybcxt.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ymk.ydjk.org.cn

[B03] switch / match / case
来源：http://ltq.fehbvm.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rwi.sufxvd.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lzb.shangyingyoupin.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ziy.daxiang520.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yhr.andypj.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wjq.yueranfly.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xkn.zhaomingkeji.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ucf.feifeiyinyue.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iah.yonumen.top

[B04] for 计数循环
来源：http://tsw.nanxinkj.top

Py:   for i in range(10): print(i)
来源：http://mtw.cashguo.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mbl.xinyue.icu

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qtj.hnqzz.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://coo.zhoulong.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://abd.zhiwuduotai.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://upq.nanxuanxn.top

Ruby: 10.times { |i| puts i }
来源：http://lkq.bjfxy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://shm.fehbvm.com

[B05] 遍历数组 / 列表
来源：http://jad.redwolf501.top

Py:   for item in arr: print(item)
来源：http://dit.yuxming.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://est.havefunace.top

JS:   for (const item of arr) { console.log(item); }
来源：http://dee.jinghuilouyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://yky.jqgufenzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ajl.chenzaomai.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hvl.hywenlv.cn

Ruby: arr.each { |item| puts item }
来源：http://jmw.xziqi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rtw.hfpthk.cn

[B06] 遍历字典 / 对象
来源：http://gyw.wangdashe.top

Py:   for k, v in d.items(): print(k, v)
来源：http://yxp.hnqzz.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dht.yj202588.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://prj.nanxuanxn.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qfn.tanke756.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zgl.redwolf501.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fnw.pycfn.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ziy.jinghuilouyu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nvs.yanxiufei.cn

[B07] while 循环
来源：http://xdx.yfazqb.com

Py:   while i < 10: i += 1
来源：http://jrl.yj20258.top

PHP:  while ($i < 10) { $i++; }
来源：http://sdv.tian-w.cn

JS:   while (i < 10) { i++; }
来源：http://euv.zdqjudy.top

TS:   while (i < 10) { i++; }
来源：http://cyd.zhijiandao.cn

Java: while (i < 10) { i++; }
来源：http://mzf.yvedp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://scp.gotoacloud.top

Ruby: while i < 10; i += 1; end
来源：http://law.yj20258888.top

C#:   while (i < 10) { i++; }
来源：http://hcx.hnxiangtu.top

[B08] do-while（至少执行一次）
来源：http://drs.316326.xyz

Py:   # 无 do-while：用 while True + break
来源：http://vdx.yuanzhike.top

PHP:  do { $i++; } while ($i < 10);
来源：http://yzl.jlsjyb.cn

JS:   do { i++; } while (i < 10);
来源：http://ygw.xuetiantiany.cn

TS:   do { i++; } while (i < 10);
来源：http://uta.yanxiufei.cn

Java: do { i++; } while (i < 10);
来源：http://wso.sxryk.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://vrz.ctjpmb.com

Ruby: begin; i += 1; end while i < 10
来源：http://tjc.jinqigufen.top

C#:   do { i++; } while (i < 10);
来源：http://glb.jqgfzy.top

[B09] break 与 continue
来源：http://hag.havefunace.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nua.yueranfly.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ygz.shanyushiyangkeji.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wsq.zhijiandao.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kuf.quarkkingdee.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://clv.iojbl.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tpz.jiagoushi.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dro.9152youxi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dws.xziqi.cn

[B10] 遍历同时拿索引
来源：http://djt.yuanzhike.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dmy.hammf.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ctz.sysykeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xnd.hammf.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ewy.yj202588.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oeo.xuanzx.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nmd.wangdashe.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gid.feifeiyinyue.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vuz.zhiwuduotai.top

[B11] 生成数字序列 / 区间
来源：http://gfy.jlsjyb.cn

Py:   list(range(0, 10, 2))
来源：http://cfq.fanxiaobao.xyz

PHP:  range(0, 10, 2);
来源：http://dkt.ybcxt.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qyi.52xcode.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iug.ywan-chungtsiang.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rqv.feifeiyinyue.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://skr.kuanghao11.cn

Ruby: (0...10).step(2).to_a
来源：http://riv.vehdjk.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vux.yvedp.cn

[B12] 跳出多层循环
来源：http://kgi.aibaodan.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zal.jinyuanbaomall.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://eix.fzhhl.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cbp.hywenlv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qia.cashguo.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://klz.dashuyun.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fby.sysykeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://phi.yueranfly.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wfc.chenlongwang.top

[B13] 判断是否为数字
来源：http://ghw.guannengcc.top

Py:   isinstance(x, (int, float))
来源：http://jrp.redwolf501.top

PHP:  is_numeric($x)
来源：http://wom.chenlongwang.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mhr.jinghuilouyu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zip.tanke756.top

Java: x instanceof Number
来源：http://lgh.zycfv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zhe.316326.xyz

Ruby: x.is_a?(Numeric)
来源：http://rob.bbcook.cn

C#:   x is int or double or decimal
来源：http://iji.yj202588.top

[B14] 判断值是否在集合内
来源：http://wuf.yj20258888.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dbl.zhaomingkeji.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gny.hywenlv.cn

JS:   [1, 2, 3].includes(x)
来源：http://vrz.zhaomingkeji.xyz

TS:   [1, 2, 3].includes(x)
来源：http://pnx.cucudq.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pvd.chenzaomai.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sve.jinyuanbaomall.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cdz.yj20258888.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bvc.ydjk.org.cn

[B15] 布尔运算与取反
来源：http://cwi.mhx1999.top

Py:   a and b or not c
来源：http://nan.jinqigfzy.top

PHP:  $a && $b || !$c
来源：http://xdw.cqqwz.cn

JS:   a && b || !c
来源：http://fym.haohaochexian.top

TS:   a && b || !c
来源：http://fvt.ppjwa.cn

Java: a && b || !c
来源：http://xeg.yuxming.cn

Go:   a && b || !c
来源：http://wsb.ctjpmb.com

Ruby: a && b || !c
来源：http://gmo.zhengqikj.top

C#:   a && b || !c
来源：http://igu.tanke756.top

[B16] 卫语句：不满足条件提前返回
来源：http://dyk.jqgfzy.top

Py:   if not data: return
来源：http://anq.guowangkeji.top

PHP:  if (!$data) { return; }
来源：http://aam.uphjek.com

JS:   if (!data) return;
来源：http://lmc.hnqzz.top

TS:   if (!data) return;
来源：http://hgd.yj20258.top

Java: if (data == null) return;
来源：http://pfk.jyoumei.cn

Go:   if data == nil { return }
来源：http://xcv.vehdjk.com

Ruby: return if data.nil?
来源：http://mok.pycfn.com

C#:   if (data == null) return;
来源：http://ecx.jinyuanbaomall.cn

================================================================================
来源：http://tgo.yuanzhike.top

C. 函数与作用域
来源：http://xrh.pengpengdd.cyou

================================================================================
来源：http://eqj.quarkkingdee.top

[C01] 定义函数
来源：http://hqo.xziqi.cn

Py:   def add(a, b): return a + b
来源：http://srm.yfazqb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dqx.zhaomingkeji.xyz

JS:   function add(a, b) { return a + b; }
来源：http://xpk.ywan-chungtsiang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nil.zdqjudy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vde.pengpengdd.cyou

Go:   func add(a, b int) int { return a + b }
来源：http://fxs.jinqigfzy.top

Ruby: def add(a, b); a + b; end
来源：http://cjn.52xcode.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ojc.hfpthk.cn

[C02] 默认参数
来源：http://mbx.fanxiaobao.xyz

Py:   def greet(name="World"): return name
来源：http://wae.jinqigfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://pda.zycfv.cn

JS:   function greet(name = "World") { return name; }
来源：http://xir.ybcxt.top

TS:   function greet(name: string = "World") { return name; }
来源：http://dme.sxryk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://why.jqgfzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tir.zhiwuduotai.top

Ruby: def greet(name = "World") = name
来源：http://jtb.chenzaomai.com

C#:   string Greet(string name = "World") => name;
来源：http://rfh.haohaochexian.top

[C03] 可变参数
来源：http://kbf.sjlbkw.cn

Py:   def total(*args): return sum(args)
来源：http://krm.iojbl.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://txr.ivvv.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tul.cqqwz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qak.cdnleiting.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rpw.xziqi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ahk.316326.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://xux.fktsv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zoo.xylfe.cn

[C04] 命名参数 / 关键字参数
来源：http://agz.uphjek.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wth.chenzaomai.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lfy.smart0.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pub.pycfn.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tjr.nanxuanxn.top

Java: // 无：用 Builder 模式或 record
来源：http://dde.snrcjt.cn

Go:   // 无：用配置结构体参数
来源：http://zkk.aizwys.cn

Ruby: f(a: 1, b: 2)
来源：http://vew.uphjek.com

C#:   f(a: 1, b: 2)
来源：http://cle.cqqwz.cn

[C05] 返回多个值
来源：http://tlc.daxiang520.top

Py:   return a, b
来源：http://yit.jinqigfzy.top

PHP:  return [$a, $b];
来源：http://pjg.ivvv.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://czz.yangfankeji.com

TS:   return { a, b };
来源：http://lns.yj20258888.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qit.sweek.top

Go:   return a, b
来源：http://trz.ppjwa.cn

Ruby: return a, b
来源：http://itj.pycfn.com

C#:   return (a, b);              // ValueTuple
来源：http://feq.yangfankeji.com

[C06] 匿名函数 / lambda
来源：http://vvk.cqqwz.cn

Py:   square = lambda x: x * x
来源：http://wcq.shzxlz.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dbf.yueranfly.top

JS:   const square = x => x * x;
来源：http://gfz.zhongyouzk.top

TS:   const square = (x: number): number => x * x;
来源：http://caw.0kj1m.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tmf.vqdsnc.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dbh.ehwqpu.com

Ruby: square = ->(x) { x * x }
来源：http://bpu.hysaishi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://crz.hongshengwenyu.top

[C07] 把函数作为参数传入
来源：http://ypt.jianghu66.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ymm.zdqjudy.top

PHP:  array_map("strtoupper", $arr);
来源：http://ici.hysaishi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lho.jlsjyb.cn

TS:   arr.map(String)
来源：http://chy.birdmap.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://osn.tian-w.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cyx.gzhubu.top

Ruby: arr.map(&:upcase)
来源：http://qop.shanyushiyangkeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://wua.hesvh.cn

[C08] 闭包
来源：http://wjl.jinqigfzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://scj.cqqwz.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bdz.feifeiyinyue.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hur.jinqigfzy.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dbw.ywan-chungtsiang.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://iuj.chenlongwang.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qsz.aizwys.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fcg.zhaomingkeji.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mbu.mhx1999.top

[C09] 递归
来源：http://pul.ydjk.org.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ffh.bjfxy.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://pww.9152youxi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mbz.hnqzz.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qjt.hcnkem.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://fkq.ybcxt.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ppy.cheryme.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ais.hywenlv.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://epa.gaohongyu789.top

[C10] 变量作用域
来源：http://lbe.ywan-chungtsiang.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wwb.guowangkeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jjm.fengsongda.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mqy.zhijiandao.cn

TS:   同 JS
来源：http://mor.sysykeji.top

Java: 方法内为块级作用域
来源：http://yrg.sufxvd.cn

Go:   花括号块级作用域
来源：http://mlm.nwbrower.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://frc.yj20258888.top

C#:   块级作用域
来源：http://joo.kuanghao11.cn

[C11] 模块导入与导出
来源：http://jyr.smart0.xyz

Py:   from module import func
来源：http://idl.jqgufenzy.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vtd.zdbjq.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rcl.jqgfzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gey.yfazqb.com

Java: import java.util.List;
来源：http://tqs.cqqwz.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nhf.0kj1m.cn

Ruby: require "json"; require_relative "./util"
来源：http://bxp.cheryme.top

C#:   using System.Text;
来源：http://nkv.zdqjudy.top

[C12] 立即执行函数 IIFE
来源：http://mtb.hongshengwenyu.top

Py:   (lambda: print("run"))()
来源：http://wtx.9152youxi.cn

PHP:  (function () { echo "run"; })();
来源：http://pgj.tianlin.xyz

JS:   (() => { console.log("run"); })();
来源：http://llh.9152youxi.cn

TS:   (() => { console.log("run"); })();
来源：http://kzj.xuetiantiany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zvr.yfazqb.com

Go:   func() { fmt.Println("run") }()
来源：http://fus.0kj1m.cn

Ruby: -> { puts "run" }.call
来源：http://npx.316326.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://ivh.fktsv.cn

[C13] 类型声明 / 类型注解
来源：http://rku.ydjk.org.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xuo.pycfn.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mbn.tanke756.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lft.zhiwuduotai.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://myr.hysaishi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lux.bjfxy.top

Go:   func add(a, b int) int
来源：http://fbq.xylfe.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pty.zhoulong.xyz

C#:   int Add(int a, int b) => a + b;
来源：http://ecs.epnwcf.com

[C14] 泛型函数
来源：http://kmc.cashguo.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zxp.fehbvm.com

PHP:  // 无泛型
来源：http://qpq.sweek.top

JS:   // 无泛型
来源：http://gep.jqgufenzy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cwn.yongpay.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mvm.fanxiaobao.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fms.52xcode.cn

Ruby: # 无泛型
来源：http://jvt.jinghuilouyu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xml.hammf.cn

[C15] 解构 / 展开参数
来源：http://fbs.daria6918.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ejz.iojbl.cn

PHP:  [$a, $b] = $pair;
来源：http://gxe.cheryme.top


<!-- 参考信息 -->