代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://uvp.zhengqikj.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://eyu.nwbrower.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nso.bbcook.cn

[A25] 字符串比较
来源：http://swi.zhoulong.xyz

Py:   s1 == s2; s1 != s2
来源：http://cmq.svipenyu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wip.zhoulong.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://obl.dashuyun.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://elv.chenjidiqi.icu

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ull.uphjek.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dfx.guannengcc.top

Ruby: s1 == s2; s1 <=> s2
来源：http://pcf.birdmap.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wbg.jianghu66.top

[A26] 类型转换总览
来源：http://oum.tarul.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mqm.sweek.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rph.zhongyouzk.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ryk.hongshengwenyu.top

TS:   Number() String() Boolean() x as number
来源：http://rav.jyoumei.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sbt.zhengqikj.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lxd.dianchejie.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://szn.xingfuxueyuan.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bcq.zhoulong.xyz

================================================================================
来源：http://yba.dianchejie.cn

B. 流程控制
来源：http://cqo.shangyingyoupin.top

================================================================================
来源：http://akx.gotoacloud.top

[B01] 条件判断 if / else
来源：http://zqc.jinqigufen.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ahe.hnqzz.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ecw.dianchejie.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://snx.shanyushiyangtech.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bwr.chenjidiqi.icu

Java: String r = x > 0 ? "正" : "非正";
来源：http://rfk.xziqi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wcg.smart0.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ule.ywan-chungtsiang.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yba.shanyushiyangtech.top

[B02] 多分支 else if / elif
来源：http://uod.fengsongda.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ewc.tanke756.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ejx.nanxuanxn.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kqn.fktsv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ifu.jinqigfzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dcf.andypj.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nzi.vehdjk.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://usu.hammf.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hko.jyoumei.cn

[B03] switch / match / case
来源：http://zmc.sjlbkw.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://quu.havefunace.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sqt.hysaishi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://edf.fzhhl.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ybj.aibaodan.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pdh.tian-w.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rjh.wangshuangyany.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ehn.gotoacloud.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://obi.yj202588.top

[B04] for 计数循环
来源：http://bsa.c1oappe.top

Py:   for i in range(10): print(i)
来源：http://xpk.yj202588.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://aks.aizwys.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ryh.hesvh.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ami.tanke756.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://fuu.tanke756.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tno.jyoumei.cn

Ruby: 10.times { |i| puts i }
来源：http://adg.hammf.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://npo.yangfankeji.com

[B05] 遍历数组 / 列表
来源：http://oce.316326.xyz

Py:   for item in arr: print(item)
来源：http://xgg.tanke756.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ewr.yonumen.top

JS:   for (const item of arr) { console.log(item); }
来源：http://wze.sysykeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://odg.wangdashe.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://pzz.hcnkem.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fqg.pengpengdd.cyou

Ruby: arr.each { |item| puts item }
来源：http://unf.epnwcf.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gcb.gaohongyu789.top

[B06] 遍历字典 / 对象
来源：http://ppw.wangshuangyany.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mpa.jqgfzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zji.yj20258888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nvb.nwbrower.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nlq.ehwqpu.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cax.yfazqb.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zne.hnqzz.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qzp.pycfn.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sqb.chenjidiqi.icu

[B07] while 循环
来源：http://jcp.kuanghao11.cn

Py:   while i < 10: i += 1
来源：http://ojd.snrcjt.cn

PHP:  while ($i < 10) { $i++; }
来源：http://vvv.pycfn.com

JS:   while (i < 10) { i++; }
来源：http://ixv.xuanzx.com

TS:   while (i < 10) { i++; }
来源：http://qqq.uphjek.com

Java: while (i < 10) { i++; }
来源：http://ubb.zycfv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://htm.sweek.top

Ruby: while i < 10; i += 1; end
来源：http://hlb.daxiang520.top

C#:   while (i < 10) { i++; }
来源：http://fbr.tanke756.top

[B08] do-while（至少执行一次）
来源：http://cqk.chenlongwang.top

Py:   # 无 do-while：用 while True + break
来源：http://cqe.yj202588.top

PHP:  do { $i++; } while ($i < 10);
来源：http://arf.ywan-chungtsiang.top

JS:   do { i++; } while (i < 10);
来源：http://itc.yj20258.top

TS:   do { i++; } while (i < 10);
来源：http://ecw.52xcode.cn

Java: do { i++; } while (i < 10);
来源：http://ejt.yongpay.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ize.zdqjudy.top

Ruby: begin; i += 1; end while i < 10
来源：http://mxr.nanxuanxn.top

C#:   do { i++; } while (i < 10);
来源：http://ddd.chenzaomai.com

[B09] break 与 continue
来源：http://zrq.daria6918.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nba.sjlbkw.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nbw.yuxming.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fso.tanke756.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fbb.mhx1999.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mtk.daria6918.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cvc.xinyue.icu

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wmm.yj20258.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tkh.snrcjt.cn

[B10] 遍历同时拿索引
来源：http://qqw.jinqigufen.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://viq.ctjpmb.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://obh.pycfn.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ltz.zhaomingkeji.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fgv.guannengcc.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lvt.sufxvd.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xsv.c1oappe.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://axx.jqgufenzy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lav.ehwqpu.com

[B11] 生成数字序列 / 区间
来源：http://hou.daria6918.cn

Py:   list(range(0, 10, 2))
来源：http://dei.fzhhl.top

PHP:  range(0, 10, 2);
来源：http://ypz.yanxiufei.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nmx.xziqi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://adv.0kj1m.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pgv.sxryk.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rqr.fengsongda.top

Ruby: (0...10).step(2).to_a
来源：http://qwc.yfazqb.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vfi.shuidangran.top

[B12] 跳出多层循环
来源：http://bdj.ehwqpu.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://erm.chenzaomai.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://ryn.shanyushiyangtech.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dtb.fehbvm.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://pmy.hysaishi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cgg.chenzaomai.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ynh.zhiwuduotai.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://knb.zdqjudy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://kqz.zhijiandao.cn

[B13] 判断是否为数字
来源：http://lya.jianghu66.top

Py:   isinstance(x, (int, float))
来源：http://emo.yangfankeji.com

PHP:  is_numeric($x)
来源：http://pkh.ctjpmb.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hha.jinghuilouyu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://idw.52xcode.cn

Java: x instanceof Number
来源：http://squ.c1oappe.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://isv.wangdashe.top

Ruby: x.is_a?(Numeric)
来源：http://kmh.jyoumei.cn

C#:   x is int or double or decimal
来源：http://jgd.ydzc1.top

[B14] 判断值是否在集合内
来源：http://gvp.nanxinkj.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pcs.jianghu66.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://piz.ehwqpu.com

JS:   [1, 2, 3].includes(x)
来源：http://eia.zhiwuduotai.top

TS:   [1, 2, 3].includes(x)
来源：http://wum.birdmap.top

Java: List.of(1, 2, 3).contains(x)
来源：http://jts.xinyue.icu

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bpr.zhaomingkeji.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://xqv.zdqjudy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xtl.iojbl.cn

[B15] 布尔运算与取反
来源：http://iue.hesvh.cn

Py:   a and b or not c
来源：http://rli.yuxming.cn

PHP:  $a && $b || !$c
来源：http://wkr.jianghu66.top

JS:   a && b || !c
来源：http://avi.sufxvd.cn

TS:   a && b || !c
来源：http://mpy.zdbjq.cn

Java: a && b || !c
来源：http://uqa.meibo888.top

Go:   a && b || !c
来源：http://zqe.jyoumei.cn

Ruby: a && b || !c
来源：http://qsc.0kj1m.cn

C#:   a && b || !c
来源：http://mbo.sysykeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://yvz.yfazqb.com

Py:   if not data: return
来源：http://kgf.gotoacloud.top

PHP:  if (!$data) { return; }
来源：http://pmk.meibo888.top

JS:   if (!data) return;
来源：http://kjb.shanyushiyangtech.top

TS:   if (!data) return;
来源：http://zld.shuidangran.top

Java: if (data == null) return;
来源：http://xub.fengsongda.top

Go:   if data == nil { return }
来源：http://fpc.shanyushiyangkeji.top

Ruby: return if data.nil?
来源：http://hnd.aizwys.cn

C#:   if (data == null) return;
来源：http://usc.gotoacloud.top

================================================================================
来源：http://reu.smart0.xyz

C. 函数与作用域
来源：http://aai.sweek.top

================================================================================
来源：http://wiw.fktsv.cn

[C01] 定义函数
来源：http://fmk.pengpengdd.cyou

Py:   def add(a, b): return a + b
来源：http://bap.shuidangran.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://luv.havefunace.top

JS:   function add(a, b) { return a + b; }
来源：http://ius.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mzq.ivvv.top

Java: static int add(int a, int b) { return a + b; }
来源：http://aho.xingfuxueyuan.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://dzq.nanxuanxn.top

Ruby: def add(a, b); a + b; end
来源：http://kjm.fzhhl.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://plp.dianchejie.cn

[C02] 默认参数
来源：http://qqp.yuanzhike.top

Py:   def greet(name="World"): return name
来源：http://opl.fzhhl.top

PHP:  function greet($name = "World") { return $name; }
来源：http://hum.zdbjq.cn

JS:   function greet(name = "World") { return name; }
来源：http://pwc.jqgfzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://yqv.feifeiyinyue.top

Java: // 无默认参数：方法重载或 Optional
来源：http://tpx.daxiang520.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qmr.kuanghao11.cn

Ruby: def greet(name = "World") = name
来源：http://qnj.zhoulong.xyz

C#:   string Greet(string name = "World") => name;
来源：http://ggy.ydzc1.top

[C03] 可变参数
来源：http://zjz.wangdashe.top

Py:   def total(*args): return sum(args)
来源：http://urw.ehwqpu.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bwe.jinghuilouyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gkq.guannengcc.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uum.zhaomingkeji.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hxb.svipenyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kjc.fktsv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gan.meibo888.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pty.ivvv.top

[C04] 命名参数 / 关键字参数
来源：http://bln.shanyushiyangkeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gws.dashuyun.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://qkx.sysykeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xzn.ydzc1.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://esr.svipenyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://mui.0kj1m.cn

Go:   // 无：用配置结构体参数
来源：http://rpy.jqgufenzy.top

Ruby: f(a: 1, b: 2)
来源：http://hjr.jqgufenzy.top

C#:   f(a: 1, b: 2)
来源：http://ent.yuanzhike.top

[C05] 返回多个值
来源：http://jet.chenzaomai.com

Py:   return a, b
来源：http://env.tanke756.top

PHP:  return [$a, $b];
来源：http://ijb.gogol.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yrp.yanxiufei.cn

TS:   return { a, b };
来源：http://shh.shzxlz.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gxa.zhengqikj.top

Go:   return a, b
来源：http://sqs.havefunace.top

Ruby: return a, b
来源：http://gmw.iojbl.cn

C#:   return (a, b);              // ValueTuple
来源：http://lki.ybcxt.top

[C06] 匿名函数 / lambda
来源：http://asn.ybcxt.top

Py:   square = lambda x: x * x
来源：http://lys.xylfe.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://emi.redwolf501.top

JS:   const square = x => x * x;
来源：http://web.tian-w.cn

TS:   const square = (x: number): number => x * x;
来源：http://mnb.jinyuanbaomall.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fnw.wangshuangyany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ajb.sjlbkw.cn

Ruby: square = ->(x) { x * x }
来源：http://rgo.ydjk.org.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dfu.nanxuanxn.top

[C07] 把函数作为参数传入
来源：http://osg.daxiang520.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vfa.shuidangran.top

PHP:  array_map("strtoupper", $arr);
来源：http://lsg.ehwqpu.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jgf.zhijiandao.cn

TS:   arr.map(String)
来源：http://lii.c1oappe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cwz.svipenyu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://imj.iojbl.cn

Ruby: arr.map(&:upcase)
来源：http://plq.c1oappe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://tig.yueranfly.top

[C08] 闭包
来源：http://ywi.jinqigufen.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ajx.aizwys.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hod.yfazqb.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://tcv.zhengqikj.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://xaf.mhx1999.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mxk.cheryme.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://djp.jqgufenzy.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mbu.dianchejie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://lgx.jyoumei.cn

[C09] 递归
来源：http://qzf.pycfn.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://her.wangshuangyany.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://sgr.ctjpmb.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hon.chenlongwang.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cor.ydjk.org.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bjp.hysaishi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://dzu.havefunace.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rcw.cdnleiting.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vis.jyoumei.cn

[C10] 变量作用域
来源：http://xmt.sufxvd.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://dvg.gaohongyu789.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wdb.ybcxt.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ohm.fktsv.cn

TS:   同 JS
来源：http://njc.ywan-chungtsiang.top

Java: 方法内为块级作用域
来源：http://koy.yvedp.cn

Go:   花括号块级作用域
来源：http://ycc.cdnleiting.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bce.zhiwuduotai.top

C#:   块级作用域
来源：http://aco.tanke756.top

[C11] 模块导入与导出
来源：http://bad.gzhubu.top

Py:   from module import func
来源：http://zvw.zhongyouzk.top

PHP:  require "file.php";  或 use App\Service;
来源：http://kkx.zhengqikj.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://vol.yueranfly.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yto.fktsv.cn

Java: import java.util.List;
来源：http://tgc.yongpay.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://msv.dashuyun.cn

Ruby: require "json"; require_relative "./util"
来源：http://csl.snrcjt.cn

C#:   using System.Text;
来源：http://faz.yvedp.cn

[C12] 立即执行函数 IIFE
来源：http://ocw.dianchejie.cn

Py:   (lambda: print("run"))()
来源：http://pzm.aizwys.cn

PHP:  (function () { echo "run"; })();
来源：http://xrq.xziqi.cn

JS:   (() => { console.log("run"); })();
来源：http://dag.jqgufenzy.top

TS:   (() => { console.log("run"); })();
来源：http://cdl.jianghu66.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nfj.ctjpmb.com

Go:   func() { fmt.Println("run") }()
来源：http://fxy.zdbjq.cn

Ruby: -> { puts "run" }.call
来源：http://kjw.birdmap.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ism.xziqi.cn

[C13] 类型声明 / 类型注解
来源：http://wqb.bjfxy.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://veg.yj202588.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wio.iojbl.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qvq.xuanzx.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rbz.cashguo.top

Java: int add(int a, int b) { return a + b; }
来源：http://iwn.hnxiangtu.top

Go:   func add(a, b int) int
来源：http://gmk.dashuyun.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ene.redwolf501.top

C#:   int Add(int a, int b) => a + b;
来源：http://nor.zhoulong.xyz

[C14] 泛型函数
来源：http://cci.daria6918.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vsx.tanke756.top

PHP:  // 无泛型
来源：http://hel.birdmap.top

JS:   // 无泛型
来源：http://qmu.yj202588.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cqk.nanxinkj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pcb.fehbvm.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bqd.iojbl.cn

Ruby: # 无泛型
来源：http://uht.shzxlz.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dbu.tanke756.top

[C15] 解构 / 展开参数
来源：http://icy.aibaodan.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://agv.bjfxy.top

PHP:  [$a, $b] = $pair;
来源：http://eec.ywan-chungtsiang.top


<!-- 参考信息 -->