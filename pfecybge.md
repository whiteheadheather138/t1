代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://upj.ywan-chungtsiang.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://utc.zhongyouzk.top

Ruby: s1 == s2; s1 <=> s2
来源：http://sjc.xuetiantiany.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://irc.bjfxy.top

[A26] 类型转换总览
来源：http://ywd.sjlbkw.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://swy.jinyuanbaomall.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ybl.ctjpmb.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ucs.yuanzhike.top

TS:   Number() String() Boolean() x as number
来源：http://ims.ehwqpu.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pip.hfpthk.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sxa.ywan-chungtsiang.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://vip.0kj1m.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://khr.yangfankeji.com

================================================================================
来源：http://sfr.yfazqb.com

B. 流程控制
来源：http://wlh.xylfe.cn

================================================================================
来源：http://wew.jinyuanbaomall.cn

[B01] 条件判断 if / else
来源：http://vmh.snrcjt.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zqj.ydzc1.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lzu.tarul.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://snx.jinyuanbaomall.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fbf.hnqzz.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://vbt.shangyingyoupin.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://elc.shanyushiyangkeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gyu.hysaishi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xjn.pycfn.com

[B02] 多分支 else if / elif
来源：http://nml.haohaochexian.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://twq.xuetiantiany.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kmk.fktsv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lps.chenjidiqi.icu

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://snv.aizwys.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mmx.ppjwa.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pni.nanxuanxn.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vvw.xylfe.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eru.yonumen.top

[B03] switch / match / case
来源：http://hsw.dashuyun.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sfu.daria6918.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fri.hesvh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bxy.nanxinkj.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nfc.hesvh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://okn.hnxiangtu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://eau.xylfe.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uvs.jqgfzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mni.xuetiantiany.cn

[B04] for 计数循环
来源：http://xon.9152youxi.cn

Py:   for i in range(10): print(i)
来源：http://vei.yfazqb.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://smf.hywenlv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mxc.wangshuangyany.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://czd.fzhhl.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ubf.ivvv.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vqe.hnxiangtu.top

Ruby: 10.times { |i| puts i }
来源：http://vhx.yuanzhike.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ljz.ydjk.org.cn

[B05] 遍历数组 / 列表
来源：http://sct.hysaishi.cn

Py:   for item in arr: print(item)
来源：http://cbp.xingfuxueyuan.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dvx.bjfxy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ajw.guowangkeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://usp.jiagoushi.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://nwv.quarkkingdee.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cwy.yvedp.cn

Ruby: arr.each { |item| puts item }
来源：http://pkt.vehdjk.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dei.yfazqb.com

[B06] 遍历字典 / 对象
来源：http://krw.aibaodan.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gxr.yangfankeji.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qbw.jinghuilouyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://juu.hcnkem.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://djj.hnxiangtu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pfp.0kj1m.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://csj.sysykeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cyb.yvedp.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ecm.fktsv.cn

[B07] while 循环
来源：http://vqk.gogol.net.cn

Py:   while i < 10: i += 1
来源：http://zfb.hnxiangtu.top

PHP:  while ($i < 10) { $i++; }
来源：http://ipq.jinghuilouyu.cn

JS:   while (i < 10) { i++; }
来源：http://ncp.fzhhl.top

TS:   while (i < 10) { i++; }
来源：http://jtn.svipenyu.cn

Java: while (i < 10) { i++; }
来源：http://lwi.cashguo.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pii.yvedp.cn

Ruby: while i < 10; i += 1; end
来源：http://rjc.zdbjq.cn

C#:   while (i < 10) { i++; }
来源：http://shj.yongpay.top

[B08] do-while（至少执行一次）
来源：http://ike.jinqigfzy.top

Py:   # 无 do-while：用 while True + break
来源：http://ccz.jinghuilouyu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ajt.hcnkem.com

JS:   do { i++; } while (i < 10);
来源：http://khe.hywenlv.cn

TS:   do { i++; } while (i < 10);
来源：http://diw.zhoulong.xyz

Java: do { i++; } while (i < 10);
来源：http://dbr.zycfv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bym.zhijiandao.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hju.ctjpmb.com

C#:   do { i++; } while (i < 10);
来源：http://gkm.gaohongyu789.top

[B09] break 与 continue
来源：http://fwp.hnqzz.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://odv.cashguo.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yrz.zhengqikj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://huc.daria6918.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zgw.cashguo.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hln.daxiang520.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ydi.gaohongyu789.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tmu.jlsjyb.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gmb.tian-w.cn

[B10] 遍历同时拿索引
来源：http://fvt.fehbvm.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://guh.xuetiantiany.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rzk.bbcook.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pvb.yj20258.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uqw.zdbjq.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jmk.zhijiandao.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cdh.dashuyun.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://iel.xuetiantiany.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cnc.jinyuanbaomall.cn

[B11] 生成数字序列 / 区间
来源：http://neo.gotoacloud.top

Py:   list(range(0, 10, 2))
来源：http://yxl.vqdsnc.cn

PHP:  range(0, 10, 2);
来源：http://vxs.guannengcc.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aqv.bjfxy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cnf.xuetiantiany.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dgc.yj20258.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hxt.yangfankeji.com

Ruby: (0...10).step(2).to_a
来源：http://gie.c1oappe.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://boo.dashuyun.cn

[B12] 跳出多层循环
来源：http://kfe.c1oappe.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://dzm.sjlbkw.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://joj.chenjidiqi.icu

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://slf.feifeiyinyue.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bpu.hfpthk.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mtu.ydzc1.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mcc.xingfuxueyuan.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://soi.fzhhl.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ddq.yangfankeji.com

[B13] 判断是否为数字
来源：http://jdw.yonumen.top

Py:   isinstance(x, (int, float))
来源：http://ibh.hongshengwenyu.top

PHP:  is_numeric($x)
来源：http://rvz.guowangkeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lpl.shuidangran.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ion.gotoacloud.top

Java: x instanceof Number
来源：http://wgz.ybcxt.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vsy.0kj1m.cn

Ruby: x.is_a?(Numeric)
来源：http://itj.birdmap.top

C#:   x is int or double or decimal
来源：http://eol.daria6918.cn

[B14] 判断值是否在集合内
来源：http://tac.hfpthk.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gtj.cdnleiting.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yab.uphjek.com

JS:   [1, 2, 3].includes(x)
来源：http://lui.birdmap.top

TS:   [1, 2, 3].includes(x)
来源：http://ncr.gaohongyu789.top

Java: List.of(1, 2, 3).contains(x)
来源：http://aot.yanxiufei.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uhp.chenlongwang.top

Ruby: [1, 2, 3].include?(x)
来源：http://ulj.yj20258.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://igu.fanxiaobao.xyz

[B15] 布尔运算与取反
来源：http://fbd.mhx1999.top

Py:   a and b or not c
来源：http://rhb.jinqigfzy.top

PHP:  $a && $b || !$c
来源：http://xpr.xuetiantiany.cn

JS:   a && b || !c
来源：http://unm.jiagoushi.top

TS:   a && b || !c
来源：http://gwc.hnqzz.top

Java: a && b || !c
来源：http://riu.cashguo.top

Go:   a && b || !c
来源：http://ewe.tanke756.top

Ruby: a && b || !c
来源：http://ggj.iojbl.cn

C#:   a && b || !c
来源：http://xgp.jiagoushi.top

[B16] 卫语句：不满足条件提前返回
来源：http://imt.chenjidiqi.icu

Py:   if not data: return
来源：http://vhj.xinyue.icu

PHP:  if (!$data) { return; }
来源：http://eeb.zdbjq.cn

JS:   if (!data) return;
来源：http://piz.chenjidiqi.icu

TS:   if (!data) return;
来源：http://zmp.xingfuxueyuan.xyz

Java: if (data == null) return;
来源：http://pbz.daria6918.cn

Go:   if data == nil { return }
来源：http://zfe.xuetiantiany.cn

Ruby: return if data.nil?
来源：http://mku.shzxlz.cn

C#:   if (data == null) return;
来源：http://qmt.bjfxy.top

================================================================================
来源：http://akw.iojbl.cn

C. 函数与作用域
来源：http://dpm.cashguo.top

================================================================================
来源：http://htf.shanyushiyangkeji.top

[C01] 定义函数
来源：http://upi.wangdashe.top

Py:   def add(a, b): return a + b
来源：http://fai.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vkf.hcnkem.com

JS:   function add(a, b) { return a + b; }
来源：http://cnu.yj202588.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rea.tarul.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://aam.mhx1999.top

Go:   func add(a, b int) int { return a + b }
来源：http://ace.yvedp.cn

Ruby: def add(a, b); a + b; end
来源：http://gkj.tarul.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lwp.yanxiufei.cn

[C02] 默认参数
来源：http://dfb.yanxiufei.cn

Py:   def greet(name="World"): return name
来源：http://prn.xinyue.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://ytv.cheryme.top

JS:   function greet(name = "World") { return name; }
来源：http://wtn.yangfankeji.com

TS:   function greet(name: string = "World") { return name; }
来源：http://wah.jinyuanbaomall.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xxa.gotoacloud.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bjw.c1oappe.top

Ruby: def greet(name = "World") = name
来源：http://odw.wangdashe.top

C#:   string Greet(string name = "World") => name;
来源：http://sit.guannengcc.top

[C03] 可变参数
来源：http://rjk.zhixingplan.top

Py:   def total(*args): return sum(args)
来源：http://hbm.tanke756.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uug.hongshengwenyu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rec.xuanzx.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uue.ctjpmb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qtg.tian-w.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://quo.feifeiyinyue.top

Ruby: def total(*nums); nums.sum; end
来源：http://fno.yvedp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xbe.gaohongyu789.top

[C04] 命名参数 / 关键字参数
来源：http://kqb.hongshengwenyu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://duw.svipenyu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fps.c1oappe.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ehd.bbcook.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://juy.redwolf501.top

Java: // 无：用 Builder 模式或 record
来源：http://ztp.cashguo.top

Go:   // 无：用配置结构体参数
来源：http://lkk.jinqigfzy.top

Ruby: f(a: 1, b: 2)
来源：http://fiu.gzhubu.top

C#:   f(a: 1, b: 2)
来源：http://rie.cqqwz.cn

[C05] 返回多个值
来源：http://aka.hongshengwenyu.top

Py:   return a, b
来源：http://qlx.wangdashe.top

PHP:  return [$a, $b];
来源：http://otm.zhiwuduotai.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://sjo.jinqigufen.top

TS:   return { a, b };
来源：http://akn.fanxiaobao.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blr.yj20258888.top

Go:   return a, b
来源：http://afz.aibaodan.cn

Ruby: return a, b
来源：http://dks.jinyuanbaomall.cn

C#:   return (a, b);              // ValueTuple
来源：http://cal.ywan-chungtsiang.top

[C06] 匿名函数 / lambda
来源：http://zst.316326.xyz

Py:   square = lambda x: x * x
来源：http://jsq.ybcxt.top

PHP:  $square = fn($x) => $x * $x;
来源：http://xhe.smart0.xyz

JS:   const square = x => x * x;
来源：http://zkd.pycfn.com

TS:   const square = (x: number): number => x * x;
来源：http://aja.nwbrower.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://thv.kuanghao11.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ctl.sxryk.cn

Ruby: square = ->(x) { x * x }
来源：http://gkn.xuanzx.com

C#:   Func<int, int> square = x => x * x;
来源：http://qmx.meibo888.top

[C07] 把函数作为参数传入
来源：http://wbo.hesvh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ufc.uphjek.com

PHP:  array_map("strtoupper", $arr);
来源：http://tus.fehbvm.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ucm.epnwcf.com

TS:   arr.map(String)
来源：http://jpy.aizwys.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vwa.tarul.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kld.epnwcf.com

Ruby: arr.map(&:upcase)
来源：http://nfy.bbcook.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nvs.zhongyouzk.top

[C08] 闭包
来源：http://nmv.zhijiandao.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://lio.xuetiantiany.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bkh.cashguo.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vtj.ivvv.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vlk.gotoacloud.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xld.ydjk.org.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jwp.fzhhl.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rvr.jinghuilouyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mpq.bbcook.cn

[C09] 递归
来源：http://dve.yj20258.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vnv.jinqigufen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rkh.sxryk.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ith.9152youxi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zey.nanxinkj.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ptj.hammf.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://udg.chenzaomai.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gle.yvedp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://aae.shangyingyoupin.top

[C10] 变量作用域
来源：http://fpo.tian-w.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uhe.zhongyouzk.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://vce.gotoacloud.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xzy.0kj1m.cn

TS:   同 JS
来源：http://hcg.nwbrower.top

Java: 方法内为块级作用域
来源：http://npm.gotoacloud.top

Go:   花括号块级作用域
来源：http://mav.hnxiangtu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rgh.hywenlv.cn

C#:   块级作用域
来源：http://ouu.gaohongyu789.top

[C11] 模块导入与导出
来源：http://nli.meibo888.top

Py:   from module import func
来源：http://ytr.redwolf501.top

PHP:  require "file.php";  或 use App\Service;
来源：http://phj.yvedp.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://foa.gotoacloud.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ucz.xingfuxueyuan.xyz

Java: import java.util.List;
来源：http://pnm.cdnleiting.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eiq.shzxlz.cn

Ruby: require "json"; require_relative "./util"
来源：http://dck.quarkkingdee.top

C#:   using System.Text;
来源：http://ybl.aizwys.cn

[C12] 立即执行函数 IIFE
来源：http://bfg.dashuyun.cn

Py:   (lambda: print("run"))()
来源：http://wgz.zdbjq.cn

PHP:  (function () { echo "run"; })();
来源：http://gke.hywenlv.cn

JS:   (() => { console.log("run"); })();
来源：http://jsr.hongshengwenyu.top

TS:   (() => { console.log("run"); })();
来源：http://tsi.snrcjt.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jju.pengpengdd.cyou

Go:   func() { fmt.Println("run") }()
来源：http://xoa.shuidangran.top

Ruby: -> { puts "run" }.call
来源：http://xnx.sxryk.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ajn.zhiwuduotai.top

[C13] 类型声明 / 类型注解
来源：http://krp.chenlongwang.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xwv.yuxming.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pqr.jqgufenzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hzm.sysykeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mcu.smart0.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://ody.guowangkeji.top

Go:   func add(a, b int) int
来源：http://jze.hcnkem.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sex.ywan-chungtsiang.top

C#:   int Add(int a, int b) => a + b;
来源：http://ogo.cashguo.top

[C14] 泛型函数
来源：http://wsg.xingfuxueyuan.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hmg.uphjek.com

PHP:  // 无泛型
来源：http://zzn.yvedp.cn

JS:   // 无泛型
来源：http://dls.bbcook.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://imx.hcnkem.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rws.pycfn.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rdc.jinqigfzy.top

Ruby: # 无泛型
来源：http://dfh.0kj1m.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://luv.jyoumei.cn

[C15] 解构 / 展开参数
来源：http://pjo.daria6918.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://clt.chenjidiqi.icu

PHP:  [$a, $b] = $pair;
来源：http://zua.xylfe.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hbv.yvedp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ueg.fanxiaobao.xyz

Java: // 无解构
来源：http://ltf.zhixingplan.top

Go:   // 无解构
来源：http://jxg.0kj1m.cn

Ruby: a, b = pair
来源：http://ulc.yuxming.cn

C#:   var (a, b) = pair;
来源：http://urt.zhoulong.xyz

[C16] 函数 / 方法重载
来源：http://ywm.sweek.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xsg.hcnkem.com


<!-- 参考信息 -->